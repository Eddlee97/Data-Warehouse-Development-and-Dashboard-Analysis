# Data Warehouse Development and Business Intelligence Dashboard Analysis

### Project Idea & Goal:

Identify how Airbnb revenue factors generated by Citibike traffic/usage. Does more Citibike stations in New York City make an Airbnb rental more attractive and lucrative to their customers, and how can Airbnb generate more revenue based on Citibike traffic/usage? Which areas in New York City contains the most Citibike traffic/usage, and how can they contribute values to Airbnb in post-pandemic season?

The goal is this project is to analyze these questions will help Airbnb have a better understanding on which areas should they promote more/less to overcome its post-pandemic financial stress and how can they generate more revenues efficiently.
  
### Project Idea & Goal:

According to Airbnb earnings in Q4. The company posted an enormous loss in the fourth quarter of 2020 as it suffered from the pandemic downturn and revenue has dropped 30% in 2020 compared to previous year. To effectively solve this issue, we want to understand the correlation between Airbnb listings revenue and the Citibike traffic/usage in New York City. The opportunity may arise based on our findings in this project which will allow Airbnb to potentially understand lucrative rental locations and hot zones that may bring profits to the company.

### Data Sources:

Main: Airbnb rentals data (New York City only) | http://insideairbnb.com/get-the-data.html

Secondary: Citibike trip data (New York City only) | https://ride.citibikenyc.com/system-data

### Tools Used:

***Documentation: Google Word Doc <br>
Data Modeling: Lucid Chart <br>
ETL Transformation: Python, Jupyter Notebook <br>
Data Warehouse Cloud: Google BigQuery <br>
Business Intelligence Dashboard: Tableau***

### Business Requirements Definition

***List of Data Warehouse KPI's:***
1. Citibike Usage per Location (Jan 2021 + Feb 2021)
2. Ratings per Location - Frequent Visits (Top 15)
3. Total Revenue per Location based on Citibike Traffic
4. Average Price per Night Visit based on Citibike Traffic
5. Rentals Generated based on Citibike Trips (# of Rentals vs Citibike Trips) per Location

### Dimensional Model

***This is the original model, however, we optimized and finalized it in python during the ETL process which only has 1 fact & 3 dimensions***

![dim](https://github.com/Eddlee97/Data-Warehouse-Development-and-Dashboard-Analysis/blob/ecd5939a6bb77e1c25460df3cfdfa27fdc29290c/Milestone%20%232%20-%20Dimensional%20Model/Dimensional%20model.png)

### Business Intelligence Dashboard Design and Development

**BI Application Wireframe design:**

![Alt text](https://github.com/Eddlee97/Data-Warehouse-Development-and-Dashboard-Analysis/blob/ecd5939a6bb77e1c25460df3cfdfa27fdc29290c/Milestone%20%234%20-%20BI%20Dashboard/BI%20wireframe%20design.png)

### Final Dashboard

![Alt text](https://github.com/Eddlee97/Data-Warehouse-Development-and-Dashboard-Analysis/blob/ecd5939a6bb77e1c25460df3cfdfa27fdc29290c/Milestone%20%234%20-%20BI%20Dashboard/Overview%20of%20NYC%20Airbnb%20Rentals%20Revenue%20with%20Citibike%20Usage%20(CIS%209440).png)

***Analysis Description for each Chart:***

- **Citibike Usage per Location (Jan 2021 + Feb 2021)** <br>
   - Treemap was used to effectively compare the number of Citibike trips per location by differentiate them with total amount and color <br>
   - Filtered the top 15 locations in terms of Citibike traffic <br>
   - The amount difference and color allow audience to easily understand the most visited locations in NYC

![dim](https://github.com/Eddlee97/Data-Warehouse-Development-and-Dashboard-Analysis/blob/d4f875180529e79f66ef1c5b6969efa140d67f19/Milestone%20%234%20-%20BI%20Dashboard/Chart/1.png)

- **Ratings per Location - Frequent Visits (Top 15)** <br>

   - Horizontal bar plot was used to display the average review scores of Airbnb per location, sort them in descending order <br>
   - Filtered the top 15 locations in terms of Citibike traffic <br>
   - Changed x-axis to 4.5 to 5, which show a clear difference in all ratings of the top 15 locations <br>
   - This allow audience to view a clear rating difference, and Airbnb executive can make business decision based on this ratings 
 
![dim](https://github.com/Eddlee97/Data-Warehouse-Development-and-Dashboard-Analysis/blob/d4f875180529e79f66ef1c5b6969efa140d67f19/Milestone%20%234%20-%20BI%20Dashboard/Chart/2.png)

- **Total Revenue per Location based on Citibike Traffic** <br>

   - Scatter plot was used with two y-axis to easily describe the relationship between the total revenue per location and the number of Citibike trips <br>
   - Filtered the top 15 locations in terms of Citibike traffic <br>
   - Left y-axis: number of citibikes trips | Right y-axis: total revenue <br>
   - This allow audience to not only look at the total revenue of all frequent visit locations, but also explain the relationship between revenue and the amount of Citibike trips in each location
   
![dim](https://github.com/Eddlee97/Data-Warehouse-Development-and-Dashboard-Analysis/blob/d4f875180529e79f66ef1c5b6969efa140d67f19/Milestone%20%234%20-%20BI%20Dashboard/Chart/3.png)

- **Average Price per Night Visit based on Citibike Traffic** <br>

   - Scatter plot was used to illustrate the average price of Airbnb per night and the amount of Citibike trips by plotting each location zipcode  <br>
   - This allow audience to glance at the overview of price for each location (by zipcode) and its relationship with Citibike traffic
   
![dim](https://github.com/Eddlee97/Data-Warehouse-Development-and-Dashboard-Analysis/blob/d4f875180529e79f66ef1c5b6969efa140d67f19/Milestone%20%234%20-%20BI%20Dashboard/Chart/4.png)

- **Rentals Generated based on Citibike Trips (# of Rentals vs Citibike Trips) per Location** <br>

   - Scatter plot was used to indicate the relationship between the number of rentals and the nuber of Citibike trips based on each location, using zipcode and neighborhood names <br>
   - Adding a trendline to the scatter plot will allow audience to easily understand that the greater the traffic/usage for Citibike, the higher the number of listings will be rented
   
![dim](https://github.com/Eddlee97/Data-Warehouse-Development-and-Dashboard-Analysis/blob/d4f875180529e79f66ef1c5b6969efa140d67f19/Milestone%20%234%20-%20BI%20Dashboard/Chart/5.png)
