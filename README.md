# 🛒 E-Commerce Product Pricing Analysis  

![Dashboard Preview]([https://lookerstudio.google.com/s/qlUFPHixQDM])

**Author:** Tapan Chandra Chud Malik  
**Last Updated:** November 2025  

---

## 📋 Overview  

This repository contains a **data analytics project** that explores electronic product pricing and availability in an e-commerce environment.  
The project demonstrates a full analytics workflow — from **data cleaning** and **exploratory analysis** in Excel to **dashboard development** in Looker Studio — designed to uncover insights about pricing strategy, stock management, and brand performance.

### 🎯 **Business Objective**  
E-commerce platforms often handle thousands of SKUs with complex pricing and availability patterns.  
The goal of this project is to:
- Analyze price distribution and outliers.  
- Examine brand-level performance.  
- Evaluate stock availability and shipping trends.  
- Present insights in an interactive dashboard.  

### 🧰 **Tech Stack**
| Tool | Purpose |
|------|----------|
| **Google Sheets** | Data gathering and initial formatting |
| **Microsoft Excel** | Cleaning, transformation, and exploratory data analysis |
| **Looker Studio (Google Data Studio)** | Dashboard creation and visualization |
| **Python (pandas, reportlab, pptx)** | Report and deck generation |

---

## 📊 Data Source & Description  

- **Dataset File:** `Electronics Products Pricing Data.xlsx`  
- **Dashboard File:** `Electronics_Products_Dashboard.pdf`  
- **Total Records:** 7,249  
- **Distinct Brands:** 10+  
- **Primary Metric Column:** `prices_amountmax`  

### **Key Metrics**
| Metric | Value |
|--------|-------:|
| Minimum Price | **$1.00** |
| Maximum Price | **$6,999.99** |
| Average Price | **$495.53** |
| Median Price | **$198.99** |
| Standard Deviation | **$763.60** |
| Records (non-null) | **7,249** |

### **Data Dimensions**
- Brand  
- Product Name  
- Category  
- Availability  
- Shipping Type  
- Condition 

---

## 🧹 Data Cleaning & Preparation  

Performed using **Excel** and **Google Sheets**:

1. **Handled Missing Values**  
   - Filled missing prices with median where applicable.  
   - Tagged unknown availability as “Undefined.”

2. **Treated Outliers**  
   - Verified extreme prices (> $6,999) for data accuracy.  
   - Retained valid premium electronics.

3. **Standardized Fields**  
   - Unified text case and removed whitespace.  
   - Standardized availability: `In Stock`, `Out Of Stock`, `Special Order`, etc.  
   - Converted currency columns to numeric.

4. **Categorized Attributes**  
   - Grouped items by brand, shipping type, and condition for aggregation in Looker Studio.

---

## 🔍 Exploratory Data Analysis (EDA)

### **Descriptive Statistics**
- Mean = $495.53 Median = $198.99 Range = $1–$6,999.99  
- Right-skewed distribution → many affordable products, few high-priced outliers.

### **Availability Breakdown**
| Availability | Count |
|---------------|------:|
| Yes | 3,692 |
| In Stock | 3,172 |
| Out Of Stock | 115 |
| Special Order | 109 |
| More on the Way | 91 |
| Undefined | 40 |
| Sold | 22 |
| No | 5 |
| Available | 2 |
| Retired | 1 |

**Insight:**  
~85 % of products are in stock or readily available — a strong supply position.

---

## 📈 Dashboard Development (Looker Studio)

The **Looker Studio Dashboard** visualizes key pricing and stock metrics for faster decision-making.  

### **Visualized Metrics**
- Average / Max / Min Prices  
- Product Quantity by Brand  
- Availability Status distribution  
- Shipping Type cost categories  
- Product Condition mix (New, Used, Refurbished)

### **Interactive Features**
- **Brand Filter** – Focus on specific manufacturers.  
- **Date Filter** – Time-based exploration.  
- **Dynamic KPIs** – Auto-updates of min/max/avg price cards.  
- **Cross-Filtering** – Click a brand or condition to filter across charts.

### **Key Visualizations & Purpose**
| Visualization | Purpose |
|----------------|----------|
| **Bar Chart – Price by Brand** | Compare pricing trends across major brands |
| **Pie Chart – Shipping Type** | Examine delivery cost distribution |
| **Stacked Chart – Condition Mix** | Assess proportion of new vs refurbished items |
| **Line Chart – Price Trend** | View pricing movement over time |

---

## 💡 Insights & Findings  

1. **Pricing Diversity** – Wide range from budget to premium products.  
2. **Brand Concentration** – Major brands like *LG, Apple, and Samsung* dominate.  
3. **Stock Health** – > 80 % availability indicates efficient supply chain.  
4. **Shipping Preference** – “Free” and “Standard” shipping dominate; opportunity for premium shipping upsell.  
5. **Condition Mix** – Predominantly *New* items; refurbished stock provides secondary margin channel.  

---

## 🧠 Tools & Technologies  

| Category | Tools |
|-----------|--------|
| Data Handling | Google Sheets, Microsoft Excel |
| Visualization | Looker Studio (Google Data Studio) |
| Reporting | Python (ReportLab · python-pptx) |
| Version Control | Git · GitHub |

---

## 🧾 Conclusion & Recommendations  

### **Conclusion**
The analysis provides a holistic understanding of pricing and availability within an e-commerce electronics catalog.  
Strong stock availability and varied pricing suggest a healthy, diversified marketplace.

### **Recommendations**
- Optimize pricing for **mid-range products** with consistent sales potential.  
- Track and replenish **out-of-stock** and **special-order** items.  
- Analyze **shipping cost tiers** for profitability improvement.  
- Extend dashboard for **category-wise** and **temporal** insights.  

---

## 💼 Author  
**Tapan Chandra Chud Malik**  
*Data Analyst | Business Intelligence Enthusiast*  
📧 *Available for analytics collaborations or portfolio feedback.*

