# ACCOUNTINGDATALAKEHOUSE
Applying Modern Data Stack to Build a Data Lakehouse for Accounting Analytics

This project builds a data lakehouse for accounting data processing and analysis, addressing the limitations of traditional data warehouses and data lakes. It ensures scalability, cost efficiency, and flexibility while maintaining data consistency and reliability.
The solution follows a three-layer Medallion architecture: raw data is imported into MySQL, transformed into Parquet, and stored in MinIO. Using Spark, data is cleaned in the silver layer and further processed into a star schema for accurate financial reporting. Dagster manages and monitors data pipelines, ensuring data integrity and automation.
With Power BI and Metabase, financial data is visualized effectively, enabling real-time insights and better decision-making. The entire system is containerized with Docker, ensuring scalability, portability, and ease of deployment.
This lakehouse approach is essential for accounting data as it handles large volumes efficiently, improves data governance, supports complex analytics, and ensures compliance with financial regulations, making financial reporting more accurate, automated, and insightful.
<p align="center">
  <img src="https://github.com/user-attachments/assets/d5d69419-0196-49aa-9776-6a4d30c966fe" alt="image" />
</p>
## System Architecture of Data Lakehouse
![image](https://github.com/user-attachments/assets/713499e4-511e-4bcc-a0cd-9d36e152f625)
## Data Quality with medallions architecture
<p align="center">
  ![image](https://github.com/user-attachments/assets/d90719f3-3814-47af-8792-198dd76adbf8)
</p>
![image](https://github.com/user-attachments/assets/d90719f3-3814-47af-8792-198dd76adbf8)

**Bronze Layer (Raw Data):** Stores data in its original format, ensuring a single source of truth and enabling easy auditing and reprocessing when needed.
**Silver Layer (Cleansed Data):** Uses Spark for data cleaning, filtering, and deduplication, improving data consistency and reliability.
**Gold Layer (Business-Ready Data):** Transforms data into a star schema tailored for accounting and financial reporting, ensuring accurate and structured insights.
![image](https://github.com/user-attachments/assets/8ae68c4d-fdaf-4856-a8e2-66b96d5dd202)
## Scalability & Performance
![image](https://github.com/user-attachments/assets/794ae9e4-489a-4204-a570-142c14c61679)
Optimized storage: Storing data in Parquet format in MinIO improves compression and read performance, reducing storage costs.
![image](https://github.com/user-attachments/assets/e115c909-be99-4190-b4c4-f07b2dbf2e7e)
![image](https://github.com/user-attachments/assets/dd88ffde-e319-44be-8a7b-801b0300e9c7)
Efficient processing: Spark enables distributed computing, allowing large-scale data transformations with high speed and efficiency.
![image](https://github.com/user-attachments/assets/f9100d5c-2e81-481f-8943-1600c3fcfed7)
![image](https://github.com/user-attachments/assets/1997cd11-2ecb-437b-8b6e-3426259d0a38)
## Flexibility & Agility
The layered approach allows different teams to access data at different levels, enabling both data engineers and business analysts to work efficiently.
It supports incremental updates and real-time data processing without disrupting existing workflows.
![image](https://github.com/user-attachments/assets/87b3cb4a-7045-4c63-9b1e-9d4be1d9fc7a)
## Enhanced Data Pipeline Management
Dagster provides orchestration, monitoring, and observability of data workflows, ensuring error handling, lineage tracking, and automation.
![image](https://github.com/user-attachments/assets/431b8301-0401-4e32-a48f-d95baaa2fd37)
![image](https://github.com/user-attachments/assets/2c482da4-1d27-42a2-af53-18cc7343fa5e)
![image](https://github.com/user-attachments/assets/20d8af89-c9db-40a4-a097-e0f1fa8f5fd0)
![image](https://github.com/user-attachments/assets/7ec6e503-2cec-4da7-b563-4a91c619915c)
![image](https://github.com/user-attachments/assets/38b0c415-6a30-4740-bbb3-3df3ab5471f8)

## Cost Efficiency & Maintainability
Decoupling storage from compute reduces costs compared to traditional data warehouses.
Supports schema evolution and data versioning, making it easier to adapt to changing business needs.
## Business Value & Better Decision-Making
Ensures compliance with financial regulations by maintaining structured, auditable data.
Power BI & Metabase enable interactive dashboards and real-time financial insights, improving reporting efficiency and accuracy.
# REPORT BUILDING BY POWER BI
## Homepage
The Homepage provides 5 reports on the Dashboard.
![image](https://github.com/user-attachments/assets/988d693f-c36c-4b7f-8334-14bbe5fcbddd)
## Balance Sheet
The Dashboard provides information on the opening and closing balances of Current Assets (CA), Non-Current Assets (NCA), and Liabilities. It compares the proportions between these components and shows the cumulative total assets over the months.
![image](https://github.com/user-attachments/assets/c29036b2-0a8d-456e-8d1a-e56a836f186b)
View the total value of assets, liabilities, and a detailed balance sheet. Track the increases, decreases, and variations of financial indicators over the year, along with their percentage changes.
![image](https://github.com/user-attachments/assets/2a1b31a5-7ecf-444b-ad93-03988ae563b4)
Shows the proportion of Current Assets (CA) and Non-Current Assets (NCA). Compares the proportions of CA and NCA as well as the capital structure ratio.
![image](https://github.com/user-attachments/assets/68b95f1f-fe17-4ef4-ade9-ed551dcddaad)
## Profit and Loss Statement
View the detailed profit and loss statement, with a breakdown of results from highest to lowest. It gives insights into business performance, including sales revenue, cost of goods sold, profit, and net profit after tax.
![image](https://github.com/user-attachments/assets/0706afeb-8715-48ea-a72c-485b048d8347)
Displays the percentage of different cost types within total costs and compares revenue from sales against revenue from financial activities.
![image](https://github.com/user-attachments/assets/df1734d9-9ebe-4871-b939-66f1aea287cb)
Shows the month-by-month cumulative figures for sales, costs, and net profit, allowing for better tracking of business performance over time.
![image](https://github.com/user-attachments/assets/5840e94d-9e6e-4e90-9633-6109a403e2a2)
## Accounts Payable Report
View the total accounts payable, top customers with the highest debts for the period, those who have repaid the most, outstanding debts at the end of the period, and customers who have made advance payments.
![image](https://github.com/user-attachments/assets/ebea7a3b-2afa-4ebd-8452-887bef9ff4c9)
Compare the ratio of accounts receivable to accounts payable, debt ratios, and accounts payable figures over several months.
![image](https://github.com/user-attachments/assets/39be9ee6-d54d-4509-a0b6-509637e94b05)
View the top inventory items with the highest intake by value and quantity.
![image](https://github.com/user-attachments/assets/cbd112b3-5b5b-4aa9-b1f8-a900cb5e7c52)
View the top inventory items with the highest outflow by value and quantity.
![image](https://github.com/user-attachments/assets/0aea8dea-f2f4-4396-bc2f-8ba323ad619b)
View the top inventory items with the highest remaining stock by value and quantity.
![image](https://github.com/user-attachments/assets/878978be-6256-4129-a921-a6615a0e28f5)
Shows the inventory turnover rate, cumulative inventory, and cost of goods sold for each month.
![image](https://github.com/user-attachments/assets/38671da5-207f-4b01-94e4-ce002564015c)
View key accounting ratios used to assess the financial health of the company and to devise effective strategies. These ratios are divided into four main groups: profitability, liquidity, asset efficiency, financial risk, and business growth.
![image](https://github.com/user-attachments/assets/99d9e8c3-03e3-4578-851a-e4764034c9db)
Displays ROA (Return on Assets), ROE (Return on Equity), and GPM (Gross Profit Margin) for each month.
![image](https://github.com/user-attachments/assets/9b2c7b11-a2d2-40c4-a4b3-fff23305b8d0)
# REPORT BUILDING BY METABASE
![image](https://github.com/user-attachments/assets/057d325c-c4a0-46de-a921-39d0dd8f34dc)
![image](https://github.com/user-attachments/assets/7e14e35a-90ba-4da2-ae44-f377c2de447e)
# Conclusion
1. Achievements
I have successfully developed a Data Lakehouse (DLH) system based on the Modern Data Stack (MDS) model to support financial reporting and analysis in accounting. This project integrates the strengths of both Data Lake and Data Warehouse, overcoming the limitations of traditional models. The system is flexible, scalable, and provides superior functionality compared to conventional solutions. By utilizing technologies like MySQL, Minio, Hive, Docker, Dagster, Spark, and PowerBI, I built a platform that efficiently handles, processes, and visualizes accounting data, enabling better financial decision-making. The Modern Data Stack approach has proven to be more cost-effective and enhances both productivity and work efficiency. This project not only expanded my understanding of data processing but also deepened my knowledge of accounting processes, allowing me to leverage data-driven decision-making.
2. Limitations
The project currently uses academic-level tools, and advanced solutions that require licensing costs have not been integrated, limiting comprehensive comparisons with industry alternatives. Although based on MDS, the system has yet to fully capitalize on the potential of these technologies, with some features still in development. The system also does not yet support the processing of semi-structured and unstructured data. Moreover, the accounting processes have not been fully addressed, and further development is needed to enhance the solution. The absence of machine learning and AI integration limits the system’s automation and optimization capabilities.
3. Future Development
Develop tools for in-depth accounting data analysis.
Assess the solution’s effectiveness and refine the reporting features.
Make the application more user-friendly for non-technical users.
Implement exchange rate prediction models to forecast market trends.











