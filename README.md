# Instagram Thrift & Handmade Business Data Model

This project contains an ER diagram for a small Instagram-based thrift and handmade business. The model shows how customers place orders, how products are organized into variants, and how payments and shipping are tracked.

<img width="969" height="1101" alt="Img" src="https://github.com/user-attachments/assets/71dee800-b6b5-4489-83e4-c4d720f9b78f" />


## Overview

The goal of this database design is to support core business operations such as:

- Managing customer information
- Storing products and their variants
- Recording orders and order items
- Tracking payments
- Tracking shipping and delivery status

## Entities

- **customers**: Stores customer details like name, phone, email, and address.
- **products**: Stores product information such as name, description, price, type, and category.
- **product_variants**: Stores different versions of a product, such as size, color, condition, and stock quantity.
- **orders**: Stores order details placed by customers.
- **order_items**: Stores the items included in each order.
- **payments**: Stores payment details for each order.
- **shipping**: Stores shipping and delivery information for each order.

## Relationships

- One customer can place many orders.
- One product can have many variants.
- One order can contain many order items.
- One product variant can appear in many order items.
- One order can have one payment record.
- One order can have one shipping record.

## Key Notes

- Primary keys are used to uniquely identify each record.
- Foreign keys connect related tables and maintain data consistency.
- The model separates products from product variants so inventory can be tracked more accurately.
- Order, payment, and shipping data are separated to keep the design clean and scalable.

## Tools Used

- **Eraser** for drawing the ER diagram
- Chen notation for representing the database structure
