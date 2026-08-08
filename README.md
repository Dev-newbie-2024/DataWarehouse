#  Data Warehouse and Analytics Project

Welcome to my **Data Warehouse and Analytics Project**! 🚀

This project is developed as part of my learning in **SQL, Data Engineering, Data Warehousing, ETL, Data Modeling, and Data Analytics**.

The main goal of this project is to understand how raw data can be collected, cleaned, transformed, stored in a data warehouse, and finally used to generate useful business insights.

---

##  Project Architecture

For this project, I followed the **Medallion Architecture**, which consists of three layers:

###  Bronze Layer – Raw Data

The Bronze layer stores the data in its original form.

* Data is collected from CSV files.
* ERP and CRM datasets are loaded into SQL Server.
* No major transformations are performed at this stage.
* The purpose is to keep the original source data available.

###  Silver Layer – Cleaned Data

The Silver layer is used for cleaning and preparing the data.

Some of the tasks performed include:

* Removing incorrect or duplicate data
* Handling missing values
* Standardizing data formats
* Correcting data types
* Cleaning and transforming columns
* Combining data from different sources

###  Gold Layer – Business Data

The Gold layer contains the final data that can be used for analysis and reporting.

Here, the data is organized using a **Star Schema** with:

* Fact tables
* Dimension tables

This makes it easier to write analytical SQL queries and generate business insights.

---

##  Project Objectives

The main objectives of this project are:

1. Build a simple data warehouse using **SQL Server**.
2. Load data from ERP and CRM CSV files.
3. Clean and transform the raw data.
4. Combine data from different sources.
5. Design a suitable data model using a **Star Schema**.
6. Create SQL queries for analyzing the data.
7. Generate useful insights about customers, products, and sales.
8. Document the complete data warehouse process.

---

##  ETL Process

The project follows an ETL process:

**Extract → Transform → Load**

### 1. Extract

The data is collected from the provided ERP and CRM CSV files.

### 2. Transform

The raw data is cleaned and transformed.

For example:

* Handling null values
* Removing duplicates
* Standardizing values
* Converting data types
* Checking data quality
* Joining related datasets

### 3. Load

After transformation, the processed data is loaded into the appropriate tables in the data warehouse.

The overall flow is:

```text
ERP CSV Files ──┐
                ├──> Bronze Layer ──> Silver Layer ──> Gold Layer
CRM CSV Files ──┘                                      │
                                                       ↓
                                                SQL Analytics
                                                       │
                                                       ↓
                                                  Business Insights
```

---

##  Data Modeling

For the Gold layer, I used a **Star Schema**.

The Star Schema contains:

### Fact Tables

Fact tables contain measurable business information such as:

* Sales
* Quantity
* Revenue
* Customer transactions

### Dimension Tables

Dimension tables provide descriptive information such as:

* Customer
* Product
* Date

The purpose of using a Star Schema is to make analytical queries easier and more efficient.

---

##  Analytics

After building the data warehouse, SQL queries are used to analyze the data.

The analysis mainly focuses on:

###  Customer Analysis

Some questions I can answer are:

* Who are the most valuable customers?
* How much has each customer spent?
* How many orders has each customer made?
* Which customers are most active?

###  Product Analysis

Examples include:

* Which products are selling the most?
* Which products generate the highest revenue?
* Which product categories perform better?
* How does product performance change over time?

###  Sales Analysis

The project can also be used to analyze:

* Total sales
* Monthly sales
* Sales trends
* Revenue by product
* Revenue by customer
* Sales performance over time

---

##  Tools and Technologies

The main tools used in this project are:

* **SQL Server** – Database and Data Warehouse
* **SQL** – Data transformation and analysis
* **SSMS** – Database management
* **Git & GitHub** – Version control
* **Draw.io** – Architecture and data model diagrams
* **CSV** – Source data

---

##  What I Learned

While working on this project, I learned about:

* Data Warehousing
* ETL processes
* Medallion Architecture
* Bronze, Silver, and Gold layers
* Data Cleaning
* SQL transformations
* Star Schema
* Fact and Dimension tables
* Data Modeling
* Data Quality
* Analytical SQL queries
* Git and GitHub

This project helped me understand how data moves from **raw source files to useful business information**.

---

##  Future Improvements

In the future, I would like to improve this project by adding:

* Automated ETL pipelines
* Apache Airflow for workflow orchestration
* Python-based data processing
* Data quality checks
* Power BI or Tableau dashboards
* Automated data validation
* Cloud data warehouse integration

---

##  Conclusion

This project helped me gain practical experience with the complete process of building a data warehouse.

Starting with raw **ERP and CRM data**, I learned how to clean, transform, model, and analyze the data using SQL Server.

The main goal is to turn raw data into meaningful information that can support **better business decision-making**.

---

##  About This Project

This is a **student learning project** created to improve my practical knowledge of **SQL, Data Engineering, Data Warehousing, and Data Analytics**.

I am continuously improving the project and adding new technologies as I learn them.
