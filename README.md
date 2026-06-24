# Customer_Shopping_Behavior_Analysis-using-MSSQL-EDA-Project-
Performed Exploratory Data Analysis (EDA) on retail sales data using MSSQL by analyzing customer, product, and transaction datasets. Utilized Joins, Aggregate Functions, Window Functions, and KPI reporting techniques to identify revenue trends, customer behavior, product performance, and business insights.
# Customer Shopping Behavior Analysis using MSSQL (EDA Project)

## Project Overview

This project focuses on performing Exploratory Data Analysis (EDA) on retail sales data using Microsoft SQL Server (MSSQL). The objective is to analyze customer behavior, product performance, sales trends, and business KPIs through SQL queries.

The project follows a dimensional data model consisting of:

* Fact Table: `fact_sales`
* Dimension Tables:

  * `dim_customers`
  * `dim_products`

The analysis helps business stakeholders understand customer demographics, product category performance, revenue generation, and sales distribution.

---

## Business Problem

Retail organizations generate large volumes of transactional data. However, without proper analysis, valuable insights remain hidden.

This project aims to answer key business questions:

* Who are our customers?
* Which products generate the highest revenue?
* Which categories perform best?
* What is the overall sales performance?
* How are sales distributed across countries?
* Which products are underperforming?

---

## Dataset Description

### 1. fact_sales

Contains transactional sales records.

| Column       | Description             |
| ------------ | ----------------------- |
| order_number | Unique order identifier |
| order_date   | Order date              |
| customer_key | Customer ID             |
| product_key  | Product ID              |
| quantity     | Quantity sold           |
| price        | Unit price              |
| sales_amount | Revenue generated       |

---

### 2. dim_customers

Contains customer information.

| Column       | Description         |
| ------------ | ------------------- |
| customer_key | Customer ID         |
| first_name   | Customer First Name |
| last_name    | Customer Last Name  |
| gender       | Gender              |
| birthdate    | Date of Birth       |
| country      | Customer Country    |

---

### 3. dim_products

Contains product information.

| Column       | Description         |
| ------------ | ------------------- |
| product_key  | Product ID          |
| product_name | Product Name        |
| category     | Product Category    |
| subcategory  | Product Subcategory |
| cost         | Product Cost        |

---

# Analysis Performed

## 1. Database Exploration

### Objectives

* Explore all available tables.
* Identify column structures.
* Understand data model relationships.

### Queries Used

* INFORMATION_SCHEMA.TABLES
* INFORMATION_SCHEMA.COLUMNS

---

## 2. Dimension Exploration

### Customer Analysis

* Distinct customer countries

### Product Analysis

* Product categories
* Product subcategories
* Product names

### Business Value

Helps understand customer distribution and product portfolio.

---

## 3. Date Exploration

### Analysis Performed

* First order date
* Last order date
* Total operational period

### Customer Age Analysis

* Youngest customer
* Oldest customer

### Business Value

Provides historical coverage and customer demographic insights.

---

## 4. KPI & Measure Analysis

### Key Metrics Calculated

* Total Sales
* Total Quantity Sold
* Average Selling Price
* Total Orders
* Total Products
* Total Customers

### Business Value

Provides an executive-level business performance overview.

---

## 5. Magnitude Analysis

### Customer Insights

* Customers by country
* Customers by gender

### Product Insights

* Products by category
* Average product cost by category

### Revenue Insights

* Revenue by category
* Revenue by customer

### Sales Distribution

* Sold items by country

### Business Value

Identifies customer segments and revenue-driving categories.

---

## 6. Product Performance Analysis

### Top Performing Products

Used:

* TOP 5
* ORDER BY Revenue DESC

### Worst Performing Products

Used:

* TOP 5
* ORDER BY Revenue ASC

### Advanced SQL

Implemented:

* ROW_NUMBER()
* Window Functions

### Business Value

Helps identify best-selling and underperforming products.

---

# SQL Concepts Used

* SELECT
* DISTINCT
* WHERE
* GROUP BY
* ORDER BY
* COUNT()
* SUM()
* AVG()
* MIN()
* MAX()
* DATEDIFF()
* JOINs
* UNION ALL
* TOP
* ROW_NUMBER()
* Window Functions
* Aggregate Functions

---

# Key Findings

1. Identified top revenue-generating products.
2. Identified lowest-performing products.
3. Analyzed customer distribution by country and gender.
4. Calculated overall business KPIs.
5. Evaluated category-wise revenue contribution.
6. Analyzed customer purchasing behavior.
7. Measured product sales performance using ranking techniques.

---

# Tools Used

* Microsoft SQL Server (MSSQL)
* SQL Server Management Studio (SSMS)
* CSV Datasets
* GitHub

---

# Future Enhancements

* Power BI Dashboard Integration
* Customer Segmentation
* RFM Analysis
* Sales Forecasting
* Cohort Analysis
* Customer Lifetime Value Analysis
