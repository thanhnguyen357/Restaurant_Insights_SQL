# Restaurant Orders Database Project

## Overview
This project demonstrates a **relational database design** for a restaurant ordering system. It includes tables for **Customers, Orders, Menu Items, and Order Items**, along with sample data and advanced SQL queries. This database showcases skills in **database design, SQL querying, indexing, window functions, and views**.

---

## Project Structure

| File | Description |
|------|-------------|
| `schema.sql` | Contains table definitions, primary/foreign keys, and indexes. |
| `sample_data.sql` | Inserts sample data into the database. |
| `queries.sql` | Contains various SQL queries, including **window functions** and **views**. |
| `analysis.sql` | Contains queries used to analyze the database and summarize insights. |
| `ERD.png` | Visual diagram showing relationships between all tables. |

---

## Database Design

- **Tables included**:
  - `Customers`: Stores customer information.
  - `Orders`: Contains order headers linked to customers.
  - `MenuItems`: Lists all menu items, categorized by type.
  - `OrderItems`: Maps items to each order with quantities.

- **Indexes implemented**:
  - `idx_orders_customer` on `Orders(CustomerID)` to speed up customer-related queries.
  - `idx_orderitems_order` on `OrderItems(OrderID)` for faster order-item lookups.

- **Views**:
  - Example: `vw_TotalSalesPerCustomer` aggregates sales by customer.  

*ERD diagram is included in the project as `ERD.png`.*

---

## Sample Queries Highlights

- **Basic queries**: Retrieve customer orders, list menu items, and calculate total sales per order.  
- **Advanced queries**:
  - **Window functions**: Rank top customers, calculate running totals of sales.
  - **Aggregations**: Count total orders per customer and per item.
  - **Views**: Predefined queries for commonly requested summaries.

---

## How to Use (MySQL)

1. **Create the database** (if needed):  
```sql
CREATE DATABASE restaurant_db;
USE restaurant_db;
```
2. **Run the schema to create tables and indexes**:
```sql
source schema.sql;
```
3. **Insert sample data into the database**:
```sql
source sample_data.sql;
```
4. **Run example queries:**
```sql
source queries.sql;
```
5. **Run analysis queries (optional, for exploring the data):**
```sql
source analysis.sql;
```
Tip: Always start your SQL session with USE restaurant_db; to ensure the correct database is selected.

## Skills Demonstrated

- Database design and normalization  
- Writing complex SQL queries with window functions, views, and aggregations  
- Using indexes for query optimization  
- Data analysis using SQL  
- Creating professional documentation for projects  

## Optional Enhancements

- Add stored procedures for automated reporting  
- Integrate with a web app or Python script for real-time querying  
- Include more complex sample data to test edge cases  

## ERD Diagram

The ERD diagram for this project is included in the repository as `ERD.png` (or the relevant file name).  

## Contact

Created by **[thanhnguyen357]**, a database and SQL enthusiast ready to build real-world projects.  
Feel free to explore the queries and analyze the data!
