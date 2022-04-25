# PyBer Exploratory Analysis
#### Files inludes in Repository:
   -  README - this file, used as Deliverable 
*********Go Back and consider how I've detected patterns, trends, correlations, and outliers
# Background
A ride-sharing app service named PyBer was investigating how to:
1.) improve access to ride-sharing services and 
2.) determine affordabililty for underserved neighboorhoods.
They requested my assistance as a data analyst to conduct an exploritory analysis providing supportive data visualization that specifically investigated the relationship between the type of city (Urban, Suburban, and Rural), and the number of drivers and riders, as well as the percentage of total fares, riders and drivers by type of city.  They provided two CVS files.  One csv shared city data including the city names, the city type and the driver count.  The second csv file shared ride data including the city name, date of ride, the fare and ride id.  The two files were merged to combine the data


# Overview of Project ****This is specifically asking for me "Explain the purpose of the new analysis."
An additional request came in after the intial exploritory analysis to create a summary of the ride-sharing data by city type and create a multiple-line graph that shows the total weekly fares for each city type, to help provide insight on how the data differs by city type and how those differences can be used by decision-makers at PyBer.

# Skills, Tools & Competencies Used and Demonstrated
 - Utilize csv files, Python, Jupyter Notebook, Pandas, and Github
  - Utilize NumPy adn SciPy statistics to determing mean, median, and mode using Pandas, NumPy, and SciPy statistics.
 - Graph data using Matplotlib library and using the object-oriented approach to create: line, bar, scatter, bubble, pie, and box-and-whisker plots.
 - Modify features of charts including, adding annotation such as, informative titles, axes labels, legends, custom colors and adding error bars to line and bar charts.

## Results:
### Deliverable 1: A ride-sharing summary DataFrame by city type

    PyBer Summary DataFrame
    ![Pyber_Summary_DF_formated_for_Deliverable1_this file can be found in C:\Users\tligh\Documents\MSU\Challenges\PyBer_Analysis\Pyber_Deliverable1_pyber_summary_df.PNG](https://github.com/Tara-Lightner/PyBer_Analysis/blob/main/Pyber_Deliverable1_pyber_summary_df.PNG)
## 


### Discussion:
Total Rides
- The total rides by city type in order from highest to lowest were: Urban 1,625, Suburban 625, and with Rural 125.  Note, the total order of rides (Urban, Suburban, and Rural) naturally make sense with population denisty.
##
Total Drivers
- The total drivers by city type in order from hightest to lowest were: Urban 2,405, Suburban 490, and Rural with 78. 
  - Note, the order of total 
drivers is in the same order as total rides, which again makes sense with population density.
  - Another consideration to look into.  There are more total drivers than rides in the Urban area.  Why is this?  What is the relationship between drivers and rides?
  -If riders to drivers were a ratio of 1 to 1, this would follow the same pattern.  Assuming drivers, do multiple rides I believe it would make sense that the numbers of total drivers should be greater than the total number of rides.  As one can see their are are siginficantly more urban drivers than rides.  This means that even if every driver provided only one ride, there are still 780 drivers that did not provide a single ride for over a full quarter.  One possibilities that there are many part time drivers.  
  - What is the ride to driver ratio?
  - - Urban:     1,625:2,405 67.67%
  - - Suburban:  645:490     131.63%
  - - Rural:     125:78      160.26%
  - What is the average ride per driver?
  - What is the driver to ride ration?
  - What is the average ride per driver?
  
  It would make sense that if you were a driver you would want to   

The relationship between drivers and ....It would also make sense with higher demand for rides that their would likely be a correlating order to meet demand.  The fact that drivers are hight
##
Total Fare
- The total fares by city type in order from hightest to lowest were:  Urban with $39,854.38, Suburban with $19,356.33, and Rural with $4,327.93.  Again this follows the same order.
##
Average fare per ride
- The average fare per ride by city type in order from highest to lowest were: Rural with $34.66, Suburban with $30.97, and Urban with $24.53.  
  - Note, the averabe fare per ride is in the inverse order from total rides, total drivers and total fares.  Assuming the pricing is the same, this is likely because due to logistics as rural location are mores spread out then suburban and suburban more spread out then urban.  If the locations for drivers are more spread out require more milage, the average price would reflect this.  
##
Average fare per driver
- The average fare per driver by city type in order from highest to lowest were: Rural with $55.49, Suburban with $39.50, and Urban with $16.57.  Note, this follows the same pattern trend as average fare per ride.  

Total rides, total drivers and total fares are highest in urban, then suburban and lastly ruaral cities.  The inverse is true for the average fare per ride and the average fare per driver, as rural is the hightest followed by suburban and then urban cities.
### Deliverable 2: A of total fares for each city type

    Total Fares by City Type multiple-line chart 
    ![Total_Fare_by_City_Type_for_Deliverable2_this file can be found in C:\Users\tligh\Documents\MSU\Challenges\PyBer_AnalysisPyber\Total_Fare_by_City_Type.PNG](https://github.com/Tara-Lightner/PyBer_Analysis/blob/main/Total_Fare_by_City_Type.PNG)
## 

## 
### Summary:

What we know from our exploritory analysis....

### Recomendations: 
for addressing any disparities among the city types
If the purpose is as explained, to:
 - 1.) improve access to ride-sharing services and 
 - 2.) determine affordabililty for underserved neighboorhoods.
 ##
The specifications Pyber requested in this analysis may not best, or at least fully, helpful in making decisions that allign with their current purpose statements for this analysis.

   To mirror their purpose statments for this analysis in question form, I might ask:
 - 1.) How can PyBer improve access to ride-sharing services? 
 - 2.) Are prices affordable for underserved neighboorhoods? 


 - For objective 1, I would also ask:
    - What is access?
      - What is access in regards to the data provided?
      - What is access in regards to the data that Pyber may have data for?
      - What is access in regards to data that Pyber might be able to collect in the future?
 - What are ride-sharing services?
      - What are ride-sharing services in regards to the data provided?
      - What are ride-sharing services in regards to the data that
 - What are underserved neighboorhoods?
 - What is affordability (for the underserved neighboorhoods)
1.) 
2.)
3.)

## Challenges and Difficulties Encountered

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
# Git Hub Files
