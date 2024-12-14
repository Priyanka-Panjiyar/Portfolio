# Project1: Retail Category Analysis Using AWS Data Analytics Platform

## Data Wrangling

### Project Description
This phase focused on cleaning and transforming the storefront inventory dataset from the Victoria-Fraserview area. The aim was to prepare the data for analysis by organizing it into raw, transformed, and curated buckets, ensuring accuracy, consistency, and completeness.

### Project Title
**Data Wrangling for Retail Storefront Inventory**

### Objective
To preprocess and structure the dataset for analysis, making it ready for insights generation by eliminating errors, duplicates, and inconsistencies.

### Dataset
The dataset contains **33,983 records**, with **782 records** filtered for the Victoria-Fraserview Geo Local Area. Each record details attributes such as business name, retail category, and status (active or vacant). The dataset spans records from 2020 to 2023 and provides critical insights into the distribution and trends of retail spaces.

### Methodology

#### **1. Data Ingestion**
- **Storage Setup**:
  - Created three Amazon S3 buckets: `si-raw-pri` (raw data), `si-trf-pri` (transformed data), and `si-cur-pri` (curated data).
  - Organized folders in these buckets for seamless access and management.
- **Dataset Upload**:
  - Uploaded the raw dataset in the `si-raw-pri/storefronts_inventory` folder with the "Standard" storage class for frequent access.

#### **2. Data Profiling**
- **Dataset Connection**:
  - Connected the raw dataset to AWS Glue DataBrew for profiling.
- **Profile Job Execution**:
  - Analyzed the dataset to identify missing values, duplicates, and data inconsistencies.
  - Stored profiling results in `si-trf-pri/data-profiling`.

#### **3. Data Cleaning**
- **Cleaning Recipe**:
  - Removed unnecessary columns like `geo_point_2d` and `Geom`.
  - Replaced invalid values (e.g., "Vacant") with null values.
  - Filled missing values with "N/A" in the `Units` column.
- **Outputs**:
  - Stored cleaned data in `si-trf-pri/data-cleaning`:
    - **CSV files** in the `User` folder for manual analysis.
    - **Parquet files** in the `System` folder for automation.

### Tools and Technologies
- **AWS Services**: S3, Glue DataBrew
- **Data Formats**: CSV, Parquet

### Deliverables
- Cleaned dataset stored in structured S3 buckets.
- Profiling results for data insights and improved quality.

---

## Descriptive Analysis

### Project Description
This phase aimed to analyze the filtered dataset to identify key trends in retail categories for the Victoria-Fraserview area. Metrics like the distribution of retail categories and active vs. vacant properties were evaluated.

### Project Title
**Descriptive Analysis of Retail Spaces**

### Objective
To summarize key metrics, including the count of retail categories and distribution of active vs. vacant properties, providing actionable insights for stakeholders.

### Methodology

#### **1. Data Pipeline Design**
- **Input Data**:
  - Selected cleaned data from the `System` folder in the transformed bucket (`si-trf-pri`).
- **Transformation**:
  - Removed unnecessary columns like `Unit`, `civic_number_parcel`, and `street_name_parcel`.
  - Grouped data by `retail_category` and aggregated `id` to compute the count of each category.
- **Outputs**:
  - Stored outputs in:
    - **User folder** (CSV format) for stakeholders.
    - **System folder** (Parquet format) for automation.

- **Results**
- Here is the result to represent the count of retail categories:
  - **Service Commercial**: 80
  - **Food & Beverage**: 37
  - **Convenience Goods**: 41
  - Others categorized accordingly.

### Tools and Technologies
- **AWS Services**: Glue Visual ETL, Athena

### Deliverables
- ETL pipeline output stored in structured S3 folders.
- Dashboards showcasing retail category counts and distributions.

---

## Exploratory Analysis

### Project Description
This phase explored trends in retail category counts over the years (2020–2023) in the Victoria-Fraserview area. A new column (`Year Recorded`) was added to analyze temporal trends in retail categories.

### Project Title
**Exploratory Analysis of Retail Category Trends**

### Objective
To analyze the distribution of retail categories over time, identifying yearly trends in active businesses.

### Methodology

#### **1. Data Enrichment**
- Added a new column (`Year Recorded`) to the dataset to track trends over time.
- Ensured uniform formatting for all entries in the `retail_category` column.

#### **2. Data Pipeline Design**
- **Input Data**:
  - Used cleaned data from the `System` folder in the transformed bucket (`si-trf-pri`).
- **Transformation**:
  - Grouped data by `Year Recorded` to calculate yearly totals for each retail category.
