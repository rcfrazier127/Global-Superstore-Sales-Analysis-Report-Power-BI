# Global Superstore Sales Analysis and Forecasting Report in Power BI

### Introduction

This Sales Analysis and Forecasting report is designed to provide a comprehensive overview of sales data, product performance, shipping analysis, profit vs loss, and predictive analytics for future sales.

### Data Preparation

The Global Superstore Dataset did not require extensive preparation, aside from standardization of formatting and removal of irrelevant columns. However, the formatting for the "Order Date" and "Shipping Date" columns were a mixture of 'dd-mm-yyyy' and 'mm-dd-yyyy' formats. For whatever reason there was no way to standardize these date formats into one single format in Excel. This required a simple fix of re-parsing the data format using Python. The file displaying this fix is attached within this repository. 

*Data format parsing fix with Python:*

<img width="375" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report/assets/63532077/4dbe322e-93dc-453a-a677-52aca7ad5792">

*Columns in Power Query Editor after fix:*

<img width="841" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/2257799d-eb07-4e89-b3f8-5c0c1fb99573">

The column profiling shows no instance of errors and all data within the dataset is 100% valid with no blanks, mismatches, or irrelevant data.

### Data Model

<img width="889" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/076e712f-7a8a-4dbc-932f-09490438baf7">

A simple Star Schema format was used to model the data in Power BI. This model contains a central fact table titled "Sales" in addition to "Product", "Orders", "Customer", and a custom "Date" table as dimensions. A separate measures table is also included.

## Report Pages

The Global Superstore Sales Analysis and Forecasting Report consists of the following pages:

### Title Page

An introduction to the report with a brief description of its purpose. This page includes interactive buttons that bring the user to the corresponding report pages.

<img width="1575" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/00dd5cba-5c62-4fc3-975f-135359f7b3ec">

### Summary

<img width="1575" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/82c4e5ca-965a-42bf-b9bf-194f023c5c7b">

Provides a high-level overview of sales, customer, and product data, and performance metrics. TopN countries, customers, and products by sales, sales % growth, and product profit ratios are showcased. In each page of this report, there is included slicers that allow filtering of the data and visualizatons by Product Category/Sub Category, Region, Customer Segment, Year, and Quarter. There is also a slicer reset button on the top right of each page.

### Sales Analysis

<img width="1575" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/6d4dd347-1c0b-45d1-b4b6-9e309e8858b2">

Provides a detailed view of sales insights, growth rates, and pertinent sales performance metrics in a tablular and graphical view.

### Product Performance

<img width="1575" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/57516faf-b9df-4304-becd-7b3edd397007">

Shows information about individual product performance and profitability. This page features tabular and graphical product data, product category time-series analyses, and a scatter plot visual which allows for the quick identification of excelling or underperforming products.

### Shipping Analysis

<img width="1575" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/b4fc046d-4571-45df-b5fe-578b3faea86a">

Provides a view of shipping cost and order volume by market divisions and shipping mode. The scatter plot allows for identification of product outliers by total units shipped and total shipping cost. This page also displays trend lines for monthly order volumes by shipping mode. 

I wanted this page to feature a more detailed view of lead times by markets, countries, and shipping mode, but due to how the data was generated in the creation of this public dataset, each of these totals amount to the same exact values across each value within the market, country, and shipping mode columns. If this were not so, then there possibly would have been an opportunity to create an additional page that extended the analysis of shipping data, thus providing the level of detail that I originally intended for this project.

### Profit vs. Loss

<img width="1575" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/7346354d-405d-41e0-afc4-b3f1aeaa29b8">

An overview of profit margins and cost analysis. Displays time series trends and monthly sales/cost comparisons. Featured in this report page is a waterfall chart displays a breakdown of monthly costs by market.

### Sales Insights

<img width="1575" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/6aeb8b38-cd45-4170-b024-7d0f0e9ffe1a">

The decomposition visual in this report page allows for deeper ad-hoc analysis and enables users to conduct root cause analysis across mutliple dimensions. 

### Forecasting

<img width="1575" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/349c9742-940e-4070-aec1-1146b195d401">

Provides predictive analytics based on future sales and profit. Displays historical sales data to compare previous trends to forecasted sales values.

### Geographic Map

<img width="1575" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/c41b69a6-f747-46de-b3e8-59c485c8d1a7">

A geospatial overview displaying sales, product, cost, shipping data, and profitability by countries and regions. The fictitious organization this dataset emulates possesses a substantial international presence which justified the showcasing of a detailed geographic map in this report. 
