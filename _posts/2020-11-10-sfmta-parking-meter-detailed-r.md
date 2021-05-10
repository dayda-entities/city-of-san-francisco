---
title: SFMTA Parking Meter Detailed Revenue Transactions
created: '2020-11-10T16:56:39.886967'
modified: '2020-12-04T19:34:12.228021'
state: active
type: dataset
tags: []
groups:
  - Local Government
csv_url: 'https://data.sfgov.org/api/views/imvp-dq3v/rows.csv?accessType=DOWNLOAD'
json_url: 'https://data.sfgov.org/api/views/imvp-dq3v/rows.json?accessType=DOWNLOAD'
layout: post

---
Parking meter transaction records where each row equals a single transaction by a single customer at a single meter. Subsequent transactions by a customer to extend time, for example, are captured as new transaction record and indicated with a METER_EVENT_TYPE of AT (Additional Time).

POST_ID is a join key that refers to the identifier for a meter. You can find that inventory including location of the meter here: https://data.sfgov.org/d/8vzz-qzz9
