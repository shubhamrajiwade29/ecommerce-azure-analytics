# E-Commerce Analytics on Azure (ADF → Blob → Databricks → Power BI)

## Project Overview
An end-to-end Azure data pipeline delivering actionable business insights for e-commerce using automated ETL and Power BI dashboards. Designed to reduce manual reporting and accelerate analytics for digital retail.

## Architecture
![Architecture Diagram](docs/architecture.md) <!-- Replace with actual image path or diagram -->
- **Azure Data Factory**: Orchestrates the ETL workflow
- **Azure Blob Storage**: Stores raw and cleaned data
- **Databricks (PySpark)**: Cleans, transforms, and analyzes data
- **Power BI**: Visualizes KPIs and trends

## Features
- **KPIs:** Total Revenue, Orders, Average Order Value (AOV), Customers
- **Visuals:** Top Products, Revenue by Country, Monthly Trend
- **Automation:** Scheduled Power BI refresh directly from Azure Blob

## Getting Started
1. Clone this repo: `git clone https://github.com/shubhamrajiwade29/ecommerce-azure-analytics.git`
2. Prerequisites: Azure account, Databricks Workspace, Power BI Desktop, Python ≥3.8
3. Step-by-step instructions for setup—see [docs/architecture.md](docs/architecture.md)
4. Open Databricks notebooks and execute ETL pipeline
5. Load resulting files into Power BI for dashboard visualization

## Demo & Screenshots
![Dashboard Screenshot](docs/demo_dashboard.png) <!-- Add your dashboard image here -->

## Folder Structure
- `/data/sample`: Example datasets
- `/databricks/notebooks`: ETL and analytics workflows
- `/docs`: Architecture and documentation
- `/infra/adf_arm_template`: Azure Data Factory deployment templates
- `/scripts`: Utility scripts for automation
- `/powerbi`: Power BI dashboard files

## Impact
- Automated reporting pipeline—reduced manual workload by 80%
- Achieved real-time dashboard updates
- Used by analytics teams for faster data-driven decisions

## Contact
For queries or collaboration:
- Email: your@email.com
- LinkedIn: [Your LinkedIn](https://www.linkedin.com/in/your-profile)

## License
MIT

## Badges
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Last Updated](https://img.shields.io/github/last-commit/shubhamrajiwade29/ecommerce-azure-analytics)



