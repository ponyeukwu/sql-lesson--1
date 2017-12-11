# SQL mission #1.
In this mission you will create a SQL database using MySql, you will create SQL tables and column inside those tables.

# Table of Contents
- [Before starting](#before-starting)
  * [Naming convention](#naming-convention)
  * [DataTypes](#datatypes)
    + [VARCHAR](#varchar)
    + [INT](#int)
    + [DATE](#date)
- [First step: Create the database](#first-step--create-the-database)
- [Second step: Create tables &amp; table columns](#second-step--create-tables--amp--table-columns)
  * [Customers table](#customers-table)
  * [Salesmans table](#salesmans-table)
  * [Purchases table](#purchases-table)
  * [Products table](#products-table)
- [Third step: Primary key &amp; Foreign Key (PK &amp; FK)](#third-step--primary-key--amp--foreign-key--pk--amp--fk-)
  * [Customers table](#customers-table-1)
  * [Salesmans table](#salesmans-table-1)
  * [Purchases table](#purchases-table-1)
  * [Products table](#products-table-1)
- [Solution](#solution)
- [Materials](#materials)
  * [Videos](#videos)
  * [Links](#links)
  * [Downloads](#downloads)

## Before starting
### Naming convention

### DataTypes
#### VARCHAR

#### INT

#### DATE

## First step: Create the database
You can create the Database using Workbench IDE or phpMyAdmin designer tools. here is the sql statement if you choose to create your Database from a query.
```sql
CREATE DATABASE northwind;
```

## Second step: Create tables &amp; table columns
### Customers table
```sql
CREATE TABLE customers (social_security INT(11), first_name VARCHAR(20), last_name VARCHAR(20), email VARCHAR(55), city VARCHAR(20));
```

### Salesmans table
```sql
CREATE TABLE salesmans (social_security INT(11), first_name VARCHAR(20), last_name VARCHAR(20), email VARCHAR(55), city VARCHAR(20), start_of_work_date DATE);
```

### Purchases table
```sql
CREATE TABLE purchases (id INT(11), customer_social_security INT(11), salesman_social_security INT(11), quantity INT(11), purchase_date DATE);
```

### Products table
```sql
CREATE TABLE products (id INT(11), name VARCHAR(20), price INT(11));
```

## Third step: Primary key &amp; Foreign Key (PK &amp; FK)
### Customers table
The column `social_security` should be **PK**.

### Salesmans table
The column `social_security` should be **PK**.

### Purchases table
The column `id` should be **PK**.
The column `customer_social_security` should be a **FK** of `social_security` field of `Customers` table.
The column `salesman_social_security` should be a **FK** of `social_security` field of `salesmans` table.

### Products table
The column `id` should be **PK**.

## Solution
Found in this repository at `northwind.sql` file.

## Materials
### Videos
How to use Brackets IDE: https://youtu.be/ZgEkwJKi_Lo

How to install and work with Github & Brackets: https://youtu.be/BSSs1RbwgWg

### Links
MySQL developers: Creating and Selecting a Database
https://dev.mysql.com/doc/refman/5.7/en/creating-database.html

MySQL developers: Creating a Table
https://dev.mysql.com/doc/refman/5.7/en/creating-tables.html

### Downloads
XAMPP
MySQL Workbench

#### Export

#### Import
