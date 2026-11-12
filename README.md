# Rent-Anything

A PHP and MySQL rental marketplace where customers browse products, add them to a cart and check out, and an admin adds new listings.

## Overview

Rent-Anything is a database-driven web application built as a group project. Customers can register, log in, browse rental products by category, view product details, manage a cart and place orders. An admin area handles adding products.

## Features

| Area | What it does |
|---|---|
| Browsing | Product listing, product details and search results pages |
| Customer accounts | Registration, login, logout, an account page and order history |
| Cart and checkout | Shopping cart, checkout, payment options and order records |
| Admin | Admin area for inserting new products with images |

## Tech Stack

PHP, MySQL, HTML and CSS. It is designed to run on a local PHP and MySQL stack such as XAMPP or WAMP.

## Project Structure

```text
Rent-anything/
├── admin_area/        # Admin pages for adding products
├── customer/          # Customer login, account and order pages
├── functions/         # Shared PHP helper functions
├── includes/          # Database connection (db.php)
├── images/            # Site images
├── styles/            # Stylesheets
├── index.php          # Home page
├── all_products.php   # Product listing
├── details.php        # Product details
├── cart.php           # Shopping cart
├── checkout.php       # Checkout
├── database/        # renteverything.sql: schema and sample data
└── LICENSE
```

The database has these tables: `cart`, `categories`, `customers`, `customer_orders`, `pending_orders` and `products`.

## Getting Started

Step 1. Install a local PHP and MySQL stack such as XAMPP, then clone this repository into its web root (for example `htdocs`). The folder must be named `renteverything`, because the admin link in the pages expects that path:

```bash
git clone https://github.com/malehaICK/Rent-anything.git renteverything
```

Step 2. Create a MySQL database named `renteverything` and import the schema from `database/renteverything.sql`, for example with phpMyAdmin.

Step 3. Open `includes/db.php` and set the host, user, password and database name to match your local setup.

Step 4. Start Apache and MySQL, then open `http://localhost/renteverything/` in your browser.

## Screenshots

Project screenshots and the original group database export are in the `##group project details##` folder.

## Notes

This is a learning project. It is not hardened for production use, so do not deploy it with real customer data or payments.

## Author

Maleha Israt Chowdhury. [Portfolio](https://malehaisratchowdhury.netlify.app/)

## License

Released under the MIT License. See the `LICENSE` file.
