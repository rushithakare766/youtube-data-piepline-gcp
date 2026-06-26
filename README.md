# 🚀 YouTube Trending Data Pipeline on Google Cloud Platform (GCP)

An end-to-end **Data Engineering** project built on **Google Cloud Platform (GCP)** using the **Medallion Architecture (Bronze → Silver → Gold)**. This pipeline ingests YouTube trending data, performs transformations, validates data quality, and creates analytics-ready datasets in **BigQuery**.

---

## 📌 Architecture

![Architecture Diagram](YouTube%20Trending%20Data%20Pipeline.png)


---

## 📖 Project Overview

This project demonstrates how to build a scalable and production-ready data pipeline using managed GCP services.

### Workflow

1. Ingest data from YouTube API and streaming sources.
2. Store raw data in the Bronze layer (Cloud Storage).
3. Clean and transform data using Cloud Functions and Apache Beam (Dataflow).
4. Validate data quality.
5. Create business-ready aggregated datasets.
6. Store analytics data in BigQuery.
7. Visualize insights using Looker Studio.

---

## 🏗️ Architecture Layers

### 🥉 Bronze Layer
- Cloud Storage
- Cloud Scheduler
- Dataplex

Stores raw JSON and CSV files.

---

### 🥈 Silver Layer
- Cloud Functions
- Apache Beam
- Dataflow
- Cloud Storage
- Data Catalog

Transforms and cleans raw data into Parquet format.

---

### ✅ Data Quality

- Cloud Functions
- Cloud Monitoring
- Cloud Pub/Sub

Validates data and sends alerts for failures.

---

### 🥇 Gold Layer

- Apache Beam
- Dataflow
- BigQuery

Creates business-ready datasets including:
- Trending Analytics
- Channel Analytics
- Category Analytics

---

### 📊 Analytics

- BigQuery
- Looker Studio

Query and visualize the processed data.

---

## ⚙️ Tech Stack

| Service | Purpose |
|----------|---------|
| Cloud Storage | Data Lake |
| Cloud Functions | Serverless Processing |
| Cloud Scheduler | Job Scheduling |
| Cloud Pub/Sub | Messaging & Notifications |
| Apache Beam | Data Processing |
| Dataflow | Stream & Batch Processing |
| BigQuery | Data Warehouse |
| Dataplex | Data Lake Governance |
| Data Catalog | Metadata Management |
| Cloud Monitoring | Monitoring & Alerts |
| Looker Studio | Dashboard & Reporting |

---

## 🔄 Pipeline Flow

```
YouTube API / Pub/Sub
          │
          ▼
Cloud Storage (Bronze)
          │
          ▼
Cloud Functions
          │
          ▼
Apache Beam (Dataflow)
          │
          ▼
Cloud Storage (Silver)
          │
          ▼
Data Quality Validation
          │
          ▼
Apache Beam (Aggregation)
          │
          ▼
BigQuery (Gold)
          │
          ▼
Looker Studio Dashboard
```

---

## ✨ Features

- Event-driven architecture
- Medallion Architecture
- Batch & Streaming Processing
- Serverless ETL
- Automated Data Validation
- Metadata Management
- Scalable Data Pipeline
- Analytics-ready Data Warehouse

---

## 📁 Repository Structure

```
youtube-trending-data-pipeline-gcp/
│
├── cloud_functions/
├── dataflow/
├── sql/
├── datasets/
├── images/
│   └── architecture.png
├── requirements.txt
└── README.md
```

---

## 🎯 Key Learnings

- Google Cloud Data Engineering
- Apache Beam Pipelines
- Dataflow Jobs
- Serverless ETL
- Data Lake Architecture
- BigQuery Analytics
- Cloud Monitoring
- Metadata Management

---

## 👨‍💻 Author

**Rushikesh Thakare**

If you found this project useful, don't forget to ⭐ the repository!
