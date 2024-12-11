# **Vancouver Parks Data Analytics Projects**

This portfolio highlights a series of data analytics projects aimed at analyzing Vancouver parks' usage and trends. The projects make use of advanced AWS services to ensure secure data storage, processing, analysis, and visualization, while providing valuable insights for city planners and stakeholders. Each project focuses on different aspects of park data and integrates AWS tools for scalable, efficient, and insightful data management.

---

## **1. Exploratory Data Analysis (EDA) on Vancouver Parks Data**  
**Project Title**: Exploring Vancouver Parks: An EDA Approach  

### **Objective**  
Perform exploratory data analysis (EDA) to uncover patterns in park usage, amenities, and geographic distribution. The goal is to understand relationships between park attributes and visitor trends to inform city planning decisions.

### **Dataset**  
- **Park ID**: Unique identifier for each park  
- **Park Name**: Name of the park  
- **Location**: Geographic coordinates (latitude, longitude)  
- **Size**: Area of the park in hectares  
- **Amenities**: List of facilities (e.g., playgrounds, trails, sports fields)  
- **Visitor Count**: Monthly or yearly visitor data  
- **Type**: Park type (e.g., community, regional, nature park)  

### **Methodology**  
- **Data Storage & Management**  
  - Store raw data in **Amazon S3** for scalable object storage.
    
