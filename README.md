# End-to-End Azure Data Engineering Project Using Microsoft Fabric  

## Introduction  

This project showcases an **end-to-end data engineering solution** using **Microsoft Fabric**, focusing on building a **Bing News Data Analytics platform**. The pipeline demonstrates data ingestion, transformation, sentiment analysis, reporting, and alerting workflows to empower data-driven decision-making.  

---

## Architecture  
<img src="Architecture.jpeg" alt="Project Architecture" width="900"/>  
![Fabric](https://github.com/user-attachments/assets/2f9a0c5b-a9e6-4f4f-b1ac-3659e70384fe)

---

## Architecture Overview  

The project integrates multiple components of **Microsoft Fabric** to create a unified and scalable pipeline:  
1. **Data Ingestion**: Fetches raw JSON data from Bing API into the **Lake Database** using Data Factory.  
2. **Data Transformation**: Processes the raw data into structured Delta Tables with Synapse Data Engineering.  
3. **Sentiment Analysis**: Utilizes machine learning in Synapse Data Science to analyze news sentiment.  
4. **Data Visualization**: Power BI dashboards visualize trends and sentiment analysis results.  
5. **Alerts**: Data Activator triggers alerts for specific conditions like negative sentiments.  

---

## Technologies  

- **Microsoft Fabric**  
  - Data Factory  
  - Synapse Data Engineering (Spark Notebooks)  
  - Synapse Data Science  
  - Power BI  
  - Data Activator  
- **Bing Search API**  
- **OneLake**  

---

## Data Used  

The project uses the following datasets to simulate news data processing:  

1. **News Dataset**: Ingests JSON data from Bing API containing articles, headlines, and publication details.  
2. **Sentiment Dataset**: Enriched data with sentiment scores (positive, neutral, negative) processed through Synapse Data Science.  

---

## Data Model  

The project employs a structured data model based on the **Medallion Architecture**:  

- **Raw Layer (Bronze)**: Stores raw JSON files ingested from the Bing API.  
- **Processed Layer (Silver)**: Holds cleaned and transformed Delta Tables.  
- **Analytics Layer (Gold)**: Contains aggregated and analyzed data ready for reporting and visualization.  

---

## Scripts for Project  

1. **Ingestion Pipeline**: Automates data ingestion from the Bing API into OneLake.  
2. **Transformation Scripts**: Spark Notebooks for processing and structuring data.  
3. **Sentiment Analysis Scripts**: ML workflows for categorizing news sentiment.  
4. **Orchestration Pipeline**: Data Factory pipeline to manage the E2E workflow.  

---

## Project Details  

1. **Data Ingestion**: Ingested data from Bing API and stored it in **Lake Database**.  
2. **Data Transformation**: Used PySpark in Synapse Data Engineering for cleaning and structuring.  
3. **Sentiment Analysis**: Leveraged Synapse Data Science to classify sentiments using ML models.  
4. **Data Visualization**: Created an interactive Power BI dashboard to present insights.  
5. **Alerts**: Configured Data Activator to notify stakeholders about negative news trends.  

---

## Power BI Dashboard  
<img src="PowerBI-Dashboard.png" alt="Power BI Dashboard" width="900"/>  

---

## Conclusion  

This project demonstrates the seamless integration of **Microsoft Fabric** components to deliver a scalable, efficient, and fully automated data pipeline. It highlights modern data engineering practices by providing actionable insights through interactive dashboards and real-time alerting systems.  

---
