# Practical 2 – ETL Process Using SQL Server

## Aim

To perform the ETL (Extract, Transform, Load) process using SQL Server.

## Software Used

- SQL Server
- SQL Server Management Studio (SSMS)

## Technologies Used

- SQL
- ETL
- SQL Server Database

## Objective

- Create a database and student data table.
- Insert student records into the source table.
- Extract data from the source table.
- Transform the data by handling missing values and standardizing city names.
- Categorize students based on their marks.
- Load the transformed data into a final table.

## Description

This practical demonstrates the ETL process using SQL Server. Student data is extracted from a source table, transformed by handling missing values and standardizing city names, and loaded into a final table.

### Part 1 – Extract

Student records are extracted from the `Student_Data` table using a SELECT query.

### Part 2 – Transform

The data is transformed by:

- Replacing missing age values with `0`.
- Standardizing city names such as `mumbai` and `PUNE`.
- Replacing missing city values with `Unknown`.
- Creating a `Performance_Category` based on marks.

### Part 3 – Load

A `Student_Final` table is created and the transformed data is inserted into it.

The final table is displayed using a SELECT query.

## Database Tables

- `Student_Data`
- `Student_Final`

## ETL Flow

```text
Student_Data
     ↓
   Extract
     ↓
  Transform
     ↓
Student_Final
     ↓
    Load
