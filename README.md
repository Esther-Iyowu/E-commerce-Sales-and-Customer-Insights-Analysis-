# E-commerce-Sales-and-Customer-Insights-Analysis-
 An end-to-end e-commerce sales analysis project using Excel and MySQL, covering data cleaning, exploratory data analysis, SQL querying, business insights, and interactive dashboard development.




## Project Overview

This project involves an end-to-end analysis of an e-commerce sales dataset to understand sales performance, customer purchasing behaviour, product performance, and marketing channel effectiveness.

The project follows a structured data analysis process, beginning with data cleaning and preparation in Microsoft Excel, followed by exploratory data analysis (EDA), SQL querying using MySQL, and the development of an interactive Excel dashboard.

The objective is to transform raw sales data into meaningful insights, identify business performance trends, and provide actionable recommendations that can support informed decision-making.

## Tools Used

- **Microsoft Excel:** Data cleaning, exploratory data analysis, descriptive statistics, correlation analysis, pivot tables, and dashboard development.
- **MySQL:** Data querying, filtering, sorting, aggregation, and trend analysis.
- **MySQL Workbench:** SQL query execution and database management.
- **GitHub:** Project documentation and version control.

## Project Workflow

### 1. Data Cleaning and Preparation (Microsoft Excel)

The project began with an audit and cleaning of a raw sales dataset containing 14 columns covering transaction details, customer information, product data, payment methods, order status, shipping information, and marketing referral sources.

The following cleaning processes were performed:

- **Duplicate Check:** Audited all 14 columns using Conditional Formatting and the Remove Duplicates feature. No duplicate records were found.
- **Date Standardisation:** Reviewed and standardised date entries to ensure consistent formatting and chronological sorting.
- **Financial Data Formatting:** Standardised the Unit Price and Total Price columns for numerical consistency.
- **Text Standardisation:** Used Excel's `PROPER()` function to correct inconsistent text casing in Product, Payment Method, and Order Status entries.
- **Missing Value Treatment:** Identified blank Coupon Code entries and replaced them with "No Coupon" using Go To Special > Blanks. This preserved the distinction between transactions with and without coupon usage.
- **Structural Formatting:** Improved the dataset's organisation through consistent headers, formatting, and alignment.

The cleaned dataset was prepared for subsequent exploratory analysis and SQL querying.

### Raw Dataset Before Cleaning

![Dataset before cleaning](Before%20Cleaning.png)


*Original dataset showing inconsistencies and data quality issues before cleaning*.


### Dataset After Cleaning

![Dataset After Cleaning](After%20Cleaning.png)


*Dataset after cleaning, with inconsistencies addressed and data prepared for analysis*.

### 2. Exploratory Data Analysis (Microsoft Excel)

Exploratory Data Analysis was performed in Excel to identify patterns, trends, relationships, and potential business opportunities within the dataset.

Techniques applied included:

- Pivot tables and data aggregation.
- Descriptive statistics using the Data Analysis ToolPak.
- Time-series and monthly sales trend analysis.
- Comparative analysis of products, payment methods, and referral sources.
- Correlation analysis.
- Charts and visualisations.

The EDA workbook was organised into multiple sheets, including Cleaned Data, Descriptive Statistics, Pivot Tables, Visualisations, and Key Observation Summary.

### 3. SQL Analysis (MySQL)

MySQL was used to query and further explore the cleaned sales dataset.

The analysis focused on answering business questions such as:

- How many orders were processed?
- What was the total revenue generated?
- Which products generated the highest sales?
- Which payment methods were most frequently used?
- Which referral source generated the most orders?
- What were the monthly sales trends?
- Which months recorded the highest and lowest sales?

SQL techniques applied included:

- `SELECT` for data retrieval.
- `WHERE` for filtering records.
- `ORDER BY` for sorting results.
- `GROUP BY` for aggregating data by categories.
- `COUNT()`, `SUM()`, and `AVG()` for calculating business metrics.
- `LIMIT` for identifying top-performing records.
- Date-based aggregation for monthly sales trend analysis.

### 4. Data Visualisation and Dashboard Development (Microsoft Excel)

