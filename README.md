# Meal Kit Delivery Service Analysis using Power BI

## Summary
In this project, I used Power BI to provide an overall analysis of the performance of a fictional meal kit delivery service.

## Data Model
Data was imported from a number of `.csv` files. Using PowerQuery, I cleaned and formatted the data, including joining multiple files to create the Payments table. I also generated a Calendar table to be used for time-dependent analyses. I connected tables where appropriate to create the Data Model seen in the image below:
<img width="1218" alt="Data Model" src="https://github.com/nwferreri/meal-kit-delivery-powerbi/assets/112211174/ecd1b120-425b-494a-8cc5-7c167ef68b02">


## Measures
I used DAX to calculate a wide array of measures to analyze the data. Some were used solely for EDA prior to developing the final dashboards. Broadly speaking, the measures fell into the following categories:
* Averages (ex. Avg Review, Avg Shipping Days)
* Counts (ex. # Meal Kits, # Shipments)
* Percentages (ex. % of Total Meal Kits, Within LSA %)
* Rankings (ex. State Shipping Rank)
* Revenue (ex. Total Revenue, Projected Revenue)
* Time-Based (ex. Revenue Previous Month, # Shipments - 3 Month Average)

## Dashboards
I created two interactive dashboards with various visualizations to provide end users with an overview of the company's performance. They can be seen below, along with notes about the functionality of each. The dashboards can be updated with new data when it is added to the data model.

### Summary Dashboard
![Oodles of Noodles- Summary Dashboard](https://github.com/nwferreri/meal-kit-delivery-powerbi/assets/112211174/d794f802-c9a8-41ae-a33a-92c345b4c271)
This dashboard gives a high level overveiw of the company's performance, and has the following features:
* Current and Projected Revenue - The sliders to the left of this visual allow users to set a timeframe and growth rate to project revenue into the future.
* \# of Shipments by Subscription Plan - The tooltip in this visual will show revenue for each subscription plan.
* Revenue by Division - Users can right click on a division to drill through to the second dashboard, focused in on the selected division.
* Bookmarks - I included 3 bookmarks on the upper left to quickly display projected revenue for a few different time horizons.

### Division Detail Dashboard
![Oodles of Noodles - Division Detail Dashboard](https://github.com/nwferreri/meal-kit-delivery-powerbi/assets/112211174/669adc93-10be-42da-a2fc-7e56c992300d)
This dashboard can be reached by drilling through the Summary Dashboard's Revenue by Division chart. It shows additional details focused on the selected division.
* Users can change the bar chart using the slicer options above it. (This is accomplished using a dynamic measure that harvests the slicer selection.)
* Revenue by Start of Month - The right side of this chart forecasts revenue 6 months into the future.

### Mobile Dashboards
In addition to the desktop dashboards, I also created mobile-friendly versions that allow at-a-glance access to the most important visualizations.

<img width="318" alt="mobile1" src="https://github.com/nwferreri/meal-kit-delivery-powerbi/assets/112211174/61d4f8df-43e5-4812-9bdc-a85e65d6b080">
<img width="311" alt="mobile2" src="https://github.com/nwferreri/meal-kit-delivery-powerbi/assets/112211174/92a54190-b73e-4756-87e6-e0e4afa63ca1"><br>
<img width="314" alt="mobile3" src="https://github.com/nwferreri/meal-kit-delivery-powerbi/assets/112211174/fe0909a6-fffe-43ee-8a31-22253a124f93">
<img width="311" alt="mobile4" src="https://github.com/nwferreri/meal-kit-delivery-powerbi/assets/112211174/17d5aab1-8790-4fc6-a98b-fcac6ed0b825">
