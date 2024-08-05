# Home_Sales
Module 22 challenge

This project involves analyzing home sales data using PySpark to answer specific business questions. The instructions and requirements are outlined below.

## Instructions
File Renaming:

Rename the Home_Sales_starter_code.ipynb file to Home_Sales.ipynb.
Imports:

Import the necessary PySpark SQL functions for this assignment.
Data Loading:

Read the home_sales_revised.csv data into a Spark DataFrame.
Temporary Table Creation:

Create a temporary table called home_sales.

## SparkSQL Queries:

Answer the following questions using SparkSQL:

1. What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.
2. What is the average price of a home for each year the home was built, that has three bedrooms and three bathrooms? Round off your answer to two decimal places.
3. What is the average price of a home for each year the home was built, that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.
4. What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? 
5. Determine the run time for this query, and round off your answer to two decimal places.
### Run time = 2.5374979972839355 seconds

## Caching:

Cache your temporary table home_sales.
Check if your temporary table is cached.
Query on Cached Data:

Using the cached data, run the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
### Run time = 1.959306001663208 seconds
### This runtime is approximately 0.6 seconds faster than before cahing was done



## Partitioning and Parquet:

Partition by the date_built field on the formatted Parquet home sales data.
Create a temporary table for the Parquet data.
Run the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
### Run time = 1.5922563076019287 seconds
### This runtime is approximately 0.4 seconds faster than before caching was done


## Uncaching:

Uncache the home_sales temporary table.
Verify that the home_sales temporary table is uncached using PySpark.


