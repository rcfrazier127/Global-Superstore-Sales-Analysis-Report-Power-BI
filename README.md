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

<img width="894" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/a207d482-2b3c-4193-9112-04f1da964681">

A simple Star Schema format was used to model the data in Power BI. This model contains a central fact table titled "Sales" in addition to "Product", "Orders", "Customer", and a custom "Date" table as dimensions. A separate measures table is also included.

## Report Pages

The Global Superstore Sales Analysis and Forecasting Report consists of the following pages:

### Title Page

An introduction to the report with a brief description of its purpose. This page includes interactive buttons that bring the user to the corresponding report pages.

<img width="1575" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/00dd5cba-5c62-4fc3-975f-135359f7b3ec">

### Summary

<img width="1531" alt="image" src="https://github.com/rcfrazier127/Global-Superstore-Sales-Analysis-Report-Power-BI/assets/63532077/5e6bbd1c-ecc7-44b6-a70b-8b7dad1b2435">

Provides a high-level overview of sales, customer, and product data, and performance metrics. TopN countries, customers, and products by sales, total products, and product profit ratios are showcased. In each page of this report, there is included a selection of slicers that allow filtering of the data and visualizatons by Product Category/Sub Category, Country, Customer Segment, Year, and Quarter. Custom KPI scorecards were created to display the % difference between the current selected year and the prior year's data for that specific card. These custom cards are featured in report pages where those metrics are relevant to the analyses contained within the page. Slicer reset buttons are also included at the top corner of each report page.

### Sales Analysis

<img width="1531" alt="image" src="https://github.com/rcfrazier127/Global-Superstore-Sales-Analysis-Report-Power-BI/assets/63532077/ddad9d27-5f83-4116-8787-e4581fcbcf76">

Provides a detailed view of sales insights, growth rates, and pertinent sales performance metrics in a tablular and graphical view.

### Product Performance

<img width="1531" alt="image" src="https://github.com/rcfrazier127/Global-Superstore-Sales-Analysis-Report-Power-BI/assets/63532077/28e68458-5032-4f0c-9f40-cfe96e5709df">

Shows information about individual product performance and profitability. This page features tabular and graphical product data, product category time-series analyses, and a scatter plot visual which allows for the quick identification of excelling or underperforming products.

### Shipping Analysis

<img width="1531" alt="image" src="https://github.com/rcfrazier127/Global-Superstore-Sales-Analysis-Report-Power-BI/assets/63532077/83699821-f6dc-4524-9e62-e274516f2093">

Provides a view of shipping cost and order volume by market divisions, country, and shipping mode. The scatter plot allows for identification of product outliers by total units shipped and total shipping cost. This page also displays time series analyses for monthly order volumes.

I wanted this page to feature a more detailed view of lead times by markets, countries, and shipping mode, but due to how the data was generated in the creation of this public dataset, each of these totals amount to the same exact values across each value within the market, country, and shipping mode columns. If this were not so, then there possibly would have been an opportunity to create an additional page that extended the analysis of shipping data, thus providing the level of detail that I originally intended for this project.

### Profit vs. Loss

<img width="1532" alt="image" src="https://github.com/rcfrazier127/Global-Superstore-Sales-Analysis-Report-Power-BI/assets/63532077/a24a7fe5-12af-463a-be3d-cbff985a3358">

An overview of profit margins and cost analysis. Displays time series trends and monthly profit/cost comparisons. Featured in this report page is a waterfall chart displays a breakdown of monthly costs by market.

### Sales Insights

<img width="1575" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/6aeb8b38-cd45-4170-b024-7d0f0e9ffe1a">

The decomposition visual in this report page allows for deeper ad-hoc analysis and enables users to conduct root cause analysis across mutliple dimensions. 

### Forecasting

<img width="1531" alt="image" src="https://github.com/rcfrazier127/Global-Superstore-Sales-Analysis-Report-Power-BI/assets/63532077/f508f124-4959-4bed-9e65-a36bffb65b8a">

Provides predictive analytics based on future sales and profit. Displays historical sales data to compare previous trends to forecasted sales values. The Yearly Sales Trend visual includes a slicer to filter by sales year only for this visual.

### Geographic Map

<img width="1575" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/c41b69a6-f747-46de-b3e8-59c485c8d1a7">

A geospatial overview displaying sales, product, cost, shipping data, and profitability by countries and regions. The fictitious organization this dataset emulates possesses a substantial international presence which justified the showcasing of a detailed geographic map in this report. 
