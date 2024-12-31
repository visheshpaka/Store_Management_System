# Store Management System

## Project Overview
The **Store Management System** project aims to design and implement a robust database application for managing supermarket operations effectively. This system helps store managers and owners track essential business aspects, such as inventory management, supplier relationships, customer transactions, and promotions, enabling data-driven decisions to improve sales and operational efficiency.

---

## Key Features
- **Centralized Management**: Consolidates all store data, including employee records, product categories, and supplier details.
- **Improved Inventory Tracking**: Monitors stock levels, expiry dates, and popular products.
- **Enhanced Customer Insights**: Tracks customer plans, purchases, and applied promotions.
- **Analytical Reporting**: Generates valuable business insights, such as top-performing employees, popular plans, and sales trends.
- **Integration**: Implements both **MySQL** and **NoSQL** for flexible data management and query capabilities.

---

## Business Problem
Managing a supermarket involves tracking numerous variables, including product availability, expiry dates, and inventory levels. Traditionally, businesses rely on paper-based records, prone to errors, losses, and inefficiency. This project addresses these challenges by implementing a database-driven store management system that improves decision-making and productivity.

---

## System Design

### Conceptual Data Modeling
An **Enhanced Entity-Relationship (EER) Diagram** is used to model the relationships between entities, including:
- **Stores**: Managed by employees, uniquely identified by an `employee_id`.
- **Products**: Supplied by suppliers and categorized by product categories.
- **Customers**: Enroll in plans and make purchases, generating orders and invoices.
- **Promotions**: Applied to plans to attract customers.

### Relational Model
The conceptual model is mapped to a relational database schema in **MySQL** with primary keys, foreign keys, and relationships to ensure data integrity. Key tables include:
- **EMPLOYEE**: Stores employee details with references to the store they work at.
- **PRODUCT**: Tracks product details, including price, expiry date, and supplier.
- **ORDER & INVOICE**: Records customer transactions and payments.
- **PLAN_PROMOTION**: Links plans to applicable promotions.

---

## Implementation

### MySQL Queries
- **Discount Analysis**: Identify the highest discount given to a customer.
- **Employee Performance**: Track employees who processed the most invoices.
- **Popular Products**: Find products with high demand to ensure stock availability.
- **Plan Recommendations**: Analyze popular plans and recommend them to new customers.
- **Store Insights**: Identify stores with the highest number of employees or sales.

### NoSQL Queries
Implemented using **MongoDB** to handle unstructured data, enabling flexible aggregation and MapReduce functionalities. Key analyses include:
- **Average and Maximum Salary**: Calculate salary statistics per store.
- **Employee and Customer Counts**: Count employees and customers by store or plan.

### Database Access via Python
- **Integration**: Accessed the MySQL database through **Jupyter Notebook** using Python.
- **Visualization**:
  - **Employee Distribution**: Pie chart showing employee count distribution across stores.
  - **Order Trends**: Bar chart comparing monthly orders in 2021 and 2022.
  - **Salary Insights**: Boxplot displaying salary distribution.

---

## Results and Insights
- **Popular Products and Plans**: Identified for better inventory and promotional strategies.
- **Employee Performance**: Fostered a competitive environment through recognition programs.
- **Sales Trends and Customer Preferences**: Provided actionable insights to optimize business operations.

---

## How to Use

### Setup Database
1. **MySQL Setup**:
   - Import `SQL_Script.sql` into MySQL.
    
### Run Queries
- Execute predefined analyses using `SQL_Script.sql`.

### Visualize Data
1. Run Data_Visualization_python_script.py to generate visual insights using Python libraries like **Seaborn** and **Plotly**.

---

## Future Enhancements
- **Real-Time Tracking**: Integrate real-time inventory and sales monitoring.
- **Machine Learning Models**: Predict customer preferences and optimize promotions.
- **Enhanced Analytics**: Expand visualization capabilities with more dashboards.