An interactive Excel dashboard titled **E-commerce Sales and Customer Insights Dashboard** was developed to present key performance indicators and business findings in an accessible visual format.

**Key Performance Indicators (KPIs)**

- Total Revenue
- Total Orders
- Total Quantity Sold
- Average Unit Price

**Dashboard Visualisations**

- Monthly Revenue Trends
- Top 5 High-Value Customers
- Customer Acquisition by Referral Source
- Order Status Analysis
- Product Performance
- Payment Method Analysis

![Dashboard Visualization](E-commerce%20dashboard.png)

*The dashboard provides an overview of sales performance and customer activity, making it easier to identify trends and areas requiring business attention*.

## Key Insights and Findings

The analysis revealed the following:

- **Top Product by Sales Volume:** Chair recorded the highest sales volume among the products analysed.
- **Preferred Payment Method:** Online payment was the most frequently used payment method.
- **Leading Referral Source:** Instagram recorded the highest contribution among the referral sources analysed.
- **Peak Sales Month:** June 2024 recorded the highest sales performance.
- **Lowest Sales Month:** April 2023 recorded the lowest revenue performance.
- **Total Orders:** 1,200 orders were recorded in the dataset.
- **Outlier Detection:** Eight outliers were identified during the statistical analysis.
- **Order Status:** A notable number of cancelled orders was observed, highlighting a potential area of revenue leakage that requires further investigation.

### Correlation Analysis

Correlation analysis was conducted to understand relationships between selected numerical variables.

| Variables | Correlation | Interpretation |
|---|---:|---|
| Unit Price and Quantity | 0.014553 | Almost no linear relationship between unit price and quantity purchased. |
| Quantity and Total Price | 0.615251 | Moderate positive relationship, suggesting that larger purchase quantities are generally associated with higher transaction values. |

## Business Recommendations

Based on the findings from the analysis, the following recommendations are proposed:

1. **Strengthen Customer Acquisition Through Effective Channels:** Instagram recorded the highest contribution among referral sources. The business should evaluate its Instagram marketing activities and identify opportunities to strengthen customer acquisition through this channel.

2. **Improve Customer Retention:** Develop customer engagement initiatives and loyalty strategies that encourage repeat purchases, particularly among high-value customers.

3. **Optimise Product Inventory:** Prioritise inventory planning for high-volume products such as chairs while monitoring the performance of other products to make informed stocking decisions.

4. **Investigate Order Cancellations:** Review the reasons behind cancelled orders to identify possible issues with payment, order processing, product availability, or delivery. Addressing these issues could help reduce potential revenue losses.

5. **Plan Around Sales Trends:** Use monthly sales performance to identify high-performing and low-performing periods. Marketing campaigns and inventory planning can be adjusted accordingly.

6. **Maintain Convenient Payment Options:** Since online payment was the most preferred method, the business should continue to provide a reliable and seamless online payment experience while monitoring other payment preferences.

## Project Structure

The repository is organised into the following folders:

```text
ecommerce-sales-and-customer-insights/
│
├── README.md
│
├── Dataset/
│   ├── Raw_Dataset.xlsx
│   └── Cleaned_Dataset.xlsx
│
├── Data-Cleaning/
│   └── Data_Cleaning.xlsx
│
├── EDA/
│   └── Exploratory_Data_Analysis.xlsx
│
├── SQL-Queries/
│   └── SQL_Data_Analysis.sql
│
└── Visualization/
    ├── E-commerce_Dashboard.xlsx
    └── Dashboard_Screenshot.png
```

*Note: Folder and file names should be adjusted to match the actual files uploaded to the repository.*

## Conclusion

This project demonstrates an end-to-end approach to sales data analysis, combining Microsoft Excel and MySQL to transform raw transactional data into meaningful business information.

Through data cleaning, exploratory analysis, SQL querying, statistical techniques, and dashboard development, the project highlights important patterns in sales performance, customer behaviour, product activity, and marketing effectiveness.

Beyond the technical analysis, the findings provide a foundation for business recommendations aimed at improving customer acquisition, product planning, sales performance, and operational efficiency.
