# ETL_Midterm_Samuel_694

## Project Overview

This ETL project extracts, transforms, and loads order data from CSV files into a structured SQLite database. The goal is to practice ETL steps.

## ETL Phases

- **Extract**: loaded and inspected raw data (raw_data.csv, incremental_data.csv), checked for missing values and duplicates.
- **Transform**: applied data cleaning (fill missing values, remove duplicates), enrichment (added total_price), and converted order_date to datetime.
- **Load**: loaded transformed data into SQLite database (full_data.db and incremental_data.db).

## Tools Used

- Python
- Pandas
- SQLite (sqlite3)
- Jupyter Notebook
- VS Code

## How to Run the Project

1. Clone the repo.
2. Run notebooks in order: `etl_extract.ipynb` → `etl_transform.ipynb` → `etl_load.ipynb`.
3. Check outputs in `/transformed/` and `/loaded/`.

## Screenshot

![Data preview](screenshot1.png)
![Data preview](screenshot2.png)
