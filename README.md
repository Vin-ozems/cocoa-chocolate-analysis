# cocoa-chocolate-analysis

## Overview
This repository contains the SQL scripts and documentation for the cocoa/chocolate analysis project. The database is designed to manage information related to cocoa and their exportation across continents.

## Database Schema
The database schema is organized into the following tables:
- cocoa_id 
- company_name 
- bean_origin ,
- review_year 
- cocoa_percent 
- company_location 
- rating 
- bean_type 
- broad_bean_origin 

## Setup
To set up the database, follow these steps:

1. Database Creation: Execute the `create_database.sql` script to create the initial database.   
2. Table Creation: Run the `create_tables.sql` script to create the necessary tables.
3. Data Population using MYSQL import wizard
4.feature engineering
5.EDA cocoa/chocholate dataset

## Sample Queries
Here are some sample SQL queries to get you started:
1. What is the distribution of ratings for chocolates with different bean types?
```sql
SELECT bean_type, 
       COUNT(*), 
       MAX(rating), 
       MIN(rating)
FROM cocoa
GROUP BY bean_type;
```

   
