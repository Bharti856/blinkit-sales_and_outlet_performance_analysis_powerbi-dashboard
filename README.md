# Blinkit Sales & Outlet Performance Analysis (Power BI)

## Dashboard Preview

![Dashboard Preview](screenshots/Sales-Overview.jpeg)

---

# Project Overview

This project analyzes Blinkit grocery sales data to uncover insights about outlet performance, product demand, and customer preferences.

An interactive dashboard was developed using Power BI to visualize sales distribution, outlet performance across locations, and product category trends.

The goal of this project is to demonstrate **data analysis, dashboard design, and DAX-based KPI calculation skills** using Power BI.

---

# Business Problem

Retail businesses like Blinkit need to understand which outlets, product categories, and customer preferences drive the most revenue.

Without clear insights, it becomes difficult to optimize inventory, improve product offerings, and maximize sales performance.

This dashboard analyzes grocery sales data to identify patterns in outlet performance, product demand, and customer satisfaction.

---

# Tools & Technologies

* Power BI
* Microsoft Excel
* Data Visualization
* Data Analysis
* DAX (Data Analysis Expressions)

---

# Dataset

The dataset contains grocery sales information including:

* Item Identifier
* Item Type
* Outlet Type
* Outlet Location Type
* Fat Content
* Item Rating
* Sales Value

Dataset location:

```
dataset/BlinkIT Grocery Data.xlsx
```

---

# Data Preparation

Before creating the dashboard, the dataset was prepared and structured in Power BI.

Steps included:

* Verifying data types
* Checking for missing values
* Creating calculated measures using DAX
* Organizing fields for analysis

---

# Key Performance Indicators (KPIs)

The dashboard tracks the following key metrics:

* **Total Sales** – Total revenue generated from all items sold
* **Average Sales** – Average revenue generated per transaction
* **Number of Items** – Total items sold across outlets
* **Average Rating** – Average customer rating of products

To improve interactivity, a **Metric Selector using Field Parameters** was implemented in Power BI.

This allows users to dynamically switch between these KPIs within the same visualization.

---

# DAX Measures Used

The following DAX measures were created and included inside the **Metric Parameter**.

### Total Sales

```DAX
Total Sales = SUM('BlinkIT Grocery Data'[Sales])
```

### Average Sales

```DAX
Avg Sales = AVERAGE('BlinkIT Grocery Data'[Sales])
```

### Number of Items

```DAX
No of Items = COUNT('BlinkIT Grocery Data'[Item Identifier])
```

### Average Rating

```DAX
Avg Rating = AVERAGE('BlinkIT Grocery Data'[Rating])
```

These measures power the KPI cards and are dynamically controlled using the **Metric field parameter**.

---

# Dashboard Features

The Power BI dashboard includes several interactive visualizations to analyze grocery sales performance.

Key features include:

* KPI cards displaying **Total Sales, Average Sales, Number of Items, and Average Rating**
* Dynamic **Metric Selector (Field Parameter)** for switching KPIs
* Sales analysis by **Outlet Type**
* Sales distribution by **Outlet Location**
* Product category analysis by **Item Type**
* Comparison between **Low Fat and Regular Fat products**
* Interactive filters for deeper analysis

---

# Dashboard Screenshots

### Sales Overview

![Sales Overview](screenshots/Sales-Overview.jpeg)

This page provides a high-level overview of Blinkit’s grocery sales performance.
It highlights KPI metrics and shows how sales are distributed across outlet types and locations.

---

### Business Insights

![Business Insights](screenshots/Business-Insights.jpeg)

This section focuses on deeper analytical insights including fat content comparison, item category performance, and outlet performance patterns.

---

# Key Business Insights

* **Tier 3 outlets generate the highest revenue**
* **Supermarket Type 1 contributes the majority of total sales**
* **Regular fat products slightly outperform low-fat products**
* Certain product categories contribute significantly to total sales
* Higher-rated products tend to perform better in sales

---

# Project Structure

```
blinkit-sales_and_outlet_performance_analysis_powerbi-dashboard
│
├── dataset
│   └── BlinkIT Grocery Data.xlsx
│
├── dashboard
│   └── Blinkit Sales & Outlet Performance Analysis.pbix
│
├── screenshots
│   ├── Business-Insights.jpeg
│   └── Sales-Overview.jpeg
│
├── images
│
└── README.md
```

---

# Learning Outcomes

Through this project, the following skills were developed:

* Data visualization using Power BI
* Creating analytical measures using DAX
* Implementing Field Parameters for dynamic metrics
* Designing interactive dashboards
* Extracting business insights from retail data

---

# Future Improvements

Possible enhancements include:

* Adding time-based sales trend analysis
* Implementing sales forecasting models
* Integrating additional datasets for deeper insights

---

# Author

Akhil Bharti
