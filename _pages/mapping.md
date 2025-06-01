---
title: "Mapping"
layout: single
sitemap: true
permalink: /mapping/
author_profile: true
header:
  overlay_color: "#000"
  overlay_filter: "0.2"
  overlay_image: assets/banner_mapping.jpg
  actions:
    - label: "Download CV"
      url: "assets/CV_DeCamillis.pdf"
toc: true
toc_label: "Mapping"
toc_icon: "gear"
toc_sticky: true
---


## Road Safety in ACT

![ArcGIS](https://img.shields.io/badge/ArcGIS-2C7AC3?logo=arcgis&logoColor=fff)

In this project, I combined local road infrastructue network data of the Australian Capital Territory (ACT) with public domain reports on cycling accidents. By merging databases and using geometry integration strategies, I mapped out sensitive safety hazard points that could inform future governance decisions.

>![Cyclist_accidents](/assets/mapping/cyclist_crashes_canberra.jpg)
>*A heatmap of cyclist crash density (pixel radius: 10 m, search radius: 200 m) highlighting the risk of accidents in proximity of major traffic intersection nodes.*
{: style="width: 85%; font-size: 0.9rem;"}

References:

- Road Cyclist Crashes data provided by TCCS at the [ACT Government Open Data Portal](https://www.data.act.gov.au/Justice-Safety-and-Emergency/Cyclist-Crashes/n2kg-qkwj/about_data).


## Navigation

![QGIS](https://img.shields.io/badge/QGIS-589632?logo=qgis&logoColor=fff)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=fff)

For planning off-trail hikes and practicing map navigation, I create high-resolution topographic maps with the my python module [qgis_nsw_act_topo](https://github.com/sdecamillis/qgis_nsw_act_topo). This tool allows for the automated generation of maps of a specific area of interest, with the possibility to include the latest data on vegetation coverage and wooded areas. I also utilise Digital Elevation Model (DEM) raster tiles to generate hillshade effects and contour lines, enhancing the map's detail and accuracy.

>[![Devils Gap hike map](/assets/mapping/Devils_Gap_hike_detail.jpg)](/assets/mapping/Devils_Gap_hike.jpg)
>*Detail of a topographic map of the Tidbinbilla Nature Reserve with vegetation coverage and hillshade effect, suitable for map and compass navigation. The purple line represents my latest hike from the Devil's Gap to Billy Billy Rocks.*
{: style="width: 85%; font-size: 0.9rem;"}

References:

- Woody extent and foliage projective cover (FPC) data provided by the NSW Office of Environment and Heritage at the [TERN Data Discovery Portal](https://data.tern.org.au/rs/public/data/spot/woody_fpc_extent/nsw-2011/),
- Digital Elevation Model (DEM) raster data provided by the Foundation Spatial Data Framework at the [Elvis Elevation and Depth Portal](https://elevation.fsdf.org.au/),
- Topographic data downloaded from the [REST server](https://portal.spatial.nsw.gov.au/server/rest/services/) of the NSW Spatial Collaboration Portal.



## ACTSES Training

![QGIS](https://img.shields.io/badge/QGIS-589632?logo=qgis&logoColor=fff)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=fff)


Orienteering and navigation are essential skills for ACTSES members, particularly during remote search operations. As the Deputy Training Officer at the local SES Unit, I planned and coordinated an offsite navigation exercise at Mount Stromlo. To support the activity, I developed a custom map highlighting key features such as ponds, rivers, hilltops, and transmission lines—key reference elements for navigating towards control points.

>[![ACTSES Navigation map](/assets/mapping/ACTSES_Navigation_map_detail.jpg)](/assets/mapping/ACTSES_Navigation_map.jpg)
>*Detail of a topographic map of Mount Stromlo developped for the ACTSES navigation exercise. The green circles represent the control points.*
{: style="width: 85%; font-size: 0.9rem;"}

References:

- ACT cadastre data downloaded from the [REST server](https://services1.arcgis.com/E5n4f1VY84i0xSjy/arcgis/rest/services/ACTGOV_BLOCKS/FeatureServer) provided by the ACTmapi database.

{% comment %}
I am interested in developing and using topographic maps for hiking and navigation activities. For this purpose, I learned how to build topo maps with the open-source software QGIS, giving me freedom to display only the features relevant for each specific exercise.

I use vegetation raster data as base layer and I superimpose a hill-shade layer generated from 5-metre DEM data. Then, I import all the vector layers, including contour lines and geographical points of interest, from the NSW and ACT GIS databases.

I crated a python script to automate the download of the required data and the map generation with the customised symbology style. Below a couple of examples. 
{% endcomment %}