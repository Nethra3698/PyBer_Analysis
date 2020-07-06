# PyBer Analysis Report
Using Pandas, jupyter notebook and matplotlib to create an analysis for data from Pyber. 
## Background and Results

### Purpose
The analysis is conducted to produce a clear and concise picture of the data from Pyber representing only the necessary and meaningful data. Also, with just the important information can be used to create visual representations and graphs in the future. 
### Technical Analysis
The line graph and the dataframe in all gives a succinct picture of the ridesharing data while also providing a multidimensional analysis of all the city types by including the averages fares, total rides, total fares and so on. Such an analysis could even help in Pyber's future endeavours.
### Results
The summary dataframe shows the total rides, total drivers, total fares, average fares per ride and average fares per driver for each city type. Such a data frame can give a better idea about the nature of each city type and which city type performs well in certain categories. In fact, the dataframe, as seen below shows that Urban areas have more total rides, total fares, and total drivers and hence a lower average fare per ride and average fare per driver whereas this is the complete opposite in the case of Rural areas. This only goes to prove how the number of people in an area have an impact on the average fare per ride and average fare per driver. 
![Fig 1. ]( /analysis/Fig9.png)

The technical analysis also included a line graph comparing the fares and the dates for the different city types as seen below. The graph is mostly steadily fluctuating for all the three city types with Urban areas showing the most amount of total fare and Rural areas having the least, but there is a significant peak in all the values near the end of February.
![Fig 2. ]( /analysis/Fig8.png)
### Summary
The summary dataframe can be analysed in multiple ways. As mentioned before, the number of people living in the area does indirectly affect these values because of the demand but another way of looking at it is that rural areas have less number of drivers compared to urban areas due to which the price is higher in rural areas for these high in demand drivers whereas low in urban areas where drivers are abundant.
Also, the peak in the line graph could be because of an event in the analysed area due to which the demand to travel increased.
## Challenges Encountered and Overcome

### Challenges and Difficulties Encountered

* Programming
The main challenge was getting stuck while coding and not kknowing how to using particular functions. 
* Data analysis
The data analysis part was pretty difficult this time because of using new functions that we were not previously aquainted with such as resample()
* Graphing, etc
Initially, I was not sure how to plot using a data frame and was stuck with it but realized this was relatively simple once I saw the syntax. 

### Technical Analyses Used

A bunch of functions help me analyze this problem and get the output that I wanted. I used df.index.name = None when I did not want the index column name to show up. One of the most useful things I learned from this code is after I tried to merge a dataframe and series and eventually realized I could just treat the series like a column. Also, pd.pivot_table() is something I learned about during this project and found it extremely useful. Overall, I had to use a lot of stack overflow and the pandas documentation for this assignment and am really accustomed to it now. This is probably how I will find the try to solve the difficulties that I face in the future too.  

## Recommendations and Next Steps

### Recommendations for Future Analysis
Including percentages of rides, fares and drivers for each city type to the data frame would greatly change the standard of the datarame. Also, the legend of the plot could be moved to the side instead of in the center as it sits right on a line graph and this can be avoided. 

### Additional Analysis 1

* Description of Approach
Instead of doing a weekly analysis a monthly analysis can be done for the average fare in different types and they can be represnted in bar graphs 
* Technical Steps
To do this the same process as the line graph can be followed but while an mean() is used for fare instead of sum() while doing a groupby and then while using resample() we can do it by monthly. At the end, it will be plotted as a bar graph so that the comparison is easier.
### Additional Analysis 2

* Description of Approach
Similar to the line graph in this assignment, a line graph of the number of rides over the time for different city types can be plotted.
* Technical Steps
To do this, the process is similar to the Total Fare by City Type line graph. The only difference is that the No.drivers column should be considered instead of the fares column when the data frame in made initially, and the rest of the process is the same — doing a groupby the city type and the date coulumn, forming a pivot table and using resample() to form bins and them plotting to a line graph.



