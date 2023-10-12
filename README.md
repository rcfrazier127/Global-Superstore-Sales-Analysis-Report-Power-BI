# Global Superstore Sales Analysis and Forecasting Report in Power BI

**Introduction**

This Sales Analysis and Forecasting report is designed to provide a comprehensive overview of sales data, product performance, shipping analysis, profit vs loss, and predictive analytics for future sales.

**Data Preparation**

The Global Superstore Dataset did not require extensive preparation, aside from standardization of formatting and removal of irrelevant columns. However, the formatting for the "Order Date" and "Shipping Date" columns were a mixture of 'dd-mm-yyyy' and 'mm-dd-yyyy' formats. For whatever reason there was no way to standardize these date formats into one single format in Excel. This required a simple fix of re-parsing the data format using Python. The file displaying this fix is attached within this repository. 

Data format parsing fix with Python:

<img width="375" alt="image" src="https://github.com/rcfrazier127/Superstore-Sales-Analysis-and-Forecasting-Report/assets/63532077/4dbe322e-93dc-453a-a677-52aca7ad5792">

These are the columns in the Power Query Editor after the fix took place:

<img width="841" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/2257799d-eb07-4e89-b3f8-5c0c1fb99573">

The column profiling shows no instance of errors and all data within the dataset is 100% valid with no blanks, mismatches, or irrelevant data.

**Data Model**

A simple Star Schema format was used to model the data in Power BI. This model contains a central fact table titled "Sales" in addition to "Product", "Orders", "Customer", and a custom "Date" table as dimensions. A separate measures table is also included.

<img width="889" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/076e712f-7a8a-4dbc-932f-09490438baf7">

**Report Pages**

The Global Superstore Sales Analysis and Forecasting Report consists of the following pages:

**Title Page:** An introduction to the report with a brief description of its purpose. This page includes interactive buttons that bring the user to the corresponding report pages.

<img width="1575" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/c2d2ab13-3b7b-4133-9989-c44612de6073">

**Summary:** Provides a high-level overview of sales, customer, product, and metrics data. TopN countries, customers, and products by sales, sales % growth, and profit ratio are showcased. In each page of this report, there is included slicers that allow filtering of the data and visualizatons by Product Category/Sub Category, Region, Customer Segment, Year, and Quarter. There is also a slicer and filter reset button on the top right of each page. THe Summary Page is the only page that also includes a slicer to filter data by Market, which is the primary data focal point in many of the pages within this report. 

<img width="1575" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/1704df7c-199f-4eb1-bb8b-a4db7d3b1287">

**Sales Analysis:** 

<img width="1575" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/a96328d9-f0f5-42c0-96f7-0a3be73c24e4">

<img width="1575" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/7e08bc64-2e4d-474f-8353-cb4e5e521a45">

<img width="1575" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/780fda37-1db6-440a-a35d-e651e28f3b1f">

<img width="1575" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/ee015b70-c851-4225-8e2d-1c20f50f3b54">

<img width="1575" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/9927efdb-5e38-4e57-9499-edd92df32b40">

<img width="1575" alt="image" src="https://github.com/rcfrazier127/SuperStore-Sales-Analysis-and-Forecasting-Report-Power-BI/assets/63532077/d7a0e768-8285-4a3c-b0a7-5431c5eabae2">
