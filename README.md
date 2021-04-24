# DATA115 - Housing Prices
Personal Dataset

# How has the price of homes in Clark County changed over recent years? 
I have spent my whole life in Clark County and as I have gotten older I began to take notice that year over year the price of homes in the area has been increasing. So I chose to get some actual data on it and make a visualization.


# Procurement 

The University of Washington makes available housing data from all of Washington state from the years 2007 - 2020. I accessed this data set and extracted just the median resale price from the Clark County row. I did this for each quarter from 2016 to 2020 and used the entries to construct my own 20 observation dataset. 

https://wcrer.be.uw.edu/archived-reports/

# Processing
Even with a simple dataset I initially ran into issues when I imported the data to R studio, the biggest being my "Date" variable. The data was indexed in my dataset by year and quarter, so when it came time to assemble a scatterplot, using just the year would give stacks of points over each year. Concatonating the year and quarter collumns together also did not help because the new column was not numeric. So I ended up adding a new collumn to my dataset known as "Date" which is the year plus the quarter turned into a decimal. So 2016 quarter 2 became "2016.25" with 2016 being quarter 1. This allowed me to construct a scatterplot showing the change over time.





<img src="https://raw.githubusercontent.com/Brodywsuv/DATA115/main/HP.png" >

This is a simple scatterplot showing the median home resale price in Clark County WA over the course of 5 years from 2016-2020 broken up by quarter. Visualizing this data shows there is definitley linear structure in the change of price over time.
