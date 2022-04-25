# PyBer Exploratory Analysis

## Background
A ride-sharing app service named PyBer was investigating how to:
1.) improve access to ride-sharing services and 
2.) determine affordability for underserved neighborhoods.
They requested my assistance as a data analyst to conduct an exploratory analysis providing supportive data visualization that specifically investigated the relationship between the type of city (Urban, Suburban, and Rural), and the number of drivers and riders, as well as the percentage of total fares, riders and drivers by type of city.  They provided two CVS files.  One csv shared city data including the city names, the city type, and the driver count.  The second csv file shared ride data including the city name, date of ride, the fare, and ride id.  The two files were merged to combine the data
## Purpose
An additional request came in after the initial exploratory analysis to create a summary of the ride-sharing data by city type and create a multiple-line graph that shows the total weekly fares for each city type, to help provide insight into how the data differs by city type and how those differences can be used by decision-makers at PyBer.

## Skills, Tools & Competencies Used and Demonstrated
 - Utilize csv files, Python, Jupyter Notebook, Pandas, and Github
  - Utilize NumPy and SciPy statistics to determine mean, median, and mode.
 - Graph data using Matplotlib library and using the object-oriented approach to create: line, bar, scatter, bubble, pie, and box-and-whisker plots.
 - Modify features of charts including, adding annotations such as informative titles, axes labels, legends, and custom colors and adding error bars to line and bar charts.

## Results:
### 

    Deliverable 1: A Ride-haring usmmary DataFrame (by city type)
## 
![Pyber_Summary_DF_formated_for_Deliverable1_this file can be found in C:\Users\tligh\Documents\MSU\Challenges\PyBer_Analysis\Pyber_Deliverable1_pyber_summary_df.PNG](https://github.com/Tara-Lightner/PyBer_Analysis/blob/main/Pyber_Deliverable1_pyber_summary_df.PNG)

### Discussion:
Total Rides
- The total rides by city type in order from highest to lowest were: Urban 1,625, Suburban 625, and Rural 125.  Note, the total order of rides (Urban, Suburban, and Rural) naturally make sense with population density.
##
Total Drivers
- The total drivers by city type in order from highest to lowest were: Urban 2,405, Suburban 490, and Rural with 78. 
  - Note, the order of total 
drivers are in the same order as total rides, which again makes sense with population density.
  - Another consideration to investigate.  There are more total drivers than rides in the Urban area.  Why is this?  What is the relationship between drivers and rides?
  -If riders to drivers were a ratio of 1 to 1, this would follow the same pattern.  Assuming drivers, do multiple rides I believe it would make sense that the number of total drivers should be greater than the total number of rides.  As one can see there are significantly more urban drivers than rides.  This means that even if every driver provided only one ride, there are still 780 drivers that did not provide a single ride for over a full quarter.  One possibility is that there are many part-time drivers.  
  This drives a few additonal questions to invistigate in with additional data: 
  - What is the ride-to-driver ratio?
  - - Urban:     1,625:2,405 
  - - Suburban:  645:490     
  - - Rural:     125:78      
  - How many rides the a driver average?
  - Is their a correlation with drivers and rides?
##
Total Fare
- The total fares by city type in order from highest to lowest were:  Urban with $39,854.38, Suburban with $19,356.33, and Rural with $4,327.93.  Again, this follows the same order.
##
Average fare per ride
- The average fare per ride by city type in order from highest to lowest was: Rural with $34.66, Suburban with $30.97, and Urban with $24.53.  
  - Note, that the average fare per ride is in the inverse order from total rides, total drivers, and total fares.  Assuming the pricing is the same, this is likely because due to logistics rural locations are more spread out than suburban and suburban more spread out than urban.  If the locations for drivers are more spread out and require more milage, the average price would reflect this.  
##
Average fare per driver
- The average fare per driver by city type in order from highest to lowest was: Rural with $55.49, Suburban with $39.50, and Urban with $16.57.  Note, that this follows the same pattern trend as average fare per ride.  

Total rides, total drivers, and total fares are highest in urban, then suburban, and lastly rural cities.  The inverse is true for the average fare per ride and the average fare per driver, as rural is the highest followed by suburban and then urban cities.
### Deliverable 2: A of total fares for each city type

    Total Fares by City Type multiple-line chart 
## 
![Total_Fare_by_City_Type_for_Deliverable2_this file can be found in C:\Users\tligh\Documents\MSU\Challenges\PyBer_AnalysisPyber\Total_Fare_by_City_Type.PNG](https://github.com/Tara-Lightner/PyBer_Analysis/blob/main/Total_Fare_by_City_Type.PNG)
# Summary:
When looking at this chart I do not see that Urban, Suburban, and Rural cities follow the same line pattern.  It might be interesting if provided further dates to see if there are trends over time for each individual city type.  One can see as previously noted that Urban, Suburban, and Rural are in order from highest to lowest total fare by city over the 2019 first quarter.  The third week of February does share one peek at all three of the city types.  Urban and Suburban seem to have a greater span on fare whereas rural seems to be more consistent within a range of $0 - $500.  Whereas Urban and Rural look like fares that range closer to $1,000.  

## Further Discussion Before Recommendations: 
With the data provided, we might be able to make rudimentary assumptions about the disparities among the city types, however, that was not the purpose that PyBer stated the ultimately wanted.
If the purpose is as explained, too:
 - 1.) improve access to ride-sharing services and 
 - 2.) determine affordability for underserved neighborhoods.
 ##
