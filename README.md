# 🏗️ SQL Data Warehouse Project

## 🚀 Project Overview
This project is a **real-world simulation of a modern data warehouse build**—designed, architected, and implemented from the ground up using **SQL Server**. It demonstrates how to **extract, clean, transform, integrate, and model structured data** to enable **business-ready analytics** and **data-driven decision-making**.

The project is fully inspired by **enterprise-grade architecture principles** and follows **best practices used in companies like Mercedes-Benz** for data engineering and analytics.

---

## 🎯 Project Objectives
- Build a **modern SQL Data Warehouse** from scratch.  
- Implement **ETL pipelines** to prepare data for analytics.  
- Design a **scalable data architecture** following the **Medallion Architecture (Bronze, Silver, Gold)**.  
- Integrate **multiple data sources (ERP + CRM)** into a unified analytical model.  
- Build **documentation and project plan** using **Notion** and **Draw.io**.  
- Ensure **data quality, standardization, and traceability** at each layer.  

---

## 🧱 Data Architecture

### Medallion Architecture (Bronze, Silver, Gold)

| Layer | Description | Object Type | Load Method | Transformation Focus |
|:------|:-------------|:-------------|:-------------|:----------------------|
| **Bronze** | Raw, unprocessed data as received from source systems (ERP, CRM). | Tables | Full Load (Truncate + Insert) | None – data stored as-is for traceability |
| **Silver** | Cleaned, standardized, and harmonized data ready for business transformations. | Tables | Full Load | Data cleansing, normalization, enrichment |
| **Gold** | Business-ready, integrated data model for analytics and reporting. | Views | Virtual (No Load) | Business logic, aggregations, KPIs, star schema |

**Separation of Concerns Principle:**  
Each layer has a unique responsibility—no duplication or overlap of transformations across layers.

---

## 🧩 Project Components

### 1. Requirement Analysis
- Consolidate sales and customer data from **ERP** and **CRM** systems.  
- Build a warehouse that supports **analytical reporting** and **decision-making**.  
- Handle **data quality issues** before analysis.  
- Focus on **non-historical (SCD Type 1)** reporting.

### 2. ETL/ELT Pipeline
- Designed using **SQL Server** stored procedures and SQL scripts.  
- ETL stages: **Extract → Transform → Load**  
- Supports **incremental & full loads**, **data cleansing**, and **data integration**.  
- Includes **naming conventions**, **standardized schema**, and **error handling**.

### 3. Data Modeling
- **Star Schema** design for analytical data marts.  
- Fact and Dimension modeling (e.g., `fact_sales`, `dim_customers`, `dim_products`).  
- Integrated ERP and CRM data into unified gold layer views.

### 4. Documentation & Planning
- **Notion** used for project management and task tracking (Epics, Subtasks, Progress Bars).  
- **Draw.io** used for architectural diagrams and layer representation.  
- **GitHub** repository used for version control and collaboration.

---

## 🧠 Core Concepts Implemented
- ETL vs ELT design thinking  
- Data Quality Management  
- Data Integration from multiple systems  
- Slowly Changing Dimensions (SCD Type 1)  
- Naming Conventions & Schema Standardization  
- Data Lineage and Traceability  
- Medallion Architecture Best Practices  
- Principle of Separation of Concerns  

---

## 🧰 Tech Stack

| Category | Tools/Technologies |
|-----------|--------------------|
| **Database Platform** | SQL Server Express |
| **Development Client** | SQL Server Management Studio (SSMS) |
| **Data Modeling** | Draw.io |
| **Project Planning** | Notion |
| **Version Control** | GitHub |
| **ETL Implementation** | SQL Scripts & Stored Procedures |
| **BI Layer (Optional)** | Power BI for Gold Layer Visualization |

---

## 🗂️ Project Folder Structure
```
c:\Users\Dinesh Kumar Verma\Desktop\Data_Warehouse\
├───.gitignore
├───LICENSE
├───README.md
├───.git\...
├───datasets\
│   ├───source_crm\
│   │   ├───cust_info.csv
│   │   ├───prd_info.csv
│   │   └───sales_details.csv
│   └───source_erp\
│       ├───CUST_AZ12.csv
│       ├───LOC_A101.csv
│       └───PX_CAT_G1V2.csv
├───docs\
│   ├───data_architecture.png
│   ├───data_catalog.md
│   ├───data_flow.png
│   ├───data_integration.png
│   ├───data_layers.pdf
│   ├───data_model.png
│   └───ETL.png
├───scripts\
│   ├───init_database.sql
│   ├───bronze\
│   │   ├───ddl_bronze.sql
│   │   └───proc_load_bronze.sql
│   ├───data_analytics\
│   │   ├───01_database_exploration.sql
│   │   ├───02_dimensions_exploration.sql
│   │   ├───03_date_range_exploration.sql
│   │   ├───04_measures_exploration.sql
│   │   ├───05_magnitude_analysis.sql
│   │   ├───06_ranking_analysis.sql
│   │   ├───07_change_over_time_analysis.sql
│   │   ├───08_cumulative_analysis.sql
│   │   ├───09_performance_analysis.sql
│   │   ├───10_data_segmentation.sql
│   │   ├───11_part_to_whole_analysis.sql
│   │   ├───12_report_customers.sql
│   │   └───13_report_products.sql
│   ├───gold\
│   │   └───ddl_gold.sql
│   └───silver\
│       ├───ddl_silver.sql
│       └───proc_load_silver.sql
└───tests\
    ├───quality_checks_gold.sql
    └───quality_checks_silver.sql
```
---

## 📊 Key Deliverables
- ✅ End-to-End SQL Warehouse following Medallion design  
- ✅ ETL pipeline handling full data refreshes  
- ✅ Data model for analytics and reporting  
- ✅ Documentation and architecture diagrams  
- ✅ BI-ready views in the Gold Layer  

---

## 🌟 Outcomes & Learnings
Through this project, I mastered:
- Designing scalable **data architectures** from scratch  
- Building **ETL/ELT pipelines** using only SQL logic  
- Applying **data governance and standardization practices**  
- Implementing **Medallion architecture** effectively for SQL-based systems  
- Creating **analytical-ready datasets** for Power BI and other tools  

---

## 🙏 Acknowledgements
I would like to express my gratitude to the YouTube channel **Data with Baraa** (@DataWithBaraa) for their invaluable tutorials and guidance, which were instrumental in the successful completion of this project.

---

## 👨‍💻 Author
**Dinesh Kumar Verma**  
🎯 *Aspiring Machine Learning & Data Engineering Professional*  
💼 Skilled in SQL, Python, Data Modeling, and Modern Data Architectures  
🔗 [LinkedIn](https://www.linkedin.com/in/dinesh-verma-707126184/)
