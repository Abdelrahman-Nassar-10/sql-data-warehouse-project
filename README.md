# sql-data-warehouse-project
building a database warehouse with SQL server, including ETL processes, data modeling, and analytics


# SQL Data Warehouse and Analytics Project

## Project Overview

This project demonstrates a complete **Data Warehouse and Analytics solution** built using **SQL Server**.  
The goal is to consolidate sales data from multiple source systems, clean and transform the data, and prepare it for analytical reporting and business decision-making.

This project follows common data engineering practices such as data ingestion, data cleaning, data modeling, and SQL-based analytics.

---

## Objective

Develop a modern data warehouse using **SQL Server** to consolidate sales data from multiple source systems, enabling analytical reporting and informed decision-making.

---

## Project Requirements

### 1. Building the Data Warehouse

#### Data Sources

The project uses data from two source systems:

- ERP system
- CRM system

The source data is provided as CSV files.

#### Data Quality

Before analysis, the data must be cleaned and checked for quality issues such as:

- Missing values
- Duplicate records
- Inconsistent formats
- Invalid or incorrect values
- Unmatched keys between datasets

#### Data Integration

The cleaned data from both source systems is integrated into a single, user-friendly data model designed for analytical queries.

#### Scope

The project focuses only on the latest available dataset.  
Historical data tracking is not required in this version.

#### Documentation

Clear documentation is provided to explain:

- The data model
- The transformation logic
- The purpose of each database layer
- The analytics outputs

---

## Data Warehouse Architecture

The data warehouse is organized into three main layers:

### Bronze Layer

The Bronze Layer stores raw data exactly as received from the source CSV files.

Purpose:

- Preserve the original source data
- Load ERP and CRM data without transformation
- Provide a backup layer for validation and debugging

### Silver Layer

The Silver Layer contains cleaned and standardized data.

Main operations:

- Remove duplicates
- Handle missing values
- Standardize naming conventions
- Fix data type issues
- Validate relationships between tables
- Prepare the data for business modeling

### Gold Layer

The Gold Layer contains the final business-ready data model.

Purpose:

- Create analytical views
- Build fact and dimension tables
- Support reporting and dashboarding
- Make the data easy to query for business users

---

## Data Model

The final data model follows a star schema design.

### Fact Table

The fact table stores measurable business events, such as sales transactions.

Example:

- Sales amount
- Quantity sold
- Order date
- Customer key
- Product key

### Dimension Tables

Dimension tables provide descriptive information for analysis.

Examples:

- Customers
- Products
- Dates
- Sales regions
- Categories

---

## Analytics and Reporting

SQL queries are used to generate insights from the final data model.

The analytics part of the project focuses on:

- Customer behavior
- Product performance
- Sales trends
- Revenue analysis
- Business performance over time

Example business questions answered by this project:

- Which products generate the highest revenue?
- Who are the top customers?
- How do sales change over time?
- Which categories perform best?
- What are the main sales trends?

---

## Tools and Technologies

- SQL Server
- T-SQL
- SQL Server Management Studio
- CSV files
- Data Warehouse Modeling
- Star Schema
- ETL Concepts
- GitHub

---




## About Me

My name is **Abdelrahman Nassar**. I am a Computer Science graduate focused on **Data Engineering, Data Analytics, SQL, and GIS**.

I work on designing structured data models, building SQL-based data pipelines, cleaning and integrating datasets, and preparing data for reporting and business analysis. My technical focus is on transforming raw data into reliable, analysis-ready systems that support better decision-making.

This project reflects my practical experience with **SQL Server, data warehousing, ETL concepts, data modeling, and analytical reporting**.
