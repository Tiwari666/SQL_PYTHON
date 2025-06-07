# Project: SQL_PYTHON — From CSV to SQL & Back with Python

This project walks through a full cycle of working with real-world e-commerce data using CSV, SQL Server, and Python (pandas + SQLAlchemy).

#  Project Structure & Flow

# SQL_PYTHON: Connecting Kaggle Data with SQL Server Using Python

This project demonstrates how to:
- Load Kaggle CSV data into SQL Server
- Run SQL queries from Python (basic → advanced)
- Analyze data using pandas and visualize insights
- Write transformed data back to SQL Server or save to CSV

---

## 🔗 Data Source
All datasets used in this project are from Kaggle’s [Brazilian E-Commerce Public Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce).

---

## 📂 Project Structure

| File / Folder                          | Purpose                                         |
|----------------------------------------|-------------------------------------------------|
| `01_Load_CSV_to_SQL.ipynb`            | Load Kaggle CSVs into SQL Server using pandas   |
| `02_SQL_Queries_From_Python_customers_basic.ipynb` | Beginner SQL queries from Python                |
| `03_SQL_Queries_From_Python_orders_intermediate.ipynb` | Intermediate-level analysis                     |
| `04_Advanced_SQL_Analysis_customers.ipynb` | Advanced queries using joins, window functions  |
| `05_Write_Back_to_SQL_or_CSV.ipynb`   | Save final results back to SQL or CSV           |
| `data/`                               | Contains original Kaggle CSV files              |
| `sql_python_env/`                     | Python virtual environment setup                |

---

## ✅ Tools Used

- Python (pandas, seaborn, matplotlib, sqlalchemy)
- SQL Server (via ODBC)
- SQLAlchemy + pyodbc connector
- VS Code + Jupyter Notebooks

---

## ✅ Flow

1. **Load CSVs** → SQL Server (`01_Load_CSV_to_SQL`)
2. **Run queries** (basic → advanced) from Python
3. **Transform & Analyze** data (aggregations, joins, window functions)
4. **Save results**: Back to SQL Server or export as CSV

---

## ✅ Example Use Cases

- Top customer locations
- Monthly revenue trends
- Product category contributions
- Delivery speed classification
- Repeat customers using `LAG()`/`LEAD()`
- YOY revenue growth with CTE + window functions

---

## ✅ Setup

1. Install dependencies:  
   `pip install pandas sqlalchemy pyodbc matplotlib seaborn`

2. Connect SQL Server with:
```python
engine = create_engine("mssql+pyodbc://NARENDRA\\SQLEXPRESS/sql_to_python?driver=ODBC+Driver+17+for+SQL+Server&trusted_connection=yes")```


## ✅ Output
Transformed data is saved to:

A SQL Server table: combined_data

Or exported to CSV via df.to_csv()

# ✅ Author
Narendra Tiwari

Built for academic + practical learning
