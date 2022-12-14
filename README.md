# New York City Motor Vehicle Collision Data Warehouse
- authors: Megan Lam, Felix Martinez, Parth Shah
- date created: 11/29/2022
- class: CIS 9440

Project Objective: Follow the Kimball Lifecycle to design and develop a public, cloud-based Data Warehouse with a functioning BI Applications

Project Tools:
The tools used to build this Data Warehouse were: 
1. For data integration - Jupyter Notebook
2. For data warehousing - Google BigQuery
3. For Business Intelligence - Tableau

## Kimball Lifecycle Project Stages

### Project Planning

Motivation for project:
As NYC residents that both drive and take public transportation, we were inspired to analyze collisions in the city. We wanted to explore why they occurred frequently, where they occurred, when they occurred, and which vehicles were most involved. 

Description of the issues or opportunities the project will address:
New York City is a very densely populated place with half of the households owning a car. About 27% of 3.8 million workers commute to work via van, car, or truck. Some questions that come to light are: What are some of the main reasons for vehicular crashes in a populated city? How can New York City reduce collisions through legislation? How can New York City improve their public transportation to reduce car usage? To answer these questions, the New York City Vehicle Collision Data Warehouse will aggregate collision data to uncover insights regarding New York City motor vehicle collisions.

Project Business or Organization Value:
The project aims to address the frequency of collisions in NYC. By analyzing these collisions, we can identify the key causes and hotspots for them. We will then be able to recommend strategies that will decrease the numbers of motor vehicle collisions, while increasing motor vehicle safety.  

Data Sources:
1. https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95

### Business Requirements Definition

List of Data Warehouse KPI's:
1. Number of pedestrians affected by a motor vehicle collision
2. Collisions by borough
3. Collisions by vehicle type
4. Collisions by contributing factor
5. Collisions by time of day 

### Dimensional Model

This project's Dimensional Model consists of 1 Fact and 5 Dimensions.

![NYC Motor Vehicle Collisions Dimensional Model](img/CIS9440_Group_Project_Dimensional_Model.jpg)

This project's Kimball Bus Matrix:

Use correct file path here to show picture of dimensional model...
![NYC Motor Vehicle Collisions Kimball Bus Matrix](img/CIS9440_Group_Project_Kimball_Bus_Matrix.png)

### Business Intelligence Design and Development

List of Visualizations for each KPI:
1. We chose to represent the total number of pedestrians affected by a collision through a line chart because this was a time-series analysis. We wanted to show which years had an increase or decrease of pedestrians affected. We also added a table to give the readers hard numbers to look at, paired with a map showing where pedestrians were injured in NYC to analyze the data geographically. This will give insight as to where pedestrians are most likely to be injured. 
2. To visualize collisions by borough, we opted to use a pie chart because this was a contribution analysis. We wanted to represent how much each borough contributed to overall collisions. We also chose to use a bar graph based on contributing factors that was filtered based on borough for a comparative analysis. Lastly, we included a map for a geographical analysis. 
3. In the case of collisions by vehicle type, we chose to use a bar graph because this was a comparative analysis of vehicle types. We wanted to see which of the five vehicles were most and least involved in collisions. 
4. Similar to the collisions by vehicle type KPI, for collisions by contributing factors, we chose to use a bar graph because this was a comparative analysis of total accidents by causation. We wanted to gain a better understand the distribution of the five contributing factors. 
5. Finally, for the collisions by the time of day KPI, we chose to use a bar graph because this was a comparative analysis of overall day and night accidents also categorized by vehicle types and contributing factors. Additionally, we chose to use a pie chart to show the contribution analysis of accidents during the day and night. 

BI Application Wireframe design:

![NYC Motor Vehicle Collisions BI Application Wireframe](img/CIS9440_Group_Project_Dashboard_Wireframe.png)

Pictures of final Dashboard:

![Pedestrian Involvement](img/Pedestrian_Involvement.png)

![Collisions by Borough](img/Collisions_by_Borough.png)

![Collisions by Time of Day](img/Collisions_by_Time_of_Day.png)

### Deployment

The project was deployed on Tableau Public: 
[NYC Motor Vehicle Collision Data Warehouse](https://public.tableau.com/app/profile/felix.martinez2775/viz/CIS9440-Group4-NYCMotorVehicleCollisionData/PedestrianInvolvement)
