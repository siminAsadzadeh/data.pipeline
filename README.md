# data.pipeline
```mermaid
flowchart LR
    A[Branch CSV Files<br>(transactions)] --> B[Azure Blob Storage<br>(Raw Data)]
    B --> C[Azure Data Factory (ADF)<br>+ Spark/Databricks<br>ETL Process]
    C --> D[Azure Synapse<br>(Clean Data Warehouse)]
    D --> E[Power BI<br>(Dashboard)]

    style A fill:#f9f,stroke:#333,stroke-width:1px
    style B fill:#bbf,stroke:#333,stroke-width:1px
    style C fill:#bfb,stroke:#333,stroke-width:1px
    style D fill:#ffb,stroke:#333,stroke-width:1px
    style E fill:#fbb,stroke:#333,stroke-width:1px
```
