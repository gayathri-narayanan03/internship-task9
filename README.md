# Task 9 – SQL Data Modeling (Star Schema)

## Objective
Design and implement a Star Schema using the Global Superstore dataset to understand warehouse modeling for BI reporting.

## Dataset
Global Superstore (Retail Sales Data)

## Schema Design

### Fact Table
Fact_Sales
- customer_key (FK)
- product_key (FK)
- date_key (FK)
- region_key (FK)
- sales
- quantity
- discount
- profit
- shipping_cost

### Dimension Tables
Dim_Customer
- customer_key (PK)
- customer_id
- customer_name
- segment

Dim_Product
- product_key (PK)
- product_id
- product_name
- category
- sub_category

Dim_Date
- date_key (PK)
- order_date
- year
- month
- quarter

Dim_Region
- region_key (PK)
- country
- state
- city
- region
- market

## Steps Performed
1. Identified fact and dimension tables.
2. Created tables with primary and foreign keys.
3. Inserted distinct records into dimensions.
4. Mapped fact records to dimension keys.
5. Created indexes on join keys.
6. Ran analytical queries.
7. Validated record counts and relationships.

## Deliverables
- task9_star_schema.sql
- star_schema_diagram.png
- analysis_outputs.csv

## Outcome
Built a structured Star Schema for efficient BI reporting and analytics.
