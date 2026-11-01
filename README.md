This project focuses on understanding and implementing modern Databricks Lakehouse capabilities using the latest Databricks terminology and features (2026).

A hands-on retail analytics project demonstrating a multi-source Lakehouse architecture on Databricks. The repository includes source datasets, Auto Loader ingestion for transaction files, Lakeflow Spark Declarative Pipelines transformations, dimensional/analytical SQL, a Metric View, and an AI/BI dashboard definition.

# 1. Project overview
Retail organizations need to combine product, inventory, customer, sales-opportunity, and transaction data to understand sales performance and operational health.

RetailQ brings these data domains together in Databricks and organizes them into a Bronze–Silver–Gold architecture:
- Bronze: source-aligned data landed in Unity Catalog tables.
- Silver: standardized and quality-checked data, with business rules applied.
- Gold: fact and dimension objects designed for analytics.
- Semantic layer: a Metric View defines reusable dimensions and measures.
- Consumption: an AI/BI dashboard visualizes sales performance.
  
Business questions supported
The included semantic model and dashboard are designed to answer questions such as:
- How is revenue trending over time?
- Which product categories and brands contribute the most revenue?
- How does revenue vary by billing state, country, and customer type?
- Which sales channels and payment modes are used most?
- How do transactions vary by opportunity stage?
- What are the total revenue, transaction count, unique customers, and average transaction value?

# 2. Architecture
<img width="1000" alt="pic1" src="https://github.com/user-attachments/assets/42c25505-e96d-434c-8f30-619597b25705" />

# 3. Technology stack
| Technology | Usage |
|---|---|
| Azure Databricks | Lakehouse development and execution platform |
| Apache Spark / PySpark | Distributed data transformations |
| Spark SQL | Gold views, calendar dimension, and Metric View definition |
| Lakeflow Spark Declarative Pipelines | Declarative Silver and Gold pipeline datasets |
| Auto Loader | Incremental file discovery and CSV ingestion |
| Delta Lake | Managed, reliable table storage |
| Unity Catalog | Data organization, governance, and access control |
| Metric Views | Reusable business measures and dimensions |
| Databricks AI/BI Dashboards | Retail performance visualization |
| PostgreSQL | Product and inventory source data |
| Salesforce extracts | Account and opportunity source data |
| CSV / cloud files | Transaction history and incremental transaction files |

Current Databricks terminology
- Delta Live Tables (DLT) is now referred to as Lakeflow Spark Declarative Pipelines.
- Databricks Workflows is now referred to as Lakeflow Jobs.
- Genie Spaces is now referred to as Genie Agents

# 14. Learning outcomes
This project provides practical exposure to:
- Multi-source data ingestion patterns
- Auto Loader and incremental file processing
- Medallion architecture
- PySpark transformations and Spark SQL
- Lakeflow Spark Declarative Pipelines
- Data-quality expectations
- Dimensional modeling and fact/dimension objects
- Unity Catalog organization and governance
- Metric Views and semantic modeling
- Databricks AI/BI dashboards
