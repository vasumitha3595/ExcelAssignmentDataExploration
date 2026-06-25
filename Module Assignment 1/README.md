Project Overview

This project presents an **interactive E-Commerce Sales Dashboard** built using **Microsoft Excel**. The objective is to transform raw transactional data into meaningful business insights through data cleaning, pivot tables, pivot charts, slicers, and KPI cards.

The dashboard enables users to analyze customer behavior, product performance, sales trends, and geographical distribution to support data-driven decision-making.

---

## 🎯 Objectives

- Analyze overall sales performance.
- Identify top-performing categories and products.
- Understand customer demographics and purchasing patterns.
- Evaluate revenue contribution by gender and loyalty level.
- Analyze regional and state-wise performance.
- Create an interactive dashboard using Excel.

---

## 🛠 Tools & Technologies

- Microsoft Excel
- Pivot Tables
- Pivot Charts
- Slicers
- Timeline Filters
- Conditional Formatting
- Dashboard Design
- Data Cleaning Techniques

---

## 📂 Dataset Features

### Customer Information
- Customer ID
- Customer Name
- Gender
- Age
- Loyalty Level

### Product Information
- Product Name
- Category
- Subcategory
- Brand

### Sales Information
- Sales ID
- Order Date
- Quantity
- Unit Price
- Total Amount

### Geographic Information
- Region
- City
- State
- Country

### Payment Information
- Payment Type

---

## 🧹 Data Cleaning

The following preprocessing steps were performed:

✔ Removed duplicates

✔ Handled missing values

✔ Standardized categorical values

✔ Converted date formats

✔ Created clean numerical columns

✔ Created age groups

### Age Group Formula

```excel
=IF([@Age]<=40,"20-40",IF([@Age]<=60,"41-60","Above 60"))
```

---

# 📈 Dashboard Components

## KPI Cards

| KPI | Value |
|------|--------|
| 💰 Total Revenue | ₹2.17M |
| 🛒 Total Orders | 2000 |
| ⭐ Top Category | Sports |
| 🏆 Top Loyalty Level | Platinum |
| 📍 Top Region | North |
| 👩 Highest Revenue Gender | Female |

---

## Pivot Charts

### Category-wise Sales
- Clustered Column Chart

### Gender-wise Sales
- Doughnut Chart

### Top Cities Analysis
- Pie Chart

### Store Type Analysis
- Doughnut Chart

### Loyalty Level Analysis
- Column Chart

### Region-wise Sales
- Horizontal Bar Chart

### Quarterly Sales Trend
- Line Chart

### Top Stores Analysis
- Bar Chart

### Age Group Analysis
- Column Chart

---

# 📊 Key Insights

## Gender-wise Revenue

| Gender | Revenue |
|----------|---------:|
| Female | ₹1.23M |
| Male | ₹0.94M |

**Insight:** Female customers contribute **56.6%** of total revenue.

---

## Category-wise Revenue

| Category | Revenue |
|-----------|---------:|
| Sports | ₹542K |
| Electronics | ₹504K |
| Home | ₹427K |
| Clothing | ₹379K |
| Beauty | ₹321K |

**Insight:** Sports is the highest revenue-generating category.

---

## Top Revenue Products

| Product | Revenue |
|----------|---------:|
| Portable Power Bank | ₹41.85K |
| Shin Guards – Adult | ₹38.28K |
| Men's Casual Sneakers | ₹35.49K |
| Gaming Mechanical Keyboard | ₹34.70K |
| Women's High Heels | ₹33.99K |

**Insight:** Revenue is well diversified across products.

---

## Loyalty Level Analysis

| Loyalty Level | Revenue |
|---------------|---------:|
| Platinum | ₹673.71K |
| Bronze | ₹522.62K |
| Gold | ₹517.64K |
| Silver | ₹460.57K |

**Insight:** Platinum members generated the highest revenue.

---

## Region-wise Transactions

| Region | Transactions |
|---------|-------------:|
| North | 596 |
| East | 590 |
| South | 581 |
| West | 233 |

**Insight:** North, East, and South account for nearly 88% of transactions.

---

## State-wise Revenue

| State | Revenue |
|---------|--------:|
| New Hampshire | ₹69.58K |
| New Jersey | ₹65.27K |
| Vermont | ₹61.73K |
| Florida | ₹60.41K |
| Oklahoma | ₹59.39K |

**Insight:** Revenue is evenly distributed across states.

---

## 💡 Recommendations

- Increase inventory for Sports and Electronics products.
- Strengthen customer loyalty programs.
- Focus marketing efforts on female customers.
- Promote Platinum membership benefits.
- Improve sales in lower-performing regions.
- Maintain inventory for top-selling products.

---

# 📈 Dashboard Preview

<img width="1000" alt="Dashboard" src="dashboard.png">

---

## 📁 Project Structure

```
E-Commerce-Sales-Dashboard/
│
├── Ecommerce_Sales_Dataset.xlsx
├── Dashboard.xlsx
├── dashboard.png
├── README.md
└── Project_Report.docx
```

---

## 🚀 Skills Demonstrated

- Data Cleaning
- Data Analysis
- Pivot Tables
- Pivot Charts
- Dashboard Design
- KPI Reporting
- Business Insights
- Data Visualization
- Excel Formulas
- Slicer and Timeline Integration

---

## 📚 Conclusion

This project demonstrates how Microsoft Excel can be used to transform raw sales data into actionable business insights. Through interactive dashboards and visualizations, stakeholders can identify trends, understand customer behavior, and make informed business decisions.
