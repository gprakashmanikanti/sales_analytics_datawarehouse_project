# sales_analytics_datawarehouse_project

## overview

 This project showcases a complete data warehousing and analytics solution, following  best practices in data engineering, ETL, and analytics. It demonstrates how to build a modern data warehouse from raw data ingestion to business-ready insights using SQL Server and SQL-based reporting.

 ## Data Architecture

 ![*data_architecture*](./images/data_architecture.drawio.svg "data_architecture")

1. Bronze Layer: Stores raw data as-is from the source systems. Data is ingested from CSV Files into SQL Server Database.
2. Silver Layer: This layer includes data cleansing, standardization, and normalization processes to prepare data for analysis.
3. Gold Layer: Houses business-ready data modeled into a star schema required for reporting and analytics.

# Project Overview

1. Data Architecture: Designing a Modern Data Warehouse Using Medallion Architecture Bronze, Silver, and Gold layers.
2. ETL Pipelines: Extracting, transforming, and loading data from source systems into the warehouse.
3. Data Modeling: Developing fact and dimension tables optimized for analytical queries.
4. Analytics & Reporting: Creating SQL-based reports and dashboards for actionable insights.

# Building the Data Warehouse 

Develop a modern data warehouse using SQL Server to consolidate sales data from ERP and CRM systems. This enables analytical reporting and informed decision-making.

## Specifications
#### Data Sources
Source 1: ERP System → Contains sales transactions, order details, and revenue.
Source 2: CRM System → Contains customer details, demographics, and interactions.
Data Format: CSV files
Data Storage: Initially stored in SQL Server staging tables (Bronze Layer).

#### Data Quality
Handle missing values and duplicates.
Standardize date formats, product codes, and customer identifiers.
Ensure data consistency between ERP & CRM.

#### Integration
Merge ERP sales data with CRM customer data.
Use common keys (e.g., Customer_ID, Order_ID) to join datasets.
Store final data in a star schema model (Gold Layer).

#### Scope
Transformations: Aggregations, standardizations, and calculations to ensure data readiness.

#### Documentation
Provide ERD (Entity-Relationship Diagram).
Maintain data dictionary with column definitions, data types, and transformations.
Include SQL scripts for table creation and ETL process.