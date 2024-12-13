# Hello, I'm Priyanka Panjiyar
<a href="https://www.linkedin.com/in/priyanka-panjiyar-188943178/"><img src="https://img.shields.io/badge/-LinkedIn-0072b1?&style=for-the-badge&logo=linkedin&logoColor=white" /></a>

[Brief Introduction]
I am an MBA graduate. 

| Skill                                         | Associated Project         |
|-----------------------------------------------|----------------------------|
| SIEM Implementation and Log Analysis          | <a href="https://github.com/Test-MyDFIR/Detection-Lab/tree/main">Detection Lab</a>|
| SIEM Implementation and Log Analysis          | <a href="https://google.com">Detection Lab</a>|
| Network Traffic Monitoring and Attack Detection | <a href="https://google.com">Detection Lab</a>|
| Security Automation with Shuffle SOAR         | SOC Automation Lab|
| Incident Response Planning and Execution      | SOC Automation Lab|
| Case Management with TheHive                  | SOC Automation Lab|
| Scripting and Automation for Threat Mitigation | SOC Automation Lab|

## Projects
- <a href="https://github.com/Test-MyDFIR/Detection-Lab/tree/main">Detection Lab</a>
- Detection Lab
- SOC Automation Project
- Test Project

## Projects
# Project 1: Retail Category Analysis 
## Project Description
This project focuses on analyzing retail categories within the Victoria-Fraserview geographic area using AWS Data Analytics Platform (DAP). The aim is to create a streamlined data pipeline to ingest, clean, transform, and analyze storefront inventory data, identifying trends and deriving actionable insights about retail spaces.

<p align="center">
<img src="https://github.com/user-attachments/assets/85907c80-35aa-45e0-b8de-db8de5dd59aa" alt="Alt Text" width="750" height="500">
</p>

## Project Title
Streamlined Retail Category Analysis with AWS

## Objective
To identify and analyze the distribution of retail categories, determining which category has the highest count, while showcasing the use of AWS services to enhance data processing and analysis efficiency.

## Dataset
The dataset contains 33,983 records collected between 2020 and 2023. After filtering for the Victoria-Fraserview area, 782 records were analyzed, detailing retail spaces categorized into Service Commercial, Convenience Goods, Food & Beverage, Comparison Goods, and more.

<p align="center">
  <img src="https://github.com/user-attachments/assets/d2574895-b383-469e-866a-d254bc994c64" alt="Alt Text" width="750" height="450">
</p>

## Methodology
1. **Data Ingestion**:
Amazon S3 was used to organize data into three buckets—raw, transformed, and curated—to ensure efficient storage and access. A structured folder hierarchy was implemented within these buckets to streamline data management and facilitate seamless data processing workflows.
2. **Data Profiling**:
AWS Glue DataBrew was utilized to analyze the dataset's quality and structure, focusing on identifying duplicates, missing values, and inconsistencies. This step ensured that the dataset met the analytical requirements before further processing.
3. **Data Cleaning**:
Unnecessary columns were removed, and formats were standardized to maintain uniformity. Missing values were handled using predefined rules, such as imputation or replacement, and invalid data entries were corrected to improve the dataset's reliability.
4. **Data Pipeline Design**:
A visual ETL (Extract, Transform, Load) pipeline was developed using AWS Glue, allowing for efficient data transformation and aggregation. The pipeline grouped data by retail categories to compute counts for each segment, aiding in trend analysis and insights generation.  
6. **Data Enrichment**:
Additional I utilized AWS Glue Data Catalog to organize and manage metadata, making the dataset more accessible and easier to analyze. Subsequently, I used SQL queries in AWS Athena to perform advanced data aggregation and extract actionable insights from the enriched dataset efficiently.
7. **Data Protection**:
Data security was ensured by implementing encryption using AWS Key Management Service (KMS). This safeguarded sensitive data in all storage layers, protecting it against unauthorized access.
8. **Data Governance**:
Policies and processes were established to ensure data accuracy, integrity, and compliance with quality standards. Data quality checks, such as completeness and uniqueness rules, were implemented using AWS Glue to validate datasets. Failed and passed data outputs were organized into separate folders, ensuring that only high-quality data was used for further analysis and reporting.
9. **Data Observability**:
AWS CloudWatch was configured to monitor key metrics and pipeline performance in real-time. This included tracking bucket sizes, object counts, and setting up alarms for anomalies, ensuring data health and operational transparency.

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

