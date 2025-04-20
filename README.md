
# 🏭Data Warehouse and Analytics Project

[](https://github.com/ayusyagol11/sql-data-warehouse-project/tree/main#data-warehouse-and-analytics-project)

Welcome to my **SQL Data Warehouse & Analytics Project**! 🚀

This project showcases a complete end-to-end solution for building a modern **data warehouse** using **SQL Server**, transforming raw data into business-ready insights. Designed as a portfolio project, it demonstrates my hands-on skills in **data engineering**, **ETL pipeline development**, and **analytics**.

----------
## **📌 Overview**


This repository presents a structured approach to data warehousing, adhering to the **Medallion Architecture**:
[![Data Architecture](https://github.com/ayusyagol11/sql-data-warehouse-project/blob/main/docs/data_architecture_diagram.png?raw=true)](https://github.com/ayusyagol11/sql-data-warehouse-project/blob/main/docs/data_architecture_diagram.png?raw=true)

-   🟤 **Bronze Layer** – Stores raw data as-is from the source systems. Data is ingested from CSV Files into SQL Server Database.
    
-   ⚪ **Silver Layer** – This layer includes data cleansing, standardization, and normalization processes to prepare data for analysis.
    
-   🟡 **Gold Layer** – Houses business-ready data modeled into a star schema required for reporting and analytics.
    

With data sourced from **ERP** and **CRM** systems (CSV format), I implemented ETL pipelines, created fact and dimension tables, and generated insights on **customer behavior**, **product performance**, and **sales trends**.

----------

## **🧱 Features**

-   🏗️ **Medallion Architecture** applied in SQL Server
    
-   🔄 **ETL Pipelines** for ingestion, cleaning, transformation, and modeling
    
-   🌐 **Star Schema Design** (Fact & Dimension tables)
    
-   📊 **Analytics-ready tables** supporting reporting needs
    
-   📚 **Documentation** for architecture, flow, and schema
    
-   💡 **SQL-based reporting** for key business metrics
    

----------

## **📂 Project Structure**

```
sql-data-warehouse-project/
│
├── datasets/                           # Raw CSV files from ERP and CRM
│
├── docs/                               # All documentation and visuals
│   ├── data_architecture_diagram.png   # Visual representation of architecture
│   ├── data_catalog.md                 # Gold Layer: Tables and column descriptions
│   ├── etl.drawio                      # ETL flow diagram
│   ├── data_models.drawio              # Star schema model
│   ├── naming-conventions.md           # Standards for naming
│
├── scripts/
│   ├── bronze/                         # Ingest raw data
│   ├── silver/                         # Transform & clean data
│   ├── gold/                           # Create business-level models
│
├── tests/                              # SQL validation and quality checks
│
├── README.md                           # This file
└── requirements.txt                    # Tools & dependencies
```

  

----------

## **🧪 Tech Stack & Tools**

-   **SQL Server Express** – Backend DBMS
    
-   **SSMS (SQL Server Management Studio)** – GUI for development
    
-   **Draw.io** – Architecture and data modeling diagrams
    
-   **Git & GitHub** – Version control and collaboration
    
-   **Notion** – Project planning and documentation
    

----------

## **📊 Key Insights Delivered**

-   📈 **Customer Behavior Analysis**
    
-   🛒 **Product Performance Metrics**
    
-   💰 **Sales Trend Insights**
    

Each of these was enabled through optimised SQL queries over the **Gold Layer**, empowering stakeholders with actionable intelligence.

----------

## **✅ What I Learned**

-   Real-world implementation of **Medallion Data Architecture**
    
-   Building efficient and reusable **ETL processes**
    
-   Hands-on practice with **dimensional modeling**
    
-   Writing performant and readable **SQL queries** for analytics
    
-   Importance of **clear documentation** and **naming conventions**
    

----------

## **🙋‍♂️ About Me**

  

Hi! I’m **Aayush Yagol**, a data enthusiast who loves turning raw data into insights that drive business decisions. This project was an exciting deep dive into data engineering, and I look forward to building more solutions that make working with data **fun**, **efficient**, and **impactful**.

  

📫 Let’s connect:
[![LinkedIn](https://camo.githubusercontent.com/8c0692475a5bfc1d9e7361074bdb648e567cae7b5b40ffd32adae31180b0d7b6/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4c696e6b6564496e2d3030373742353f7374796c653d666f722d7468652d6261646765266c6f676f3d6c696e6b6564696e266c6f676f436f6c6f723d7768697465)](https://www.linkedin.com/in/aayush-yagol-046874145/)  [![Website](https://camo.githubusercontent.com/6be01d8a2b092b992e6e78ace77c196697168ee95374472c7f7990733aed7de3/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f576562736974652d3030303030303f7374796c653d666f722d7468652d6261646765266c6f676f3d676f6f676c652d6368726f6d65266c6f676f436f6c6f723d7768697465)](https://www.aayushyagol.com/)
----------

### ⭐ If you found this project helpful or inspiring, feel free to star the repo and connect with me!⭐

  