![Data Ingestion](https://github.com/kartick-11/Data-Analyst-Kar/blob/main/Data_ingestion.png)

  - Use **AWS Data Pipeline** to automate data movement and transformation.  
  - **Amazon DynamoDB** stores metadata for park amenities and location details.  

- **Data Processing & Transformation**  
  - Clean and transform data using **AWS Glue**.  
  - Employ **AWS Glue DataBrew** for visual data wrangling.  

- **Data Analysis & Analytics**  
  - Query data using **Amazon Athena** with SQL.  
  - Use **Amazon SageMaker** to build ML models for park usage prediction.  

- **Security & Compliance**  
  - Encrypt data with **AWS Key Management Service (KMS)**.  
  - Monitor activities with **AWS CloudTrail** for auditing.  

- **Monitoring & Logging**  
  - Monitor pipeline health using **Amazon CloudWatch**.  

---

## **2. Descriptive Analysis of Park Visitor Patterns**  
**Project Title**: Analyzing Visitor Trends at Vancouver Parks  

### **Objective**  
Analyze visitor patterns by considering factors like park size, amenities, seasonal trends, and events. Provide insights and recommendations to improve park utilization.

### **Dataset**  
- **Visitor Count**: Daily, weekly, or monthly data.  
- **Park Features**: Information on amenities and characteristics.  
- **Weather Data**: Conditions such as temperature and rainfall.  
- **Event Data**: Local events affecting park usage.  

### **Methodology**  
- **Data Storage & Management**  
  - Store data in **Amazon S3**.  
  - Automate transformations with **AWS Data Pipeline**.  

- **Data Processing & Transformation**
  
![Data Profiling](https://github.com/kartick-11/Data-Analyst-Kar/blob/main/Data_profiling.png)

  - Use **AWS Glue** for data cleaning and transformation.  
  - Visualize transformations with **AWS Glue DataBrew**.  

- **Data Analysis & Analytics**  
  - Query with **Amazon Athena**.  
  - Predict trends using **Amazon SageMaker** ML models.  

- **Security & Compliance**  
  - Encrypt sensitive data with **AWS KMS**.  
  - Log activities with **AWS CloudTrail**.  

- **Monitoring & Logging**  
  - Use **Amazon CloudWatch** for real-time monitoring.  

---

## **3. Diagnostic Analysis of Visitor Decline in Parks**  
**Project Title**: Diagnosing Visitor Decline in Vancouver Parks  

### **Objective**  
Identify causes behind a decline in park visitor numbers and pinpoint issues such as accessibility, amenities, or seasonal variations.

### **Dataset**  
- **Visitor Count**: Trends at parks with declining numbers.  
- **Park Features**: Amenities and factors influencing visitation.  
- **External Factors**: Economic indicators or construction impacts.  

### **Methodology**  
- **Data Storage & Management**  
  - Secure data in **Amazon S3** and manage movement with **AWS Data Pipeline**.  

- **Data Processing & Transformation**  
  - Clean data using **AWS Glue**.

![Data Cleaning](https://github.com/kartick-11/Data-Analyst-Kar/blob/main/Data_cleaning.png)

  - Prepare data visually with **AWS Glue DataBrew**.  

- **Data Analysis & Analytics**  
  - Query data using **Amazon Athena**.  
  - Diagnose causes using ML models in **Amazon SageMaker**.  

- **Security & Compliance**  
  - Encrypt data with **AWS KMS**.  
  - Track API activity with **AWS CloudTrail**.  

- **Monitoring & Logging**  
  - Monitor workflows with **Amazon CloudWatch**.  

---

## **4. Data Quality Control for Vancouver Parks Data**  
**Project Title**: Data Quality Control for Vancouver Parks Data  

### **Objective**  
Implement a robust framework for ensuring the integrity, completeness, and accuracy of the park dataset.

### **Methodology**  
- **Data Storage & Management**  
  - Use **Amazon S3** for reliable storage.  
  - Automate data checks with **AWS Data Pipeline**.  

- **Data Processing & Transformation**  
  - Validate data quality with **AWS Glue**.  
  - Visual wrangling with **AWS Glue DataBrew**.  

- **Data Analysis & Analytics**  
  - Detect anomalies using **Amazon Athena**.  
  - Index datasets with **Amazon ElasticSearch Service**.  

- **Security & Compliance**  
  - Encrypt data with **AWS KMS**.  
  - Audit activities using **AWS CloudTrail**.  

- **Monitoring & Logging**  
  - Monitor processes with **Amazon CloudWatch**.  

---

## **5. Data Wrangling for Vancouver Parks Analytics**  
**Project Title**: Data Wrangling for Vancouver Parks Analytics  

### **Objective**  
Prepare raw data for downstream analysis using advanced wrangling techniques.

### **Dataset**  
- **Park Data**: Raw park information.  
- **Weather Data**: Temperature and rainfall data.  
- **Event Data**: Local events impacting visitation.  

### **Methodology**  
- **Data Storage & Management**  
  - Store raw data in **Amazon S3**.  
  - Transform data with **AWS Data Pipeline**.

![Data Pipeline](https://github.com/kartick-11/Data-Analyst-Kar/blob/main/Data_pipeline.png)

- **Data Processing & Transformation**  
  - Clean and structure data using **AWS Glue**.  
  - Use **AWS Glue DataBrew** for intuitive wrangling.  

- **Data Analysis & Analytics**  
  - Query structured data using **Amazon Athena**.  
  - Predict trends with **Amazon SageMaker**.  

- **Security & Compliance**  
  - Secure data with **AWS KMS**.  
  - Log actions using **AWS CloudTrail**.  

- **Monitoring & Logging**  
  - Monitor processes via **Amazon CloudWatch**.  

---

## **Additional Resources**  
To further explore the methodologies and tools utilized in these projects, refer to the following resources:

### **CC - Part 1: 
Descriptive Analysis**  
1. **Data Ingestion**: Collect raw data from various sources.  
2. **Data Profiling**: Understand data structure and anomalies.  
3. **Data Cleaning**: Ensure data quality and consistency.  
4. **Pipeline Design**: Automate data transformation and movement.  
   *For a detailed guide on implementing descriptive analysis, refer to the full **[CC - Part 1.docx](https://github.com/kartick-11/Data-Analyst-Kar/blob/main/CC%20-%20Part%201.docx)** document.*

### **Exploratory Analysis**  
1. **Data Enriching**: Integrate external data like weather or events.  
2. **Data Profiling and Cleaning**: Refine datasets for deep analysis.  
3. **Data Pipeline Design**: Support scalable data exploration.  

### **CC - Part 2: 
Advanced Processes**  
5. **Data Enriching**: Add calculated fields for deeper analysis.  
6. **Data Protection**: Secure data with encryption and access controls.  
7. **Data Governance**: Establish policies for compliance and accuracy.  
8. **Data Observability**: Monitor pipelines to ensure performance.  
   *For more insights on advanced processes, refer to the **[CC - Part 2.docx](https://github.com/kartick-11/Data-Analyst-Kar/blob/main/CC%20-%20Part2.docx)** document.*

---

## **Conclusion**  
These projects leverage AWS tools like **Amazon S3**, **AWS Data Pipeline**, **AWS Glue**, **Amazon Athena**, and **Amazon SageMaker** to enable efficient and secure data analytics. Insights derived from these projects can aid city planners in making data-driven decisions for better park management and urban planning.
```
