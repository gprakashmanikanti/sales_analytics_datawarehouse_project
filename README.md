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

![*data_integration*](./images/schema.png "data_integratios")
Merge ERP sales data with CRM customer data.
Use common keys (e.g., customer_id, product_id) to join datasets.
Store final data in a star schema model (Gold Layer).


### SQL Server Tables and Views structure
![*Tables and Views structure*](./images/sql_server_sc.png "Tables and Views structure")

### Analytical queries
##### 1. Monthly Sales Trend

![*Monthly Sales Trend*](./images/Analytical_query_1.png "Monthly Sales Trend")

##### 2. Year-over-Year Growth in Sales

![*Year-over-Year Growth in Sales*](./images/Analytical_Query_2.png "Year-over-Year Growth in Sales")
