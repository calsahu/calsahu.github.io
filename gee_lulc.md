# Land Cover Analysis using Google Earth Engine

I prepared a Land Cover classification workflow in Google Earth Engine, for the city of Bhubhaneswar. I used NDVI (Normalized Difference Vegetation Index) to classify land cover categories. 

`
// Ensure the FeatureCollection is not empty
var featureCount = bhubaneswar.size();
print('Number of features in Bhubaneswar:', featureCount);

// If the FeatureCollection is not empty, proceed
if (featureCount.gt(0)) {
  // Get the first feature's geometry
  var bhubaneswarGeometry = bhubaneswar.first().geometry();
  
  // Import Landsat 5 Collection 2 Tier 1 Surface Reflectance data
  var landsat5 = ee.ImageCollection("LANDSAT/LT05/C02/T1_L2")
    .filterBounds(bhubaneswarGeometry)
    .filterDate('2009-01-01', '2009-12-31')
    .filter(ee.Filter.lt('CLOUD_COVER', 30))
    .sort('CLOUD_COVER')
    .first();

  // Print the image to check available bands
  print('Landsat 5 image:', landsat5);
  print('Landsat 5 image bands:', landsat5.bandNames());

  // Select the correct bands and apply scaling factors
  var bands = ['SR_B1', 'SR_B2', 'SR_B3', 'SR_B4', 'SR_B5', 'SR_B7'];
  var image = landsat5.select(bands).multiply(0.0000275).add(-0.2).clip(bhubaneswarGeometry);

  // Calculate NDVI
  var ndvi = image.normalizedDifference(['SR_B4', 'SR_B3']).rename('NDVI');

  // Simple classification based on NDVI
  var classified = ee.Image(0)
    .where(ndvi.gte(-1).and(ndvi.lt(0.3)), 1)  // Water
    .where(ndvi.gte(0.3).and(ndvi.lt(0.5)), 2)  // Built-up
    .where(ndvi.gte(0.5).and(ndvi.lt(0.55)), 3)  // Open land
    .where(ndvi.gte(0.55).and(ndvi.lt(0.65)), 4)  // Grassland/Cropland
    .where(ndvi.gte(0.65), 5);  // Dense vegetation

  // Clip the final classified image to Bhubaneswar's boundary
  var clippedClassified = classified.clip(bhubaneswarGeometry);

  // Visualization parameters
  var vis = {
    min: 1,
    max: 5,
    palette: ['0000FF', 'FF0000', 'FFFF00', '00FF00', '008000']
  };

  // Add the classified image to the map
  Map.centerObject(bhubaneswarGeometry, 10);
  Map.addLayer(image)
  Map.addLayer(clippedClassified, vis, 'Clipped Classification');

  // Calculate areas for each class within Bhubaneswar's boundary
  var areaImage = ee.Image.pixelArea().addBands(clippedClassified.rename('class'));
  
  var areas = areaImage.reduceRegion({
    reducer: ee.Reducer.sum().group({
      groupField: 1,
      groupName: 'class',
    }),
    geometry: bhubaneswarGeometry,
    scale: 30,
    maxPixels: 1e13
  });

  print('Areas:', areas);
} else {
  print('Error: Bhubaneswar FeatureCollection is empty');
}

// Add legend
var legend = ui.Panel({style: {position: 'bottom-left', padding: '8px 15px'}});
var legendTitle = ui.Label({value: 'Land Cover Classes', style: {fontWeight: 'bold', fontSize: '18px', margin: '0 0 4px 0', padding: '0'}});
legend.add(legendTitle);

var makeRow = function(color, name) {
  var colorBox = ui.Label({style: {backgroundColor: color, padding: '8px', margin: '0 0 4px 0'}});
  var description = ui.Label({value: name, style: {margin: '0 0 4px 6px'}});
  return ui.Panel({widgets: [colorBox, description], layout: ui.Panel.Layout.Flow('horizontal')});
};

var palette = ['0000FF', 'FF0000', 'FFFF00', '00FF00', '008000'];
var names = ['Water', 'Built-up', 'Open space', 'Grassland/Cropland', 'Dense Vegetation'];
for (var i = 0; i < 5; i++) {
  legend.add(makeRow(palette[i], names[i]));
}

Map.add(legend);
`
