# Write a query that will return every column & every row from the dataset:
SELECT
    *
FROM
    banking_data;

# Return the first 5 rows of the table (only the borrower & due to IDA column):
SELECT 
    borrower, 
    "Due to IDA" 
FROM 
    banking_data
LIMIT
    5; 

# Refer to that column as "due" instead of "Due to IDA". Select the region & due column & limit the response to the first 20 rows:
SELECT 
    region, 
    "Due to IDA" AS due 
FROM 
    banking_data 
LIMIT 20;

# Return all transactions where the country is equal to Nicaragua:
SELECT 
    *  
FROM 
    banking_data 
WHERE 
    country = 'Nicaragua';

# How many rows are in this banking table?:
SELECT 
    COUNT(*)  
FROM 
    banking_data;

# How many rows in the table are from the country Nicaragua?:
SELECT 
    COUNT("Due to IDA") 
FROM 
    banking_data 
WHERE country = 'Nicaragua';

# Return the number of transactions per country:
SELECT 
    country, 
    COUNT(*) 
FROM 
    banking_data 
GROUP BY 
    country;

# Find the max owed to the IDA:
SELECT 
    MAX("Due to IDA") 
FROM 
    banking_data;

# How much is owed to the IDA?:
SELECT 
    SUM("Due to IDA") 
FROM 
    banking_data;

# What is the average service charge rate for a loan?:
SELECT
    AVG("Service Charge Rate")
FROM
    banking_data;

# Find out what transactions have the lowest service charge rate. Return all columns. Place the smallest rates at the top:
SELECT 
    * 
FROM 
    banking_data 
ORDER BY 
    "Service Charge Rate" ASC;

# Return all loans from the country of Honduras where the service charge rate is larger than 1:
SELECT 
   * 
FROM 
   banking_data 
WHERE 
   country = 'Honduras' AND "Service Charge Rate" > 1;

# Return the loans that have a project name of 'COTTON' or the name of 'RIVER':
SELECT 
   * 
FROM 
   banking_data 
WHERE 
   "Project Name" = 'COTTON' OR "Project Name" = 'RIVER';

# Return all the loans that are not of the project name 'COTTON':
SELECT 
   * 
FROM 
   banking_data 
WHERE 
   NOT "Project Name" = 'COTTON';


