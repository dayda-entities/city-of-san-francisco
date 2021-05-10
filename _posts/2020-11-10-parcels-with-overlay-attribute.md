---
title: Parcels with overlay attributes
created: '2020-11-10T16:56:18.163913'
modified: '2020-12-04T19:33:04.689741'
state: active
type: dataset
tags:
  - Boundaries
  - City Reference Data
groups:
  - Local Government
csv_url: 'https://data.sfgov.org/api/views/9grn-xjpx/rows.csv?accessType=DOWNLOAD'
json_url: 'https://data.sfgov.org/api/views/9grn-xjpx/rows.json?accessType=DOWNLOAD'
layout: post

---
<strong>A. SUMMARY</strong>
This dataset is derived from <a href="https://data.sfgov.org/Geographic-Locations-and-Boundaries/Parcels-Active-and-Retired/acdm-wktn">parcels</a> and several other overlay administrative boundaries (listed below). The dataset was developed by DataSF as a convenience for matching parcels to districts where appropriate. This can be simpler than running a geospatial process every time you want to join parcels to a boundary. The districts provided here run along streets and are non-overlapping so that the parcels will be contained within a single district.

The boundaries included are:
1. <a href="https://data.sfgov.org/Geographic-Locations-and-Boundaries/Analysis-Neighborhoods/p5b7-5n3h">Analysis Neighborhoods</a>
2. <a href="https://data.sfgov.org/Geographic-Locations-and-Boundaries/Current-Supervisor-Districts/8nkz-x4ny">Supervisor Districts</a>
3. <a href="https://data.sfgov.org/Public-Safety/Current-Police-Districts/wkhw-cjsf">Police Districts</a>
4. <a href="https://data.sfgov.org/Geographic-Locations-and-Boundaries/Planning-Districts/ttns-6zj3">Planning Districts</a>

<strong>B. HOW THE DATASET IS CREATED</strong>
A script runs daily that overlays parcels with each of the boundaries to produce the composite dataset.

<strong>C. UPDATE PROCESS</strong>
Updated daily by a script based on the upstream parcels dataset which is also updated daily.

<strong>D. HOW TO USE THIS DATASET</strong>
You can use this dataset to match to administrative districts provided here to datasets that contain a parcel number. This can be a simpler process than running these joins spatially. 

In short, we pre-process the spatial overlays to make joins simpler and more performant.
