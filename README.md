# Sales Analysis

## Project Overview

This project aims to derive insights into the food delivery business, its successes, and challenges. The objective of this project is to measure the delivery performance, analyse the revenue and profitability, analyse the drivers’ efficiency, understand customer ordering behavior

### Data Source

The data is sourced from [FP20 Analytics](https://fp20analytics.com/datasets/)

### Tools

- Power BI

 

  
 ### Data Cleaning/Preparation

 1. The data was imported into Power Query, and the following steps were taken to clean and prepare the data for analysis:
 2. The datatype of the time columns was corrected from datetime to time.
 3. The values of the columns were checked for errors and wrong syntax. There was none observed.
 4. A new column was created for the time of day of the order placed (morning, afternoon, and night).
 5. The table was duplicated, and a dimension table was created for the driver (driver ID and driver name), and duplicates were removed.
 6. In the fact table, the driver name column was removed.
 7. Empty cells in each column were removed.

### Data Modelling

Moving into the Power BI interface, the first thing done under data modelling was creating a dimension date table using DAX. This was done using the formula below.
[put the image]
The next step was to turn off the auto time intelligence in the settings and mark the above table as the date table.
Furthermore, a one-to-many relationship was created between the dimension tables and the fact table.
[put the image]
A new column was created to get the total delivery time using the formula below.
[put the image]
The following DAX formulas were created for the analysis:
[put the images]


