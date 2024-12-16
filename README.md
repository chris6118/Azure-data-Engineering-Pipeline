
## Cloud Data Engineering and Visualization with Azure 

### Problem Statement

The aim of this project was to transform an unstructured sales dataset into a structured and visualized format to enable better insights for business decision-making. The key problem addressed was organizing raw data into a clean and structured form and then visualizing the results in Power BI for actionable insights. The insights derived help improve operational efficiency and customer satisfaction for the airline industry.

### Solution Overview

The project employed Azure tools and Power BI to build a data pipeline for processing and visualizing data using ETL proccesses( Extract, Transform and Load), following these steps:

### Project Architecture
![Screenshot 2024-12-16 221832](https://github.com/user-attachments/assets/64f92120-3a22-4245-86c3-6cee1e00f29c)


### Data Integration:

 Connected SQL Server Management Studio (SSMS) with Azure Data Factory using Self-Integration Runtime to securely move data.
Data Transformation: Utilized Azure Data Lake for layered storage (Bronze, Silver, and Gold) and Azure Databricks for data cleaning and transformation.

### Data Analytics:

Loaded the clean, structured data into Azure Synapse Analytics for further preprocessing.

### Schema Tables: 
Integrated Power BI with Azure Synapse to create dashboards for visual analytics.

![Screenshot 2024-12-16 023404](https://github.com/user-attachments/assets/0f085487-725b-4cfc-a5ea-59b7937a15ec)

### Data Visualization
![Screenshot 2024-12-10 083922](https://github.com/user-attachments/assets/5b7d51fb-e809-4d28-a1c4-f8a15428dc30)


### Steps
1. Data Loading
Raw, unstructured sales data was imported into SQL Server Management Studio.
Connected SQL Server Management Studio to Azure Data Factory using Self-Integration Runtime.

2. Data Storage in Azure Data Lake
Created a link service between Azure Data Factory and Azure Data Lake.
Raw data was copied to the Bronze layer in Azure Data Lake for initial ingestion.
Moved data to the Silver layer for preprocessing, including:
Date reformatting
Missing value checks
Transformation rules applied using Azure Databricks.
Cleaned and semi-structured data was stored in the Gold layer, ready for further analysis.

3. Data Preprocessing in Azure Synapse
Data from the Gold layer was transferred to Azure Synapse Analytics.
Conducted additional preprocessing using SQL pools in Synapse for improved query performance and data analytics.

4. Data Visualization in Power BI
Connected Azure Synapse to Power BI for real-time analytics and visualization.
Designed a Power BI dashboard showcasing key metrics and insights for airline performance.

### Conclusion
The implementation of this end-to-end pipeline allowed for the seamless processing of unstructured data into a structured format and enabled actionable business insights through Power BI/moving company's dataset to cloud. The airline industry can leverage this dashboard to focus on critical areas like reducing delays, improving customer satisfaction, and enhancing key services such as Wi-Fi and online booking.
Further improvements in the pipeline could include real-time data ingestion for live analytics and the incorporation of advanced AI models for predictive analytics with the help of Azure Fabrics.

