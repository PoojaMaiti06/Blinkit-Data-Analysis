# Blinkit-Dashboard

### Dashboard Link 
https://app.powerbi.com/view?r=eyJrIjoiNjdhYmE0YTMtZDJkYi00MmU5LWEzOWItN2U0NDQ2ZGVhODQ2IiwidCI6ImUxNGU3M2ViLTUyNTEtNDM4OC04ZDY3LThmOWYyZTJkNWE0NiIsImMiOjEwfQ%3D%3D


## Problem Statement

The Blinkit Data Analysis project focuses on enhancing the company’s understanding of its sales performance, customer satisfaction, and inventory distribution. With a dataset of 8,523 rows, the objective is to analyze key metrics such as total sales, average sales, and customer ratings. By leveraging Power BI, the project aims to create insightful visualizations that highlight trends and opportunities for improvement.

These visualizations will cover various aspects, including sales by fat content, item type, outlet establishment, and location. The goal is to provide Blinkit with actionable insights that can drive data-driven decisions, leading to optimized inventory management, improved customer satisfaction, and enhanced overall sales performance across different outlets.


## KPI's Requirements

1. Total Sales: The overall revenue generated from all items sold.
2. Average Sales: The average revenue per sale.
3. Number of Items: The total count of different items sold.
4. Average Rating: The average customer rating for items sold.


## Chart's Requirements

1. Total Sales by Fat Content
2. Total Sales by Item Type
3. Fat Content by Outlet for Total Sales
4. Total Sales by Outlet Establishment:
5. Sales by Outlet Size:
6. Sales by Outlet Location
7. All Metrics by Outlet Type


## Steps In Project

### Requirement Gathering/ Business Requirements
1. Data Connection
2. Data Walkthrough

### Data Cleaning / Quality Check
1. Data Modeling
2. Data Processing
3. DAX Calculations

### Data Visualization
1. Dashboard Lay outing
2. Charts Development and Formatting Dashboard / Report Development


## Requirement Gathering/ Business Requirements

The dataset for the Blinkit Data Analysis project, comprises 8,523 rows 
and 12 columns, focusing on sales data analysis. The columns included are Item Fat Content, Item Identifier, Item Type, Outlet Establishment Year, Outlet Identifier, Outlet Location Type, Outlet Size, Outlet Type, Item Visibility, Item Weight, Sales, and Rating. This dataset provides a comprehensive view of various attributes related to items and outlets, enabling detailed analysis.

https://github.com/PoojaMaiti06/Blinkit-Data-Analysis/issues/1#issue-2502001107

## Data Cleaning / Quality Check

Data cleaning involves identifying and correcting errors or inconsistencies in a dataset to improve its quality and usability.

## Column Quality

Column quality refers to the assessment of the validity, accuracy, and completeness of data within each column of a dataset. It helps identify errors, missing values, and inconsistencies that could impact the reliability of the analysis.

https://github.com/PoojaMaiti06/Blinkit-Data-Analysis/issues/2#issue-2502003925

## Column Profile

A column profile is a summary of the key characteristics and distribution of data within a specific column of a dataset. It includes statistics such as the number of entries, distinct values, errors, and the frequency of each value, helping to understand the content and structure of the data in that column.

https://github.com/PoojaMaiti06/Blinkit-Data-Analysis/issues/3#issue-2502005410

## Column Distribution

Column distribution refers to the breakdown of data within a specific column, showing the frequency and proportion of each unique value. It helps in understanding how different values are represented in the dataset, revealing patterns, trends, and outliers.

https://github.com/PoojaMaiti06/Blinkit-Data-Analysis/issues/4#issue-2502007093

## Standardizing Data

Standardizing data is a crucial step in data preprocessing, ensuring consistency and improving the accuracy of analyses. In this context, standardizing involves replacing specific abbreviations or variations with a common term. 

### For instance, in the "Item Fat Content" column:
1. LF, low fat should be replaced with Low Fat to maintain uniformity in representing lowfat items.
2. Reg should be replaced with Regular to standardize the representation of regular-fat item.

https://github.com/PoojaMaiti06/Blinkit-Data-Analysis/issues/5#issue-2502008228

## DAX Calculation

