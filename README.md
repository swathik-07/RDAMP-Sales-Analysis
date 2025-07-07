# RDAMP-Sales-Analysis
## About the Project
This repository contains my submission for Task 1 of the RDAMP program. The project involves cleaning raw sales data using Python and performing business analysis with Power BI to uncover insights related to regional performance, discount strategies, and product-level profitability.

## Tools Used

- Python (Pandas) - data cleaning and preparation
- Power BI - creating interactive dashboards and visualizations
- GitHub - version control, project submission and portfolio presentation

## My Approach

### Data Cleaning (Python):

1. Loaded sales data and store location data using pandas.
2. Fixed missing Country and Region values:
    - Merged both datasets using Postal Code.
    - Filled missing values from the store mapping.
3. Fixed missing Category values:
    - Mapped each Sub-Category to its most common Category.
    - Manually filled any unmatched cases (e.g., “Dog Supplies” - “Pets”).
4. Filled missing Discount values with 0.0.
5. Exported the cleaned data to a CSV file for Power BI analysis.

### Visualization (Power BI):

1. Imported the cleaned dataset from CSV.
2. Converted and corrected data types (e.g., Dates, Numeric fields like Total Sales, Profit, Cost Price).
3. Created calculated columns/measures using DAX:
	  - Total Sales, Profit, Profit Margin, Discount %
4. Handled inconsistent date formats (e.g., U.S. date + DateTime) to enable proper time series analysis.
5. Split Category column using the '-' delimiter to extract Segment information.
6. Standardized column names for easier navigation and consistency.
7. Designed visual pages to highlight:
	  - Sales trends over time
	  - Segment-level discount and profit patterns
	  - Regional and product performance
8. Added slicers for Region, Category, and Year to enable dynamic filtering.
9. Used conditional formatting and comparative visuals to highlight underperformance and key drivers


## Key Insights

1. Online vs In-Store Behavior
Online sales slightly outperformed in-store sales in both revenue and profit.
However, both channels performed strongly, with relatively balanced contribution.

2. Regional Sales Gaps
Regions like Yorkshire & the Humber, East of England, Wales, and Northern Ireland underperformed in both sales and profit.
High discount rates in some of these areas (e.g., East of England) did not lead to increased profitability, suggesting discount ineffectiveness.

3. Profitability by Category
Outdoor, Kitchen and Clothing categories are the most profitable and strong revenue.
In contrast, Food and Home Improvement categories generated reasonable sales but lower margins.

4. Segment-Level Discounts
Segments like Jams & Jellies, Home Improvement, and Canned Soups consistently applied high average discounts (up to ~28%).
These segments require review, as heavy discounting may be cutting into profitability.

5. Top vs Underperforming Products
Electric Bike and Portable Refrigerator were among the best-selling products.
On the other hand, items like Rice Pudding and Zucchini showed low or negative profits despite sales activity, highlighting inefficiency in certain Food subcategories.

## Sample Visualizations

- Online vs In-Store Sales Distribution

<img width="193" alt="image" src="https://github.com/user-attachments/assets/c7565458-a4fb-4e3f-b42d-45fc5142e043" />

- Segment-wise Discount Trends

<img width="404" alt="image" src="https://github.com/user-attachments/assets/07f87a81-61ea-4af9-ad2c-8200f1b14604" />

- Top Best selling Products by Sales

<img width="227" alt="image" src="https://github.com/user-attachments/assets/a5510976-002b-461e-976b-877fd657443d" />

- Profitability by Category

<img width="417" alt="image" src="https://github.com/user-attachments/assets/513800e7-c94b-4641-afa4-9d2f61e2822f" />

## Submission Summary

This task provided valuable hands-on experience in transforming raw data into meaningful insights. By combining Python's data preparation capabilities with Power BI's rich visualizations, I was able to highlight key trends, identify underperforming regions, and evaluate product profitability.

