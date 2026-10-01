# Practical 3 – Data Cleaning and Normalization

## Aim

To perform data cleaning and normalization using Python and Pandas.

## Software Used

- Python IDLE
- Python 3

## Technologies Used

- Pandas
- Python

## Objective

- Create a sample dataset using Pandas.
- Handle missing values.
- Remove duplicate records.
- Normalize numerical data using Min-Max normalization.
- Save the final cleaned dataset as a CSV file.

## Description

This practical demonstrates basic data preprocessing techniques using Pandas.

### Part 1 – Handling Missing Values

Missing values in the `Age`, `Marks`, and `Name` columns are handled using:

- Mean value for Age.
- Mean value for Marks.
- `Unknown` for missing Name.

### Part 2 – Removing Duplicate Rows

Duplicate records are identified and removed using the `drop_duplicates()` function.

### Part 3 – Data Normalization

Age and Marks are normalized using Min-Max normalization.

The formula used is:

`(x - min) / (max - min)`

This converts the values into a range between 0 and 1.

### Part 4 – Saving Cleaned Data

The final processed dataset is saved as:

`output/cleaned_data.csv`

## Result

Thus, missing values were handled, duplicate records were removed, numerical data was normalized, and the final cleaned dataset was successfully saved using Python and Pandas.
