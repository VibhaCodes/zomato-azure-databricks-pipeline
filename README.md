# zomato-azure-databricks-pipeline
End-to-End Data Engineering Project using Azure Data Lake, Databricks, and Medallion Architecture

# 🍽️ Zomato Data Engineering Pipeline using Azure & Databricks

## 📌 Project Overview

This project implements an **end-to-end data engineering pipeline** using **Azure Data Lake Storage and Databricks**.

The pipeline follows the **Medallion Architecture (Bronze, Silver, Gold layers)** to process and transform raw Zomato dataset into meaningful business insights.

---

## 🚀 Objectives

- Ingest raw data from Azure Storage
- Clean and transform the dataset
- Generate business insights using Spark
- Store data in Delta format
- Build a structured data pipeline

---

## 🛠️ Technologies Used

- Azure Resource Group
- Azure Data Lake Storage (ADLS Gen2)
- Azure Databricks
- Apache Spark (PySpark)
- Unity Catalog
- Delta Lake
- GitHub

---

## 🏗️ Architecture
Azure Resource Group
↓
Storage Account
↓
Container (zomato-external)
↓
raw → bronze → silver → gold
↓
Databricks (Spark Processing)
↓
Unity Catalog
↓
Analytics Tables


---

## 📂 Project Structure

zomato-azure-databricks-pipeline/

│── notebooks/
│ ├── 01_bronze_ingestion.py
│ ├── 02_silver_transformation.py
│ ├── 03_gold_analytics.py
│ ├── 04_business_insights.py

│── screenshots/
│ ├── 01_resource_group.png
│ ├── 02_storage_account.png
│ ├── 03_container.png
│ ├── 04_folders_structure.png
│ ├── 05_databricks_workspace.png
│ ├── 06_cluster.png
│ ├── 07_catalog.png
│ ├── 08_bronze.png
│ ├── 09_silver.png
│ ├── 10_gold.png
│ ├── 11_pipeline.png



---

## 🔄 Pipeline Flow

### 1️⃣ Data Ingestion (Bronze Layer)
- Raw CSV file is stored in Azure Storage (`raw` folder)
- Data is read using Spark and stored in Delta format
- Saved in Bronze layer

### 2️⃣ Data Cleaning (Silver Layer)
- Remove duplicates
- Remove null values
- Clean invalid ratings
- Convert data types (e.g., rating → double)

### 3️⃣ Data Transformation (Gold Layer)
- Perform aggregations
- Calculate average ratings
- Generate business insights
- Store results in Gold layer

---

## 📊 Key Features

- End-to-end data pipeline
- Implementation of Medallion Architecture
- Use of Delta Lake for optimized storage
- Spark-based data processing
- Integration with Unity Catalog
- Automated pipeline using Databricks Jobs

---

## 📈 Business Insights Generated

- Top restaurants based on ratings
- City-wise restaurant count
- Average dining rating per city
- Average price per city

---

## 📸 Screenshots

### Azure Setup
![Resource Group](screenshots/01_resource_group.png)
![Storage Account](screenshots/02_storage_account.png)
![Container](screenshots/03_container.png)

### Data Pipeline
![Bronze Layer](screenshots/08_bronze.png)
![Silver Layer](screenshots/09_silver.png)
![Gold Layer](screenshots/10_gold.png)

### Pipeline Execution
![Pipeline](screenshots/11_pipeline.png)

---

## 🎯 Conclusion

This project demonstrates how to build a **real-world data engineering pipeline** using cloud technologies.

It showcases:
- Data ingestion
- Data transformation
- Data modeling
- Analytics generation

---

## 📌 Future Improvements

- Add real-time data ingestion
- Integrate Power BI dashboards
- Automate pipeline triggers
- Add advanced analytics

---

## 👩‍💻 Author

**Vibha Pateshwari**

---

## ⭐ Note

This project demonstrates practical implementation of **Data Engineering concepts using Azure and Databricks**, making it suitable for academic and professional use.
