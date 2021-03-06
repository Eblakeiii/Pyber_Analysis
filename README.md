# Pyber Fare Analysis
# Overview
Purpose of the analysis was to review the weekly total fares by type of city (Urban, Suburban and Rural, on a weekly basis, for a specified period of time.  The results of parsing the specified data were plotted on a multi-line graph.  The three types of cities on one figure was performed to showcase any differences and commonalities.

# Results
Two data files were provided, city_data.csv and ride_data.csv, for this analysis.  After checking for completeness and lack of nulls/errors, the were merged into one dataframe.  The merged dataframe was modified by making the "date" field the new index.  Reindexing allowed a pivot table, based on the new index, to be created.  Data elements, from January 1, 2019 through April 29, 2019, was extracted.  The date field/new index, in the filtered dataset, was then converted the date data type using "to_datetime" function.   Using the resample() function, rearranged the fare data to sum by weeks.  Based on this final dataset, created three data series of weekly fare information for the three city types. 

The three different series were plotted onto one figure using the df.plot() function.  Formatting was performed for readability and chart information.  

The results showed the highest total fares by week was Urban city type.  The sheer number of riders and drivers would indicate the total volume would be greater, thus the higher weekly fare total.  Suburban city type was second in ranking for overall weekly fares with the Rural type finishing last.  Please see [chart](https://github.com/Eblakeiii/Pyber_Analysis/blob/master/analysis/Pyber_fare_summary.png) for the graphical representation.

The trend for all three city types were similar, only the volume of rides/fares differed.  There were even parallel spikes, compared to the previous week, for all city types at the end of February (week ending 2019-02-24: Rural was $419.06, Suburban was $1,412.74, and Urban was $2,466.29).  Information was not provided to determine what triggered the spike.  One can surmise the uptick was due to Presidents Day holiday and people traveling to the airport.  

Fares for the week ending 2019-04-14 (Rural was $269.79, Suburban was $784.82 and Urban was $2,390.72) show a slight dip in activity, from the previous week, across all city types, particularly in Rural and Suburban city types.  One could make an assumption that the week leading up to April 15, tax day, was the factor for this drop.  People are not using the ride service as they're otherwise engaged in their tax return preparation.  

For a comprehensive chart of the weekly fares, from January 1, 2019 to April 29, 2019, for each type of city, is shown [here](https://github.com/Eblakeiii/Pyber_Analysis/blob/master/Pyber_fare_summary_Grid.png).

Looking at the overall weekly fares, the Rural city type is consistently lower in weekly fares than Suburban and Suburban is less than Urban.  It can be assume that those living in the Rural areas have their own transportation as the walkable rating would be low.  Alternativey, those living in Urban areas will opt for using public transportation as it is more readily available.  Additionally, the Urban walkability rating would be high.  Suburban areas would be somewhere in the middle, being close enough to access public transportation to a commutable city, but far enough way outside of the city limits where walkability rating would be lower.

# Summary
The weekly fare data represent the different city types ridership levels.  It shows how less rides are being taken in the areas where there is a lack of public transport, walkability is low and the majority of residents have access to a vehicle.  And conversely, ridership is higher in areas where public transportation is prevalent and walkability is high.  To help mitigate this inversely-related environment, listed below are some recommendations to promote additional drivers and riders.

### 1 Offer special monetary incentives to drivers.
- Bonus based on achieving certain number of 4 or 5 star rated reviews; 
- Bonus if driver exceeds certain number of rides;
- Bonus for working during peak hours.
    
### 2 Offer promotions/discounts to riders.
- Discount of fares during non-peak hours;
- Institute a frequent ridership program, i.e., take 5 rides, get the 6th free or reduce fare by 50%;
- Earn ride points for every ride and the points to be used for future rides or be given as gifts.
  
### 3 Conduct a social campaign.
- Carpool because it saves money and helps the environment;
- Establish relationships with to promote ridership with Pyber such as with 1) bars/restaurants; 2) doctors' offices; 3) auto mechanics and other vendors where rides would useful.
      

