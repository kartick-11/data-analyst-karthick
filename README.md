# **Analyzing Park Visits: An Exploratory Data Analysis**

## **Project Description**
This project performs an exploratory data analysis (EDA) on a dataset of parks in Vancouver, enriched with visitor count information. The goal is to analyze how park features such as washrooms, facilities, and special features influence visitor counts and provide insights for urban planning and park management.

---

## **Project Objectives**
1. Enrich the dataset with the **Number of Visits** feature.  
2. Analyze the relationships between park amenities and visitor engagement.  
3. Provide actionable insights to improve park planning and resource allocation.  

---

## **Dataset Overview**
The dataset contains detailed information about parks, including:  
- **Park_ID:** Unique identifier for each park.  
- **Name:** Name of the park.  
- **Facilities:** Availability of features like playgrounds, picnic areas, or sports courts.  
- **Washrooms:** Presence of washroom facilities.  
- **Special_Features:** Unique features such as monuments or attractions.  
- **Neighbourhood:** The geographic location of the park.  
- **Number_of_Visits:** Total number of visits to each park (added during data enrichment).  

---

## **Methodology**

### **Step 1: Data Collection and Preparation**
1. **Data Storage:**  
   - The dataset was stored using **AWS S3 Glacier Instant Retrieval** for secure and cost-effective storage.  
2. **Data Retrieval:**  
   - The enriched dataset was loaded into the analysis environment for processing.  
3. **Enrichment:**  
   - Added the **Number_of_Visits** feature to enable visitor analysis.  

---

### **Step 2: Descriptive Statistics**
1. **Numerical Features:**  
   - Calculated summary statistics for **Number_of_Visits** (mean, median, max, and total visits).  
2. **Categorical Features:**  
   - Generated frequency distributions for parks with **Facilities**, **Washrooms**, and **Special_Features**.  

---

### **Step 3: Data Profiling and Cleaning**
1. **Profiling:**  
   - Used **AWS Glue DataBrew** to identify missing values, inconsistencies, and data quality issues.  
2. **Cleaning Steps:**  
   - Renamed columns for clarity (e.g., `NeighbourhoodName` to `Neighbourhood_Name`).  
   - Removed leading/trailing white spaces in categorical fields.  
   - Replaced missing values in critical columns (`EW_Street`, `NS_Street`) with "null".  

---

### **Step 4: Data Visualization**
1. **Bar Charts:** Compared visit counts for parks with and without specific amenities.  
2. **Pie Charts:** Showed the proportion of parks with comprehensive features.  
3. **Heatmaps:** Visualized correlations between park amenities and visitor counts.  

---

### **Step 5: Analysis of Parks with All Three Features**
1. Focused analysis on parks with **Washrooms**, **Facilities**, and **Special_Features**:  
   - Total Visits: Of the 122,936 visits, 5,981 were to parks with all three amenities.  
   - Key Insight: Parks with comprehensive features attract fewer but more engaged visitors.  

---

### **Step 6: Data Protection**
1. **Secure Storage:** Used **AWS S3 Glacier Instant Retrieval** to protect data and ensure cost-effective access.  
2. **Access Management:** Configured access policies to restrict unauthorized access.  

---

### **Step 7: Data Governance**
1. **Documentation:** Maintained metadata for all features, including descriptions and data types.  
2. **Compliance:** Ensured adherence to data privacy and security regulations.  

---

### **Step 8: Data Observability**
1. **Monitoring:** Implemented data quality checks to ensure the integrity of the enriched dataset.  
2. **Logging:** Recorded changes during profiling and cleaning to maintain auditability.  

---

## **Key Findings**
1. Parks with all three features (**Washrooms, Facilities, Special Features**) accounted for 4.86% of total visits.  
2. Parks with **Facilities** and **Special Features** consistently attracted higher visitor counts.  
3. Neighborhoods varied significantly in visitation rates, highlighting opportunities for targeted improvements.  

---

## **Tools and Technologies**
1. **Data Storage and Retrieval:**  
   - **AWS S3 Glacier Instant Retrieval** for secure and cost-effective storage.  
2. **Data Profiling and Cleaning:**  
   - **AWS Glue DataBrew** for detecting and resolving data issues.  
3. **Analysis and Visualization:**  
   - Python Libraries: Pandas, Matplotlib, Seaborn  
4. **Environment:**  
   - Jupyter Notebook for interactive data exploration and documentation.  

---

## **Deliverables**
1. **Jupyter Notebook:**  
   - Includes data enrichment, descriptive statistics, visualizations, and detailed insights.  
2. **Presentation:**  
   - Summarizes findings with key visualizations for stakeholders.  

---
