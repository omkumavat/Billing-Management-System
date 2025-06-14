# 🧾 Billing Management System

A simple desktop-based **Billing Management System** built using **Java Swing** for the UI, **JDBC** for database connectivity, and **MySQL** as the backend. This application helps manage buyers, products, and generate bills efficiently.

---

## 📌 Features

- Add, update, delete buyers and products
- Search buyers/products by ID or name
- Generate and print customer bills
- Store and retrieve billing history
- User-friendly GUI using Java Swing

---

## 🛠️ Tech Stack

| Layer        | Technology       |
|-------------|------------------|
| Frontend     | Java Swing       |
| Backend      | Java (JDBC)      |
| Database     | MySQL            |

---

## 🧱 Database Schema

### 🔹 `buyer` Table
| Column Name | Data Type    | Description         |
|-------------|--------------|---------------------|
| id          | INT (PK)     | Unique Buyer ID     |
| name        | VARCHAR      | Buyer's Name        |
| contact     | VARCHAR      | Phone Number        |
| email       | VARCHAR      | Email Address       |
| address     | VARCHAR      | Address             |
| gender      | VARCHAR      | Gender              |

---

### 🔹 `product` Table
| Column Name | Data Type    | Description         |
|-------------|--------------|---------------------|
| id          | INT (PK)     | Unique Product ID   |
| name        | VARCHAR      | Product Name        |
| price       | DOUBLE       | Price per Unit      |
| quantity    | INT          | Available Stock     |
| description | TEXT         | Product Description |

---

### 🔹 `bills` Table
| Column Name  | Data Type    | Description            |
|--------------|--------------|------------------------|
| buyer_id     | INT (FK)     | Linked Buyer ID        |
| product_id   | INT (FK)     | Linked Product ID      |
| P_quantity   | INT          | Total Product Quantit  |

---

## 💻 Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/omkumavat/Billing-Management-System.git
