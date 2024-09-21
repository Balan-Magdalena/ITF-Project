<h1>Database Project for **Online Store Management System** </h1>

The scope of this project is to use all the SQL knowledge gained throught the Software Testing course and apply them in practice.

Application under test: **Online Store Management System**

Tools used: MySQL Workbench

Database description: **The purpose of this database is to manage information about products, customers, employees, and orders placed in an online store. The database will store data on products (name, price, category), customers (name, address, email), employees (name, position), and orders (ordered products, quantity, price). The relationships between the tables in the database reflect the natural connections between entities, such as customers and orders or products and categories.**

<ol>
<li>Database Schema </li>
<br>
You can find below the database schema that was generated through Reverse Engineer and which contains all the tables and the relationships between them.

The tables are connected in the following way:

<ul>
  
**Customers** is connected with **Orders** through a **one-to-many** relationship, which is implemented using **customers.customer_id** as the primary key and **orders.customer_id** as the foreign key. Each customer can place multiple orders.

**Products** is connected with **Orders** through a **many-to-many** relationship, which is implemented using an intermediate table **Order_Products**, utilizing **products.product_id** and **orders.order_id**. Each order can contain multiple products, and each product can appear in multiple orders.

**Employees** is connected with **Orders** through a **one-to-many** relationship, implemented using **employees.employee_id** as the primary key and **orders.employee_id** as the foreign key. Each employee can handle multiple orders.

</ul><br>

<li>Database Queries</li><br>

<ol type="a">
  <li>DDL (Data Definition Language)</li>

  The following instructions were written in the scope of CREATING the structure of the database (CREATE INSTRUCTIONS)

  **CREATE DATABASE OnlineStore, 
    CREATE TABLE Customers(customer_id, customer_name, address, email),
    CREATE TABLE Employees(employee_id employee_name, job_title),
    CREATE TABLE Products(product_id, product_name, price, category),
    CREATE TABLE Orders(order_id, order_date, customer_id, employee_id),
    CREATE TABLE Order_Products(order_id, product_id, quantity)** 
   
    

  After the database and the tables have been created, a few ALTER instructions were written in order to update the structure of the database, as described below:

  **-Add phone column to the Customers table : ALTER TABLE Customers ADD phone_number**
  
 **- Rename category column in product_category in Products table: ALTER TABLE Products CHANGE category product_category**
 
 **- Add AUTO_INCREMENT property to the employee_id column in the Employees table:ALTER TABLE Employees MODIFY employee_id INT AUTO_INCREMENT**
 
 **- Add primary key : PRIMARY KEY (product_id)**
 
 **- Add primary key : PRIMARY KEY (order_id)**
 
 **- Add foreign key : FOREIGN KEY (customer_id) REFERENCES Customers(customer_id)**
 
 **- Add foreign key : FOREIGN KEY (employee_id) REFERENCES Employees(employee_id)**
 
 
  
  <li>DML (Data Manipulation Language)</li>

  In order to be able to use the database I populated the tables with various data necessary in order to perform queries and manipulate the data. 
  In the testing process, this necessary data is identified in the Test Design phase and created in the Test Implementation phase. 

  Below you can find all the insert instructions that were created in the scope of this project:

  **-Insert data into the Customers table : INSERT INTO Customers (customer_name, address, email)**
  
  **-Insert data into the Employees table : INSERT INTO Employees (employee_name, job_title)**
  
  **-Insert data into the Products table : INSERT INTO Products (product_name, price, product_category)**

  **-Insert product orders : INSERT INTO Orders (order_date, customer_id, employee_id)**
  
  **-Insert product orders : INSERT INTO Order_Products (order_id, product_id, quantity)**


  After the insert, in order to prepare the data to be better suited for the testing process, I updated some data in the following way:

  **Inserati aici toate instructiunile de UPDATE pe care le-ati scris folosind filtrarile necesare astfel incat sa actualizati doar datele de care aveti nevoie**


  <li>DQL (Data Query Language)</li>

