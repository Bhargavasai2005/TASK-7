# Task 7 - Data Analyst Internship

## 📝 Objective
To connect Python with an SQLite database, run simple SQL queries, and visualize sales summary data.

---

## 🧰 Tools Used
- Python
- SQLite (`sqlite3`)
- pandas
- matplotlib

---

## 🗃 Dataset
Created a SQLite database (`sales_data.db`) with a single table called `sales`.  
Sample data included product name, quantity sold, and price per unit.

---

## 🔍 SQL Query Used
```sql
SELECT product, 
       SUM(quantity) AS total_qty, 
       SUM(quantity * price) AS revenue 
FROM sales 
GROUP BY product;
