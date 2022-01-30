# PyBer_Analysis
## Overview of the PyBer analysis
We are a new data analyst at the Pyber, a ride sharing company. Our first task is to preform some emploratory analysis on some ride share data from 2019. The CEO loves looking at visualizations, so we will be using matplotlib to create these. 
There are 3 city types that we will be looking at: Rural, Suburban and Urban. Amongst these 3 city types we will be looking at the following areas:
1. Total Rides
2. Total Drivers
3. Total Fares
4. Average Fare per Ride
5. Average Fare per Driver
6. Total Fare by City Type over the four months of data

## Resources
- Data Sources: city_data.csv, ride_data.csv
- Software: Jupyter Notebook (python, pandas, matplotlib, dataframe_image), VS Code

## Results
The next 5 sections will refer to this table:

![Chart](/Analysis/pyber_summary_df.png)


### Total Rides by City Type
The rural city type has the fewest total rides with 125. Suburban had the second most, and urbran was first, they had 5 times and 13 times as many rides as rural respectively. This is to be expected as the urban city types tend to have a higher population density than the rural and suburban areas.  

### Total Drivers by City Type
Total drivers folows the same trend as total rides. Rural has the fewest drivers and urban has the most. Urban has almost 31 times as many drivers as rural and suburban has almost 5 times as many drivers as rural. It isn't surprising that urban has the most drivers. They have the most rides and the biggest population, so it stands to reason that they would have the most drivers. What is suprising is that the average driver only had .67 rides during this time period. Whereas rural average 1.6 rides/driver and suburban averaged 1.3 rides/driver.This could use a little further analysis. 

### Total Fares by City Type
This follows the trend of total rides. Rural is in third place with $4,327.93 of total fares during the time period. Suburban was in the middle with 4.5 times more fares than rural and urban was the leader with 9.2 times the fares of rural. The one thing that stands out is that urban had 13 times more rides than rural but only 9.5 times the fares. We will look at this in the next section.

### Average Fare per Ride
This is the reverse of the first three section. Urban is last averaging $24.53 fare per ride. Suburban is still in the middle averaging 26% higher average fares per ride than urban and rural is 41% higher. After some thought, this makes logical sense. Urban city types tend to have a higher density of places of interest. This would result in short commutes and less average fare per trip. Being in the rural areas, there is less that is close by so the average trip would be longer thus increase average fare. I would like to look into ride duration and ride mileage to confirm these ideas. 

### Average Fare per Driver
Urban is in third place averaging $16.57 per driver. Suburban drivers average fare is about   2.4 times than urban and rural is 3.3 times higher. Urban fare per driver is so low when compared to others because of two reasons: urban fare per ride is the lowest pluse the average rides/driver is less than 1 which would cause an even lower rate. 

### Total Fare by City Type over the four months of data
Chart per the insturctions 

![Chart](/Analysis/PyBer_fare_summary.png)

Chart that matches what is in the challenge

![Chart](/Analysis/PyBer_fare_summary-edited.png)

The first chart runs the PyBer data from dates 2019-01-01 : 2019-04-29, per the instructions in the code that we were given

![Chart](/Analysis/instructions.png)

The second chart was created to match what is in the challenge. To do this, I used code

```
date_type_jan_apr_pivot = date_type_summary_pivot.loc['2019-01-01':'2019-04-28']
```