After the testing process, I deleted the data that was no longer relevant in order to preserve the database clean: 

**-Update customer address with customer_id = 1 : UPDATE Customers SET address = '789 Elm St' WHERE customer_id = 1**

**-Update price for product with product_id = 2 : UPDATE Products SET price = 850.00 WHERE product_id = 2**


In order to simulate various scenarios that might happen in real life I created the following queries that would cover multiple potential real-life situations:

**- Select all customers:**  **SELECT** * **FROM** Customers;

**- Selection of products priced over 1000:**  **SELECT** * **FROM** Products **WHERE** price > 1000;

**- Select John Doe customer orders:** 
**SELECT** Orders.order_id, Orders.order_date **FROM** Orders
**JOIN** Customers **ON** Orders.customer_id = Customers.customer_id
**WHERE** Customers.customer_name = 'John Doe';

**- Select orders and associated products:** 
**SELECT** Orders.order_id, Products.product_name, Order_Products.quantity **FROM** Orders
**JOIN** Order_Products **ON** Orders.order_id = Order_Products.order_id
**JOIN** Products **ON** Order_Products.product_id = Products.product_id;

**- Aggregate functions: the total number of products ordered:** 
**SELECT COUNT**(*) AS total_products **FROM** Order_Products;

**- Group by and having: group orders on customers with more than one order:**
**SELECT** customer_id, **COUNT**(*) as total_orders 
**FROM** Orders
**GROUP BY** customer_id
**HAVING COUNT**(*) > 1;

**-Extract the orders that were placed by a specific customer and processed by a specific employee :**
**SELECT** orders.order_id, orders.order_date, customers.customer_name, employees.employee_name **FROM** orders
**INNER JOIN** customers **ON** orders.customer_id = customers.customer_id
**INNER JOIN** employees **ON** orders.employee_id = employees.employee_id
**WHERE** customers.customer_name = 'John Doe' **AND** employees.employee_name = 'Jane Smith';

**Extract products that belong to a certain category or have a price greater than 100:**
**SELECT** product_name, price, product_category
**FROM** products
**WHERE** product_category = 'Electronics' **OR** price > 100;

**Extract all orders that have not been processed by a specific employee:**
**SELECT** orders.order_id, orders.order_date, employees.employee_name
**FROM** orders
**INNER JOIN** employees **ON** orders.employee_id = employees.employee_id
**WHERE NOT** employees.employee_name = 'Jane Smith';

**Extract customers who have "gmail" in their email address:**
**SELECT** customer_name, email
**FROM** customers
**WHERE** email **LIKE** '%gmail.com';

**Extract all orders and products associated with each order:**
**SELECT** orders.order_id, products.product_name, order_products.quantity
**FROM** orders
**INNER JOIN** order_products **ON** orders.order_id = order_products.order_id
**INNER JOIN** products **ON** order_products.product_id = products.product_id;

**Extract all orders, including those that have no associated products (if such cases exist):**
**SELECT** orders.order_id, order_products.product_id, products.product_name
**FROM** orders
**LEFT JOIN** order_products **ON** orders.order_id = order_products.order_id
**LEFT JOIN** products **ON** order_products.product_id = products.product_id;

**Extract all possible combinations of customers and products:**
**SELECT** customers.customer_name, products.product_name
**FROM** customers
**CROSS JOIN** products;

**Extract the total amount of products ordered in a particular order:**
**SELECT** order_id, SUM(order_products.quantity) AS total_quantity
**FROM** order_products
**GROUP BY** order_id;









<br>
<br>

</ol>

<li>Conclusions</li>

**Inserati aici o concluzie cu privire la ceea ce ati lucrat, gen lucrurile pe care le-ati invatat, lessons learned, un rezumat asupra a ceea ce ati facut si orice alta informatie care vi se pare relevanta pentru o concluzie finala asupra a ceea ce ati lucrat**

</ol>
