# Azure End-to-End Data Engineering Project

## Project Overview
This project demonstrates an end-to-end Azure Data Engineering pipeline following the Medallion architecture (Bronze → Silver → Gold).  
It covers data ingestion, storage, transformation, and visualization using multiple Azure services.

## Technologies Used
- Azure Data Factory (ADF) for data ingestion  
- Azure Data Lake Storage Gen2 (ADLS Gen2) as the data lake  
- Azure Databricks for data transformation using PySpark  
- Azure Synapse Analytics for serving the transformed data  
- Power BI for data visualization and reporting  

## Architecture and Workflow
1. Data is ingested from source (CSV/API/GitHub) using Azure Data Factory and stored in the Bronze container.  
2. Raw data from Bronze is cleaned, validated, and transformed in Azure Databricks, then stored in the Silver container.  
3. Transformed Silver data is further aggregated and modeled into the Gold container for analytics.  
4. Azure Synapse Analytics is used to query Gold data and build tables/views.  
5. Power BI connects to Synapse to build dashboards and visualize insights.  

## Architecture Diagram
![Resource Group](https://github.com/hetvisundarkar/azure-end-to-end-data-engineering-project/blob/main/Architecture.png?raw=true)

## Azure Resources Setup
This shows the initial Azure setup of Resource Group.  
![Containers](https://github.com/hetvisundarkar/azure-end-to-end-data-engineering-project/blob/main/resource_group.png?raw=true)

## Data Lake Containers
This shows the Bronze, Silver, and Gold containers created in Azure Data Lake Storage Gen2.  
![Containers](https://github.com/hetvisundarkar/azure-end-to-end-data-engineering-project/blob/main/Containers.png?raw=true)

## Databricks Notebook
This shows the Databricks notebook where data is cleaned and transformed from Bronze to Silver.  
![Containers](https://github.com/hetvisundarkar/azure-end-to-end-data-engineering-project/blob/main/databricks_notebook1.png?raw=true)
![Containers](https://github.com/hetvisundarkar/azure-end-to-end-data-engineering-project/blob/main/databricks_notebook2.png?raw=true)
![Containers](https://github.com/hetvisundarkar/azure-end-to-end-data-engineering-project/blob/main/databricks_notebook3.png?raw=true)
![Containers](https://github.com/hetvisundarkar/azure-end-to-end-data-engineering-project/blob/main/databricks_notebook4.png?raw=true)


## Synapse Tables
This shows the tables and views created in Azure Synapse Analytics from the Silver/Gold layer data.  
![Containers](https://github.com/hetvisundarkar/azure-end-to-end-data-engineering-project/blob/main/synapse.png?raw=true)
![Containers](https://github.com/hetvisundarkar/azure-end-to-end-data-engineering-project/blob/main/synapse_tables.png?raw=true)

## Power BI Dashboard
This shows the Power BI dashboard built on top of Synapse data for reporting and insights.  
![Containers](https://github.com/hetvisundarkar/azure-end-to-end-data-engineering-project/blob/main/Power%20BI.png?raw=true)

