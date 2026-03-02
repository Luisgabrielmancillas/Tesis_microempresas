# 🌱 NexoEco

**Web E-Commerce Platform for Micro-Entrepreneurship Management**

NexoEco is a Full Stack web application designed to empower micro-entrepreneurs by providing a simple, scalable, and secure e-commerce platform. The system allows users to manage products, categories, inventory, and orders while offering customers an intuitive online shopping experience.

---

## 📌 Project Overview

NexoEco is built using a **three-tier architecture**:

* **Frontend:** Blade templates (Laravel) with responsive design
* **Backend:** Laravel Framework
* **Authentication:** Laravel Breeze
* **Database:** MySQL (Relational Database)
* **Architecture Style:** Client–Server with RESTful API

The platform supports role-based access control and follows best practices in security, performance, and usability.

---

## 👥 User Roles

### 🔹 Administrator

* Full system management
* CRUD operations for products and categories
* Order status management
* Sales reports access

### 🔹 Client

* User registration and login
* Browse products
* Add products to cart
* Place orders
* View order history

### 🔹 Visitor

* Public product browsing

---

## 🚀 Functional Requirements Implemented

| ID    | Description                               |
| ----- | ----------------------------------------- |
| RF-01 | User registration                         |
| RF-02 | Secure authentication                     |
| RF-03 | Role-based access control                 |
| RF-04 | CRUD operations for products              |
| RF-05 | CRUD operations for categories            |
| RF-06 | Shopping cart management                  |
| RF-07 | Inventory availability validation         |
| RF-08 | Order generation with product details     |
| RF-09 | Automatic inventory update after purchase |
| RF-10 | Order status management by admin          |
| RF-11 | Basic sales reports                       |

---

## 🔐 Non-Functional Requirements

### Security

* Password encryption (Laravel hashing)
* Authentication using Laravel Breeze
* Role-based authorization
* Input validation (Frontend & Backend)
* SQL Injection protection via Eloquent ORM

### Performance

* API response time under 2 seconds (normal load)
* Pagination for large datasets

### Usability

* Responsive web interface
* Mobile compatibility
* Intuitive checkout flow

---

## 🗄️ Database Model (Core Entities)

* **Users**
* **Categories**
* **Products**
* **Orders**
* **Order_Details**

### Relationships

* User → (1:N) → Orders
* Order → (1:N) → Order_Details
* Category → (1:N) → Products

---

## 🔌 API Documentation

The system exposes a RESTful API documented using:

* Postman Collection
  or
* Swagger (if implemented)

### Main Endpoints

* Authentication
* Product Management
* Category Management
* Order Management
* Reports

---

## 🛠️ Tech Stack

* **Backend:** Laravel
* **Authentication:** Laravel Breeze
* **Database:** MySQL
* **ORM:** Eloquent
* **Architecture:** MVC + REST API

---

## ⚙️ Installation Guide

### 1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/nexoeco.git
cd nexoeco
```

### 2️⃣ Install dependencies

```bash
composer install
npm install && npm run dev
```

### 3️⃣ Configure environment

Copy `.env.example` to `.env` and configure database credentials:

```bash
cp .env.example .env
```

Update:

```
DB_DATABASE=your_database
DB_USERNAME=your_username
DB_PASSWORD=your_password
```

### 4️⃣ Generate application key

```bash
php artisan key:generate
```

### 5️⃣ Run migrations

```bash
php artisan migrate
```

### 6️⃣ Start development server

```bash
php artisan serve
```

---

## 🧪 Testing & Validation

The system includes functional testing for:

* CRUD operations
* Authentication & role validation
* Inventory validation
* Order processing

Testing evidence is documented using Postman requests and screenshots.

---

## 📊 Future Improvements

* Payment gateway integration
* Logistics API integration
* Advanced analytics dashboard
* Multi-vendor support
* Product image optimization

---

## 📄 License

This project is developed for academic and educational purposes.

---
---

> NexoEco — Connecting micro-entrepreneurs to the digital economy.
