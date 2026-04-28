# 📊 Sales Analytics Dashboard (Power BI Capstone Project)

## 🚀 Project Overview  
This project showcases an interactive **Sales Analytics Dashboard** built using Power BI. The goal is to analyze business performance across regions, products, and customer segments, and convert raw data into actionable insights.

The dashboard helps stakeholders track key metrics, identify inefficiencies, and make data-driven decisions.

---

## 🎯 Business Problem  
Businesses often face challenges in:
- Monitoring revenue and profit trends  
- Identifying underperforming products  
- Understanding the impact of discounts on profitability  
- Tracking regional performance vs targets  
- Detecting operational inefficiencies like delivery delays  

This dashboard addresses these challenges through interactive visualizations and KPI tracking.

---

## 📂 Dataset Description  
The dataset includes:
- Sales & Revenue  
- Profit & Profit Margin  
- Orders & Returns  
- Customer Segments  
- Products & Categories  
- Regional Data  
- Shipping Modes & Delivery Time  
- Discounts & Sales Targets  

---

## 🛠️ Tools & Technologies  
- Power BI (Data Visualization)  
- Power Query (Data Cleaning & Transformation)  
- DAX (Calculations & KPIs)  
- Excel (Data Source)  

---

## 📈 Dashboard Features  

### 🔹 KPI Metrics  
- Total Revenue  
- Total Profit  
- Total Orders  
- Profit Margin %  
- YoY Growth %  
- MoM Growth %  

---

### 🔹 Sales & Trend Analysis  
- Monthly sales trends to identify seasonality  
- Year-over-Year growth by region  
- Identification of declining sales trends  

---

### 🔹 Product & Profitability Analysis  
- Top 10 products by profit margin  
- Products with declining sales  
- Impact of discount percentage on profit  

---

### 🔹 Regional Performance  
- Sales vs target comparison  
- Regions with high revenue but low profit  
- Regions with highest return rates  

---

### 🔹 Customer Insights  
- Revenue contribution by customer segments  
- Customer behavior patterns  

---

### 🔹 Operational Analysis  
- Shipping modes causing delivery delays  
- Delivery time vs customer satisfaction  
- Sales representative performance vs targets  

---

### 🔹 Forecasting  
- Next quarter revenue prediction using historical trends  

---

## 📊 Sample DAX Measures  

```DAX
Total Revenue = SUM(Sales[Revenue])

Profit Margin % = DIVIDE(SUM(Sales[Profit]), SUM(Sales[Revenue]))

YoY Growth % =
DIVIDE(
    [Total Revenue] - CALCULATE([Total Revenue], SAMEPERIODLASTYEAR(Date[Date])),
    CALCULATE([Total Revenue], SAMEPERIODLASTYEAR(Date[Date]))
)

MoM Growth % =
DIVIDE(
    [Total Revenue] - CALCULATE([Total Revenue], DATEADD(Date[Date], -1, MONTH)),
    CALCULATE([Total Revenue], DATEADD(Date[Date], -1, MONTH))
)

📦 Sales-Analytics-Dashboard
 ┣ 
 ┣ 📂 Capstone_Project Dashboard Screenshots
 ┣ 📄 Capstone_Project.pbix
 ┣ 📄 10000 Rows Dataset
 ┣ 📄 Capstone Project Questions
 ┗ 📄 README.md
