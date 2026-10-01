**# Practical 5 – Extracting Data from APIs and Flat Files Using Python

## Aim

To extract data from a REST API and a CSV file, merge the data, and save the processed data using Python.

## Software Used

- Google Colab
- Python 3

## Technologies Used

- Python
- Pandas
- Requests
- REST API
- CSV
- JSON

## Objective

- Extract data from a public REST API.
- Convert JSON API data into a DataFrame.
- Extract data from a CSV file.
- Merge API and CSV data using a common ID.
- Save the merged data as a CSV file.

## Description

This practical demonstrates how to extract and combine data from different sources using Python and Pandas.

### Part 1 – API Data Extraction

Data is fetched from the JSONPlaceholder REST API using the `requests` library and converted into a Pandas DataFrame.

### Part 2 – CSV Data Extraction

A CSV file containing city and country information is created and read using Pandas.

### Part 3 – Data Transformation and Merging

Required API columns are selected and the `company.name` column is renamed to `company`.
The API data and CSV data are merged using the common `id` column.

### Part 4 – Saving Processed Data

The merged data is saved as:
`cleaned_warehouse_profiles.csv`

## Output Files

- `locations.csv`
- `cleaned_warehouse_profiles.csv`

## Result

Thus, data was successfully extracted from a REST API and a CSV file, transformed, merged, and saved using Python and Pandas in Google Colab.**
