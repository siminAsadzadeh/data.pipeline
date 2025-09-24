# data.pipeline
```mermaid
flowchart LR
    A[Branch CSV Files (transactions)] --> B[Azure Blob Storage (Raw Data)]
    B --> C[Azure Data Factory (ADF) + Spark/Databricks ETL Process]
    C --> D[Azure Synapse (Clean Data Warehouse)]
    D --> E[Power BI (Dashboard)]

```
