# Practical 8 – PySpark DataFrame Operations

## Aim

To perform data processing and analysis on a CSV dataset using PySpark.

## Software Used

* Google Colab
* Python 3
* Apache Spark

## Technologies Used

* PySpark
* Spark DataFrame
* CSV
* Pandas-style DataFrame Operations

## Objective

* Create a Spark session.
* Create and read a CSV dataset using PySpark.
* Display the dataset schema.
* Perform filtering, grouping, and aggregation.
* Remove duplicate records.
* Join two datasets.
* Calculate average sales by product category.

## Description

This practical demonstrates DataFrame operations using PySpark.

### Part 1 – Create and Read CSV Dataset

A sample sales dataset is created using PySpark and saved as a CSV file.
The CSV dataset is then read using a Spark DataFrame.

### Part 2 – Display Schema

The structure and data types of the dataset are displayed using the `printSchema()` function.

### Part 3 – Filtering

Products with sales greater than `5000` are filtered using the `filter()` function.

### Part 4 – Grouping and Aggregation

The dataset is grouped by product category and the following operations are performed:

* Count the number of records.
* Calculate total sales for each category.

### Part 5 – Removing Duplicates

Duplicate records are identified and removed using the `dropDuplicates()` function.
The record count before and after removing duplicates is displayed.

### Part 6 – Joining Datasets

A second dataset containing product locations is created.
The sales dataset and location dataset are joined using `Product_ID`.

### Part 7 – Average Sales Calculation

The average sales for each product category are calculated using the `avg()` function.

## Output Files

* `sales_csv`

## Result

Thus, CSV data was successfully processed using PySpark by performing filtering, grouping, aggregation, duplicate removal, dataset joining, and average sales calculation.
