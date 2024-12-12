# Projects
Here are the projects I have done during my Clould Computing class in University. 
# Project 1: Retail Category Analysis 
## Project Description
This project focuses on analyzing retail categories within the Victoria-Fraserview geographic area using AWS Data Analytics Platform (DAP). The aim is to create a streamlined data pipeline to ingest, clean, transform, and analyze storefront inventory data, identifying trends and deriving actionable insights about retail spaces.

![dap](https://github.com/user-attachments/assets/85907c80-35aa-45e0-b8de-db8de5dd59aa)

## Project Title
Streamlined Retail Category Analysis with AWS

## Objective
To identify and analyze the distribution of retail categories, determining which category has the highest count, while showcasing the use of AWS services to enhance data processing and analysis efficiency.

## Dataset
The dataset contains 33,983 records collected between 2020 and 2023. After filtering for the Victoria-Fraserview area, 782 records were analyzed, detailing retail spaces categorized into Service Commercial, Convenience Goods, Food & Beverage, Comparison Goods, and more.

![dataset](https://github.com/user-attachments/assets/d2574895-b383-469e-866a-d254bc994c64)

## Methodology
1. **Data Ingestion**:
- Used Amazon S3 to organize raw, transformed, and curated data into dedicated buckets.
- Implemented a structured folder hierarchy for better data management.
2. **Data Profiling**:
- Analyzed data quality and structure using AWS Glue DataBrew.
- Verified dataset integrity with checks for duplicates and missing values.
3. **Data Cleaning**:
- Removed unnecessary columns and standardized formats.
- Handled missing and invalid values using predefined rules.
4. **Data Pipeline Design**:
- Developed a visual ETL pipeline using AWS Glue to process and aggregate data.
- Grouped data by retail categories to compute counts for each segment.
![visual-etl](https://github.com/user-attachments/assets/81ec5ea8-57ff-45d1-945c-25ed462a7471)
  
5. **Data Enrichment**:
- Enhanced datasets by integrating additional columns, such as "Year Recorded."
6. **Data Protection**:
- Secured data using AWS Key Management Service (KMS) encryption.
7. **Data Observability**:
- Implemented AWS CloudWatch for real-time monitoring of data and pipeline metrics.
# Exploratory Analysis:
Identified key trends, such as the dominance of Service Commercial spaces in the area.
## Tools and Technologies
- AWS Services: S3, Glue, DataBrew, Athena, CloudWatch, KMS
- Data Formats: CSV, Parquet
- Visualization Tools: AWS Glue Visual ETL
- Programming Languages: SQL for querying data in Athena
## Deliverables
- A cleaned and enriched dataset ready for analysis.
- An ETL pipeline for aggregating and processing retail data.
- Visualizations representing retail distribution and trends.
- A secure, monitored data management solution.
# Conclusion
This project demonstrates the practical application of AWS services to streamline data analysis workflows. By leveraging modern tools, the analysis provided a clear view of retail trends in Victoria-Fraserview, supporting data-driven decision-making for stakeholders.

