# 📊 Data Directory

## Overview
This directory contains the core datasets used in the SKLOTH E-Commerce Sales Dashboard project. The data represents a comprehensive e-commerce transaction dataset with customer, product, and sales information.

## Data Files

### 1. Orders_clean.csv
**Description**: Master order information with customer and location details
- **Records**: 327 unique orders
- **Date Range**: July 2018 - December 2018
- **Geographic Coverage**: 15+ states across India

**Schema:**
| Column | Data Type | Description |
|--------|-----------|-------------|
| Order ID | String | Unique identifier for each order (Primary Key) |
| Order Date | Date | Date when the order was placed |
| CustomerName | String | Customer's name |
| State | String | Customer's state |
| City | String | Customer's city |

### 2. Details.csv
**Description**: Detailed transaction information with product and financial data
- **Records**: 1,501 transaction line items
- **Products**: 4 major categories with 15+ subcategories
- **Financial Data**: Revenue, profit, and quantity metrics

**Schema:**
| Column | Data Type | Description |
|--------|-----------|-------------|
| Order ID | String | Order identifier (Foreign Key) |
| Amount | Currency | Revenue amount for the transaction |
| Profit | Currency | Profit amount for the transaction |
| Quantity | Integer | Number of items purchased |
| Category | String | Product category |
| Sub-Category | String | Product subcategory |
| PaymentMode | String | Payment method used |

## Data Quality

- **Completeness**: 100% data coverage across all required fields
- **Consistency**: Standardized formats and naming conventions
- **Accuracy**: Cross-validated relationships between tables
- **Timeliness**: Recent data suitable for trend analysis

## Usage Guidelines

- Load CSV files into Power BI via Power Query
- Use Orders_clean.csv as the Orders table
- Use Details.csv as the transaction details table
- Model as a star schema for best performance

---

**Note**: This dataset is for educational and portfolio demonstration purposes only. No real customer data is included. 