# Practical 6 – Setting Up Apache Airflow and Creating a DAG

## Aim

To set up Apache Airflow and create a DAG to orchestrate an ETL pipeline.

## Software Used

- Google Colab
- Python 3
- Apache Airflow

## Technologies Used

- Python
- Apache Airflow
- DAG
- BashOperator
- EmptyOperator
- Pandas
- REST API
- CSV

## Objective

- Install and configure Apache Airflow.
- Initialize the Airflow database.
- Create an ETL extraction script.
- Create an Airflow DAG.
- Define sequential task dependencies.
- Start the DAG processor.
- Detect, display, and trigger the DAG.

## Description

This practical demonstrates how Apache Airflow can be used to schedule and orchestrate an ETL pipeline in Google Colab.

### Part 1 – Airflow Setup

Apache Airflow is installed and its version is checked.
The `AIRFLOW_HOME` directory is configured and the Airflow database is initialized.

### Part 2 – ETL Extraction Script

A Python script is created to:
- Extract data from a REST API.
- Read location data from a CSV file.
- Merge the API and CSV data.
- Save the processed data as a CSV file.

### Part 3 – Creating the DAG

An Airflow DAG named `university_etl_orchestration` is created with three sequential tasks:

- `start_pipeline`
- `run_extraction_script`
- `log_pipeline_success`

The task dependency is:

```text
start_pipeline
       ↓
run_extraction_script
       ↓
log_pipeline_success
