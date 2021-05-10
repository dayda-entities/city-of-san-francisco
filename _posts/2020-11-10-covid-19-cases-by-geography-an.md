---
title: COVID-19 Cases by Geography and Date
created: '2020-11-10T16:56:26.415639'
modified: '2020-12-04T19:33:28.174570'
state: active
type: dataset
tags:
  - Cases
  - Census Tract
  - Covid
  - Covid 19
  - Mapping
  - Maps
  - Neighborhoods
  - Zip
  - Zip Code
groups:
  - Local Government
csv_url: 'https://data.sfgov.org/api/views/d2ef-idww/rows.csv?accessType=DOWNLOAD'
json_url: 'https://data.sfgov.org/api/views/d2ef-idww/rows.json?accessType=DOWNLOAD'
layout: post

---
<strong>A. SUMMARY</strong>
This dataset contains COVID-19 positive confirmed cases aggregated by several different geographic areas and by day. COVID-19 cases are mapped to the residence of the individual and shown on the date the positive test was collected. In addition, 2018 American Community Survey (ACS) 5-year population estimates are included to calculate the cumulative rate per 10,000 residents.

Dataset covers cases going back to March 2nd, 2020 when testing began. This data may not be immediately available for recently reported cases and data will change to reflect as information becomes available. Data updated daily.

Geographic areas summarized are:
1. <a href="https://data.sfgov.org/Geographic-Locations-and-Boundaries/Analysis-Neighborhoods/p5b7-5n3h">Analysis Neighborhoods</a>
2. <a href="https://data.sfgov.org/Geographic-Locations-and-Boundaries/Census-2010-Tracts-for-San-Francisco/rarb-5ahf">Census Tracts</a>
3. <a href="https://www.census.gov/programs-surveys/geography/guidance/geo-areas/zctas.html">Census Zip Code Tabulation Areas</a>

<strong>B. HOW THE DATASET IS CREATED</strong>
Addresses from the COVID-19 case data are geocoded by the San Francisco Department of Public Health (SFDPH). Those addresses are spatially joined to the geographic areas. Counts are generated based on the number of address points that match each geographic area for a given date.

The 2018 ACS estimates for population provided by the Census are used to create a cumulative rate which is equal to ([cumulative count up to that date] / [acs_population]) * 10000) representing the number of total cases per 10,000 residents (as of the specified date).

COVID-19 case data undergo quality assurance and other data verification processes and are continually updated to maximize completeness and accuracy of information. This means data may change for previous days as information is updated.

<strong>C. UPDATE PROCESS</strong>
Geographic analysis is scripted by SFDPH staff and synced to this dataset each day.

<strong>D. HOW TO USE THIS DATASET</strong>
This dataset can be used to track the spread of COVID-19 throughout the city, in a variety of geographic areas. Note that the new cases column in the data represents the number of new cases confirmed in a certain area on the specified day, while the cumulative cases column is the cumulative total of cases in a certain area as of the specified date.

<em>Privacy rules in effect</em>
To protect privacy, certain rules are in effect:
1. Any area with a cumulative case count less than 10 are dropped for all days the cumulative count was less than 10. These will be null values.
2. Once an area has a cumulative case count of 10 or greater, that area will have a new row of case data every day following.
3. Cases are dropped altogether for areas where acs_population < 1000
4. Deaths data are not included in this dataset for privacy reasons. The low COVID-19 death rate in San Francisco, along with other publicly available information on deaths, means that deaths data by geography and day is too granular and potentially risky. Read more in our <a href="https://data.sfgov.org/COVID-19/COVID-19-Data-Tracker-Publishing-Privacy-Guideline/9aj4-um47">privacy guidelines</a>

<em>Rate suppression in effect where counts lower than 20</em>
Rates are not calculated unless the cumulative case count is greater than or equal to 20. Rates are generally unstable at small numbers, so we avoid calculating them directly. We advise you to apply the same approach as this is best practice in epidemiology.

<em>A note on Census ZIP Code Tabulation Areas (ZCTAs)</em>
ZIP Code Tabulation Areas are special boundaries created by the U.S. Census based on ZIP Codes developed by the USPS. They are not, however, the same thing. ZCTAs are areal representations of routes. Read how the Census develops ZCTAs on their website.

<em>Rows included for Citywide case counts</em>
Rows are included for the Citywide case counts and incidence rate eve
