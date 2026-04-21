# 🧠 SSIS ETL Sales OLAP Project

## 📌 Overview

This project implements a full-scale **ETL pipeline** using SQL Server Integration Services (SSIS) to build a **Sales Data Warehouse** optimized for analytical processing (OLAP).

The solution follows best practices in data engineering, including staging, transformation, and dimensional modeling.

---

## 🎯 Business Problem

Organizations often struggle with fragmented sales data across multiple sources, making it difficult to generate insights.

This project solves that by:

* Consolidating data into a centralized Data Warehouse
* Structuring it for fast analytical queries
* Enabling business intelligence and reporting

---

## 🏗️ Architecture

The architecture follows a classic **ETL + Data Warehouse** design:

1. **Data Sources**
2. **Staging Layer**
3. **Data Transformation (SSIS)**
4. **Data Warehouse (Star Schema)**
5. **OLAP / Reporting Layer**

---

## 🧱 Data Warehouse Design

### ⭐ Star Schema

* **Fact Table**

  * Fact_Sales

* **Dimension Tables**

  * Dim_Customer
  * Dim_Product
  * Dim_Time

✔ Designed for:

* High query performance
* Simplified reporting
* Scalability

---

## 🔄 ETL Pipeline (SSIS)

### مراحل التنفيذ:

1. **Extract**

   * Pull raw data from source systems

2. **Staging**

   * Load raw data into staging tables

3. **Transform**

   * Data cleaning
   * Handling null values
   * Data type conversion
   * Business rules application

4. **Load**

   * Load into dimension tables
   * Load into fact table

---

## ⚙️ Tools & Technologies

* SQL Server
* SSIS (SQL Server Integration Services)
* SSMS
* Visual Studio (SSDT)

---

## 📂 Project Structure

```bash
SSIS_ETL_SalesOLAP_Project/
│
├── SSIS Packages/
│   ├── Load_Dimensions.dtsx
│   ├── Load_FactSales.dtsx
│
├── SQL Scripts/
│   ├── Create_DW.sql
│   ├── Staging.sql
│
├── Data/
└── README.md
```

---

## ▶️ How to Run

1. Open the project in Visual Studio (SSDT)
2. Update connection strings
3. Execute SSIS packages in order:

   * Load Dimensions
   * Load Fact Table

---

## 📊 Expected Output

* Fully structured Data Warehouse
* Clean and consistent data
* Ready for reporting tools (Power BI, SSRS)
* [Sample CSV Output]
* [(images\SalesAnalysis.png)]

---

## 🚀 Future Enhancements

* 🔁 Incremental Load (CDC)
* ⚠️ Error Handling & Logging
* 📊 Power BI Dashboard Integration
* ⏱️ Scheduling using SQL Server Agent

---

## 🧠 Key Learnings

* Building end-to-end ETL pipelines
* Designing Star Schema
* Working with SSIS Data Flows
* Data Cleaning & Transformation techniques

---

## 👤 Author

**Youssif Hussein**

*Data Engineer*

---
