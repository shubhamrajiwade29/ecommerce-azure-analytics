# Architecture
See the main README for the end-to-end diagram. Screenshots live in `docs/screenshots/`.

```mermaid
flowchart LR
  subgraph Source
    R[Marketplace CSVs]
  end
  subgraph Azure
    ADF[Azure Data Factory<br/>Copy Activity]
    RAW[(Blob: rawdata/)]
    DBX[Databricks Notebook<br/>PySpark]
    CLN[(Blob: outputdata/cleaned_csv)]
  end
  subgraph BI
    PBI[Power BI Dataset & Report<br/>Scheduled Refresh]
  end

  R --> ADF --> RAW --> DBX --> CLN --> PBI

