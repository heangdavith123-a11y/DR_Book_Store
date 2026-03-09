# Education Book Shop Management System

A web-based bookstore management system designed to handle inventory, sales transactions, and business reporting. Built with PHP and MySQL, it features a responsive dashboard and a Point of Sale (POS) interface.

## Features

### 📊 Dashboard
*   **Overview Stats**: Instant view of total books, daily sales, and total revenue.
*   **Visual Analytics**: Interactive line charts powered by Chart.js showing sales trends (24 Hours, 3 Days, 7 Days).
*   **Top Sellers**: List of top 5 best-selling books by quantity.

### 🛒 Point of Sale (POS)
*   **Create Sales**: User-friendly interface to add books to a cart.
*   **Stock Management**: Real-time stock validation prevents selling out-of-stock items.
*   **Transaction Processing**: Calculates subtotals, taxes (10%), and grand totals.
*   **Auto-Update**: Automatically deducts sold quantities from the main inventory.

### 📚 Inventory & Sales
*   **Book Management**: View and manage book details (ISBN, Category, Price).
*   **Soft Delete**: Books are marked as deleted rather than removed permanently to preserve historical data.
*   **Receipts**: Generate and print detailed sale receipts.
*   **Sales History**: Track all past transactions.

## Tech Stack

*   **Language**: PHP
*   **Database**: MySQL
*   **Frontend**: HTML, CSS, JavaScript (Chart.js)
*   **Environment**: XAMPP (Apache/MySQL)

## Setup & Installation

1.  **Prerequisites**: Ensure you have a local server environment like XAMPP or WAMP installed.
2.  **Files**: Place the project folder in your `htdocs` directory (e.g., `c:\xampp\htdocs\Web-Small-Project`).
3.  **Database**:
    *   Create a database named `booksalsedb` (as defined in `ConnDB.php`).
    *   Import the required tables. *Note: Ensure table names match the application code (e.g., `salse_details` for sale items).*
4.  **Configuration**:
    *   Check `ConnDB.php` to ensure database credentials match your local setup:
        ```php
        $host = "localhost";
        $user = "root";
        $password = "";
        $database = "booksalsedb";
        
