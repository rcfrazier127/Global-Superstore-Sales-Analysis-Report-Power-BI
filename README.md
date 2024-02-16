# Sales Performance Report in Power BI

### Introduction

This Sales Performance Report is designed to provide a comprehensive overview of key performance indicators, sales data, product performance, and order and shipping analysis.


### Data Preparation

The publically available Superstore Sales Dataset did not require extensive preparation, aside from standardization of formatting and removal of irrelevant columns.

<img width="841" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/2257799d-eb07-4e89-b3f8-5c0c1fb99573">

The column profiling shows no instance of errors and all data within the dataset is 100% valid with no blanks, mismatches, or irrelevant data.


### Data Model

<img width="1214" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/b9e92d50-a3e4-425e-9563-04e341457ab5">

A simple Star Schema format was used to model the data in Power BI. This model contains a central fact table titled "Sales" in addition to "Product", "Orders", "Customer", and a custom "Date" table as dimensions. Separate sales measures, KPI card measures, layered donut chart measures, and product metric selection measure tables are also included.


## Report Pages

The Sales Performance Report consists of the following pages:

_Note: This report includes a page navigation pane and clear active filters button on each page._


### Executive KPIs

<img width="1528" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/41af3910-e6ad-48f8-a154-f9012aa42384">

Provides a comprehensive overview of organizational sales performance with key performance indicators to monitor the following metrics: sales, profit, profit ratio %, units sold, shipping cost, and average sales. The trends for the current year are measured against the prior year and custom KPI card visuals reflect the nominal and percent difference between the compared years. The Lines/Bars bookmark navigator allows for toggling between the display of lines and bars in the card visuals to allow the user to choose how to compare performance trends.

<img width="1528" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/e697d849-69f6-4bf7-91b5-9df44b4598c9">


### Sales Overview

<img width="1528" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/430498c1-baa8-4f26-a158-6584fb9ad064">

Provides a detailed view of categorical sales data and trends across customer segments, product categories, and market divisions. Segment and Category performance is compared using a custom multi-layered donut chart, providing an engaging visual that disrupts the frequency of which bar charts are used. A date granularity bookmark breaks down the sales trend visuals to allow for detailed comparisons. The Visuals/Details bookmark navigator brings the user to a tabular view displaying additional sales details.

<img width="1528" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/d72ab8ff-ce0f-47ab-b72b-b80cff6637a9">


### Product Analysis

<img width="1528" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/4b278bea-549f-431f-98c0-df6c00e0add3">

Provides sales data for individual product performance and profitability. This page features a bar column visual with a slicer that allows for the dynamic filtering of sales metrics between individual products and produxt subcategories. A scatter plot also shows the profitability of product subcategories. This is the only page that uses tooltips, which update dynamically as the user filters between sales metrics. This was accomplished with the use of dynamic title names to accurately reflect details for the metric being currently viewed. The bookmark navigator above brings the user to a tabular visual that displays additional product performance details.

<img width="1528" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/3e1ea021-d461-4214-a2ef-0bdec5679928">


### Order Insights

<img width="1528" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/ca159d2d-e5c8-49ba-b117-795a520f3614">

Provides a detailed view of order volume and shipping cost and by product subcategory, monthly trends, order priority, and shipping mode. The page's main feature is a matrix heat map with accompanying vertical and horizontal bar charts that simultaneously display volume by month and subcategory, which identifies how demand varies between various months. There was very little variance between shipping days across market divisions and countries within this dataset so a detailed analysis of this area was not conducted. The bookmark allows the user to view order volume in nominal and percentage format in addition to shipping cost across all visuals on this page.

<img width="1528" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/d6fc065d-2c35-4a7e-91fe-93caf686dd0e">

<img width="1528" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/b904de2e-b6b0-4e90-872c-b56c9410c74b">

