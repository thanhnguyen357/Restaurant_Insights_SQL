# Restaurant Orders Database Project

This project is a sample restaurant order management database designed to demonstrate database design, SQL querying skills, and data analysis techniques. It includes normalized tables, indexes, complex queries, window functions, and views.

---

## ERD Diagram

The database structure is illustrated in the included **ERD diagram** (`ERD.png`), showing all relationships between tables.

---

## Database Structure

This database includes the following tables:

- **Customers** – Stores customer details.  
- **Orders** – Stores order information linked to customers.  
- **OrderItems** – Contains items in each order.  
- **MenuItems** – Contains menu item details.  
- **Servers** – Staff who take orders in the restaurant.  
- **DineInOrders** – Orders placed for dine-in.  
- **ToGoOrders** – Orders placed for takeout.  
- **[Other tables if any]** – Additional supporting tables as required.

All tables are normalized, linked with foreign keys, and use indexes for optimized queries.

---

### How to Use

1. **Install MySQL**  
   Make sure MySQL Server and MySQL Workbench are installed on your computer.

2. Create a new schema/database or use the existing one in `schema.sql`:  
   ```sql
   CREATE DATABASE IF NOT EXISTS restaurant_db;
   USE restaurant_db;
     ```

3. **Run schema.sql to create tables and indexes**  
   - Open `schema.sql` in MySQL Workbench.  
   - Execute the file to create all tables and indexes.  

4. **Run sample_data.sql to insert example data**  
   - Open `sample_data.sql` in MySQL Workbench.  
   - Execute the file to populate the tables with sample records.

5. **Run queries.sql to explore sample queries**  
   - Open `queries.sql` in MySQL Workbench.  
   - Execute the file to see examples of:  
     - Joins across all tables  
     - Aggregations (SUM, COUNT, AVG)  
     - Window functions for ranking and running totals  
     - Views for reusable reporting  

6. **Run analysis.sql to analyze the database**  
   - Open `analysis.sql` in MySQL Workbench.  
   - Execute the file to get insights like:  
     - Top customers by number of orders or total spending  
     - Most popular menu items  
     - Server performance metrics  
     - Total revenue and other statistics  

---

### Skills Demonstrated

- Database design and normalization  
- Writing complex SQL queries with window functions, views, and aggregations  
- Using indexes for query optimization  
- Data analysis using SQL  
- Creating professional documentation for projects  

---

### Optional Enhancements

- Add **stored procedures** for automated reporting  
- Integrate with a **web app or Python script** for real-time querying  
- Include more complex **sample data** to test edge cases  

---

### Contact

Created by **[thanhnguyen357]**, a database and SQL enthusiast ready to build real-world projects.  
Feel free to explore the queries and analyze the data!
