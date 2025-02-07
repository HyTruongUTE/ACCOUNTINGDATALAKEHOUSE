# ACCOUNTINGDATALAKEHOUSE
Applying Modern Data Stack to Build a Data Lakehouse for Accounting Analytics

This project builds a data lakehouse for accounting data processing and analysis, addressing the limitations of traditional data warehouses and data lakes. It ensures scalability, cost efficiency, and flexibility while maintaining data consistency and reliability.
The solution follows a three-layer Medallion architecture: raw data is imported into MySQL, transformed into Parquet, and stored in MinIO. Using Spark, data is cleaned in the silver layer and further processed into a star schema for accurate financial reporting. Dagster manages and monitors data pipelines, ensuring data integrity and automation.
With Power BI and Metabase, financial data is visualized effectively, enabling real-time insights and better decision-making. The entire system is containerized with Docker, ensuring scalability, portability, and ease of deployment.
This lakehouse approach is essential for accounting data as it handles large volumes efficiently, improves data governance, supports complex analytics, and ensures compliance with financial regulations, making financial reporting more accurate, automated, and insightful.
## System Architecture of Data Lakehouse
![image](https://github.com/user-attachments/assets/713499e4-511e-4bcc-a0cd-9d36e152f625)
## Data Quality with medallions architecture
![image](https://github.com/user-attachments/assets/d90719f3-3814-47af-8792-198dd76adbf8)
**Bronze Layer (Raw Data):** Stores data in its original format, ensuring a single source of truth and enabling easy auditing and reprocessing when needed.
**Silver Layer (Cleansed Data):** Uses Spark for data cleaning, filtering, and deduplication, improving data consistency and reliability.
**Gold Layer (Business-Ready Data):** Transforms data into a star schema tailored for accounting and financial reporting, ensuring accurate and structured insights.
![image](https://github.com/user-attachments/assets/8ae68c4d-fdaf-4856-a8e2-66b96d5dd202)
## Scalability & Performance
Optimized storage: Storing data in Parquet format in MinIO improves compression and read performance, reducing storage costs.
Efficient processing: Spark enables distributed computing, allowing large-scale data transformations with high speed and efficiency.
## Flexibility & Agility
The layered approach allows different teams to access data at different levels, enabling both data engineers and business analysts to work efficiently.
It supports incremental updates and real-time data processing without disrupting existing workflows.
![image](https://github.com/user-attachments/assets/87b3cb4a-7045-4c63-9b1e-9d4be1d9fc7a)
## Enhanced Data Pipeline Management
Dagster provides orchestration, monitoring, and observability of data workflows, ensuring error handling, lineage tracking, and automation.
## Cost Efficiency & Maintainability
Decoupling storage from compute reduces costs compared to traditional data warehouses.
Supports schema evolution and data versioning, making it easier to adapt to changing business needs.
## Business Value & Better Decision-Making
Ensures compliance with financial regulations by maintaining structured, auditable data.
Power BI & Metabase enable interactive dashboards and real-time financial insights, improving reporting efficiency and accuracy.
![image](https://github.com/user-attachments/assets/988d693f-c36c-4b7f-8334-14bbe5fcbddd)
![image](https://github.com/user-attachments/assets/c29036b2-0a8d-456e-8d1a-e56a836f186b)
![image](https://github.com/user-attachments/assets/2a1b31a5-7ecf-444b-ad93-03988ae563b4)
![image](https://github.com/user-attachments/assets/68b95f1f-fe17-4ef4-ade9-ed551dcddaad)
![image](https://github.com/user-attachments/assets/0706afeb-8715-48ea-a72c-485b048d8347)
![image](https://github.com/user-attachments/assets/df1734d9-9ebe-4871-b939-66f1aea287cb)
![image](https://github.com/user-attachments/assets/5840e94d-9e6e-4e90-9633-6109a403e2a2)
![image](https://github.com/user-attachments/assets/ebea7a3b-2afa-4ebd-8452-887bef9ff4c9
![image](https://github.com/user-attachments/assets/39be9ee6-d54d-4509-a0b6-509637e94b05)
![image](https://github.com/user-attachments/assets/cbd112b3-5b5b-4aa9-b1f8-a900cb5e7c52)
![image](https://github.com/user-attachments/assets/0aea8dea-f2f4-4396-bc2f-8ba323ad619b)
![image](https://github.com/user-attachments/assets/878978be-6256-4129-a921-a6615a0e28f5)
![image](https://github.com/user-attachments/assets/38671da5-207f-4b01-94e4-ce002564015c)
![image](https://github.com/user-attachments/assets/99d9e8c3-03e3-4578-851a-e4764034c9db)
![image](https://github.com/user-attachments/assets/9b2c7b11-a2d2-40c4-a4b3-fff23305b8d0)
![Uploading image.png…]()










