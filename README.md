# Pyber Fare Analysis
# Overview
Purpose of the analysis was to review the weekly total fares by type of city (Urban, Sururban and Rural, on a weekly basis, for a specified period of time.  The results of parsing the specified data were plotted on a multi-line graph.  The three types of cities on one in figure was performed to too showcases any difference and commonalities.


# Results
Took data - merged city and ride csv files.  Modified the dataframe by making the "date" the new index.  Created a pivot table based on the new index.  Extracted data items occuring between 1/1/1/19 through 4/29/19.  Converted the date field using "to_datetime". Using the resample() function, rearranged the fare data to sum by weeks.  Based on this final dataset, created 3 data series to of weekly fare information for the 3 city types.  

The 3 different series were plotted onto 1 figure using the df.plot() function.  Formatting was performed for readability and chart information.

The results showed the highest total fares by week was Urban city type.  The sheer number of riders and drivers would indicate the total volume would be greater, thus the higher weekly fare total.  Suburban city type came was second in ranking for overall weekly fares with the Rural type finishing last.  There were similiar spikes for all city types at the end of February.  Not enough information was provided to determine what the trigger for the spike.  One can surmise the uptick was due to Presidents Day holiday.  
Week ending: 2019-02-24	419.06	1412.74	2466.29

The week endng 2019-04-14	269.79	784.82	2390.72 show a slight dip in activity (from the previous week) across all city types, particularly in Rurall and Suburban.  One could make an assumption that the weeking leading up to April 15, tax day, was the factor for this drop.  People are not using the ride service as they're otherwise engaged in their tax return preparation.  For a detailed look at the weekly fares for each type of city is shown [here](insert url here).  For the graphical representation, please see this [chart](insert url here)

Looking at the overall weekly fares, the Rural city type is consistently lower in weekly fares than Suburban and Suburban is less than Urban.  It can be assume that those living in the Rural areas have their own transportation as the walkable rating would be low.  Conversely, those living in Urban tend to have less of their transportation as public transit is available and on top of that, the walkability rating would be high.  Suburban areas would be somewhere in the middle, being close enough to access public transportation to a commutable city, but far enough way outside of the ura
walkability rating would be low

Describe the differences in ride-sharig data among the different city types
Add url to graph link




# Summary
Provide 3 recommendations to the CEO for addressing any disparities among the city types
-promotions to drivers - bonus based on star rated reviews; number of ride exceed certain level
-promotions/discounts to riders - rush hour surcharge/low time discount
-social campaign to carpool - save the earth/economy and ecology savings