<p align="center">
  <img src="https://github.com/user-attachments/assets/1342231d-29cc-48f6-96dc-0169d83d415b" alt="Alt Text" width="750" height="500">
</p>

# Conclusion
This project demonstrates the practical application of AWS services to streamline data analysis workflows. By leveraging modern tools, the analysis provided a clear view of retail trends in Victoria-Fraserview, supporting data-driven decision-making for stakeholders. The robust data pipeline ensured efficiency, accuracy, and scalability, making it adaptable for similar projects in the future. Furthermore, the integration of data security and monitoring measures enhanced the reliability of the results, ensuring compliance with best practices. These insights empower stakeholders to optimize retail operations and plan strategic initiatives effectively.

# Project 2: Student Registration Office: Admission Process Analysis
## Project Description 
In this project, a dataset from the Student Registration Office is used to analyze and streamline the student admissions process. The data had to be cleaned, transformed, and analyzed in order to provide information on admission rates, applicant patterns, and typical problems with the registration process. Through the use of contemporary tools and a structured data pipeline, this initiative improved the admissions process's dependability and efficiency.

## Project Title 
Optimizing the Student Admission Process with Data Analysis

## Objective 
The primary objective was to ensure data integrity, analyze key metrics related to student applications. This involved identifying inconsistencies, trends, and areas of improvement in the workflow.

## Methodology 
1) **Data Ingestion**:
- The dataset was organized into raw, transformed, and curated formats for efficient storage and access.
- A structured folder hierarchy was created to streamline data management and processing workflows.
2) **Data Profiling**:
- The dataset was analyzed using tools like AWS Glue DataBrew to assess quality and structure.
- Issues such as duplicates, missing values, and inconsistencies were identified and documented for resolution.
3) **Data Cleaning**:
- Unnecessary columns were removed, and all data formats were standardized to maintain consistency.
- Missing and invalid data entries were addressed using imputation techniques and predefined rules.
4) **Data Enrichment**:
- Additional fields, such as demographic details and application submission dates, were added to enhance the dataset.
- The enriched dataset provided a comprehensive view, enabling deeper analysis and actionable insights.
5) **Data Pipeline Design**:
- An ETL pipeline was developed using AWS Glue, automating data transformation and aggregation processes.
- Applicants were grouped by key attributes like program preferences and admission status to identify trends and patterns.
6) **Data Protection**:
- Encryption methods were applied using AWS Key Management Service (KMS) to safeguard sensitive applicant information.
- Security policies ensured compliance with data protection regulations, protecting privacy and confidentiality.
7) **Data Governance**:
- Policies and rules were established to ensure data accuracy, completeness, and integrity.
Quality checks, including completeness and uniqueness rules, were implemented to validate data.
- Data that failed governance checks was isolated in designated folders, ensuring only high-quality data was used for reporting and analysis.
8) **Data Observability**:
- AWS CloudWatch was configured to monitor pipeline performance and data health in real-time.
- Alerts and notifications were set up to detect anomalies, such as spikes in missing values or irregular patterns.

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
## Conclusion 
This project successfully demonstrated the application of advanced data analysis techniques to optimize the student admission process. By implementing a structured data pipeline and ensuring data quality through governance and protection measures, the analysis provided actionable insights into applicant trends and process bottlenecks. The deliverables, including a cleaned dataset, visualizations, and a secure data management solution, empower stakeholders to make informed decisions. This structured approach to data analysis not only enhances operational efficiency but also supports a seamless and fair admission experience for applicants.


