# Customers and Products Analysis Using SQL



 📊 Project Overview

This SQL analytics project transforms raw sales data from a scale model car company into actionable business intelligence. By answering three critical business questions, we demonstrate how data-driven decisions can optimize inventory, enhance customer relationships, and guide marketing investments.

## 🎯 Business Questions Answered

### 1. Inventory Optimization
**"Which products should we order more of or less of?"**
- Identifies low-stock, high-performance products
- Prevents stockouts of best-selling items
- Optimizes inventory investment

### 2. Customer Segmentation  
**"How should we tailor marketing strategies to customer behaviors?"**
- Identifies VIP (high-profit) customers
- Pinpoints less-engaged customers
- Enables targeted communication strategies

### 3. Marketing Investment
**"How much can we spend on acquiring new customers?"**
- Calculates Customer Lifetime Value (LTV)
- Guides marketing budget allocation
- Predicts future profit from new customers

## 🗄️ Database Schema

The project analyzes a comprehensive sales database with 8 tables:

- **Customers**: Customer master data
- **Products**: Product catalog and inventory
- **Orders**: Sales order headers
- **OrderDetails**: Sales order line items
- **Payments**: Customer payment history
- **Employees**: Sales team information
- **Offices**: Regional office details
- **ProductLines**: Product category hierarchy

## 🛠️ Technical Implementation

### SQL Features Demonstrated
- **Complex JOIN operations** across multiple tables
- **Correlated subqueries** for advanced calculations
- **Common Table Expressions (CTEs)** for query organization
- **Aggregate functions** with GROUP BY
- **Window functions** for ranking and analysis
- **Mathematical operations** for business metrics

### Key Metrics Calculated
- **Low Stock Ratio**: `SUM(quantityOrdered) / quantityInStock`
- **Product Performance**: `SUM(quantityOrdered * priceEach)`
- **Customer Profit**: `SUM(quantityOrdered * (priceEach - buyPrice))`
- **Customer Lifetime Value (LTV)**: Average customer profit

## 📈 Key Findings

### Inventory Insights
- **Vintage Cars** and **Motorcycles** are priority for restocking
- Top products show high demand with low inventory levels
- Strategic reordering can prevent $390K+ in potential lost sales

### Customer Analysis
- **VIP Customers** generate 60x more profit than average customers
- Geographic concentration in Spain, USA, and Australia
- Opportunity to develop loyalty programs for high-value segments

### Marketing Strategy
- **LTV per customer**: $39,039
- Justified marketing spend up to $390K for 10 new customers
- Data supports aggressive customer acquisition campaigns

## 🚀 Quick Start

### Prerequisites
- MySQL Database
- Sample database loaded ([ClassicModels](https://www.mysqltutorial.org/mysql-sample-database.aspx))

