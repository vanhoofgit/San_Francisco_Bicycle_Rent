# San Francisco Bicycle Rent
![sf](https://user-images.githubusercontent.com/60714369/93361786-88d03600-f845-11ea-92cb-ab212e7e6974.jpg)

**1) Motivation** </br>
The jupyter notebook tries to find patterns in the bicycle rentals in San Francisco and present the findings with some matplotlib and seaborn charts.</br>
</br>
**2) Libraries** </br>
The following libraries need to be installed : </br>
import numpy as np </br>
import pandas as pd </br>
import matplotlib.pyplot as plt </br>
import matplotlib.ticker as ticker </br>
%matplotlib inline </br>
import seaborn as sb </br>
import glob </br>
from math import radians, cos, sin, asin, sqrt</br>
</br>

**3) Upload Files**</br>
This document explores a dataset containing information (duration, location, time, user type) about 1.8 m bike rentals in San Francisco in 2018.
The upload files are 12 monthly csv files. The original files can be found here :
https://s3.amazonaws.com/baywheels-data/index.html </br>
</br>
<br>
**4)Summary of Findings** </br>
In the exploration I found that: </br>
- The vast majority of the trips (95%) have a duration of half an hour or less. In that
group the most frequent is a trip that takes between 6 and 7 minutes.</br>
- Surprisingly, October is the top month for Baywheels, even better than the summer
months. This high rental is not due to a specific event in October but is high during the whole month October. Unsurprisingly, in January the activity is the lowest. The lowest week is the week of Thanksgiving.</br>
- When you look at the rentals on specific days, the midweek days (Tue-Thu) are the busiest, followed by Monday and Friday. Sunday is the least busy day.</br>
- Most of the rents starts with the start (8-9 am) and the end (5 pm – 6pm) of the business hours. </br>
- 75% of the trips are 2km or less long. The vast majority drives from point A to B (whatever time that my take). Only 3% delivers the bicycle at the same station they took it from.</br>
- There are two types of users with a different rental pattern: Subscribers and Customers (non-subscribers, casual). The subscribers are by far the biggest group (85%).</br>
## Key Insights for Presentation
For the presentation, I focus on :
- The impact of the day on the rental start hours. During weekend the start hours of the
bicycle rentals are not the same. They tend to be very low in the morning and have their maximal frequency between 12 pm and 4 pm.</br>
- User of type Subscriber and Customers (occasional rental) don't have the same daily rental frequency. The users of type Customer are the lowest on Mondays and gradually increase to a peak on Saturday. Then there is a drop from Saturday to Sunday and a sharper drop from Sunday to Monday. The rental by users of type 'Subscriber' are the highest on Tuesday and Wednesday and the lowest on Sunday.
 The weekend rentals come to an end at 4 am, while on weekdays, the activity starts between 4am
 and5am.Both type of days have a two hours break but this break is two hours later on weekends.</br>
 
- The different driving behavior of users of type Subscribers and Customers , especially on the shorter time frames of the duration of the trip (max half an hour). The link between duration and distance of the trip is stronger for the Subscriber. This means the Subscriber takes more a bicycle to drive from point A to B. The user of type Customer takes relatively more a bicycle to explore the neighborhood.

