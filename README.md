# 📈 Stock Market Data Pipeline

This is a data engineering portfolio project designed to demonstrate a complete, production-grade data pipeline using the [Astro](https://www.astronomer.io/) platform. The pipeline ingests stock market data from an external API, processes and stores it using modern data engineering tools, and visualizes the results in Metabase. Real-time error notifications are sent to Slack if the pipeline fails.

## 🚀 Project Architecture
API → Airflow → MinIO → Spark → PostgreSQL → Metabase

### 🔧 Tools and Technologies

| Tool          | Purpose                                                  |
|---------------|----------------------------------------------------------|
| **Astro**     | Orchestrates and manages the entire Airflow environment |
| **Airflow**   | Schedules and monitors the ETL pipeline                  |
| **MinIO**     | Stores raw and intermediate data (S3-compatible object storage) |
| **Apache Spark** | Transforms and processes data efficiently in batch      |
| **PostgreSQL**| Stores the cleaned and transformed data                 |
| **Metabase**  | Visualizes stock market data and trends                 |
| **Slack**     | Sends alerts on pipeline failures                       |

---

## 🧪 Features

- 🔄 Scheduled data ingestion from a stock market API
- 🗂️ Storage of raw data in MinIO as Parquet/CSV
- ⚙️ Data transformation with Spark (cleaning, type casting, aggregations)
- 🛢️ Loading cleaned data into PostgreSQL for BI consumption
- 📊 Dashboarding using Metabase
- 🚨 Slack integration for real-time pipeline failure notifications
