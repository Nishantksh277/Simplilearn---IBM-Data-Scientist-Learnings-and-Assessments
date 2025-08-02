# Shopping App Python Project 🛒

[![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Assessment](https://img.shields.io/badge/Assessment-IBM%20Data%20Scientist-orange.svg)](https://www.simplilearn.com/)

> A comprehensive backend e-commerce application developed as part of the **IBM Data Scientist Course** assessment by **Simplilearn**. This project demonstrates advanced Python programming concepts including Object-Oriented Programming, user authentication, inventory management, and payment processing.

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Technical Architecture](#technical-architecture)
- [Installation & Setup](#installation--setup)
- [Usage Guide](#usage-guide)
- [Code Structure](#code-structure)
- [Assessment Requirements](#assessment-requirements)
- [Demo Screenshots](#demo-screenshots)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Project Overview

This Shopping App is a **backend-focused e-commerce application** that simulates real-world online shopping functionality. Built entirely in Python using Object-Oriented Programming principles, it provides a complete shopping experience from user authentication to payment processing.

### 🎓 Educational Context
- **Course**: IBM Data Scientist Program
- **Module**: Programming Essentials with Python
- **Assessment Type**: Practical Implementation Project
- **Institution**: Simplilearn

### 🔧 Technical Scope
- **Backend Implementation Only** (No UI/Frontend required)
- **In-Memory Data Storage** (No database connectivity required)
- **Console-Based Interface** for demonstration
- **Production-Ready Code Structure** with proper error handling

## ✨ Features

### 🔐 Authentication System
- **Admin Login**: Full administrative privileges
- **Public Access**: Guest user functionality
- **Session Management**: Secure user state management

### 📦 Category Management
- **Pre-loaded Categories**: Footwear, Clothing, Electronics, Accessories
- **Dynamic Category Operations**:
  - ➕ Add new categories
  - ✏️ Update existing categories
  - 👁️ View all categories
- **Admin-Only Access** for category modifications

### 🛍️ Product Management
- **Product Operations**:
  - Add products to specific categories
  - Set pricing and stock quantities
  - View products by category
  - Automatic stock management
- **Product Attributes**:
  - Name, Price, Stock Quantity
  - Category Association
  - Real-time inventory tracking

### 🛒 Shopping Cart System
- **Cart Operations**:
  - Add items with quantity selection
  - Remove items from cart
  - View cart with total calculation
  - Real-time stock validation
- **Smart Features**:
  - Automatic subtotal calculation
  - Stock availability checking
  - Quantity management

### 💳 Payment Processing
- **Multiple Payment Methods**:
  - 📱 **UPI Payments**: Secure UPI ID-based transactions
  - 💳 **Debit Card Payments**: Card-based payment processing
- **Payment Features**:
  - Transaction validation
  - Payment confirmation
  - Order completion workflow

## 🏗️ Technical Architecture

### Class Structure
```
Shopping App
├── User Class
│   ├── Authentication Management
│   ├── Session Handling
│   └── Role-Based Access Control
├── CategoryManager Class
│   ├── Category CRUD Operations
│   ├── Data Validation
│   └── Category Display Logic
├── ProductManager Class
│   ├── Product Management
│   ├── Inventory Control
│   └── Category Integration
└── Cart Class
    ├── Shopping Cart Operations
    ├── Payment Processing
    └── Order Management
```

### Design Patterns Used
- **Object-Oriented Programming (OOP)**
- **Separation of Concerns**
- **Single Responsibility Principle**
- **Data Encapsulation**

## 📖 Usage Guide

### For Administrators

1. **Login as Admin**
   ```
   Username: Admin
   Password: Admin@123
   ```

2. **Admin Dashboard Options**
   - Add new product categories
   - Update existing categories
   - Add products to categories
   - View all products and categories
   - Manage inventory

### For Public Users

1. **Access as Guest**
   - Use any invalid credentials to login as public user
   - Or simply press enter when prompted

2. **Shopping Features**
   - Browse categories and products
   - Add items to shopping cart
   - Manage cart contents
   - Proceed to checkout with payment

### Sample Workflow

```python
# Example interaction flow
1. Login (Admin/Public)
2. Browse Categories → Electronics, Footwear, Clothing, Accessories
3. View Products → Select from available inventory
4. Add to Cart → Choose quantity
5. Checkout → Select Payment Method (UPI/Debit Card)
6. Payment Confirmation → Order Complete
```

## 📁 Code Structure

```
project/
│
├── Shopping App Python Project.ipynb    # Main Jupyter Notebook
├── README.md                            # This file
└── src/                                # (Optional) Python modules
    ├── user.py                         # User management
    ├── category.py                     # Category operations
    ├── product.py                      # Product management
    └── cart.py                         # Shopping cart logic
```

### Key Components

| Component | Responsibility | Key Methods |
|-----------|---------------|-------------|
| `User` | Authentication & Authorization | `login()`, `is_admin()` |
| `CategoryManager` | Category Operations | `add_category()`, `update_category()`, `display_categories()` |
| `ProductManager` | Product Management | `add_product()`, `display_products()` |
| `Cart` | Shopping Cart & Payments | `add_to_cart()`, `checkout()`, `view_cart()` |

## 📸 Demo Screenshots

### Admin Dashboard
```
Admin Options:
1. Add Category
2. Update Category  
3. View Categories
4. Add Product
5. View All Products
6. Exit
```

### Public Shopping Interface
```
Public Options:
1. View Categories
2. View Products
3. Add to Cart
4. Remove from Cart
5. View Cart
6. Checkout
7. Exit
```

### Sample Product Display
```
📁 Electronics:
  - Smartphone | ₹25000 | Stock: 50
  - Laptop | ₹65000 | Stock: 25

📁 Footwear:
  - Running Shoes | ₹3500 | Stock: 100
  - Formal Shoes | ₹4500 | Stock: 75
```
## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Simplilearn** for providing the comprehensive IBM Data Scientist course
- **IBM** for the structured learning path and assessment framework
- **Python Community** for excellent documentation and resources

## 📞 Contact & Support

**Developer**: Nishant sharma
- 📧 Email: Nish.sh27@gmail.com
- 💼 LinkedIn: https://www.linkedin.com/in/nishantsharma2k1/
- 🐙 GitHub: https://github.com/Nishantksh277

**Course Information**:
- 🎓 **Course**: IBM Data Scientist
- 🏫 **Platform**: Simplilearn
- 📚 **Module**: Programming Essentials with Python

---

<div align="center">

**⭐ If you found this project helpful for your learning journey, please consider giving it a star! ⭐**

*Built with ❤️ for the IBM Data Scientist Course Assessment*

</div>
