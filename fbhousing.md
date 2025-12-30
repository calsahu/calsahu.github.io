# Faith-based Housing Project

<div class="top-nav">
  <a href="index.html">About Me</a
  <a href="https://docs.google.com/document/d/e/2PACX-1vTdXMOxjDVlwPxPEMZ2_DTfDJnAC52xALzhIjLUhGW5FnHeF41MyVcPV0RUxzgMhcjNPmRNMxvVOgRB/pub">Resume</a>
  <a href="project.html">Projects</a>
  <a href="paper.html">Papers</a>
  <a href="contact.html">Contact</a>
  <a href="awards.html">Awards</a>
</div>

<style>
.top-nav {
  margin: 10px 0 18px;
}

.top-nav a {
  display: inline-block;
  padding: 8px 14px;
  margin-right: 8px;
  border-radius: 20px;
  background: #f2f2f2;
  font-weight: 600;
  text-decoration: none;
}

.top-nav a:hover {
  background: #e0e0e0;
}
</style>

This project was completed for the class "Command Line GIS" in collaboration with Jyotsna Kumar. The visualizations made by me are attached. You can see the whole project 
[here](https://jyotsnakumarg.github.io/Faith_Based_Affordable_Housing_Project/):

<em>
"This project is based on the research of Dr. Nadia Mian at the Voorhees Center for Civic Engagement on "YIGBY" developments. 
YIGBY refers to "Yes in God's Backyard" in which faith-based insitutions such as churches, synagouges, mosques, etc that had 
redeveloped a part of their sites to be turned into affordable housing units. The following map intreprets data that 
has been collected through scraping data about the developments created from 2015-2025, 
as well as data from the US Census and current YIBGY legislature."
</em>

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
<img src="image/YIGBYMap (2).png" width = "400" alt="YIGBY Legislation and Development Counts">

The status of YIGBY legislation* compared with statewise development counts, as of 2025, can be compared here. The list of states was prepared by the research team for the Faith-based Affordable Housing project. This data was initially in excel format, which was spatially joined with shoreline-clipped state shapefiles from NHGIS. 
Each state is colored based on whether they have passed laws, considered laws, declined to pass laws, or have not considered YIGBY legislation. Overlaid are circles representing the total number of developments passed in each state. 

<em>*This map includes statewise legislation. YIGBY laws have also been passed at the local level, which is not included in the visualization.</em>
