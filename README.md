# Meal Kit Delivery Service Analysis with Power BI

## Summary
In this project, I use Power BI to provide an overall analysis of the performance of a fictional meal kit delivery service.

## Data Model
Data was imported from a number of `.csv` files. Using PowerQuery, I cleaned and formatted the data, including joining multiple files to create the Payments table. I also generated a Calendar table to be used for time-dependent analyses. I connected tables where appropriate to create the Data Model seen in the image below:

[Data Model Image]

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
[image of summary dashboard]
This dashboard gives a high level overveiw of the company's performance, and has the following features:
* Current and Projected Revenue - The sliders to the left of this visual allow users to set a timeframe and growth rate to project revenue into the future.
* \# of Shipments by Subscription Plan - The tooltip in this visual will show revenue for each subscription plan.
* Revenue by Division - Users can right click on a division to drill through to the second dashboard, focused in on the selected division.

### Division Detail Dashboard
[image]
This dashboard is can be reached by drilling through the Summary Dashboard's Revenue by Division chart. It shows additional details focused on the selected division.
* Users can change the bar chart using the slicer options above it. (This is accomplished using a dynamic measure that harvests the slicer selection.)
* Revenue by Start of Month - This chart forecasts revenue 6 months into the future.
