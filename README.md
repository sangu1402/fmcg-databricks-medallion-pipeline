# FMCG Databricks Medallion Pipeline

An end-to-end **Data Engineering project** that builds a scalable analytics platform to solve **post-merger data chaos** in the FMCG domain using **Databricks Lakehouse architecture**.

---

## 📌 Project Overview

After a corporate acquisition, data from a startup company was scattered across spreadsheets, APIs, and inconsistent formats, making unified reporting impossible.  
This project simulates that real-world challenge and delivers a **centralized, BI-ready analytics layer**.

**Goal:**  
Transform raw, messy data into reliable insights using a **Bronze–Silver–Gold Medallion Architecture**.

---
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/a5d42fe7-f637-4f56-ab83-18cbbf7a8b2f" />


## 🏗️ Architecture

**Tech Stack**
- Databricks (Lakehouse)
- PySpark
- SQL
- AWS S3
- Databricks Jobs
- Databricks Dashboards
- AI Genie

**Data Flow**

OLTP / Files → S3 → Bronze → Silver → Gold → Dashboards / AI Genie

---

## 🥉 Bronze Layer (Raw Ingestion)
- Ingest raw files from AWS S3
- Preserve source data with minimal transformation
- Supports historical backfill

---

## 🥈 Silver Layer (Cleaned & Standardized)
- Data cleansing using PySpark & SQL
- Regex-based sanitization
- Date normalization across formats
- Handling null, negative, and “unknown” values
- Surrogate key generation using SHA hashing

---

## 🥇 Gold Layer (Analytics Ready)
- Aggregated, business-level tables
- Revenue and product performance metrics
- Unified reporting across parent & child companies
- Optimized for dashboards and analytics

---

## ⚙️ Pipelines & Orchestration
- Batch pipelines for historical data
- Incremental pipelines for daily updates
- Automated using Databricks Jobs

---

## 📊 Analytics & Insights
- Databricks Dashboards for leadership reporting
- AI Genie used for natural language analytics
- KPIs:
  - Revenue trends
  - Top-performing products
  - Cross-company performance comparison

---

## 🧠 Key Learnings
- Designing scalable Medallion architectures
- Handling unreliable source identifiers
- Building fault-tolerant ETL pipelines
- Applying real-world data engineering best practices

---

## 🚀 How to Run
1. Upload raw data files to AWS S3
2. Configure Databricks cluster / SQL Warehouse
3. Run Bronze → Silver → Gold notebooks
4. Trigger jobs for automated ingestion
5. Query Gold tables or view dashboards

---

## 🙌 Acknowledgements
Inspired by hands-on learning from **Dhaval Patel** and **Hemanand Vadivel**  
(Codebasics YouTube Channel)

---

## 📎 Tags
#DataEngineering #Databricks #PySpark #SQL #AWS #ETL #Lakehouse #FMCG
