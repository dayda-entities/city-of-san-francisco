---
title: Dwelling Unit Completion Counts by Building Permit
created: '2020-11-10T16:56:40.694110'
modified: '2020-11-20T17:23:06.146076'
state: active
type: dataset
tags:
  - Development
  - Housing
  - Permits
  - Residential
groups:
  - Local Government
csv_url: 'https://data.sfgov.org/api/views/j67f-aayr/rows.csv?accessType=DOWNLOAD'
json_url: 'https://data.sfgov.org/api/views/j67f-aayr/rows.json?accessType=DOWNLOAD'
layout: post

---
A. SUMMARY 

This dataset reports the number of new residential units made available for occupancy in San Francisco since January 2018. Each row in this dataset shows the change in the number of new units associated with a building permit application. Each row also includes the date those units were approved for occupancy, the type of document approving them, and their address.

Values in the column [Number of Units Certified] can be added together to produce a count of new units approved for occupancy since January 2018. 

These records provide a preliminary count of new residential units. The San Francisco Planning Department issues a Housing Inventory Report each year that provides a more complete account of new residential units, and those results may vary slightly from records in this dataset. The Housing Inventory Report is an in-depth annual research project requiring extensive work to validate information about projects. By comparison, this dataset is meant to provide more timely updates about housing production based on available administrative data. The Department of Building Inspection and Planning Department will reconcile these records with future Housing Inventory Reports.

B. METHODOLOGY 

At the end of each month, DBI staff manually calculate how many new units are available for occupancy for each building permit application and enters that information into this dataset. These records reflect counts for all types of residential units, including authorized accessory dwelling units. These records do not reflect units demolished or removed from the city’s available housing stock.

Multiple records may be associated with the same building permit application number, which means that new certifications or amendments were issued. Only changes to the net number of units associated with that permit application are recorded in subsequent records. 

For example, Building Permit Application Number [201601010001] located at [123 1st Avenue] was issued an [Initial TCO] Temporary Certificate of Occupancy on [January 1, 2018] approving 10 units for occupancy. Then, an [Amended TCO] was issued on [June 1, 2018] approving [5] additional units for occupancy, for a total of 15 new units associated with that Building Permit Application Number. The building will appear as twice in the dataset, each row representing when new units were approved.

If additional or amended certifications are issued for a building permit application, but they do not change the number of units associated with that building permit application, those certifications are not recorded in this dataset. For example, if all new units associated with a project are certified for occupancy under an Initial TCO, then the Certificate of Final Completion (CFC) would not appear in the dataset because the CFC would not add new units to the housing stock.
See data definitions for more details.

C. UPDATE FREQUENCY 

This dataset is updated monthly.

D. DOCUMENT TYPES

Several documents issued near or at project completion can certify units for occupation. They are: Initial Temporary Certificate of Occupancy (TCO), Amended TCO, and Certificate of Final Completion (CFC). 

•	Initial TCO is a document that allows for occupancy of a unit before final project completion is certified, conditional on if the unit can be occupied safely. The TCO is meant to be temporary and has an expiration date. This field represents the number of units certified for occupancy when the TCO is issued. 
•	Amended TCO is a document that is issued when the conditions of the project are changed before final project completion is certified. These records show additional new units that have become habitable since the issuance of the Initial TCO. 
•	Certificate of Final Completion (CFC) is a document that is issued when all work is completed according to approved plans, and the building is ready for complete occupancy. These records show additional new units that were not accounted for in the Initial o
