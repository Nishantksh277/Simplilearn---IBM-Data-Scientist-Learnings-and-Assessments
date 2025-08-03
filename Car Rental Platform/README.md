# 🚗 Car Rental Management System

A Python-based car rental management system that provides an intuitive console interface for managing car rentals, inventory, and billing. Built with object-oriented programming principles and designed for both learning and practical use.

[![Python Version](https://img.shields.io/badge/python-3.6%2B-blue.svg)](https://python.org)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Code Style](https://img.shields.io/badge/code%20style-PEP8-orange.svg)](https://www.python.org/dev/peps/pep-0008/)

## ✨ Features

- **🔄 Real-time Inventory Management**: Automatic tracking of available cars with instant updates
- **💰 Flexible Pricing System**: Support for hourly, daily, and weekly rental options
- **📊 Automated Billing**: Dynamic cost calculation with detailed bill summaries
- **🔙 Easy Returns**: Streamlined car return process with inventory restoration
- **✅ Input Validation**: Robust error handling with user-friendly feedback
- **📱 Interactive Interface**: Clean console-based user experience
- **🎯 Object-Oriented Design**: Well-structured, maintainable codebase

## 🎮 Usage

### Basic Workflow

1. **Launch Application** → System displays welcome message and available cars
2. **Customer Registration** → Enter your name
3. **Car Selection** → Choose number of cars and rental type
4. **Duration Input** → Specify rental period
5. **Bill Review** → Check generated bill summary
6. **Return Process** → Optionally return cars immediately

### Example Session

```
=== Welcome to Car Rental System ===

 Total available cars: 100

Enter your name: Alice Johnson
How many cars would you like to rent? 2
Choose rental type (hourly/daily/weekly): daily
Enter rental duration in daily: 5

 Bill Summary:
Type: daily
Cars: 2
Duration: 5
Total: ₹4990

Do you want to return the car? (yes/no): yes
✅ Cars returned successfully!

 Total available cars: 100
```

## 💵 Pricing Structure

| Rental Type | Rate per Car | Best For |
|-------------|--------------|----------|
| **Hourly**  | ₹149/hour   | Short trips, city tours |
| **Daily**   | ₹499/day    | Day trips, business travel |
| **Weekly**  | ₹699/week   | Extended stays, vacations |

## 🏗️ System Architecture

### Core Classes

#### 🚙 CarInventory
- **Purpose**: Fleet management and availability tracking
- **Key Methods**:
  - `display_available_cars()` - Shows current inventory
  - `rent_car(num)` - Processes car rentals
  - `return_car(num)` - Handles car returns

#### 💼 RentalService
- **Purpose**: Pricing management and bill generation
- **Key Methods**:
  - `generate_bill()` - Calculates costs and displays bills
- **Features**: Flexible rate structure for different rental types

#### 👤 Customer
- **Purpose**: Customer data and rental request management
- **Key Methods**:
  - `request_car()` - Handles rental requests with validation
  - `return_car()` - Manages return process

### Data Flow

```
Customer Input → Validation → Inventory Check → Bill Generation → Transaction Complete
```

## 📁 Project Structure

```
car-rental-system/
│
├── 📓 Car Rental Python Project.ipynb  # Jupyter notebook version
├── 🐍 car_rental.py                    # Standalone Python script
├── 📋 requirements.txt                 # Project dependencies
├── 📖 README.md                        # Project documentation
├── 📄 LICENSE                          # License file
└── 📁 docs/                           # Additional documentation
    ├── api_reference.md
    └── user_guide.md
```
## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Team & Contact

**Project Maintainer**: Nishant Sharma  
**Email**: Nish.sh27@gmail.com  
**GitHub**: https://github.com/Nishantksh277

## 🙏 Acknowledgments

- **Python Community** for excellent documentation and support
- **Open Source Contributors** for inspiration and best practices
- **Real-world Car Rental Services** for business logic insights
- **Educational Institutions** promoting hands-on learning projects
