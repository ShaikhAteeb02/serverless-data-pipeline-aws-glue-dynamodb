# Serverless Data Pipeline on AWS

An end-to-end solution for building a scalable serverless data pipeline on AWS using DynamoDB, Glue, and Athena for automated ingestion, ETL, and analytics.

---

## Features

- Seamless data ingestion into DynamoDB tables
- Schema and metadata discovery with AWS Glue crawlers
- Automated ETL transformation jobs using Glue
- Secure access management via IAM roles and policies
- Fast analytics with Athena SQL querying

---

## Architecture Overview

This pipeline uses AWS DynamoDB to store incoming order data, Glue crawlers to catalog metadata and create tables in the Data Catalog, and Glue ETL jobs to transform and store processed data in Amazon S3. Athena enables fast, serverless querying for analytics purposes. IAM policies and roles manage secure permissions across each service component.

- **DynamoDB**: Stores order details with efficient schema-free structure.
- **Glue Crawler**: Automatically catalogs S3 data, enabling integration with Athena.
- **Glue ETL Job**: Transforms raw data and loads it into optimized S3 locations.
- **Athena**: Executes SQL queries against processed datasets for reporting.
- **IAM Roles**: Ensure least-privilege access and auditability.

---

## Setup Instructions

1. **Create DynamoDB Table**
    - Set order table with required keys.
    - Enable on-demand capacity for scalability.
2. **Configure Glue Crawler**
    - Define S3 source location.
    - Set up Glue Data Catalog database.
    - Run crawler to detect schema.
3. **Write Glue ETL Job**
    - Create a Python or Spark script to read, transform, and write data.
    - Schedule as needed or trigger manually.
4. **Define IAM Roles**
    - Attach read/write permissions for Glue, DynamoDB, and S3.
    - Use least-privilege principle.
5. **Athena Query Setup**
    - Connect Athena to Glue Data Catalog.
    - Write sample SQL queries and visualize as needed.

---

> For questions or collaborations, connect using the links below.

<p align="center">
  <a href="https://github.com/ShaikhAteeb02">
    <img src="https://img.shields.io/badge/GitHub-Profile-black?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
  </a>
  <a href="https://www.linkedin.com/in/ateeb-ahmed-shaikh-932234192/">
    <img src="https://img.shields.io/badge/LinkedIn-Profile-blue?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
</p>
