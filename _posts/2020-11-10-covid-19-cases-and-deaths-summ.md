---
title: COVID-19 Cases and Deaths Summarized by Geography
created: '2020-11-10T16:56:56.015609'
modified: '2020-12-04T19:35:19.216807'
state: active
type: dataset
tags: []
groups:
  - Local Government
csv_url: 'https://data.sfgov.org/api/views/tpyr-dvnc/rows.csv?accessType=DOWNLOAD'
json_url: 'https://data.sfgov.org/api/views/tpyr-dvnc/rows.json?accessType=DOWNLOAD'
layout: post

---
<strong>A. SUMMARY</strong>
Medical provider confirmed COVID-19 cases and confirmed COVID-19 related deaths in San Francisco, CA aggregated by several different geographic areas and normalized by 2018 American Community Survey (ACS) 5-year estimates for population data to calculate rate per 10,000 residents.

Cases and deaths are both mapped to the residence of the individual, not to where they were infected or died. For example, if one was infected in San Francisco at work but lives in the East Bay, those are not counted as SF Cases or if one dies in Zuckerberg San Francisco General but is from another county, that is also not counted in this dataset.

Dataset is cumulative and covers cases going back to March 2nd, 2020 when testing began. It is updated daily.

Geographic areas summarized are:
1. <a href="https://data.sfgov.org/Geographic-Locations-and-Boundaries/Analysis-Neighborhoods/p5b7-5n3h">Analysis Neighborhoods</a>
2. <a href="https://data.sfgov.org/Geographic-Locations-and-Boundaries/Census-2010-Tracts-for-San-Francisco/rarb-5ahf">Census Tracts</a>
3. <a href="https://www.census.gov/programs-surveys/geography/guidance/geo-areas/zctas.html">Census Zip Code Tabulation Areas</a>

<strong>B. HOW THE DATASET IS CREATED</strong>
Addresses from medical data are geocoded by the San Francisco Department of Public Health (SFDPH). Those addresses are spatially joined to the geographic areas. Counts are generated based on the number of address points that match each geographic area. The 2018 ACS estimates for population provided by the Census are used to create a rate which is equal to ([count] / [acs_population]) * 10000) representing the number of cases per 10,000 residents.

<strong>C. UPDATE PROCESS</strong>
Geographic analysis is scripted by SFDPH staff and synced to this dataset each day.

<strong>D. HOW TO USE THIS DATASET</strong>
<em>Privacy rules in effect</em>
To protect privacy, certain rules are in effect:
1. Case counts greater than 0 and less than 10 are dropped - these will be null (blank) values
2. Death counts greater than 0 and less than 10 are dropped - these will be null (blank) values
3. Cases and deaths dropped altogether for areas where acs_population < 1000

<em>Rate suppression in effect where counts lower than 20</em>
Rates are not calculated unless the case count is greater than or equal to 20. Rates are generally unstable at small numbers, so we avoid calculating them directly. We advise you to apply the same approach as this is best practice in epidemiology.

<em>A note on Census ZIP Code Tabulation Areas (ZCTAs)</em>
ZIP Code Tabulation Areas are special boundaries created by the U.S. Census based on ZIP Codes developed by the USPS. They are not, however, the same thing. ZCTAs are areal representations of routes. <a href="https://www.census.gov/programs-surveys/geography/guidance/geo-areas/zctas.html">Read how the Census develops ZCTAs on their website</a>.

<em>Row included for Citywide case counts, incidence rate, and deaths</em>
A single row is included that has the Citywide case counts and incidence rate. This can be used for comparisons. Citywide will capture all cases regardless of address quality. While some cases cannot be mapped to sub-areas like Census Tracts, ongoing data quality efforts result in improved mapping on a rolling bases.
