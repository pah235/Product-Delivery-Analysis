# Product-Delivery-Analysis
This project showcases a Power BI dashboard analyzing order delivery performance for an e-commerce platform. It includes insights on shipping status, delivery timelines, and key operational metrics by merchandise type and location.

---

# 🚚 Product Delivery Analysis | Business Intelligence Portfolio Project
![image](https://github.com/user-attachments/assets/1560d2f1-80cb-46aa-bf1d-cf7a205e26f9)

## 📌 A. Project Overview

### 1. Tools & Skills Used

- ✅ Power Query: Data cleaning and transformation
- ✅ Data Modeling: Establishing data relationships for multidimensional analysis
- ✅ DAX: Calculating KPIs and lead time metrics
- ✅ Power BI Visualizations: Donut charts, bar charts, scatter plots, column charts, shape maps
- ✅ Report Features: Drill-down, Tooltips Page, Drill-through, Buttons, Bookmarks, Parameters
- ✅ Dashboard Design: Complete report pages with interactive insights for business users

---

### 2. Business Background

#### 🔹 About the Company
**ABC** is a U.S.-based e-commerce platform providing a seamless, fast, and secure online shopping experience. The company offers a wide variety of products — from home decor, furniture, and electronics to beauty, health, and entertainment goods. A key business focus is ensuring fast and accurate delivery experiences for all customers.

#### 🔹 About the Dataset
The dataset used in this analysis is a single fact table containing key order details:
- `Order Number`: Order identifier
- `Package ID`, `Product ID`, `Customer ID`
- `Ordered Quantity`, `Total Amount`
- `Merchandise Type`: Product category
- `Ship From` / `Ship To`: State-level delivery information
- `Order Date`, `Ship Date`, `Delivery Date`: Delivery lifecycle timestamps

---

## 📊 B. Project Goals & Stakeholder Needs

### 1. Role in the Organization
You are a BI Analyst in the **Operations Department**, tasked with building a dashboard for the Operations Manager and other executive stakeholders.

### 2. Business Requirements

#### a. Delivery Performance Overview
- Calculate the total number of **Ordered**, **Shipped**, and **Delivered** orders.
- Calculate % of orders that are **Delivered** vs. **Not Delivered**.
- Identify orders placed but **not yet delivered**.
- Perform similar analysis on the number of **Packages**, **Customers**, and **Products**.

#### b. Lead Time Analysis
- Compute **Shipping Lead Time** (Order → Ship) and **Delivery Lead Time** (Ship → Deliver).
- Analyze **Shipping/Delivery Lead Time** distribution across time ranges and delivery status.
- Create maps showing volume of Packages, Customers, Products, and Orders by **origin and destination states**.
- Add filters for:
  - **Order Date**
  - **Ship From** / **Ship To** locations
  - **Delivery Status**

---

## 🛠️ C. Project Execution

### 1. Data Exploration & Cleaning
- Reviewed data schema and relevant dimensions (e.g., product, time, geography).
- Created a custom `dim_date` table for reusable time-based reporting.
- Cleaned and transformed fields in Power Query:
  - Standardized column names
  - Converted fields to appropriate data types (date, text, number)

### 2. Data Modeling
- Established relationships between `dim_date` and main order table
- Defined clear field hierarchies for slicing/filtering

### 3. KPI Calculations using DAX
- Total Ordered Orders
- Total Shipped Orders
- Total Delivered Orders
- Delivery Success Rate
- Shipping Lead Time (days)
- Delivery Lead Time (days)

### 4. Dashboard Design & Visualizations

#### ✅ Dashboard Features:
- **Donut Charts**: Share of Packages, Customers, Products, Orders by delivery status
- **Scatter Plot**: Relationship between average delivery time and quantity, by merchandise type
- **Shape Map**: Delivery volume by **origin** and **destination**
- **Bar Chart**: Packages/Customers/Products/Orders per merchandise type
- **Column Chart**: Shipping and delivery lead times by category and status
- **Slicers**: Interactive filters by Order Date, Locations, and Delivery Status

---

## 🎯 5 Key Insights from the Report:
Easily monitor the overall order delivery process with a breakdown of total orders placed, delivered, and not yet delivered, along with clear delivery completion rates.

Detailed analysis by delivery status enables performance tracking across merchandise types, customers, products, and shipping/receiving locations.

The report provides a comprehensive view of shipping timelines, including both shipping lead time and delivery lead time, supporting process optimization.

An interactive map visualizes shipment volume by state, helping stakeholders identify key regions in the logistics network.

The dashboard supports flexible data exploration with filters by order date, delivery status, and locations, empowering timely and informed decision-making.

---

## 📦 E. Files Included

| File Name                    | Description                                 |
|-----------------------------|---------------------------------------------|
| `Product Delivery Report.pbix` | Power BI dashboard project file             |
| `README.md`                 | Documentation for GitHub portfolio           |

---

## 📚 References

- 📊 Dataset: Simulated product delivery data from internal operations
- 🛠 Tools Used: Power BI, DAX, Power Query

---

