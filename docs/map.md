---
currentMenu: map
---

# Map

## Georeferencing images
- Mission Planner can geo-reference images [<i class="fa fa-fw fa-external-link"></i>](http://ardupilot.org/planner/docs/common-geotagging-images-with-mission-planner.html)
- When geo-referencing images in Mission Planner, it will also try and include system files
  - If you copied images off the memory card using OSX you may end up with hidden files such as `._DSC0098.JPG` that will mess up the message count compared to file count

## Ground control points


![](img/map/gcp.jpg)

## Image processing

**OpenDroneMap (ODM)** is an open source toolkit for processing aerial drone imagery.
[<i class="fa fa-fw fa-external-link"></i>](http://opendronemap.org/)
[<i class="fa fa-fw fa-twitter"></i>](https://twitter.com/opendronemap)
[<i class="fa fa-fw fa-github-alt"></i>](https://github.com/OpenDroneMap/OpenDroneMap)

![](img/map/odm.png)

**WebODM** is a free, user-friendly, extendable application and API for drone image processing (it uses ODM for the processing).
[<i class="fa fa-fw fa-external-link"></i>](https://www.webodm.org/)
[<i class="fa fa-fw fa-github-alt"></i>](https://github.com/OpenDroneMap/WebODM)

![](img/map/webodm.png)

**Portable OpenStreetMap (POSM)** integrates best-of-breed tools from a variety of sources and developers on a single device that can be deployed to the field to facilitate mapping efforts, particularly when internet access is absent. It includes a version of ODM as well as an imagery API.
[<i class="fa fa-fw fa-external-link"></i>](http://posm.io/)
[<i class="fa fa-fw fa-twitter"></i>](https://twitter.com/awesomeposm)
[<i class="fa fa-fw fa-github-alt"></i>](https://github.com/posm)

![](img/map/posm.png)

---

## Viewing

**QGIS** is a free and open source geographic information system that can be used for viewing and editing raster data such as the orthorectified imagery outputs from ODM.
[<i class="fa fa-fw fa-external-link"></i>](http://www.qgis.org/)
[<i class="fa fa-fw fa-twitter"></i>](https://twitter.com/qgis)
[<i class="fa fa-fw fa-github-alt"></i>](https://github.com/qgis/)

![](img/map/qgis.png)

---

## Sharing

**OpenAerialMap (OAM)** is an open service to provide access to a commons of openly licensed imagery and map layer services. Anyone can download or contribute imagery to this growing commons of openly licensed imagery.
[<i class="fa fa-fw fa-external-link"></i>](https://openaerialmap.org/)
[<i class="fa fa-fw fa-twitter"></i>](https://twitter.com/openaerialmap)
[<i class="fa fa-fw fa-github-alt"></i>](https://github.com/hotosm/OpenAerialMap)

![](img/map/oam.png)

- OAM will handle data in any CRS
  - The way to bundle the `*.tfw` and `*.prj`files is to use `gdal_translate` to write it out as a single file where that same data is included in the geotiff metadata (which may already be the case; try moving those sidecar files and run `gdalinfo` on the geotiff)

---

## Mapping

OpenStreetMap (OSM) is built by a community of mappers that contribute and maintain data about roads, trails, buildings, transportation infrastructure, and much more, all over the world. Imagery hosted on OAM can be loaded as a base layer and used to trace features into OSM.
[<i class="fa fa-fw fa-external-link"></i>](https://www.openstreetmap.org)
[<i class="fa fa-fw fa-twitter"></i>](https://twitter.com/openstreetmap)

![](img/map/osm.png)