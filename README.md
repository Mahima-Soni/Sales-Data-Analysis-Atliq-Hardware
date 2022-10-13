# Sales-Data-Analysis-Atliq-Hardware
This is a case study project where I’ve simulated as a data analyst to leverage business problem solution to a hardware company in India.

## AtliQ Hardware
- Is a company which supplies computer hardware and peripherals to many clients across India;
- The company has a head office in Dehli and regional offices throughout India.

## Business Problem
To unlock Sales Insights that are not visible before for sales team for decision support & automate them to reduced time spend in data gathering.

## Solution:
Create a simple and informative dashboard about the company sales.

I used **SQL** queries in **MySQL Workbench** to take a look into the data and **Power BI** for **ETL** and visualizations to create the insights.
Overview

After a quick data exploration in MySQL, here are some initial findings:
-The database contains 5 tables: **customers**, **date**, **markets**, **products**, and **transactions**;

-There are **17 markets, 279 products, and 38 customers**;

-The observation period is from **january 2018 to june 2020**;

-The total revenue in 2020 was INR 142,23 M, 42% less than 2019, which was  INR 336,45 M;

-Most of the transactions data are in **INR currency**, but we have 4 records in **USD currency**.

-And we got **Paris** and **New York** on the **“sales markets”** table. We’re going to deal with it in the ETL process.
    
## ETL (Extract, Transform, Load)

**Data Modeling Step**
We got five tables and we need to ensure that the tables are correctly connected.

![Modelling](https://user-images.githubusercontent.com/91668225/183046123-af16c8f9-54c2-4602-821d-56c1ff0bec91.png)

**[sales transactions]** — Fact table

TABLES CONNECTED
- sales customers > connected by “**customer_code**” column;
- sales date> connected by “**date**” column;
- sales products > connected by “**product_code**” column;
- sales markets > connected by **“market_code**” column.

I have made three Dashboards named - Revenue Analysis ,Profit Analysis and Performance insights for tracking profit and revenue of the company.

The Insights contains -
-Revenue by Markets

-Sales Quantity by Markets

-Profit Margin by Markets

-Profit trend by Year

-Revenue by Year

-Top 5 Customers by Profit and Revenue

-Top 5 Products by Profit and Revenue

![Screenshot (193)](https://user-images.githubusercontent.com/91668225/183050633-5aff0feb-b692-49cf-88df-d7f57bebc051.png)

![Screenshot (195)](https://user-images.githubusercontent.com/91668225/183050682-69e6de05-132a-49a7-85ea-2d47c9c2213d.png)

![Screenshot (194)](https://user-images.githubusercontent.com/91668225/183050661-a5a6e1a0-de0f-4152-9368-f266155a8c3b.png)

## Recommendations 
Based on the dashbaords insights, I have made some recommendation that Sales Marketing team should/can -

-consider making a sales strategy for especially **lucknow** since its showing **lowest revenue and negative profit margin** and if possible so as for **Surat** and **Bhubhaneshwar** also.

-try to **increase its sales quantity** in **Patna**, **Surat** and **Kanpur** since they have lowest sales quantity.

-start their target campagin for **Prod047** and **Prod061** since they two are the **most profitable and most selling** products.

-try to **give special benefits** to **Electronics** and **_Excel store_s** as they are their **most profitable customers**.

-make their **campgain strategy for mid year** as they are showing high sales among other months.





