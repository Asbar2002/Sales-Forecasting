# Sales-Forecasting
Power BI meets business strategy. This dashboard uncovers what's selling, what's killing profit, and where the business should focus next , all backed by clean visuals and hard numbers.

# Sales & Profit Performance Dashboard – Power BI

##  Project Overview

This Power BI dashboard provides a complete view of a furniture business's sales performance, profitability, and customer segmentation. It leverages interactive visuals, DAX measures, and Power BI's forecasting engine to uncover trends, highlight margin issues, and support data-driven decision-making.

The dashboard was built to demonstrate advanced skills in business analytics, data visualization, and storytelling using Power BI.

---

##  Tools & Skills Demonstrated

- **Power BI Desktop**
- **Power Query**: Data cleaning and transformation
- **DAX**: KPIs, calculated measures, time intelligence
- **Forecasting**: Built-in analytics pane forecasting
- **Slicers & Interactivity**: Drilldowns by Region, Segment, Sub-category
- **Data storytelling & layout design**

---

##  Dataset Overview

A retail order dataset containing ~1700 records of transactions across US regions.

### Fields Used:
| Field          | Purpose |
|----------------|---------|
| `order_date`   | Time-based analysis, forecasting |
| `region`, `state`, `segment` | Regional and customer-level analysis |
| `sub_category` | Product-level performance |
| `sales`, `profit`, `discount`, `quantity` | Core KPIs |
| `order_id`     | For calculating distinct orders (AOV)

*Unnecessary fields like `row_id`, `ship_date`, `product_id`, and `customer_id` were removed during cleaning to simplify the model.*

---

##  Dashboard Pages

###  Page 1: Executive Overview
- KPI Cards: Total Sales, Profit, Orders, Avg Discount
- Sales & Profit Trends (with Forecast)
- Sales vs Profit by Region
- Sales Distribution by Segment
- Slicers: Year, Region, Segment, Sub-category

###  Page 2: Sub-Category Deep Dive
- Sales vs Profit by Sub-Category
- Loss-making vs Profit-driving items
- Discount vs Profit Scatter Plot
- Slicers for dynamic drilldowns

---

##  Key Business Insights

- **Tables** had strong sales but **negative profit** due to heavy discounting.
- **Chairs** and **Furnishings** were top profit drivers with healthy margins.
- The **South region** showed concerning margin performance.
- Forecasting revealed **slow but steady sales growth** year-over-year.

---

##  DAX Measures Used
```DAX
Total Sales = SUM(Sales)
Total Profit = SUM(Profit)
Total Orders = DISTINCTCOUNT(OrderID)
Avg Discount = AVERAGE(Discount)
Average Order Value = [Total Sales] / [Total Orders]
```
Screenshots
![image](https://github.com/user-attachments/assets/4e9033a6-d502-40bd-987c-f89448619ca6)
![image](https://github.com/user-attachments/assets/bc2f6b75-2139-4ccf-9260-37760d5cb2eb)



**## Author**
Muhammadh Asbar
Master of IT (Enterprise Management), University of South Australia
 Business & Data Analyst | Power BI | Python | SQL
 LinkedIn Profile (www.linkedin.com/in/muhammadh-asbar)

 Note
Dataset was downloaded from Kaggle.
Link: https://www.kaggle.com/datasets/tanayatipre/store-sales-forecasting-dataset
