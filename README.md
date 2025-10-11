# E-Commerce Analytics on Azure (ADF → Blob → Databricks → Power BI)

**Azure Data Factory** → **Azure Blob Storage** → **Databricks (PySpark)** → **Power BI**.

- **KPIs**: Total Revenue, Orders, AOV, Customers  
- **Visuals**: Top Products, Revenue by Country, Monthly Trend  
- **Automation**: Power BI scheduled refresh (Blob connection)

---

## Architecture

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
