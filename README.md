# Retail Sales Dashboard

### Dashboard File: `sales_analysis_powei_bi_dashboard.pbix` (included in this repository)

## Problem Statement

This dashboard helps a retail business understand its sales, profit, and discounting performance across products, cities, customers, and promotions. It allows stakeholders to quickly answer key business questions such as:

1. Which products are the top and bottom performers by sales, profit, and quantity sold?
2. How do sales trends vary over time (daily, monthly, quarterly, annually)?
3. What is the relationship between sales and profit?
4. How do sales, profit, and quantity sold compare between any two user-selected periods?
5. What is the average discount offered in each discount category?
6. What is the total number of orders?
7. What are the sales, profit, discount, net sales, and other details for each individual order, filterable by product, date, customer, and promotion?
8. How do sales vary across different cities?

By answering these questions, the business can identify its best- and worst-performing products, track sales trends over time, evaluate the impact of discount campaigns, and drill down into order-level detail for deeper analysis.

## Steps Followed

- **Step 1:** Loaded the sales data into Power BI Desktop from an Excel source file.
- **Step 2:** Cleaned and profiled the data in Power Query Editor (checked column distribution, column quality, and column profile based on the entire dataset).
- **Step 3:** Created measures — **Net Sales**, **Units Sold**, **PROFIT**, **Avg Discount %**, and **Total Orders** — and used them to build the KPI card visuals on the **Overview** page.
- **Step 4:** Added a line chart (Date vs. Net Sales) with a range slider on the Overview page to show the sales trend over time.
- **Step 5:** Added a bar chart of **Product Name vs. Net Sales** (Top 5 products) and a clustered bar chart of **City vs. Net Sales** on the Overview page, plus a scatter chart plotting **Net Sales vs. PROFIT** to visualize their relationship.
- **Step 6:** Built a dedicated **Top/bottom** page with six bar charts: Top 5 and Bottom 5 products by Net Sales, by PROFIT, and by Units Sold — each broken down by Product Name.
- **Step 7:** Built a **Sale trend** page with the Net Sales vs. PROFIT scatter chart, a Date vs. Net Sales line chart, a City vs. Net Sales bar chart, and a bar chart of **Discount Value by Promotion Name** to compare discounting across promotional campaigns.
- **Step 8:** Built a **compare with dates** page with two independent Date slicers, each paired with its own set of Net Sales, Units Sold, and PROFIT bar charts — letting users select any two time periods and compare them side by side.
- **Step 9:** Built a **table** page with a detailed order-level table (CustomerID, Date, Discount Percentage, Discount Value, Net Sales, PROFIT, Product ID, PromotionID, Total Sales, Units Sold), filterable using Date, Customer Name, Product Name, and Promotion Name slicers.
- **Step 10:** Applied a consistent report theme and formatting across all visuals and pages for a clean, professional look.

## Dashboard Screenshots

### Overview Page
![Overview Page](https://github.com/user-attachments/assets/97e85c25-9a61-484d-94b2-f0bec79e80d6)

### Top/Bottom Products Page
![Top Bottom Page](https://github.com/user-attachments/assets/d9b3714b-5475-4c26-ad49-5c99f8fec89c)

### Sale Trend Page
![Sale Trend Page]((https://github.com/user-attachments/assets/383ac42c-4e01-42ce-a572-cd840ef30c5e))

### Compare with Dates Page
![Compare With Dates Page](https://github.com/user-attachments/assets/0581448f-d25c-4fc4-9290-fd1ff00c68c5)

### Table (Order Detail) Page
![Table Page](https://github.com/user-attachments/assets/4aabbc39-9f9f-4163-ad59-775a463d64a0)

## Insights

### Overall Performance
- **Total Net Sales:** 122.31M
- **Total Units Sold:** 7.125K
- **Total Profit:** 12.23M
- **Average Discount %:** 5.66
- **Total Orders:** 3.51K

### Top 5 Products
| Metric | #1 | #2 | #3 | #4 | #5 |
|---|---|---|---|---|---|
| By Total Sales | Apple iPhone 14 (21.4M) | Apple MacBook Air (19.6M) | Sony Bravia 55" TV (19.4M) | Samsung Galaxy S21 (15.3M) | HP Pavilion Laptop (14.4M) |
| By Profit | Apple iPhone 14 (2.14M) | Apple MacBook Air (1.96M) | Sony Bravia 55" TV (1.94M) | Samsung Galaxy S21 (1.53M) | HP Pavilion Laptop (1.44M) |
| By Quantity Sold | Apple iPhone 14 (281) | HP Pavilion Laptop (238) | Samsung Galaxy S21 (230) | Sony Bravia 55" TV (228) | Apple MacBook Air (225) |

### Bottom 5 Products
| Metric | #1 | #2 | #3 | #4 | #5 |
|---|---|---|---|---|---|
| By Total Sales | Tupperware Lunch Box (0.26M) | L'Oreal Shampoo (0.17M) | Nivea Body Lotion (0.08M) | Dove Soap Pack (0.08M) | Colgate Toothpaste (0.02M) |
| By Profit | Tupperware Lunch Box (26K) | L'Oreal Shampoo (17K) | Nivea Body Lotion (8K) | Dove Soap Pack (8K) | Colgate Toothpaste (2K) |
| By Quantity Sold | Dove Soap Pack (248) | L'Oreal Shampoo (248) | Colgate Toothpaste (226) | Nivea Body Lotion (219) | Tupperware Lunch Box (215) |

thus, high-value electronics (iPhone 14, MacBook Air, Sony Bravia TV) dominate both sales and profit, while low-ticket personal care and household items make up the bottom performers.

### Net Sales by City (Top Cities)
Bhopal (15.4M) leads, followed by Kanpur (14.1M), Indore (13.4M), Lucknow (10.5M), Mumbai (10.0M), Pune (9.4M), Patna (7.3M), Jaipur (6.1M), Nagpur (6.0M), Delhi (5.5M), Chennai (5.5M), Ahmedabad (5.0M), and Kolkata (4.7M).

thus, Tier-2 cities like Bhopal, Kanpur, and Indore outperform several metro cities in net sales.

### Sales Trend by Year
Net sales stayed fairly stable from 2020 to 2023 (31M → 30M → 29M → 32M), with 2023 being the strongest year, before the visible drop-off into 2024 (likely due to partial-year data).

### Discount by Promotion
Grouping Discount Value by Promotion Name shows Weekend Flash Sale carries the highest average discount, followed by Clearance Sale, Summer Sale, New Year Special, and Festive Diwali (lowest).

thus, flash and clearance sales are the most heavily discounted promotional campaigns.

### Sales vs. Profit Relationship
The scatter chart shows a strong, consistent positive linear relationship between sales and profit — as net sales increase, profit increases proportionally, indicating a stable margin across orders.

### Period Comparison & Order-Level Detail
Two independent date-range slicers let users compare Net Sales, Profit, and Units Sold across any two custom time periods side by side. A separate detail page lets users filter by Customer, Product, Promotion, and Date to view granular, order-level figures (Discount %, Discount Value, Net Sales, Profit, Total Sales, Units Sold).
