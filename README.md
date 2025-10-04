# 🛒 Blinkit Sales Analytics – Excel → SQL → Power BI

## 📌 Project Overview

This project demonstrates an end-to-end **data analytics pipeline** applied to a comprehensive **Blinkit sales dataset**. It begins with raw data in **Excel**, progresses through structured analysis using **SQL**, and concludes with a fully **interactive Power BI dashboard**.

The main objective is to analyze sales performance across various dimensions like product type, outlet location, and establishment year to uncover key business insights and identify drivers of revenue.

---

## 🧾 Step 1: Data Cleaning & Excel Preparation

The dataset consisted of over 8,500 rows with 13 columns, including:
- `Item_Identifier`: Unique ID for each product
- `Item_Fat_Content`: Fat level (e.g., Low Fat, Regular)
- `Item_Type`: Product category
- `Item_MRP`: Maximum retail price of the product
- `Outlet_Identifier`: Unique ID for each store
- `Outlet_Establishment_Year`: The year the store was established
- `Outlet_Size`: Size of the store (e.g., Small, Medium, High)
- `Outlet_Location_Type`: Tier of the city where the store is located
- `Outlet_Type`: Type of store (e.g., Supermarket, Grocery)
- `Sales`: Total sales for the product in a particular outlet

Tasks in Excel included:
- Initial data profiling and understanding
- Identifying and handling inconsistencies in categorical data (e.g., standardizing 'Low Fat' and 'LF')
- Checking for missing values in columns like `Item_Weight` and `Outlet_Size`
- Ensuring data formats were correct before importing into a database

---

## 🗃️ Step 2: SQL Data Analysis (MySQL)

The cleaned dataset was imported into a **MySQL database** (`blinkit`) for structured querying and in-depth analysis. A script containing 20 distinct SQL queries was written to derive key insights.

Key queries included:
1.  **Calculating core KPIs** (Total Sales, Average Sales, Total Items)
2.  **Analyzing sales trends** by establishment year
3.  **Aggregating sales** by Item Type, Outlet Size, and Location Tier
4.  **Comparing sales** between Low Fat and Regular fat products
5.  **Identifying Top 10 selling products** and **Top 5 performing outlets**
6.  **Calculating sales contribution percentage** by Outlet Type
7.  **Ranking the top 3 products** within each item category
8.  **Segmenting sales** by different price ranges (Low, Medium, High)
9.  **Identifying outlets performing above the company average**
10. **Finding the most sold item** in each location tier

These queries used MySQL features such as:
- Aggregations (`SUM`, `AVG`, `COUNT`)
- `CASE` statements for conditional logic and data cleaning
- `GROUP BY` and `ORDER BY` for data segmentation
- Window Functions (`RANK() OVER...`) for advanced ranking
- Subqueries for complex filtering and calculations

---

## 📊 Step 3: Data Visualization with Power BI

The analysis culminated in an interactive **Power BI dashboard** designed to provide a comprehensive overview of sales performance at a glance.

The dashboard highlights:
- **KPIs**: Total Sales ($1.2M), Average Sales ($141), Number of Items (8523), and Average Rating (3.9)
- **Trend Analysis**: An area chart showing total sales performance from 2011 to 2022.
- **Categorical Insights**: Donut charts for sales distribution by Outlet Size and Fat Content, and bar charts for sales by Item Type and Outlet Location.
- **Detailed Summaries**: A matrix visualizing Total Sales, Item Count, and Average Rating for each Outlet Type.
- **Pivoted Analysis**: A stacked bar chart comparing sales of Low Fat vs. Regular items across different outlet tiers.

The dashboard enables **dynamic exploration** with interactive slicers for Outlet Location Type, Outlet Size, and Item Type.

---

## 🧠 Skills Demonstrated

- **Excel**: Data cleaning, handling data inconsistencies, data preparation for SQL import.
- **SQL (MySQL)**: Database design, complex queries, aggregations, conditional logic (`CASE`), window functions (`RANK`), and subqueries.
- **Power BI**: Dashboard design, creating calculated measures (DAX), KPI visualization, interactive filtering (slicers), and data storytelling.
- **Data Analysis**: Sales performance analysis, trend identification, product categorization, and uncovering actionable business insights.

---

## 📈 Conclusion

This project successfully transforms a raw sales dataset into **actionable insights** through a structured analytical approach. It showcases how the powerful combination of **Excel for data prep, SQL for deep analysis, and Power BI for compelling visualization** can create a strategic tool for business decision-making.

The resulting dashboard provides a clear and data-driven view of Blinkit's performance, enabling stakeholders to easily identify growth opportunities and areas for improvement.
