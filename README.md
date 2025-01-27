## Tech Stack: 
Azure Data Factory, Azure Databricks, Azure Data Lake Storage, Apache Spark, Azure Synapse Analytics, Python, SQL.


### Project Introduction

In this project, we will:
- Extract data from an API using Azure Data Factory.
- Transform the data using Azure Databricks.
- Load the transformed data back into Azure Data Lake Storage.
- Perform data analysis using Azure Synapse Analytics.


**Project Overview:**
- Execute a complete data engineering project on Azure Cloud from start to finish.
- Extract data, perform transformations, load data, and conduct analysis.
- Build a simple data pipeline to copy, transform, and load data.

### Data
Link : https://www.kaggle.com/datasets/arjunprasadsarkhel/2021-olympics-in-tokyo

About Dataset
Details
This contains the details of over 11,000 athletes, with 47 disciplines, along with 743 Teams taking part in the 2021(2020) Tokyo Olympics.
This dataset contains the details of the Athletes, Coaches, Teams participating as well as the Entries by gender. It contains their names, countries represented, discipline, gender of competitors, name of the coaches.

Will update the dataset with medals(gold, silver, bronze), more details about the athletes after few weeks.

### Architecture & Prerequisites

**Architecture Diagram:**
![architecture](Architectue.png)
- Built on the ETL (Extract, Transform, Load) process using Azure Cloud services.
- Data source → Ingestion mechanism → Data storage → Transformation using Apache Spark.

**Prerequisites:**
- Basics of Python and SQL.
- An Azure account.

### Understanding the Dataset & APIs

**Dataset Details:**
- Contains information about 11,000 athletes, 47 disciplines, and 743 teams from the Tokyo Olympics 2021.
- Data includes team names, country names, athletes, coaches, and medals.
- Data is stored in CSV format on a GitHub repository.

### Azure Basics, Services Understanding, Account Setup

**Azure Account Setup:**
1. **Create an Azure Account:**
   - Sign up on the Azure portal with your email.
   - Create a free trial subscription with $200 USD credit.

2. **Create Resource Groups:**
   - Logical grouping of different resources based on subscriptions.

3. **Azure Data Factory:**
   - A data integration service to create, schedule, and manage data pipelines.

4. **Azure Data Lake Storage Gen 2:**
   - Combines capabilities of data lakes with Azure Blob Storage.

5. **Azure Databricks:**
   - A managed service for Apache Spark to write transformation code.

6. **Azure Synapse Analytics:**
   - An analytics service for SQL queries and data analysis.

### Complete Project Execution

**Step-by-Step Execution:**

1. **Set Up Azure Data Lake Storage:**
   - Create a storage account with hierarchical namespace enabled.
   - Create containers for raw data and transformed data.

2. **Use Azure Data Factory:**
   - Create a Data Factory pipeline to extract data from GitHub and load it into Azure Data Lake Storage.
   - Configure linked services for data sources (GitHub) and sinks (Azure Data Lake Storage).
   - Create pipelines and activities for data movement.

3. **Set Up Azure Databricks:**
   - Create an Azure Databricks workspace and cluster.
   - Write and execute PySpark code for data transformation.
   - Connect Databricks to Azure Data Lake Storage using service principal credentials.

4. **Transform Data Using Azure Databricks:**
   - Read raw data from Azure Data Lake Storage.
   - Perform basic transformations using PySpark.
   - Write transformed data back to Azure Data Lake Storage.

5. **Analyze Data Using Azure Synapse Analytics:**
   - Load transformed data into Synapse Analytics.
   - Perform SQL queries and analysis.
   - Optionally, build dashboards using Power BI or other tools.

### Important Steps in Azure for This Project

1. **Create Azure Account:**
   - Sign up and create a free trial subscription.

2. **Set Up Resource Group:**
   - Create a logical group for project resources.

3. **Create Storage Account:**
   - Enable hierarchical namespace and create containers for raw and transformed data.

4. **Configure Azure Data Factory:**
   - Set up linked services, create pipelines, and define activities for data extraction and loading.

5. **Set Up Azure Databricks:**
   - Create a workspace and cluster, write PySpark transformation code, and connect to Azure Data Lake Storage.

6. **Use Azure Synapse Analytics:**
   - Load transformed data and perform SQL queries for analysis.

By following these steps, you will be able to execute the entire data engineering project on Azure Cloud, from data extraction to transformation and analysis.
