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
Amazon S3 was used to organize data into three buckets—raw, transformed, and curated—to ensure efficient storage and access. A structured folder hierarchy was implemented within these buckets to streamline data management and facilitate seamless data processing workflows.
2. **Data Profiling**:
AWS Glue DataBrew was utilized to analyze the dataset's quality and structure, focusing on identifying duplicates, missing values, and inconsistencies. This step ensured that the dataset met the analytical requirements before further processing.
3. **Data Cleaning**:
Unnecessary columns were removed, and formats were standardized to maintain uniformity. Missing values were handled using predefined rules, such as imputation or replacement, and invalid data entries were corrected to improve the dataset's reliability.
4. **Data Pipeline Design**:
A visual ETL (Extract, Transform, Load) pipeline was developed using AWS Glue, allowing for efficient data transformation and aggregation. The pipeline grouped data by retail categories to compute counts for each segment, aiding in trend analysis and insights generation.
![visual-etl](https://github.com/user-attachments/assets/81ec5ea8-57ff-45d1-945c-25ed462a7471)
  
5. **Data Enrichment**:
Additional contextual information was integrated into the dataset by adding new columns, such as "Year Recorded." This step enhanced the dataset's analytical value by enabling temporal analysis and deeper insights.
6. **Data Protection**:
Data security was ensured by implementing encryption using AWS Key Management Service (KMS). This safeguarded sensitive data in all storage layers, protecting it against unauthorized access.
7. **Data Governance**:
Policies and processes were established to ensure data accuracy, integrity, and compliance with quality standards. Data quality checks, such as completeness and uniqueness rules, were implemented using AWS Glue to validate datasets. Failed and passed data outputs were organized into separate folders, ensuring that only high-quality data was used for further analysis and reporting.
8. **Data Observability**:
AWS CloudWatch was configured to monitor key metrics and pipeline performance in real-time. This included tracking bucket sizes, object counts, and setting up alarms for anomalies, ensuring data health and operational transparency.
## Exploratory Analysis:
Identified key trends, such as the dominance of Service Commercial spaces in the area.
## Tools and Technologies
- **AWS Services**:
The project utilized AWS S3 for organizing data into raw, transformed, and curated buckets, enabling efficient data storage and access. AWS Glue and DataBrew were key in building the ETL pipeline, automating data profiling, cleaning, and transformation. Other services like AWS Athena supported SQL-based querying, CloudWatch enabled real-time monitoring, and KMS ensured robust encryption for data security.
- **Data Formats**:
Two formats, CSV and Parquet, were used to balance accessibility and efficiency. CSV files provided user-friendly outputs for stakeholders, facilitating easy analysis in tools like Excel. Parquet, a columnar format, optimized system performance and storage for advanced data processing tasks.
- **Visualization Tools**:
AWS Glue Visual ETL was the primary visualization tool, providing a clear representation of the data pipeline. It enabled intuitive drag-and-drop configurations for data transformation and aggregation processes. This tool ensured transparency in the ETL workflow, making complex processes easier to understand and troubleshoot.
- **Programming Languages**:
SQL was employed in AWS Athena to query and analyze large datasets efficiently. The language facilitated precise data filtering, grouping, and aggregation, enabling actionable insights. Its simplicity and effectiveness made it a powerful tool for data exploration and reporting within the project.
## Deliverables
- **Cleaned and Enriched Dataset**:
The project delivered a cleaned and enriched dataset, free of inconsistencies and prepared for detailed analysis. Missing values were addressed, and additional context, such as "Year Recorded," was integrated to enhance usability. This dataset served as the foundation for accurate insights and decision-making.
- **ETL Pipeline**:
A robust ETL pipeline was developed using AWS Glue to automate data ingestion, cleaning, transformation, and aggregation. The pipeline ensured efficient processing and maintained the integrity of data across all stages. This deliverable streamlined the workflow, making it reusable for similar data processing tasks in the future.
- **Secure and Monitored Data Management Solution**:
The project implemented a secure data management system using AWS KMS for encryption and CloudWatch for monitoring. This solution ensured that sensitive data remained protected and that pipeline performance was tracked in real time. Together, these measures enhanced reliability, compliance, and operational transparency.
- **Visualizations**:
The project provided visualizations that highlighted key trends and distributions within retail categories. Charts and graphs depicted insights, such as category-wise distribution and yearly trends, making complex data more understandable. These visual outputs facilitated better decision-making for stakeholders.

![retail-count](https://github.com/user-attachments/assets/07be60b6-f07b-4e96-8b19-ff77d9deed79)
# Conclusion
This project demonstrates the practical application of AWS services to streamline data analysis workflows. By leveraging modern tools, the analysis provided a clear view of retail trends in Victoria-Fraserview, supporting data-driven decision-making for stakeholders.