- **Outputs**:
  - Stored CSV output in `retail-category-by-year/User`.
  - Stored Parquet output in `retail-category-by-year/System`.

#### **3. Visualization**
- Data flow diagram with Visual ETL.

### Tools and Technologies
- **AWS Services**: Glue Visual ETL, Athena


### Deliverables
- Yearly insights into retail category counts.
- Dashboards visualizing trends over time.

---

## Conclusion
This project demonstrated the use of AWS services to analyze retail category data efficiently. Through data wrangling, descriptive analysis, and exploratory analysis, insights were derived to support stakeholders in decision-making. The structured approach, combined with secure data management and governance, ensures scalability and reliability for similar projects.

![Flowchart drawio](https://github.com/user-attachments/assets/1d95e9a8-75cc-4c88-af06-7ed7de8e06b3)

# Project2: Student Rights and Responsibilities Procedure Analysis

## Data Wrangling

### Project Description
This phase involved organizing and structuring the dataset extracted from the "Student Rights and Responsibilities Procedure" document. The goal was to prepare the data for analysis by cleaning and formatting it into structured datasets.

### Project Title
**Data Wrangling for Policy Analysis**

### Objective
To extract, clean, and structure policy data into a high-quality format suitable for analysis, ensuring completeness and consistency.

### Dataset
The dataset included sections from the policy document, organized with attributes such as:
- **Section Title**: Main section headings, e.g., "Rights of Students."
- **Subsection**: Subheadings, e.g., "Right to Free Expression."
- **Content**: Detailed descriptions of each policy.
- **Page Number**: Reference to the original document's page.

### Methodology

#### **1. Data Ingestion**
- created three Amazon S3 bucket - raw, transform, and curated.
- Uploaded the dataset in the raw bucket with "Standard" storage class

#### **2. Data Profiling**
- Reviewed the dataset for missing values, duplicates, and inconsistencies.
- Ensured all critical fields were present and populated.

#### **3. Data Cleaning**
- Removed duplicate entries and redundant sections.
- Standardized formatting for section titles and content.
- Addressed missing values by merging related sections or adding placeholders.

#### **Deliverables**
- Cleaned dataset stored in structured S3 buckets.
- profiling results for data insights and improved quality.

## Descriptive Analysis

### Project Description
This phase analyzed the structured dataset to summarize key metrics, such as the frequency of sections and subsections, and identify the document's focus areas.

### Project Title
**Descriptive Analysis of Policy Structure**

### Objective
To summarize the distribution of content across sections and subsections, providing an overview of the policy's structure.

### Methodology

#### **1. Data Aggregation**
- Removed unnecessary columns 
- Grouped data by `Section` and `Subsection` to count the occurrences of each.
- Calculated the percentage distribution of content across sections.

#### **2. Visualization**
- Created dashboard to represent 

#### **Outputs**
- Stores

---

## Exploratory Analysis

### Project Description
This phase explored relationships and trends in the dataset, such as analyzing the content density of sections and correlating page numbers with section lengths.

### Project Title
**Exploratory Analysis of Policy Content**

### Objective
To uncover patterns and trends within the dataset, such as identifying detailed sections and analyzing the correlation between page numbers and content density.

### Methodology

#### **1. Data Enrichment**
- Added a `Content Length` column to measure the number of words or characters in each section.
- Derived a `Content Density` metric by correlating section lengths with page numbers.

#### **2. Data Analysis**
- Analyzed content length to identify the most detailed policy sections.
- Examined correlations between page numbers and content density to understand the distribution of information across the document.

#### **3. Visualization**
- Created histograms in Excel to illustrate the distribution of content lengths.
- Generated scatter plots to analyze the correlation between page numbers and section lengths.

#### **Outputs**
- Visualizations highlighting the most detailed sections and their density trends across the document.

---

## Tools and Technologies

- **Data Cleaning and Structuring**: Excel
- **File Formats**: Excel, CSV, Parquet
- **Visualization**: Excel (charts and graphs)

---

## Deliverables

- A structured dataset saved in:
  - **Excel** format for detailed editing and manual use.
  - **CSV** format for sharing and lightweight analysis.
  - **Parquet** format for optimized storage and integration into analytics tools.
- Visual reports and dashboards summarizing the document's structure, focus areas, and patterns.

---

## Conclusion
This project demonstrates a structured approach to extracting and analyzing policy data. Through data wrangling, the dataset was cleaned and prepared for analysis, ensuring accuracy and completeness. Descriptive analysis provided a clear summary of the policy structure, while exploratory analysis uncovered detailed insights into content density and focus areas. The structured outputs in Excel, CSV, and Parquet formats provide a versatile foundation for further use and sharing.

---








