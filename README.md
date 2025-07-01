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

## Lab 5 Schema Info

For the load step, I used `pandas.to_sql()` to write both datasets into SQLite databases. This function automatically creates the table structure based on the columns in the DataFrame.

The result is basically the same as the schema shown in the instructions with fields like customer_name, product, quantity, unit_price, total_price, and order_date. Both `full_data.db` and `incremental_data.db` follow this format.

## Screenshot

![Data preview](screenshot1.png)
![Data preview](screenshot2.png)