The specifications PyBer requested in this analysis may not best, or at least fully, helpful in making decisions that align with their current purpose statements for this analysis.

   To mirror their purpose statements for this analysis in question form, I might ask:
 - 1.) How can PyBer improve access to ride-sharing services? 
 - 2.) Are prices affordable for underserved neighborhoods? 

 For purpose objective 1, I would also ask:
    - 1.) What is access?  
    -  A.) As a company how does PyBer want to define access?
  - Is it for every ride request that there is someone available?  
  - Has PyBer investigated inquiries for rides that were not scheduled or not able to be scheduled to a lack of available drivers?
      - B.) What is access regarding the data provided?
With the data provided, for anyone wanting or desiring services there would be two possible obstacles in the way 1.) Was a driver available and 2.) Was the customer willing and able to pay the price of the fare?  The data is limited in the fact that we know that there are a certain number of drivers within a city, but we have no knowledge if they were available within the time frame they were needed. 
      - C.) What is access regarding the data that PyBer may have data for?
One would hope if there was other relevant information to the analysis it would already be provided.  But that is not always the case.  For example, does PyBer have a list of all api calls made to the server to look up a ride vs. the rides that were scheduled, what time did they occur, and how many drivers were on shift then. Is there a pattern to when the call is being made and not resulting in rides?  If they are not resulting in rides were drivers available?  How far away was the driver? What was the estimated price for the driver?
      - C.) What is access regarding data that PyBer might be able to collect in the future?
 - What is ride-sharing services?
      - What is ride-sharing services regarding the data provided?
      - What is ride-sharing services regarding the data that
 - What are underserved neighborhoods?
 - What is affordability (for the underserved neighborhoods)  

## Recommendations: 

1.) Create an agreed-upon evaluation plan, for the future, that includes, key questions, and definitions such as access, underserved, and affordability.  This should answer the purpose of why PyBer is looking into the information and how they plan on using it.  Then a much more powerful and appropriate analysis can be run to make decisions.  With a good plan, they can even utilize their app to gather more pertinent information.  For example, if someone looks up a ride but doesn't choose to execute it maybe have a three-button survey option to click out.
2.) Rerun the analysis at the city level including the number of drivers and riders, as well as the percentage of total fares, riders, and drivers by city.
   - Why? PyBer wanted to know this at the neighborhood level, yet they requested this information at the city type level.  Although the current data provided only goes down the city level, this would still help provide additional insight and get closer to the drill-down level of the neighborhood.  I recommend reusing the script and adjusting it to grouping by cities within city types as well as cities by bins. I'm not sure if PyBer is limited in making an intuitive due to the business structure in which they can only focus resources on making changes to one city type.  However, if they are not limited, it might be better to look per city, to see where there might be gaps asking the same question as to the city type analysis.
3.) Check if there is even a relationship between rides and drivers.
Why?  We could look at the data and assume a.) If the ratio of drivers to rides is key in improving access, then Suburban and Rural cities may want to more closely reflect a higher ratio like Urban cities, in which PyBer makes more money.  However, as previously noted the number of drivers should be further investigated regarding this data set. We could also assume b.) As rural cities have the highest ride fares, this might be an indication that the affordability of PyBers service might be a barrier to clientele.
But is there an actual relationship?

## Challenges and Difficulties Encountered

- What can you conclude about the Outcomes based on Goals?
I am honestly not sure what I can conclude except some general trends and not anything I'd want to decide without further information.
- What are some limitations of this dataset?
They provided a data range from Jan 1- to May 8th.  However, I'm not sure why it wouldn't be at least on an even quarter or month marker.  So when we do run something like the line chart they are not in sync with the previous analysis.  It was never explicitly stated that the fare was the out-of-pocket price, but that was my assumption.  Driver ID would have been helpful, and customer ID, also neighborhood-level drill down. 



