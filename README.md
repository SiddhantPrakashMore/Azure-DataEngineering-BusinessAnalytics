# Azure Data Engineering Project

## Overview
This project demonstrates an end-to-end data engineering pipeline using Azure services. It involves fetching, storing, transforming, analyzing, and visualizing data sourced from the GitHub API.

## Data Source
- **GitHub API**: The pipeline uses GitHub API data as its primary data source.

## Project Architecture
The solution follows a **medallion architecture** with distinct layers to efficiently manage data:

### Bronze Layer (Raw Data)
- **Data Ingestion**: Data is fetched using Azure Data Factory (ADF) via HTTP from GitHub API and stored unprocessed.

### Silver Layer (Cleaned Data)
- **Data Transformation**: Data transformation is performed using Databricks with PySpark. This process involves cleaning, structuring, and enriching raw data from the bronze layer, resulting in refined data ready for analysis.

### Gold Layer (Optimized Data)
- **Analytics & BI**: The gold layer stores the final, optimized datasets suitable for analytical queries. Azure Synapse Analytics is utilized for executing analytical queries, and Power BI provides dashboards and visual insights.

## Technologies Used
- **Azure Data Factory (ADF)** for data ingestion.
- **Azure Data Lake** for structured data storage following medallion architecture.
- **Databricks (PySpark)** for efficient data processing and transformation.
- **Azure Synapse Analytics** for advanced analytical querying.
- **Power BI** for interactive dashboards and visualization.

## Key Benefits
- Efficient, scalable data management with Azure.
- Structured approach to data storage and processing.
- Seamless integration with analytical and visualization tools to derive actionable insights.

