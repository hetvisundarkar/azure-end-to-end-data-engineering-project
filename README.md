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
<img width="1536" height="1024" alt="Architecture" src="https://github.com/user-attachments/assets/abe07093-0696-4ba7-9140-d11110eda36b" />

## Azure Resources Setup
This shows the initial Azure setup of Resource Group.  
<img width="1476" height="794" alt="resource_group" src="https://github.com/user-attachments/assets/fd5c76aa-e24a-41a8-9c8b-8759f7d2ea7c" />

## Data Lake Containers
This shows the Bronze, Silver, and Gold containers created in Azure Data Lake Storage Gen2.  
<img width="1920" height="912" alt="Containers" src="https://github.com/user-attachments/assets/b1145b22-a7c1-4ad8-9438-05adb2f7858c" />

## Databricks Notebook
This shows the Databricks notebook where data is cleaned and transformed from Bronze to Silver.  
<img width="1920" height="912" alt="databricks_notebook1" src="https://github.com/user-attachments/assets/ed32bdfa-e162-4494-9618-842fa2903bde" />
<img width="1920" height="912" alt="databricks_notebook2" src="https://github.com/user-attachments/assets/e6c508b7-847b-4476-8f0c-5b5d7f406d33" />
<img width="1920" height="912" alt="databricks_notebook3" src="https://github.com/user-attachments/assets/e9905511-b556-4e16-a800-f5b8aa2d717d" />
<img width="1920" height="912" alt="databricks_notebook4" src="https://github.com/user-attachments/assets/5a0d9a42-0ac0-4679-86d5-7b97cc562bb1" />


## Synapse Tables
This shows the tables and views created in Azure Synapse Analytics from the Silver/Gold layer data.  
<img width="1920" height="912" alt="synapse" src="https://github.com/user-attachments/assets/6dcaf203-c377-4bfe-96cc-d0c052cb8f81" />
<img width="1920" height="912" alt="synapse_tables" src="https://github.com/user-attachments/assets/9ef9dc0f-e922-4edc-a241-496deb5061eb" />

## Power BI Dashboard
This shows the Power BI dashboard built on top of Synapse data for reporting and insights.  
<img width="1632" height="1080" alt="Power BI" src="https://github.com/user-attachments/assets/4dd899a5-02e6-43bb-880f-1a89ab82da90" />

