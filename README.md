# 🍕 SQL Pizza Sales Analysis Project

## 📌 Project Overview
This project analyzes pizza sales data using **SQL** to extract meaningful business insights such as revenue trends, customer ordering behavior, popular pizza types, and category-wise performance.

The analysis is performed on a relational dataset consisting of orders, order details, pizzas, and pizza types.  
All questions solved and results shown are documented in the attached PDF presentation.

👤 **Created by:** Mayank Kapoor  
📊 **Role Focus:** Data Analyst / SQL Analyst  
📄 **Project Documentation:** `pizza_sales.pdf`

---

## 🗂️ Dataset Description

The project uses the following CSV files:

| File Name | Description |
|---------|-------------|
| `orders.csv` | Order date & time details |
| `order_details.csv` | Quantity of pizzas per order |
| `pizzas.csv` | Pizza size and price |
| `pizza_types.csv` | Pizza name and category |

---

## 🧩 Database Schema Overview

- **orders** (`order_id`, `order_date`, `order_time`)
- **order_details** (`order_details_id`, `order_id`, `pizza_id`, `quantity`)
- **pizzas** (`pizza_id`, `pizza_type_id`, `size`, `price`)
- **pizza_types** (`pizza_type_id`, `name`, `category`)

---

## 🧠 Questions Solved Using SQL

### 🔹 Basic Analysis
1. Retrieve the total number of orders placed
2. Calculate the total revenue generated from pizza sales
3. Identify the highest-priced pizza
4. Identify the most common pizza size ordered
5. List the top 5 most ordered pizza types along with their quantities

### 🔹 Intermediate Analysis
6. Find the total quantity ordered for each pizza category
7. Determine the distribution of orders by hour of the day
8. Find category-wise distribution of pizzas
9. Calculate the average number of pizzas ordered per day
10. Identify the top 3 pizza types based on revenue

### 🔹 Advanced Analysis
11. Calculate the percentage contribution of each pizza category to total revenue
12. Analyze cumulative revenue generated over time
13. Determine the top 3 pizza types by revenue for each pizza category

---

## 🧾 Sample SQL Queries

### 🔸 Total Number of Orders
```sql
SELECT COUNT(order_id) AS total_orders
FROM orders;
