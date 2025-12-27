# Projects

## Mapping

### Faith-based Housing (Fall 2025- Present)
This project is based on the research of Dr. Nadia Mian at the Voorhees Center for Civic Engagement on "YIGBY" developments. YIGBY refers to "Yes in God's Backyard" in which faith-based
insitutions such as churches, synagouges, mosques, etc that had redeveloped a part of their sites to be turned into affordable housing units. The following map intreprets data that 
has been collected through scraping data about the developments created from 2015-2025, as well as data from the US Census and current YIBGY legislature. 

It was completed for the class "Command Line GIS" in collaboration with Jyotsna Kumar. The visualizations made by me are attached. You can see the whole project [here](https://jyotsnakumarg.github.io/Faith_Based_Affordable_Housing_Project/):

#### US Developments
<iframe src="InteractiveWebmapFB.html" height="855" width="95%"></iframe>
All 200 developments in the database (as of December 2025) are included in this map. These developments were cleaned extensively and geocoded using ArcGIS geocoder in Python, and visualized using the folium library. The pattern of faith-based housing developments being constructed can be visualized using the timeline slider, which populates the developments by year*. The construction time data was cleaned to bring it to a visualizable format in folium’s timeline slider tool. 

Clicking on each development reveals a small popup which provides information on:
- The project name
- The congregation name and denomination/religion
- The year the project was completed
- The type of housing
- The project size
- The developer’s name
- If the property has a historic status
- The project description

Statewise trends can be toggled on/off, in the upper right-hand corner of the map. They provide information on the rent-burdened population, the status of YIGBY law implementation**, and the number of developments in each state. Hovering over each feature reveals information on each trend. These datasets were prepared from the static maps.

The basemap can also be switched between a simple Carto Positron basemap and Open Street Map, which can be helpful to examine other local features if you zoom into the basemap.

<em>*4 developments’ opening dates have not been identified. They populate in the final year of the timeline slider, 2025. **As per December, 2025.</em>

#### YIGBY States
<img src="YIGBYMap (2).png" alt="YIGBY Legislation and Development Counts">

The status of YIGBY legislation* compared with statewise development counts, as of 2025, can be compared here. The list of states was prepared by the research team for the Faith-based Affordable Housing project. This data was initially in excel format, which was spatially joined with shoreline-clipped state shapefiles from NHGIS. 
Each state is colored based on whether they have passed laws, considered laws, declined to pass laws, or have not considered YIGBY legislation. Overlaid are circles representing the total number of developments passed in each state. 

<em>*This map includes statewise legislation. YIGBY laws have also been passed at the local level, which is not included in the visualization.</em>

### NYC Squirrel Census

<iframe src="squirrel_map_NYC (1).html" height="855" width="95%"></iframe>

### Housing Affordability in San Francisco

<img src="MAP4_Rentburden_Principles of Housing.png" alt="Rent Burden in San Francisco">

<img src="MAP5_RentBurdenAffordableHousing_Principles of Housing.png" alt="Rent Burden and Affordable Housing in San Francisco">

### Bhubhaneswar EPIC Project

<img src="EPIC_BBSR_KP_2.png" alt="EPIC BBSR Projects">

### Groundwater Situation of Delhi
Made for NIUA, under the supervision of Dr. Victor Shinde and Banibrata Choudhury.
<iframe src="GWSTRESSDELHI.pdf" width="100%" height="600px"></iframe>
<iframe src="GWRecharge_Parks.pdf" width="100%" height="600px"></iframe>
<iframe src="GWQualityDELHI.pdf" width="100%" height="600px"></iframe>
<iframe src="GWDepthtoLevelDecadalDELHI.pdf" width="100%" height="600px"></iframe>
<iframe src="GWDelhi_Recharge_Waterbodies.pdf" width="100%" height="600px"></iframe>
<iframe src="GWDelhiInfiltrationParks.pdf" width="100%" height="600px"></iframe>
<iframe src="GWDelhiInfiltration.pdf" width="100%" height="600px"></iframe>
<iframe src="GWDelhiDischarge.pdf" width="100%" height="600px"></iframe>
<iframe src="FIXEDBuiltUp.pdf" width="100%" height="600px"></iframe>
<iframe src="DelhiGWDischargeRate.pdf" width="100%" height="600px"></iframe>

## Presentations

### Earth Day and Shallow Aquifers Instagram Post
<img src="1.png" alt="1">
<img src="2.png" alt="2">
<img src="3.png" alt="3">
<img src="4.png" alt="4">
