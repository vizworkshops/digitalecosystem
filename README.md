# Welcome to the Digital Ecosystem workshop repository. 

This repo contains materials and a wiki that will help walk you through how to set up a simple digital ecosystem using software and data that is freely and (mostly) readily available. 

One of the underlying motivations for this workshop is to provide a model for how to easily create a digital map that incorporates point data with raster data (historical maps). 
--------------
You will need at least 3 accounts to participate in this workshop.

* CARTO - Mapping and spatial analysis tool.
* GitHub - A software development platform where you can build, collaborate, and share projects.
* MapBox - Open source mapping platform that can help you host maps among many other features.

GitHub now offers a Student Developer Pack for current students with valid institution email accounts. 
Please go here and sign up for a pack BEFORE the workshop:

* GitHub Student Developer Pack - https://education.github.com/pack/join
* MapBox - https://www.mapbox.com/signup/

In the case you do not get your Student Developer Pack in time for the workshop, sign up for a 30 day trial to CARTO and get a GitHub and MapBox account separately. There will be no problem doing the workshop with the trial version of CARTO!

* Carto - https://carto.com/signup/
* Mapbox - https://www.mapbox.com/signup/
* GitHub - https://github.com/join?source=header-home
----------
What makes a good project? The easiest answer is a meaningful question or inquiry. For this workshop we will use Los Angeles as our site of analysis. One of the best examples of a digital mapping project is South Carolina's Green Book project:

* http://library.sc.edu/digital/collections/greenbook.html 

We will seek to recreate a version of this project at the local level in order to learn more about Los Angeles, race, and place.

----------
For most digital projects you will have an assortment of materials that you will then want to visualize on a map or some other method. For this example project we want to learn more about the history of Los Angeles through the lens of the GreenBook. We will use the following data to build out our project:

* a dataset created by pulling data from the GreenBook
* georeferenced historical maps of Los Angeles
* census data
* Los Angeles Times neighborhood boundary data
* Historical HOLC (Insurance map) boundary and rating data

Using these datasets we will create a digital project that will let us explore Los Angeles and provide opportunities for meaningful engagement, interpretation, discovery, and critical thinking.
----------------
For this project we will use a collection of different types of data.

All files are located in this google drive:

https://drive.google.com/file/d/1FIy-UBg48NLZfYIjiJYTXSHISJpfzGE9/view?usp=sharing

CSV files

CSV files with locations of places listed in the GreenBook. Special thanks to Professor Genevieve Carpio at UCLA and student research assistant Jose Cardona for creating and sharing the data. Jose compiled the data for these two sheets last year while doing research for an ongoing project. We used google sheets to store the data and a script that plugs into google sheets to geocode the addresses. Each address was manually transcribed by Jose from the NYPL GreenBook website - https://digitalcollections.nypl.org/collections/the-green-book#/?tab=about - then checked against current street data to verify each location.

* 39GreenBook.csv
* 47GreenBook.csv

Historical Maps These maps are already georeferencedgeo-referenced. This means that they have been processed using GIS software so that they have been associated or pinned to real world locations. The files are all .tiff files that have been geo-referenced.

* wattsmap.zip
* 4 HOLC Maps: NorthEastLA.zip, NorthernLA.zip, SouthernLA.zip, CentralLA.zip
* LA Times article using Watts Map - http://graphics.latimes.com/watts-riots-1965-map/
* Richmond Panoroma project - https://dsl.richmond.edu/panorama/redlining/#loc=9/34.0050/-118.1565&opacity=0.8&city=los-angeles-ca
* QGIS tutorial for georeferencing - https://docs.qgis.org/2.18/en/docs/training_manual/forestry/map_georeferencing.html

Polygon Boundary Files These files show distinct boundaries with associated metadata. The HOLC_LosAngeles.geojson files is a geojson file which is a geographic encoding format. The la_county-neigbhorhoods-v6.zip file contains a shapefile, which is a vector data format developed by ESRI. The shapefile format requires specialized software to be opened. CARTO allows for shapefiles (up to a certain size) to be uploaded as long as they are zipped.

* la-county-neighborhoods-v6.zip _ Los Angeles Neighborhood boundaries as developed by the LA Times.
* HOLC_LosAngeles.geojson Boundaries showing grades for defined neighborhoods in 1939.
* Lots of boundary files provided by the LA Times - http://boundaries.latimes.com/sets/
----------------

Lets try CARTO!

https://cartorutkowski.carto.com/builder/5bbac628-f4c2-4a56-9574-ba0f6ef2430d/embed

Try your own map with the data.

Download any of the following files from the Google Drive:

39GreenBook.csv
47GreenBook.csv
HOLC_LosAngeles.geojson
la-county-neighborhoods-v6.zip

HOVER Image code:

<div class="cartodb-tooltip-content-wrapper">
  <div class="cartodb-tooltip-content"> <p><img width=100 src={{image}}></p> </div> </div>

