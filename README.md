**Task Overview**

This project demonstrates data analysis using SQL on a sample sales database. The goal is to extract, aggregate, and visualize insights using queries, joins, subqueries, views, and indexes.

**Database Structure**

**1. Customers Table**
Column	Type	Description
customer_id	NUMBER	Unique ID for each customer
customer_name	VARCHAR2(50)	Name of the customer
country	VARCHAR2(30)	Country of the customer

**2. Products Table**
Column	Type	Description
product_id	NUMBER	Unique ID for each product
product_name	VARCHAR2(50)	Product name
category	VARCHAR2(30)	Product category
price	NUMBER(10,2)	Price of the product

**3. Orders Table**
Column	Type	Description
order_id	NUMBER	Unique order ID
customer_id	NUMBER	References customers
product_id	NUMBER	References products
quantity	NUMBER	Quantity of product ordered
order_date	DATE	Date of the order

**SQL Operations**

**1. Data Insertion**

10 customers, 10 products, and 30 orders inserted.

Dates formatted using TO_DATE('YYYY-MM-DD','YYYY-MM-DD') for Oracle.


**2. Queries**

SELECT, WHERE, ORDER BY → Filter orders by country and sort by date.

GROUP BY & Aggregates → Calculate total sales per product.

JOINS (INNER, LEFT) → Analyze orders per customer.

Subqueries → Identify customers who spent above average.

Views → Monthly sales aggregation (monthly_sales).

Indexes → Optimized queries on order_date.
