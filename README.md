![Image](https://github.com/user-attachments/assets/094b7fbc-0d97-43e1-876e-8e1647c90340)


# 📚 Bookstore SQL Analysis Project

![SQL](https://img.shields.io/badge/Language-SQL-blue) ![PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-336791) ![GitHub](https://img.shields.io/badge/Platform-GitHub-black)

---

## 📖 Project Overview

This project simulates a **Bookstore Database System** containing three main entities:

- **Books**
- **Customers**
- **Orders**

I performed a variety of SQL queries for **data exploration, analysis, and reporting**.  
The goal is to demonstrate strong command over **SQL fundamentals** and **advanced analytical queries**.

---

## 📂 Project Structure

| File / Folder         | Description                                      |
| ----------------------| ------------------------------------------------ |
| `Books.csv`            | Dataset containing book details                 |
| `Customers.csv`        | Dataset containing customer information         |
| `Orders.csv`           | Dataset containing order records                |
| `bookstore_queries.sql`| SQL script file with all queries and solutions   |

---

## 🛠️ Tech Stack

- **Database:** PostgreSQL 
- **Tools:** pgAdmin
- **Version Control:** Git and GitHub

---

## 🎯 Key SQL Operations

✅ Create tables and define relationships  
✅ Simple data retrieval with filtering and sorting  
✅ Aggregations like `SUM()`, `AVG()`, `COUNT()`  
✅ Joining multiple tables  
✅ Grouping and advanced analytics (`GROUP BY`, `HAVING`)  
✅ Finding top-selling books and best customers  
✅ Stock management after orders  

---

## 🔥 Highlights of SQL Analysis

- **List of fiction genre books**
- **Customers from specific countries (e.g., Canada)**
- **Revenue calculation and order trends**
- **Top 3 expensive fantasy books**
- **Customer spending analysis**
- **Remaining stock after all orders fulfilled**
- **Genre-wise and author-wise book sales breakdown**

---

## 📊 Example Query Snippets

**1. Find all books in the "Fiction" genre:**

```sql
SELECT * FROM Books
WHERE genre = 'Fiction';
```

**2. Calculate total revenue:**

```sql
SELECT SUM(total_amount) AS Revenue
FROM Orders;
```

**3. Find the customer who spent the most:**

```sql
SELECT c.customer_id, c.name, SUM(o.total_amount) AS Total_Spend
FROM Customers c
JOIN Orders o ON c.customer_id = o.customer_id
GROUP BY c.customer_id, c.name
ORDER BY Total_Spend DESC
LIMIT 1;
```

---

## 🤝 Let's Connect!

If you liked this project or have any feedback, feel free to connect:

- 📧 Email: mayurpatil11801@gmail.com
- 💼 LinkedIn: https://www.linkedin.com/in/mayurpatil1130

---

# ⭐ Don't forget to give a star to the repository if you find it useful!

