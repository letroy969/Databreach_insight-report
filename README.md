# Data Breach Insights Report

## Overview:


This repository contains a practical data analysis project focused on understanding data breach incidents across industries, regions, and time. The work demonstrates applied data analysis skills using Excel, Power BI, SQL, and Python, with an emphasis on producing insights that are relevant to cybersecurity teams and decision-makers.

The project covers the full workflow: data preparation, analysis, visualization, and reporting.

------------------------------------------------------------------------------------------------------------

## Objectives:

•Analyze historical data breach incidents to identify trends and patterns
•Compare breach frequency by year, geography, and industry
•Demonstrate structured data analysis using common enterprise tools
•Produce outputs suitable for both technical review and executive reporting

------------------------------------------------------------------------------------------------------------

## Tools and Technologies:

•Excel – data cleaning, pivot tables, charts, and exploratory analysis
•Power BI – interactive dashboards and executive-level reporting
•SQL (SQLite / PostgreSQL) – structured querying and aggregation
•Python – data processing, automation, and validation
•Jupyter Notebooks – exploratory and advanced analysis

------------------------------------------------------------------------------------------------------------

## How to Use the Project

### 1. Excel Analysis
Open the workbook located in the excel/ directory.

### Key worksheets:

•RAW – original imported data
•CLEAN – processed data with derived fields
•PIVOT_BreachesByYear – interactive pivot tables
•CHARTS – visual summaries with slicers

This workbook is designed to allow quick filtering and trend exploration.

### 2. Power BI Dashboard
Open the Power BI file in the powerbi/ directory.

Dashboard pages include:

•Overview – KPIs and high-level trends
•Geography – breach distribution by location
•Industry – industry-level comparisons

### 3. Data Pipeline (Optional)
If you want to regenerate or inspect the data pipeline:

bash

Copy code

pip install -r requirements.txt
python scripts/produce_sample_csv.py
python scripts/ingest_csv_to_postgres.py --db sqlite://./data.db
python scripts/test_project.py

### 4. SQL Analysis
Run analytical queries using the scripts provided:

### bash
### Copy code

python scripts/test_queries.py
These queries support the findings shown in Excel and Power BI.

## Key Deliverables

•Cleaned and structured breach dataset
•Interactive Excel analysis with pivot tables and charts
•Multi-page Power BI dashboard with executive summary
•SQL schema and reusable queries
•Python scripts for data ingestion and validation
•Supporting documentation and reports

## Repository Structure
### graphql
### Copy code

data-breach-insights/

├── data/        # Datasets and data documentation
├── sql/         # Database schema and queries
├── excel/       # Excel analysis workbook
├── powerbi/     # Power BI dashboard files
├── notebooks/   # Jupyter notebooks
├── scripts/     # Python automation and tests
├── docs/        # Architecture and reporting documents
└── README.md


### Architecture Summary
Data flows through a simple, reproducible pipeline:

CSV Data → Database → SQL Queries → Excel / Power BI → Reports

Python is used to automate ingestion and validation, while Excel and Power BI are used for analysis and presentation.

## Results Summary
500 breach records analyzed across multiple dimensions

Clear year-over-year breach trends identified

Industry-specific risk patterns observed

Clustering techniques used to group breach types

Findings presented in both technical and executive-friendly formats

## License
This project is released under the MIT License. See the LICENSE file for details.

Notes
This repository represents a completed analysis project intended for portfolio and evaluation purposes. The focus is on clarity, structure, and practical use of tools rather than experimentation.
