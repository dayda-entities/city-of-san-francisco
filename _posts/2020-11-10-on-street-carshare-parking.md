---
title: On-street Carshare Parking
created: '2020-11-10T16:56:32.977573'
modified: '2020-12-04T19:33:48.042077'
state: active
type: dataset
tags:
  - Car Share
  - Carshare
  - On Street Car Share
  - On Street Car Share Pilot
  - Onstreet
groups:
  - Local Government
csv_url: 'https://data.sfgov.org/api/views/g2t6-cyw6/rows.csv?accessType=DOWNLOAD'
json_url: 'https://data.sfgov.org/api/views/g2t6-cyw6/rows.json?accessType=DOWNLOAD'
layout: post

---
A. SUMMARY This dataset was first created as part of the SFMTA On Street Car Share Pilot Program (approved by the MTA Board in July 2013) to illustrate the location of implemented and planned (various stages) spaces throughout the city.

B. METHODOLOGY  The locations were originally provided to the MTA as requests by the three car share organizations (CSOs). These were given as a .kml file, which was converted to a .shp. Additional fields were created using spatial joins (zipcode, supervisor district, CNN, etc). Use definition query tool to display those locations with a certain attribute. For example, query Existing = 1 to display those locations that are on street operating. 500 submissions were given by CSOs to the MTA, but only a portion of those were brought to the MTA Board for approval, and even fewer were implemented as operational on street spaces. With no definition query, you can see all spaces as features, with varying levels of data completion. 

C. UPDATE FREQUENCY  During periods of implementation/construction, updates were as frequent as daily or weekly. However, as the frequency of newly implemented spaces slowed over the course of the pilot, updates occurred less frequently--weekly or monthly. Updates will be needed as new spaces are implemented--many of the spaces not taken past MTA Board approval have incomplete data.  

D. OTHER CRITICAL INFO  Each feature (or each row, or point) represents a single car share parking space. Some parking spaces belong to a "pod" where there are two adjacent car share parking spaces, indicated by the "PodType" field. To summarize or analyze by pod, use the "POD" field.
