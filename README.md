# Azure Data Lakehouse Project (Medallion Architecture)

## Overview
This project implements an end-to-end data lakehouse platform on Azure, transforming on-premise SalesLT data into a governed, analytics-ready layer using the Medallion (Bronze-Silver-Gold) architecture.

## 🏗️ Architecture

<img width="2507" height="1145" alt="image" src="https://github.com/user-attachments/assets/4012ca5f-2473-4303-ad1c-3fb5cda9f75a" />


## 🛠️ Tech Stack
| Layer | Technology |
|-------|------------|
| Ingestion | Azure Data Factory |
| Storage | Azure Data Lake Gen2 |
| Data Processing | Azure Databricks (PySpark, Delta Lake) |
| Data Serving | Azure Synapse Analytics (Serverless SQL) |
| Visualization | Power BI |
| Security | Azure Key Vault + Microsoft Entra ID |

## 📊 Data Flow
1. **Bronze Layer:** Raw data is ingested and stored as-is in ADLS Gen2.
2. **Silver Layer:** Data is cleaned, standardized (date format), and stored as Delta tables.
3. **Gold Layer:** Data is transformed (column naming to snake_case) and aggregated for analytics.

## 🔧 Setup Instructions
1. Clone this repository.
2. Deploy Azure resources using the scripts in `docs/`.
3. Configure ADF pipelines using JSON templates.
4. Run Databricks notebooks in sequence.
5. Connect Power BI to Synapse views.

## 📈 Dashboard Preview
<img width="1798" height="975" alt="image" src="https://github.com/user-attachments/assets/ca29db14-eecb-43d9-9b08-c3edd8e897fd" />


## 👤 Author
Haijun