DAX (Data Analysis Expressions) is a formula language used in Microsoft Power BI to create custom calculations and perform advanced data analysis. It helps users build formulas and expressions to aggregate, filter, and analyse data efficiently. DAX is essential for creating complex measures and calculated columns in data models.

### Total Sales
DAX can sum up the revenue from all sales records. This involves creating a measure that aggregates the sales amount column in your dataset.
           
            Total Sales = SUM('BlinkIT Grocery Data'[Sales])

### Average Sales
DAX can find average up the revenue from all sales records. This involves creating a measure that aggregates the sales amount column in your dataset.

            Avg Sales = AVERAGE('BlinkIT Grocery Data'[Sales])

### Number of Items 
DAX can count the distinct number of items sold. This involves creating a measure that counts the unique entries in the items column or table.

            No of Items = COUNTROWS('BlinkIT Grocery Data')

### Average Rating
DAX can compute the average customer rating by averaging the ratings across all sales records. This involves creating a measure that calculates the mean of the ratings column.

            Avg Rating = AVERAGE('BlinkIT Grocery Data'[Rating])

### Creating a New Metrix

            Metrix = {
               ("Total Sales", NAMEOF('BlinkIT Grocery Data'[Total Sales]), 0),
               ("Avg Sales", NAMEOF('BlinkIT Grocery Data'[Avg Sales]), 1),
               ("No of Items", NAMEOF('BlinkIT Grocery Data'[No of Items]), 2),
               ("Avg Rating", NAMEOF('BlinkIT Grocery Data'[Avg Rating]), 3)
            }


## Data Visualization

Data visualization is the graphical representation of data, making complex information easier to understand and analyze. It transforms data into visual elements like charts, graphs, and maps, enabling users to identify patterns, trends, and insights that may not be immediately apparent in raw data. Effective data visualization is crucial for decision-making, as it allows stakeholders to quickly grasp the significance of data and make informed decisions.

## Visualizations and Insights

### Total Sales by Fat Content

Regular fat items contribute more to total sales ($776.32K) than low-fat items ($425.36K), indicating higher customer preference for regular fat products.

https://github.com/PoojaMaiti06/Blinkit-Data-Analysis/issues/6#issue-2502010335

### Total Sales by Item Type

"Fruits and Vegetables" and "Snack Foods" are top-selling categories, each generating $0.18M, followed by "Household" and "Frozen Foods."

https://github.com/PoojaMaiti06/Blinkit-Data-Analysis/issues/7#issue-2502011236

### Fat Content by Outlet for Total Sales

Tier 3 outlets lead in sales for regular fat items ($0.31M), while Tier 1 performs better with low-fat items ($0.22M), suggesting regular fat 
products are more popular in lower-tier outlets.

https://github.com/PoojaMaiti06/Blinkit-Data-Analysis/issues/8#issue-2502012630

### Total Sales by Outlet Establishment

Sales peaked in 2018 at $205K but have since stabilized around $130K-$132K, indicating a plateau in performance for newer outlets.

https://github.com/PoojaMaiti06/Blinkit-Data-Analysis/issues/9#issue-2502013903

### Sales by Outlet Size

Large outlets dominate with $507.90K in sales, followed by medium ($444.79K) and small outlets ($248.99K).

https://github.com/PoojaMaiti06/Blinkit-Data-Analysis/issues/10#issue-2502014920

### Sales by Outlet Location

Tier 3 locations lead in sales ($472.13K), suggesting outlets in less urbanized or more affordable areas are more profitable.

https://github.com/PoojaMaiti06/Blinkit-Data-Analysis/issues/11#issue-2502016041

### All Metrics by Outlet Type

Supermarket Type 1 leads in total sales ($787.55K) and the number of items sold (5,577), though it has lower item visibility. Grocery stores, while having 
lower sales, maintain consistent average sales and ratings.

https://github.com/PoojaMaiti06/Blinkit-Data-Analysis/issues/12#issue-2502016987

## Conclusion

The Blinkit sales data project involved analysing 8,523 rows and 12 columns of product and outlet information, which were meticulously cleaned and processed for accuracy. The resulting Power BI dashboard provides a comprehensive overview of key metrics like total sales, average sales, number of items, and average ratings. It effectively visualizes sales distribution across various dimensions, including item type, fat content, and outlet characteristics, with interactive filters for deeper insights. This project highlights the power of data analysis and visualization in driving informed business decisions and enhancing strategic planning.
