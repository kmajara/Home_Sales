Home Sales Analysis with SparkSQL
Project Overview

This project involves analyzing home sales data using SparkSQL to answer specific questions related to home prices. The tasks include creating a temporary table, performing various queries to calculate average home prices based on different criteria, caching data for performance optimization, and comparing runtimes between cached and uncached data.
Getting Started
Prerequisites

    Apache Spark
    PySpark
    Jupyter Notebook or any other Python IDE

Dataset

The dataset used in this project contains information about home sales, including features like the number of bedrooms, bathrooms, floors, square footage, year built, and view rating.
Project Tasks
1. Create a Temporary Table

Create a temporary table called home_sales to facilitate querying with SparkSQL.
2. Questions to Answer

    Average Price for Four-Bedroom Houses:
        Calculate the average price for a four-bedroom house sold for each year. Round off the answer to two decimal places.
    Average Price for Homes Built with Specific Features:
        Calculate the average price of homes for each year they were built, with the following criteria:
            Three bedrooms and three bathrooms.
            Three bedrooms, three bathrooms, two floors, and a minimum of 2,000 square feet.
        Round off the answers to two decimal places.
    Average Price per "View" Rating:
        Calculate the average price of a home per "view" rating where the average home price is greater than or equal to $350,000. Determine the runtime for this query and round off the answer to two decimal places.

3. Cache the Temporary Table

Cache the home_sales temporary table to optimize query performance.
4. Verify Caching

Check if the home_sales temporary table is cached using PySpark.
5. Compare Runtimes with Cached Data

Using the cached data, rerun the query that calculates the average price of a home per "view" rating where the average home price is greater than or equal to $350,000. Determine the runtime and compare it to the uncached runtime.
6. Partition the Data by "date_built"

Partition the home sales data by the date_built field and save it as a formatted Parquet file.
7. Create a Temporary Table for Parquet Data

Create a new temporary table from the partitioned Parquet data.
8. Rerun the Query with Partitioned Data

Rerun the query calculating the average price of a home per "view" rating where the average home price is greater than or equal to $350,000. Determine the runtime and compare it to previous runtimes.
9. Uncache the Temporary Table

Uncache the home_sales temporary table to free up memory.
10. Verify Uncaching

Verify that the home_sales temporary table is uncached using PySpark.
