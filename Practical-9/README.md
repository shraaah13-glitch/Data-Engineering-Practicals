# Practical 9 – End-to-End E-Commerce ETL Pipeline

## Aim

To build an end-to-end ETL pipeline using CSV files, Pandas, and SQLite for e-commerce data processing and reporting.

## Software Used

* Google Colab
* Python 3
* SQLite

## Technologies Used

* Python
* Pandas
* CSV
* SQLite
* SQL
* ETL

## Objective

* Create and extract historical e-commerce data from CSV files.
* Clean and transform customer, product, order, and payment data.
* Load the processed data into a SQL database.
* Generate sales and customer reports.
* Handle newly arriving data using incremental loading.
* Generate a final sales report.

## Description

This practical demonstrates an end-to-end ETL pipeline for an e-commerce dataset using Pandas and SQLite.

### Part 1 – Historical Data Creation

Historical data for customers, products, orders, and payments is created and saved as separate CSV files.

### Part 2 – Data Extraction and Cleaning

The CSV files are read using Pandas.
The data is cleaned by:

* Removing duplicate records.
* Handling missing values.
* Converting order dates into the proper date format.
* Removing invalid orders.
* Standardizing payment status values.

### Part 3 – Data Transformation

Orders are joined with product information.
The total order amount is calculated using:

```text
Total Amount = Quantity × Price
```

### Part 4 – Load Data into SQL Database

A SQLite database named `ecommerce.db` is created.
The processed data is loaded into the following tables:

* `Customers`
* `Products`
* `Orders`
* `Payments`
* `Sales_Report`

### Part 5 – Report Generation

SQL queries are used to generate:

* Sales report by product category.
* Customer sales report showing total spending.

### Part 6 – Incremental Data Loading

New orders are checked against existing Order IDs.
Only newly arriving orders are added to the database.

### Part 7 – Final Report

The existing sales data and newly arriving sales data are combined to generate the final e-commerce sales report.

## Database Tables

* `Customers`
* `Products`
* `Orders`
* `Payments`
* `Sales_Report`
* `New_Sales`

## Output Files

* `customers.csv`
* `products.csv`
* `orders.csv`
* `payments.csv`
* `ecommerce.db`

## Result

Thus, an end-to-end e-commerce ETL pipeline was successfully developed using Pandas and SQLite to extract, clean, transform, load, and report historical and newly arriving data.
