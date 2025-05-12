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


## Topographic maps with QGIS

I am interested in developing and using topographic maps for hiking and navigation activities. For this purpose, I learned how to build topo maps with the open-source software QGIS, giving me freedom to display only the features relevant for each specific exercise.

I use vegetation raster data as base layer and I superimpose a hill-shade layer generated from 5-metre DEM data. Then, I import all the vector layers, including contour lines and geographical points of interest, from the NSW and ACT GIS databases.

I crated a python script to automate the download of the required data and the map generation with the customised symbology style. Below a couple of examples. 


### Off-trail Hiking

As deputy training officer at the local ACTSES Unit, I planned and coordinated an offsite navigation exercise at Mount Stromlo. For this event, I developped a topo map with contour lines and geographical points of interests of the area.

>![Devils Gap hike map](/assets/mapping/Devils_Gap_hike_detail.jpg)
>*Detail of the topo map developped for the ACTSES navigation exercise.*
{: style="width: 85%; font-size: 0.9rem;"}

### ACTSES Navigation Exercise

As deputy training officer at the local ACTSES Unit, I planned and coordinated an offsite navigation exercise at Mount Stromlo. For this event, I developped a topo map with contour lines and geographical points of interests of the area.

>![ACTSES Navigation map](/assets/mapping/ACTSES_Navigation_map_detail.jpg)
>*Detail of the topo map developped for the ACTSES navigation exercise.*
{: style="width: 85%; font-size: 0.9rem;"}