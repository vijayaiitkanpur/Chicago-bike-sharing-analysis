# Chicago-bike-sharing-analysis
Identified demographic &amp; geographical features affecting the rider behavior for a bike sharing company using Linear regression model in Python to minimize supply and demand gap of the bikes at popular stations

Problem Statement

Divvy is Chicagoland’s bike share system with 6,000 bikes available at 570+ stations across Chicago and Evanston. Divvy provides residents and visitors with a convenient, fun and affordable transportation option to explore Chicago, commute to work or school and many more. Divvy is available 24*7 and riders have access to all bikes and stations across the system.  
Divvy has decided to shut down its operation in Chicago due to Federal regulation. A new company 'Ecoride' would be launching its bike sharing business & would be replacing Divvy in Chicago. Our problem statement is to explore & analyze the customers trip behavior under different scenarios using Divvy's past 4 years data. We can help the new company analyze various factors that shapes the decision of riding a bike by customers and we can help EcoRide establish their business and minimize the supply and demand gap. 

The Objective of this Study

There are a few opportunity areas & potential customer segments that Divvy was unable to tap. We can help Ecoride identify these segments that they should focus on to increase their customer base and maximize the profits.
We are helping Ecoride to understand the bike sharing market and help them strategize a plan to minimize the gap between supply and demand of the bikes at popular stations. We also want to come up with an analysis of the past data of customers to make Ecoride understand the customer behavior and the important factors which have some major influences such as geographical conditions, customer demographics, etc.   

Data Background 

We are taking trip data from Divvy. This data is available online openly for 2013-2017. We performed basic cleaning of this dataset first (dropping null values etc.). This dataset was then loaded into Jupyter Notebook and later filtered for the year 2017 and stored in a dataframe (named "datan").  This data contains 2.9 million rows and 23 attributes. 
The original Divvy study available online was focused on answering questions like: 
•	How far do the riders go? Where do riders go? Most frequent time when they ride? 
•	The busiest pick-up & drop-off stations?
•	Which days of the week are the busiest one?


Computational Steps 

•	Data was loaded using pandas, cleaned (rows with null values were dropped) and filtered(columns that were not required were dropped) to prep it for analysis
•	We conducted an Exploratory analysis of the dataset. In this analysis we examined the following
	Number of trips by hour, day, gender, weather, temperature, usertype
	Trip duration by hour, day
•	Reducing the data size to 1% of original dataset by using Random Sampling
•	Plotting pair-plot and correlation coefficient of independent variables and extracting the relevant attributes
•	Built Single & Multi variable Linear regression models to understand the effect of attributes such as time, duration, temperature and day on number of trips & distance travelled
•	Applied K-means clustering to group the customers based on similar characteristics from the information given in the dataset
•	Calculated Distance covered for each trip using longitude & latitude of start & end points for 2.9 Million observations
•	Plotted Heatmap of the pick-up stations during peak/rush hour on the map of Chicago using Folium
•	Plotted all the unique pick-up stations on the map of Chicago using Folium
•	Plotted route maps of Top 5 pick-up stations using Folium
•	Monte Carlo Simulation of the survey conducted for onboarding more female riders
