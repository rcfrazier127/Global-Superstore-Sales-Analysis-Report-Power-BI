# Global Superstore Sales Analysis and Forecasting Report in Power BI

### Introduction

This Sales Analysis and Forecasting report is designed to provide a comprehensive overview of sales data, product performance, shipping analysis, profit vs loss, and predictive analytics for future sales.

### Data Preparation

The Global Superstore Dataset did not require extensive preparation, aside from standardization of formatting and removal of irrelevant columns.

<img width="841" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/2257799d-eb07-4e89-b3f8-5c0c1fb99573">

The column profiling shows no instance of errors and all data within the dataset is 100% valid with no blanks, mismatches, or irrelevant data.

### Data Model

<img width="1018" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/35a542f5-6648-4794-aaa5-a203dacc19cc">

A simple Star Schema format was used to model the data in Power BI. This model contains a central fact table titled "Sales" in addition to "Product", "Orders", "Customer", and a custom "Date" table as dimensions. Separate sales measures, KPI card measures, and forecasting measure tables are also included.

## Report Pages

The Global Superstore Sales Analysis and Forecasting Report consists of the following pages:

### Title Page

<img width="1560" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/7bf3ef26-5d17-4a2a-84bd-4465311a3b18">

An introduction to the report with a brief description of its purpose. This page includes interactive buttons that bring the user to the corresponding report pages.

### Summary

<img width="1575" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/4d95200d-b329-495d-b3a1-cb4e4883427b">

Provides a high-level overview of sales, customer, and product data, and performance metrics. TopN countries, customers, and products by sales, total products, order volume, and product profit ratios are showcased. In each page of this report, there is included a selection of slicers that allow filtering of the data and visualizatons by Product Category/Sub Category, Country, Customer Segment, and Year. Custom KPI scorecards were created to display the % difference between the current selected year and the prior year's data for that specific card. These custom cards are featured in report pages where those metrics are relevant to the analyses contained within the page. Slicer reset buttons are also included at the top corner of each report page.

### Sales Analysis

<img width="1575" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/c9059be9-a7b7-41f9-86a3-3134fb2422b8">

Provides a detailed view of sales, profit, and % of sales over time, sales growth rates, and sales performance metrics in a tablular and graphical view.

### Product Performance

<img width="1575" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/b90c8303-98ca-49dd-a596-0493a156cdba">

Shows information about individual product performance and profitability. This page features tabular and graphical product data, product category time-series analyses, and a scatter plot visual which allows for the quick identification of excelling or underperforming products.

### Shipping Analysis

<img width="1575" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/b3f7d9ec-c407-40fa-bd9e-0d64bc3c5c4b">

Provides a view of shipping cost and order volume by market divisions, country, and shipping mode. The scatter plot allows for identification of product outliers by total units shipped and total shipping cost. This page also displays time series analyses for monthly order volumes.

I wanted this page to feature a more detailed view of lead times by markets, countries, and shipping mode, but due to how the data was generated in the creation of this public dataset, each of these totals amount to the same exact values across each value within the market, country, and shipping mode columns. If this were not so, then there possibly would have been an opportunity to create an additional page that extended the analysis of shipping data, thus providing the level of detail that I originally intended for this project.

### Profit vs. Loss

<img width="1575" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/3a6dc3fc-b724-4b88-ac67-6584b5999d69">

An overview of profit margins and cost analysis. Displays time series trends and monthly profit/cost comparisons. Featured in this report page is a waterfall chart displays a breakdown of monthly costs by market.

### Sales Insights

<img width="1433" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/4f2c8b3c-1d4b-4ec1-8066-8ce095ef027b">

The decomposition visual in this report page allows for deeper ad-hoc analysis and enables users to conduct root cause analysis across mutliple dimensions. 

### Sales Forecast (2015)

<img width="1433" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/bd75273a-c537-4b67-8ec3-e3371ff6c1f3">

Provides predictive analytics based on future sales, profit, costs, and profit ratio %. Displays historical sales data to compare previous trends to forecasted sales values. The time series forecasting visuals provide a short-term projection of both sales and profit while the stacked bar visual displays a comprehensive, medium-term forecast of sales, profit, and costs. KPI cards also show % change between the current and forecasted years.

### Anomaly Detection

<img width="1433" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/bb961949-263a-4c63-89b8-ef367c6a907d">

This page offers a fully interactive visual to closely examine sales anomalies between different sales years. This allows for users to identify when sales peaked during specific periods of time. Clicking on the orange indicators returns a detailed overview on the right-hand side of the report page that delivers the user further insights behind the selected anomaly.

### Geographic Map

<img width="1575" alt="image" src="https://github.com/rcfrazier127/Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/4a92bd25-eab0-4380-9d88-e44e7c0b47c8">

A geospatial overview displaying sales, product, cost, shipping data, and profitability by countries and regions globally.
