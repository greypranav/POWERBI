<span style="font-family: Georgia;">
<SPAN STYLE="font-size:16.0pt">
<span style="line-height: 1.5em;">

****

### High Cloud Airlines Data Analysis Dashboard
* * *
**#1) Project Overview**
* * *

- This project analyzes the performance of High Cloud Airlines, a regional airline, using flight data from 2008 to 2013. The dashboard provides insights into key performance indicators (KPIs) such as load factor trends, passenger preferences, flight distances, and route popularity. The data pipeline processes raw flight data, and the results are visualized using Tableau Desktop Public Edition and Power BI.

***
**#2) Introduction**
***
* High Cloud Airlines, a regional airline, operates a fleet of 207 aircraft, serving millions
of passengers annually. This project aims to analyze the airline’s performance from 2008
to 2013, focusing on the following objectives:
  * Evaluate load factor trends over the years.
  *  Identify passenger preferences for carriers and routes.
  *  Analyze flight distribution by distance and week type.
  *  Provide actionable insights for operational improvements.
 
 ***
 ### Snapshot of Dashboard (Power BI Service) & Dashboard Link
 ***

[**Dash_Board_Link**](https://tinyurl.com/pbixexcelR)
 
![image](https://github.com/user-attachments/assets/45f4ed55-e50d-4687-b33e-e365987e3f16)

![image](https://github.com/user-attachments/assets/01ff1f13-38d3-443e-b2f8-1b28ca6906ed)


 

***
**#3) ETL Process and Modelling**
***

- We have processed and thoroughly cleaned the data using **Power Query**, handling various data quality issues including null values, inconsistent formats, and duplicate entries
- Once the data was cleaned and transformed, We used **Power Pivot to build a robust data model**. The model follows a **star schema design**,
- It cconsist of 1 fact table and 9 dimensions Table.
- This is the Data Model.

  ![image](https://github.com/user-attachments/assets/f67dbbc3-650a-4462-b648-e67c58aff710)


***
**#4) Tools Used**
***
* **Excel**: Power Query is used for ETL and Power Pivot for Data Modelling
* **SQL**: For cleaning heavy files and exporting as CSV
* **Tableau & PowerBI**: Visualisation

***
**#5) Key Perfomance Indicators**
***
***5.1_Metrics***
* * *

The analysis highlights the following aggregate metrics:
* Total Passengers: **187M**
* Transported Freight: 8B
* Transported Mail: 298M
* Total Airlines: 207

***
***5.2_Load Factor Trends***
* * *
* The load factor, a measure of operational efficiency, shows a general upward trend from 2008 to 2013, with a slight dip in 2012:

![35015c87434d2bbe9d8110892682fe47.png](:/ce78d103feac4e129a6962d7a3f4597a)

![86eaece1c7813a764520a7370edbff56.png](:/f3afd6a351ea4666b366fc39e5c5519f)

* Globespan Airways Limited, operating as Flyglobespan, leads with the highest load factor at 90.999%, reflecting excellent capacity utilization

***
***5.3_Carrier Preferences***
* * *

![157505f5452076dcf792a473acd343f2.png](:/42b6a2e2c3fc4b6e87ac76bc6b9a6b70)

* Southwest Airlines Co. leads with the highest passenger preference, serving around 35 million passengers.
* Delta Air Lines Inc. is the second most preferred, with approximately 30 million passengers.
* Smaller airlines like JetBlue and AirTran lag behind.

***
***5.4_Top Routes***
* * *

![2b10dbaf4ab1d0a4a3cb0701d9c2b432.png](:/7ca6fcc5f4d349ecb26b5ef1d6c4f2f4)

* This chart evaluates the popularity of airline routes based on the number of Airlines operating between specific city pairs
* The route "Chicago, II - Detroit, MI" has the highest count of airline IDs, approaching 100, indicating it is the most serviced route.
* The second most popular route is "Washington, DC - New York, NY," with a count slightly below 90.
* Cities like Chicago, Atlanta, Washington, DC, and New York appear frequently, indicating they are major airline hubs with high connectivity.

***
***5.5_ Load Factor by Week Type***
* * *
* This covers Weekend vs Weekday Load Factor: Analyzed how much load factor is occupied on weekends vs weekdays.
* Weekend load factors are slightly lower than weekdays, suggesting a need for targeted promotions

![91bb5ff28e0d13d8563f253f60a8e700.png](:/97eb2fcc0d1a494d902ceabacb5c10c4)

***
***5.6_Flight Distance Distribution***
* * *

![0212259937fd6e6af4624a18bc35fa67.png](:/55357327cb6e4626aa03130cf3e62a15)

* It categorizes Flights by Distance groups. It categorizes flights based on distance groups.
* The majority of flights fall into the **"Less than 500 miles"** category, as indicated by the tallest bar on the far left. This suggests that short-haul flights are the most common.
* There is a significant drop in the number of flights as the distance increases. 
* Flights with distances beyond 2000 miles are relatively rare, with only a few flights in each subsequent interval 
* The longest flights, in the "10500-11000 miles" range, are extremely rare, with very few flights recorded.

***
**#6) Insights and Conclusions**
***

- The load factor varies significantly by quarter, with Q3 showing the highest due to peak travel seasons.
- Top carriers maintain a consistent load factor, indicating efficient capacity management.
- Distance-based flight analysis reveals longer routes have lower load factors, possibly due to pricing or demand.
