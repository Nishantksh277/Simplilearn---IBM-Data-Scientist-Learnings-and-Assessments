# 🚀 ScienceQtech Employee Performance Mapping

[![SQL](https://img.shields.io/badge/SQL-MySQL-blue.svg)](https://www.mysql.com/)
[![Database](https://img.shields.io/badge/Database-Design-green.svg)](#)
[![Analytics](https://img.shields.io/badge/Analytics-HR%20Insights-orange.svg)](#)

### 🌟 Key Achievements
- **Advanced Analytics**: Comprehensive employee performance tracking and analysis
- **Automated Reporting**: Streamlined data extraction for management decisions
- **Performance Optimization**: Strategic bonus calculations and role standardization
- **Global Insights**: Multi-continental workforce analysis and salary benchmarking

## 📊 Database Architecture

### Entity Relationship Design
The system is built around three core entities:

```
📋 emp_record_table (Main Employee Repository)
├── Employee Demographics (ID, Name, Gender)
├── Professional Details (Role, Department, Experience)
├── Geographic Information (Country, Continent)
├── Compensation Data (Salary, Performance Rating)
└── Organizational Structure (Manager ID, Project ID)

🎯 proj_table (Project Management)
├── Project Metadata (ID, Name, Domain)
├── Timeline Tracking (Start/End Dates, Quarter)
└── Status Monitoring

👥 data_science_team (Specialized Team View)
└── Focused dataset for Data Science department analysis
```

### Core Features Implemented

#### 🔍 **Advanced Query Operations**
- **Multi-condition Filtering**: Dynamic employee rating categorization
- **Department-specific Analysis**: Targeted queries for Finance and Healthcare teams
- **Union Operations**: Consolidated cross-departmental reporting

#### 📈 **Performance Analytics**
- **Rating-based Segmentation**: Employees categorized by performance levels
- **Experience Ranking**: DENSE_RANK() implementation for merit-based analysis
- **Salary Benchmarking**: Min/Max compensation analysis by role

#### 🎖️ **Role Standardization System**
Automated job profile validation using stored functions:
- `≤ 2 years` → **JUNIOR DATA SCIENTIST**
- `2-5 years` → **ASSOCIATE DATA SCIENTIST**
- `5-10 years` → **SENIOR DATA SCIENTIST**
- `10-12 years` → **LEAD DATA SCIENTIST**
- `12-16 years` → **MANAGER**

#### 💰 **Intelligent Bonus Calculation**
```sql
-- Performance-based bonus formula: 5% of salary × employee rating
(0.05 * SALARY * EMP_RATING) AS BONUS
```

## 🔧 Key SQL Features Utilized

### Window Functions & Analytics
- `MAX() OVER(PARTITION BY DEPT)` - Department-wise maximum ratings
- `DENSE_RANK() OVER(ORDER BY EXP DESC)` - Experience-based ranking
- Advanced grouping and aggregation functions

### Database Optimization
- **Index Creation**: Performance optimization for name-based searches
- **Execution Plan Analysis**: Query cost reduction strategies
- **Stored Procedures**: Reusable business logic encapsulation

### Advanced Data Operations
- **Nested Queries**: Complex filtering for experience-based analysis
- **Views Creation**: Streamlined access to high-salary international employees
- **Stored Functions**: Business rule automation and validation
