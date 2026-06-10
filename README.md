# Power BI Dashboard Project – Mexican Restaurant Reviews

## Overview

Academic project completed as part of the **Big Data Technologies** course. The project focuses on analyzing customer reviews and restaurant attributes using **Power BI**, enabling data-driven insights into customer satisfaction, restaurant performance, and operational trends.

### Key Contributions

* Designed and developed an interactive **Power BI dashboard** by integrating data from multiple sources.
* Utilized **Power Query** for data cleaning, transformation, and preparation.
* Created advanced **DAX measures** and calculated columns for business analysis.
* Developed **6 interactive reports** featuring drill-down capabilities, slicers, filters, KPIs, and ranking metrics.
* Analyzed customer ratings and restaurant characteristics to identify trends that support operational decision-making.

---

# Data Dictionary

## Ratings Table

### Columns

| Column Name   | Description                                                                                                |
| ------------- | ---------------------------------------------------------------------------------------------------------- |
| OverallRating | Overall customer rating for the restaurant (0 = Unsatisfactory, 1 = Satisfactory, 2 = Highly Satisfactory) |
| FoodRating    | Customer rating of food quality (0 = Unsatisfactory, 1 = Satisfactory, 2 = Highly Satisfactory)            |
| ServiceRating | Customer rating of service quality (0 = Unsatisfactory, 1 = Satisfactory, 2 = Highly Satisfactory)         |

### Measures

| Measure          | Description                                        |
| ---------------- | -------------------------------------------------- |
| AvgOverallRating | Average overall rating across all customer reviews |
| AvgFoodRating    | Average food rating across all customer reviews    |
| AvgServiceRating | Average service rating across all customer reviews |
| NoOfRatings      | Total number of ratings submitted by customers     |

---

## Restaurants Table

### Columns

| Column Name    | Description                                                                                 |
| -------------- | ------------------------------------------------------------------------------------------- |
| RestaurantID   | Unique identifier for each restaurant                                                       |
| Name           | Restaurant name                                                                             |
| City           | City where the restaurant is located                                                        |
| Latitude       | Geographic latitude of the restaurant                                                       |
| Longitude      | Geographic longitude of the restaurant                                                      |
| AlcoholService | Indicates whether the restaurant serves no alcohol, wine & beer, or offers a full bar       |
| SmokingAllowed | Indicates whether smoking is permitted (including bar areas or designated smoking sections) |
| Franchise      | Indicates whether the restaurant is part of a franchise                                     |
| Parking        | Indicates parking availability (None, Yes, Public, Valet, etc.)                             |

### Measures

| Measure        | Description                                                                                                                                                                               |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| HasAlcohol     | Converts AlcoholService into a binary value (1 = Alcohol Available, 0 = No Alcohol)                                                                                                       |
| HasParking     | Converts Parking availability into a binary value (1 = Parking Available, 0 = No Parking)                                                                                                 |
| SmokingArea    | Converts SmokingAllowed into a binary value (1 = Smoking Allowed, 0 = Not Allowed)                                                                                                        |
| CompositeScore | Composite performance score calculated using average ratings (overall and food ratings) along with operational attributes such as alcohol service, parking, and smoking area availability |
| RestaurantRank | Ranking of restaurants based on CompositeScore                                                                                                                                            |

---

## Dashboard Features

* Customer Satisfaction Analysis
* Food and Service Performance Tracking
* Restaurant Ranking System
* Geographic Restaurant Distribution Analysis
* Operational Feature Comparison (Alcohol Service, Parking, Smoking Areas)
* Interactive Drill-Down Reports and KPI Monitoring

## Tools & Technologies

* **Power BI**
* **Power Query**
* **DAX (Data Analysis Expressions)**
* **Data Modeling**
* **Business Intelligence & Data Visualization**

## Outcome

The dashboard provides actionable insights into restaurant performance, customer preferences, and operational characteristics, helping stakeholders identify top-performing restaurants and areas for business improvement.
