# Practical 7 – ETL Pipeline Using CSV, JSON and SQLite Database

## Aim

To develop an ETL pipeline using CSV and JSON data, clean and transform the data, validate it, and load it into a SQLite database.

## Software Used

- Google Colab
- Python 3
- SQLite

## Technologies Used

- Python
- Pandas
- CSV
- JSON
- SQLite
- ETL

## Objective

- Create and extract data from multiple CSV files.
- Combine CSV datasets.
- Identify and remove invalid records.
- Transform and validate the data.
- Extract and transform JSON data.
- Load CSV and JSON data into a SQLite database.
- Perform incremental data loading.

## Description

This practical demonstrates an ETL pipeline using CSV, JSON, Pandas, and SQLite.

### Part 1 – Extract Data

Student data is extracted from multiple CSV files and combined into a single dataset.
JSON data is also created, extracted, and converted into a DataFrame.

### Part 2 – Clean and Transform Data

Invalid records are identified based on age and marks.
The invalid records are removed, student names are converted to uppercase, and a performance category is created based on marks.

### Part 3 – Data Validation

The data is validated by checking:
- Missing values
- Duplicate Student IDs
- Valid age range
- Valid marks range

### Part 4 – Load Data into SQLite

A SQLite database is created.
The cleaned CSV data is loaded into the `Students` table and JSON data is loaded into the `Student_Courses` table.

### Part 5 – Incremental Loading

New student records are checked against existing Student IDs.
Only new records are added to the database using incremental loading.

## Database Tables

- `Students`
- `Student_Courses`

## Output Files

- `students1.csv`
- `students2.csv`
- `students.json`
- `ETL_Practical7.db`

## Result

Thus, an ETL pipeline was successfully developed to extract, clean, transform, validate, and load CSV and JSON data into a SQLite database, including incremental data loading.
