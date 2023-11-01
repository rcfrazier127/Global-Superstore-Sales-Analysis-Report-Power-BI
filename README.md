# Global Superstore Sales Analysis and Forecasting Report in Power BI

### Introduction

This Sales Analysis and Forecasting report is designed to provide a comprehensive overview of sales data, product performance, shipping analysis, profit vs loss, and predictive analytics for future sales.

### Data Preparation

The Global Superstore Dataset did not require extensive preparation, aside from standardization of formatting and removal of irrelevant columns.

<img width="841" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/2257799d-eb07-4e89-b3f8-5c0c1fb99573">

The column profiling shows no instance of errors and all data within the dataset is 100% valid with no blanks, mismatches, or irrelevant data.

### Data Model

<img width="954" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/6427709b-9b32-4e88-a6d3-ce04b8c50063">

A simple Star Schema format was used to model the data in Power BI. This model contains a central fact table titled "Sales" in addition to "Product", "Orders", "Customer", and a custom "Date" table as dimensions. Separate sales measures, KPI card measures, and forecasting measure tables are also included.

## Report Pages

The Global Superstore Sales Analysis and Forecasting Report consists of the following pages:

### Title Page

<img width="1519" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/bd283504-3e88-4d43-b7a8-41c320fadd71">

An introduction to the report with a brief description of its purpose. This page includes interactive buttons that bring the user to the corresponding report pages.

### Summary

<img width="1518" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/ef7cfa31-68bc-4214-bbef-d912032efba9">

Provides a high-level overview of sales, customer, and product data, and performance metrics. TopN countries, customers, and products by sales, total products, and product profit ratios are showcased. In each page of this report, there is included a selection of slicers that allow filtering of the data and visualizatons by Product Category/Sub Category, Country, Customer Segment, Year, and Quarter. Custom KPI scorecards were created to display the % difference between the current selected year and the prior year's data for that specific card. These custom cards are featured in report pages where those metrics are relevant to the analyses contained within the page. Slicer reset buttons are also included at the top corner of each report page.

### Sales Analysis

<img width="1518" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/c8a52943-a10b-4284-96ba-d9aaf9d5d836">

Provides a detailed view of sales, profit, and % of sales over time, sales growth rates, and sales performance metrics in a tablular and graphical view.

### Product Performance

<img width="1518" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/325c1fda-a609-4c0a-8e9c-ea7d6b6498f9">

Shows information about individual product performance and profitability. This page features tabular and graphical product data, product category time-series analyses, and a scatter plot visual which allows for the quick identification of excelling or underperforming products.

### Shipping Analysis

<img width="1518" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/0d28c500-2a50-4138-b6e8-a2ad2103c54a">

Provides a view of shipping cost and order volume by market divisions, country, and shipping mode. The scatter plot allows for identification of product outliers by total units shipped and total shipping cost. This page also displays time series analyses for monthly order volumes.

I wanted this page to feature a more detailed view of lead times by markets, countries, and shipping mode, but due to how the data was generated in the creation of this public dataset, each of these totals amount to the same exact values across each value within the market, country, and shipping mode columns. If this were not so, then there possibly would have been an opportunity to create an additional page that extended the analysis of shipping data, thus providing the level of detail that I originally intended for this project.

### Profit vs. Loss

<img width="1518" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/3aa84111-cdbf-40c1-a709-4645e7d41535">

An overview of profit margins and cost analysis. Displays time series trends and monthly profit/cost comparisons. Featured in this report page is a waterfall chart displays a breakdown of monthly costs by market.

### Sales Insights

<img width="1518" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/ef3f7db4-ff4f-4976-92b9-e22095678baf">

The decomposition visual in this report page allows for deeper ad-hoc analysis and enables users to conduct root cause analysis across mutliple dimensions. 

### Forecast (2015)

<img width="1518" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/a0cafcca-75e7-4b1d-94b4-8bfbca89966c">

Provides predictive analytics based on future sales, profit, costs, and profit ratio %. Displays historical sales data to compare previous trends to forecasted sales values. The time series forecasting visuals provide a short-term projection of both sales and profit while the stacked bar visual displays a comprehensive, medium-term forecast of sales, profit, and costs. KPI cards also show % change between the current and forecasted years.

### Anomaly Detection

<img width="1518" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/5271c74e-1ddb-4941-a7ff-52eb8f54e817">

This page offers a fully interactive visual to closely examine sales anomalies between different sales years. This allows for users to identify when sales peaked during specific periods of time. Clicking on the orange indicators returns a detailed overview on the right-hand side of the report page that delivers the user further insights behind the selected anomaly.

### Geographic Map

<img width="1519" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/c606da98-03b7-4dde-afa7-6ecb3fabff9f">

A geospatial overview displaying sales, product, cost, shipping data, and profitability by countries and regions globally.
