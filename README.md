# E-commerce Store Database

## Overview
This project is a **relational database management system** designed for an E-commerce Store using **MySQL**.  
It includes tables for users, products, orders, payments, and more, with proper constraints and relationships.

## Features
- Users, roles, and addresses
- Products with categories, inventory, and images
- Orders, order items, and statuses
- Payments, shipments, coupons, and reviews
- Shopping carts and audit logs

## Database Details
- **Database Name:** `ecommerce_store`
- **Engine:** InnoDB
- **Charset:** utf8mb4

## How to Use
1. Open MySQL Workbench or CLI.
2. Run the provided SQL file:

   ```bash
   mysql -u root -p < ecommerce_schema.sql

3.The database will be created with all tables and constraints.

Relationships

One-to-Many: User → Orders, User → Addresses

Many-to-Many: Products ↔ Categories, Users ↔ Roles

Orders contain multiple Order Items.

Payments and Shipments are linked to Orders.
