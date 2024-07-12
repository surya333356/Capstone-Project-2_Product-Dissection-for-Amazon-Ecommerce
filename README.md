# Capstone-Project-2_Product-Dissection-for-Amazon-Ecommerce(Relation Database)
# Project Type - Relational Database Contribution - Individual-SURYA SINGH
# Company Overview:
Amazon is one of the most influential companies today, impacting culture and society across all age groups. Known as Amazon.com, Inc., it is often considered the most valuable brand and is one of the top five American tech companies. Jeff Bezos started Amazon on July 5, 1994, in Washington, USA. Based in Seattle, Amazon serves customers worldwide.
Amazon has a large presence globally, including a significant customer base in India. Its various services, like Amazon Prime Video, Kindle, and Audible, each have their own advertisements and dedicated customers. Amazon's online shopping platform offers over 10,000 products, covering categories like lifestyle, home decor, and education.

![image](https://github.com/user-attachments/assets/b566e914-6746-432b-912a-58ca1492217c)

# Schema Description: 
A schema description typically refers to a structured representation of data elements and their relationships within a database or a data format.
For Amazon, a schema description might involve outlining how product information is organised and stored in their database or how data is structured for their e-commerce platform. Here’s a basic schema description for Amazon's product catalogue:

# Product Entity:
product_id: Unique identifier for each product (primary key).
product_name: Name of the product.
description: Detailed description of the product.
category_id: Identifier linking to the category table (foreign key).
price: Price of the product.
stock_quantity: Current available stock quantity.
brand: Brand or manufacturer of the product.
ratings: Average customer rating for the product.
reviews_count: Number of customer reviews.
created_at: Date and time when the product was added to the catalogue.
updated_at: Date and time of the last update to the product information.
# Category Entity:
category_id: Unique identifier for each category (primary key).
category_name: Name of the category (e.g., Electronics, Books, Home & Kitchen).
parent_category_id: Identifier linking to the parent category (if applicable).
# Cart Entity:
cart_id: Unique identifier for each cart (primary key).
customer_id: Identifier linking to the customer who owns the cart (foreign key).
product_id: Identifier linking to the product added to the cart (foreign key).
quantity: Quantity of the product added to the cart.
added_at: Date and time when the product was added to the cart.
# Customer Reviews Entity:
review_id: Unique identifier for each review(primary key).
product_id: Identifier linking to the product reviewed(foreign key).
customer_id: Identifier linking to the customer who wrote the review(foreign key).
rating: Numeric rating given by the customer (e.g., 1-5 stars).
review_text: Text of the customer review.
review_date: Date when the review was posted.
# Orders Entity:
order_id: Unique identifier for each order(primary key).
customer_id: Identifier linking to the customer who placed the order (foreign key).
order_date: Date and time when the order was placed.
total_amount: Total amount charged for the order.
shipping_address: Address where the order will be shipped.
status: Current status of the order (e.g., processing, shipped, delivered).
# Customer Entity:
customer_id: Unique identifier for each customer (primary key).
name: Name of the customer.
email: Email address of the customer (used as a login username).
password: Encrypted password for customer authentication.
phone_number: Phone number of the customer.
address: Complete mailing address of the customer.
city: City of residence for the customer.
state: State or province of residence.
country: Country of residence.
postal_code: Postal or ZIP code of the customer's address.
# Payment Entity:
payment_id: Unique identifier for each payment transaction (primary key).
customer_id: Identifier linking to the customer making the payment (foreign key).
order_id: Identifier linking to the order for which the payment is made (foreign key).
payment_method: Method used for payment (e.g., credit card, debit card, PayPal).
amount: Amount paid for the order.
payment_date: Date and time when the payment transaction occurred.
payment_status: Status of the payment transaction (e.g., pending, completed, failed).
transaction_id: Unique identifier provided by the payment processor for the transaction.



# Conclusion: 
In this case study, the well-organised database schema and detailed ERD (Entity-Relationship Diagram) show Amazon's careful planning in designing their database. This ensures data is managed efficiently and accurately. Key parts of the database, like Product, Orders, Customer Reviews, Payment, Category, Cart, and Customer, are all connected. This setup reduces duplicate data and makes retrieving information faster. This thorough design helps Amazon run a smooth e-commerce platform, allowing easy transactions, personalised shopping experiences, and the ability to grow. All of this contributes to Amazon's success and leadership in the market.


