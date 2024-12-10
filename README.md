# Exploratory Data Analysis (EDA) on Vancouver's Green Spaces

## Project Description  
This project conducts an exploratory data analysis (EDA) on Vancouver's park datasets, enriched with visitor count data, to uncover trends in park sizes, distribution, features, and visitor engagement. The goal is to generate insights that will inform urban planning, park resource allocation, and overall management.

## Project Objectives  
- Analyze the distribution and features of Vancouver’s parks.
- Enrich the dataset with visitor count data to explore engagement trends.
- Provide actionable insights to support urban planning and efficient resource allocation for park management.

## Dataset Overview  
The dataset includes detailed park information, such as:  
- **ParkID**: Unique identifier for each park.
- **Name**: Name of the park.
- **Neighbourhood**: Geographic location of the park.
- **Hectare**: Size of the park in hectares.
- **Facilities**: Available amenities (e.g., playgrounds, picnic areas, sports courts).
- **Washrooms**: Availability of washroom facilities.
- **SpecialFeatures**: Unique features like monuments or other attractions.
- **Number_of_Visits**: Enriched visitor count data.
- **GoogleMapDest**: Location coordinates for mapping.

---

## Methodology

### 1. Data Collection and Preparation  
- Load and clean the dataset, ensuring consistency and handling missing values.  
- **Data Enrichment**: Add visitor count data to enable analysis of engagement patterns.
- **Data Storage**: Store data securely in AWS S3 Glacier Instant Retrieval for cost-effective and reliable access.

### 2. Descriptive Statistics  
- Compute summary statistics to better understand park sizes, facilities, and visitor counts.  
  ![Descriptive Statistics](Stats.png)

### 3. Data Profiling and Cleaning  
- Use **AWS Glue DataBrew** for data profiling, identifying missing values and inconsistencies.  
- **Cleaning Steps**:  
  - Renaming columns for clarity (e.g., "NeighbourhoodName" to "Neighbourhood").  
  - Replace missing values with "null" where necessary.  
  - Remove extra spaces in categorical fields.

### 4. Data Visualization  
- **Park Size Distribution**: Use histograms to show park size distributions in hectares.  
  ![Park Size Distribution](park_size_hist.png)
  
- **Top 10 Neighborhoods by Number of Parks**: Display bar charts of neighborhoods with the most parks.  
  ![Top 10 Neighborhoods by Number of Parks](Top_10_neigh_bar.png)
  
- **Facilities Availability**: Create pie charts for the proportion of parks with different features.  
  ![Facilities Availability](Faci_dist_pie.png)

- **Visitor Engagement by Amenities**: Bar charts comparing visitor counts for parks with and without key amenities.

### 5. Geospatial Visualization  
- Use geospatial data to map the distribution of parks across Vancouver.  
  ![Geospatial Visualization](Dist_map.png)

### 6. Analysis of Parks with All Three Features  
- Focus on parks offering washrooms, facilities, and special features.  
- **Key Insight**: Parks with all three amenities attract fewer but more engaged visitors (5,981 visits out of 122,936 total).  
  ![Parks with All Three Features](all_3.png)

---

## Insights and Trends  

- **Neighborhoods**: Variation in visitation rates suggests areas with fewer parks could benefit from improved resources or amenities.
- **Facilities**: Parks with amenities like washrooms and playgrounds experience higher visitor counts.
- **Park Sizes**: A small number of large parks contribute significantly to visitor engagement, while most parks are smaller.

---

## Tools and Technologies  

- **Data Storage**: AWS S3 Glacier Instant Retrieval for cost-efficient storage.  
- **Data Profiling and Cleaning**: AWS Glue DataBrew for data quality checks.  
- **Analysis and Visualization**: Python libraries (Pandas, Matplotlib, Seaborn, GeoPandas, Shapely) for data analysis and visualization.  
- **Environment**: Jupyter Notebook for interactive data analysis and documentation.

---

## Deliverables  
- **Jupyter Notebook**: Contains data enrichment steps, descriptive statistics, visualizations, and detailed insights.  
- **Presentation**: Summarizes findings with key visualizations for stakeholders, offering actionable recommendations.
