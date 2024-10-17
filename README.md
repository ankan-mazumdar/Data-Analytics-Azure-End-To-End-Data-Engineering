## Azure Olympic Data Analytics Project

This project demonstrates an end-to-end data engineering solution on Azure Cloud, focusing on extracting, transforming, and analyzing data from the Olympics. The project utilizes various Azure services, including Azure Data Factory, Databricks, Data Lake Storage, and Synapse Analytics, to showcase the capabilities of data engineering and analytics.

![image](https://github.com/user-attachments/assets/cdacf093-1b75-4e0c-b2bd-241d05fc8249)

### Project Overview

The dataset includes information about 11,000 athletes, 47 disciplines, and 743 teams participating in the  Olympics . The data is processed, transformed, and analyzed using Azure services to extract meaningful insights.

### Step-by-Step Implementation

1. **Azure Account Setup**
   - Create an Azure account and sign in to access Azure services.
   - Set up a new subscription and create a dedicated resource group for organizing the project resources.



![image](https://github.com/user-attachments/assets/83d59550-8096-4b03-81d9-4318fc003c21)

![image](https://github.com/user-attachments/assets/064b74be-606d-4590-b2fb-154c0f4881d8)


2. **Storage and Data Factory Setup**
   - Create an Azure Storage Account in your preferred region, enabling the hierarchical namespace for easy data management.
   - Set up Azure Data Factory (ADF) within the same resource group and configure networking and encryption settings.

![image](https://github.com/user-attachments/assets/56a5e972-d3db-4e13-8450-24b9362e4a45)


![image](https://github.com/user-attachments/assets/99373983-60c9-4d4c-b614-d3140a6c9f3d)


![image](https://github.com/user-attachments/assets/a2aa25f8-7e43-4990-8f11-0ddea0e6c7ea)

![image](https://github.com/user-attachments/assets/afcb179e-78ad-4575-82cf-b5ff08ffeaf8)


![image](https://github.com/user-attachments/assets/8cdabd27-95f1-4613-8edb-aa2b21fb452c)


3. **Data Extraction and Loading**
   - Extract data from a public API or a GitHub repository using Azure Data Factory.
   - Establish a connection (linked service) between the source (API/GitHub) and Azure Data Factory.
   - Create a pipeline in ADF to copy the data into Azure Data Lake Storage (ADLS). Validate and execute the pipeline to verify successful data transfer.
   - 
![image](https://github.com/user-attachments/assets/a3649c8e-93ad-4eaf-9589-89d8ab22f921)

![image](https://github.com/user-attachments/assets/73134a81-4623-4986-8a45-5b60e897779b)

![image](https://github.com/user-attachments/assets/09c05f17-7bdc-4e79-b712-bb34bcce507d)




![image](https://github.com/user-attachments/assets/8d8d381c-59a1-4203-a411-785bf36013c0)



![image](https://github.com/user-attachments/assets/1ccd97d0-2e03-42b1-92f2-3e7949e1291f)


![image](https://github.com/user-attachments/assets/9bd8d4bb-a5ad-4f79-bc56-9d0c1560849a)


![image](https://github.com/user-attachments/assets/ddd7297d-1c86-40d2-a724-0109ab4705ef)


Repeat copy for all files  

![image](https://github.com/user-attachments/assets/042dc953-5d07-454a-9226-9f457e5bf83e)

![image](https://github.com/user-attachments/assets/dfb5f899-0f15-45be-9103-29ff2fd9d7c2)

![image](https://github.com/user-attachments/assets/fdc20618-ccc1-4581-90d4-0880f358fcfc)

![image](https://github.com/user-attachments/assets/2f29c1f1-da99-4f66-af86-ad55d0e2358c)


![image](https://github.com/user-attachments/assets/27c52a44-0f46-4e95-add0-84fddbb4b10d)

![image](https://github.com/user-attachments/assets/14a6884e-7d53-44a4-90c4-a1036eb3516d)

![image](https://github.com/user-attachments/assets/aa517c8d-3415-45af-8fb0-f93ec8151770)




![image](https://github.com/user-attachments/assets/70877525-de12-42cc-8e83-d4e2b79be3e8)

![image](https://github.com/user-attachments/assets/65b589c8-1f65-4010-88ba-199ab9d171b2)


4. **Data Transformation with Azure Databricks**
   - Set up Azure Databricks and create a Spark cluster.
   - Establish a connection between Databricks and ADLS by mounting the storage using the necessary credentials (client ID, tenant ID, and secret).
   - Write and execute Spark code to transform the data as needed, such as filtering, aggregating, and reshaping the dataset.

![image](https://github.com/user-attachments/assets/10a793aa-0bea-4cd2-8581-d5815392954a)

![image](https://github.com/user-attachments/assets/1af86a03-c56e-4388-89a8-20823dcc91e9)


App registration to connect AzDF to AzDatadbricks-

![image](https://github.com/user-attachments/assets/db9e9d20-29fc-4193-9024-1d7121e5d5ee)


Put the Clientid and secrety ID in place-
![image](https://github.com/user-attachments/assets/d1bb7e01-0db6-4d1b-9aad-6bdd46905967)

![image](https://github.com/user-attachments/assets/fc762656-5fb1-4874-ad00-d6aac2d26835)

Access Control iAm for further permission-

![image](https://github.com/user-attachments/assets/5fbab87c-e81d-4c86-9bd0-6157e133fd43)

![image](https://github.com/user-attachments/assets/50dfd4d9-32c2-4023-a69f-a7d365256350)



![image](https://github.com/user-attachments/assets/7c62281a-d8e8-4670-b57e-26bef92f848f)


![image](https://github.com/user-attachments/assets/c55132df-09b4-4677-9d3f-b947911b6e60)


transformation, Appropriate datatype connversion with help of infer schema in spark-
![image](https://github.com/user-attachments/assets/e820562b-6075-422f-a9f8-424f385835e3)

![image](https://github.com/user-attachments/assets/d5e0dc4f-fb74-49e3-9f5e-c7dfb2c7b043)

![image](https://github.com/user-attachments/assets/c2d9a9a2-9de3-4216-998e-4865ce97ac97)


![image](https://github.com/user-attachments/assets/7e512965-8317-4d97-b1d7-1be9766e52f5)

Repartition-


![image](https://github.com/user-attachments/assets/9948ad7a-8aea-4402-bffc-48b15e4df02f)

![image](https://github.com/user-attachments/assets/84242272-66ae-4a53-a39d-fa3f2db55dd8)



5. **Data Analysis with Azure Synapse Analytics**
   - Set up an Azure Synapse Analytics workspace for further data exploration and analysis.
   - Load the transformed data into Synapse and write SQL scripts to perform analytics, including calculating total medals per country, filtering data based on athlete information, and other relevant metrics.
  
   - 
![image](https://github.com/user-attachments/assets/0c2d1535-4390-4ed4-9f90-0b3f0549f8c3)


![image](https://github.com/user-attachments/assets/bb4035b7-bd68-4457-92e6-4fd5aa9034f9)

If we need to create Apache spark Pool-
![image](https://github.com/user-attachments/assets/8c920eef-1c63-4288-abdd-2fc2534bd903)



![image](https://github.com/user-attachments/assets/2a701e7f-ed66-4f2a-99ec-dd265ba6e371)


![image](https://github.com/user-attachments/assets/b7644cd2-8d30-4956-b831-051442b689a7)


![image](https://github.com/user-attachments/assets/3c56502b-2b0a-49e3-87d6-d4464ff36c1d)


further tables-
![image](https://github.com/user-attachments/assets/42b55613-c1ed-4d0d-b36b-7b44350623ed)

![image](https://github.com/user-attachments/assets/c7c5b378-436b-474f-b317-49d7f66953ef)

![image](https://github.com/user-attachments/assets/3cfc484f-24f5-40af-896a-e2b6f55feea5)


6. **Visualization and Insights**
   - Use Power BI or Synapse Studio to visualize the data insights. Create dashboards that highlight key statistics such as medal distribution by country, athlete demographics, and performance metrics.
   - Customize charts and graphs to make the data easily understandable and interactive.


![image](https://github.com/user-attachments/assets/d7331d84-688d-4e95-9fb4-69006b7b4b49)


![image](https://github.com/user-attachments/assets/3b2028a8-8e94-49b6-aa10-8414ae57aa94)










### Additional Notes
- Ensure proper access permissions are configured when connecting services like Azure Databricks and ADLS.
- Validate and test each step thoroughly before moving on to the next to ensure data integrity and accuracy.
- Explore various Synapse features, including building pipelines, integrating data flows, and creating visualizations for enhanced analytics.



