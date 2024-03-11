# For the fully interactive Power BI report, please view my portfolio on https://www.novypro.com/profile_projects/ryanfrazier
-----------------------------------------------------------------------------------------------------------------------------

# Sales Performance Report in Power BI

### Introduction

This Sales Performance Report is designed to provide a comprehensive overview of key performance indicators, sales data, product performance, and order and shipping analysis.


### Data Preparation

The publicly available Superstore Sales Dataset did not require extensive preparation, aside from standardization of formatting and removal of irrelevant columns.

<img width="841" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/2257799d-eb07-4e89-b3f8-5c0c1fb99573">

The column profiling shows no instance of errors and all data within the dataset is 100% valid with no blanks, mismatches, or irrelevant data.


### Data Model

<img width="1188" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/ca2f8d71-8920-4c93-94a7-1d26b0f092b3">

A simple Star Schema format was used to model the data in Power BI. This model contains a central fact table titled "Sales" in addition to "Product", "Orders", "Customer", and a custom "Date" table as dimensions. Separate sales measures, KPI card measures, layered donut chart measures, and product metric selection measure tables are also included.


## Report Pages

The Sales Performance Report consists of the following pages:

_Note: This report includes a page navigation pane and clear active filters button on each page._



### Executive KPIs

<img width="1557" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/a193f923-90b0-4ec4-b985-394cefc4f14b">

Provides a comprehensive overview of organizational sales performance with key performance indicators to monitor the following metrics: sales, profit, profit ratio %, units sold, shipping cost, and average sales. The trends for the current year are measured against the prior year and custom KPI card visuals reflect the nominal and percent difference between the compared years. The Lines/Bars bookmark navigator allows for toggling between the display of lines and bars in the card visuals to allow the user to choose how to compare performance trends (_See below_).

<img width="1557" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/f6ee94db-bbba-41bc-8c72-56a87bb95f74">



### Sales Overview

<img width="1557" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/4bb37254-b566-4f6b-bc8c-41ce6184e116">

Provides a detailed view of categorical sales data and trends across customer segments, product categories, and market divisions. Segment, Market, and Product Category performance is compared against the previous sales year with a native overlapping clustered bar chart. A date granularity bookmark breaks down the sales trend visuals to allow for detailed comparisons. The Visuals/Details bookmark navigator brings the user to a tabular view displaying additional sales details (_See below_).

<img width="1557" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/eccb122b-eb1c-4973-8d7f-5feadfd80272">



### Product Analysis

<img width="1557" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/7620885a-a112-4fd8-a7a5-319f19eb4413">

Provides sales data for individual product performance and profitability. This page features a bar column visual with a slicer that allows for the dynamic filtering of sales metrics between individual products and produxt subcategories. A scatter plot also shows the profitability of product subcategories. This is the only page that uses tooltips, which update dynamically as the user filters between sales metrics. This was accomplished with the use of dynamic title names to accurately reflect details for the metric being currently viewed. The bookmark navigator above brings the user to a tabular visual that displays additional product performance details (_See below_).

<img width="1557" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/e4e8bca9-43c9-4d88-aae9-05836abc3bc9">



### Order Insights

<img width="1557" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/1a354356-02ac-4168-a3dc-6c5430cc718d">

Provides a detailed view of order volume and shipping cost and by product subcategory, monthly trends, order priority, and shipping mode. The page's main feature is a matrix heat map with accompanying vertical and horizontal bar charts that simultaneously display volume by month and subcategory, which identifies how demand varies between various months. There was very little variance between shipping days across market divisions and countries within this dataset so a detailed analysis of this area was not conducted. The bookmark allows the user to view order volume in nominal and percentage format in addition to shipping cost across all visuals on this page (_See below_).

Percentage View:
<img width="1557" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/1990dfef-fc38-4c18-a758-388c6f4a8bac">


Shipping Cost View:
<img width="1557" alt="image" src="https://github.com/rcfrazier127/Sales-Performance-Report-Power-BI/assets/63532077/22bc7129-9c99-4029-b798-e1b107a4ff47">

