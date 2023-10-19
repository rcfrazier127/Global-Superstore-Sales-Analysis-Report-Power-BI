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

A simple Star Schema format was used to model the data in Power BI. This model contains a central fact table titled "Sales" in addition to "Product", "Orders", "Customer", and a custom "Date" table as dimensions. A separate measures table is also included.

<img width="889" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/076e712f-7a8a-4dbc-932f-09490438baf7">

## Report Pages

The Global Superstore Sales Analysis and Forecasting Report consists of the following pages:

### Title Page

An introduction to the report with a brief description of its purpose. This page includes interactive buttons that bring the user to the corresponding report pages.

<img width="1545" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report/assets/63532077/0e027dc0-6347-4272-9e30-a8a7f55b01ee">

### Summary

Provides a high-level overview of sales, customer, and product data, and performance metrics. TopN countries, customers, and products by sales, sales % growth, and product profit ratios are showcased. In each page of this report, there is included slicers that allow filtering of the data and visualizatons by Product Category/Sub Category, Region, Customer Segment, Year, and Quarter. There is also a slicer reset button on the top right of each page.

<img width="1575" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/1704df7c-199f-4eb1-bb8b-a4db7d3b1287">

### Sales Analysis

Provides a detailed view of sales insights, growth rates, and pertinent sales performance metrics in a tablular and graphical view.

<img width="1575" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/a96328d9-f0f5-42c0-96f7-0a3be73c24e4">

### Product Performance

Shows information about individual product performance and profitability. This page features tabular and graphical product data, product category time-series analyses, and a scatter plot visual which allows for the quick identification of excelling or underperforming products.

<img width="1545" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report/assets/63532077/07b9d5d1-804a-4d91-8752-2ecc84cf87d1">

### Shipping Analysis

Provides a view of shipping cost and order volume by market divisions and shipping mode. The scatter plot allows for identification of product outliers by total units shipped and total shipping cost. This page also displays trend lines for monthly order volumes by shipping mode. 

I wanted this page to feature a more detailed view of lead times by markets, countries, and shipping mode, but due to how the data was generated in the creation of this public dataset, each of these totals amount to the same exact values across each value within the market, country, and shipping mode columns. If this were not so, then there possibly would have been an opportunity to create an additional page that extended the analysis of shipping data, thus providing the level of detail that I originally intended for this project. 

<img width="1545" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report/assets/63532077/fd2fe07c-9aff-4fec-9fe0-09f771e4e1d6">

### Profit vs. Loss

An overview of profit margins and cost analysis. Displays time series trends and monthly sales/cost comparisons. Featured in this report page is a waterfall chart displays a breakdown of monthly costs by market.

<img width="1545" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report/assets/63532077/a5391b83-f724-45f1-b59a-e429a7b6aa80">

### Sales Decomposition

The decomposition visual in this report page allows for deeper ad-hoc analysis and enables users to conduct root cause analysis across mutliple dimensions. 

<img width="1545" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report/assets/63532077/c75a6aec-454c-47ad-8b53-8ee0156403de">

### Forecasting

Provides predictive analytics based on future sales and profit. Displays historical sales data to compare previous trends to forecasted sales values.

<img width="1575" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/9927efdb-5e38-4e57-9499-edd92df32b40">

### Geographic Map

A geospatial overview displaying sales, product, cost, shipping data, and profitability by countries and regions. The fictitious organization this dataset emulates possesses a substantial international presence which justified the showcasing of a detailed geographic map in this report. 

<img width="1575" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/d7a0e768-8285-4a3c-b0a7-5431c5eabae2">

## Future Works

Currently in production is a customer details page featuring graphical and tabular customer data including an analysis of customer lifetime value and churn rates.
