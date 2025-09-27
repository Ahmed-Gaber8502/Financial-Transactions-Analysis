🏦 Integrated Financial Data Analysis & Outlier Management
This project focuses on the complex challenge of integrating and cleaning raw, disparate transactional data to create a unified, statistically sound dataset ready for advanced business intelligence. It showcases an end-to-end pipeline from SQL Server ingestion to Power BI visualization.

🔑 Key Technical Features
Data Governance (SQL): Enforcing PRIMARY KEY and FOREIGN KEY constraints across three tables (Transactions, Cards, Users) to ensure data integrity.

Robust Data Ingestion: Successfully implemented BULK INSERT while troubleshooting critical filesystem permissions and data type errors.

Advanced Data Cleaning: Sequential cleaning of the Amount column (removing $ signs, converting to FLOAT, handling negative values via .abs()).

Outlier Filtering: Applied the Three-Sigma Rule (Mean + 3*Std) to identify and remove statistical outliers, guaranteeing reliable analytical results.

Multi-Source Integration: Executed a Three-Way INNER JOIN logic, implemented both in SQL and using pandas.merge() in Python, to link all customer, card, and transaction records.

📊 Power BI Dashboard
The interactive dashboard includes:

Customer Segmentation: Analysis of spending trends by Age and Gender.

Fraud & Risk Indicators: Visualization of transactions that were close to the calculated outlier limit.

Card Performance: Breakdown of spending volume by Card Type and Card Status.

Merchant Activity: Mapping transaction value (Amount) across Merchant City and State.

🔗 Financial Transactions Dashboard (Placeholder link for your deployed dashboard)

📈 Tools & Technologies
SQL Server – Data storage, BULK INSERT, and INNER JOIN queries.

Python (Jupyter Notebook) – Pandas (Cleaning, Merging, Outlier Filtering), NumPy, Matplotlib, Seaborn.

Power BI – Interactive reporting and dashboards.

📥 Dataset
The project utilizes integrated data from three distinct sources, combined for comprehensive analysis:

Transactions Data: Core financial records and merchant details.

Cards Data: Card type and status information.

Users Data: Customer demographics (Age, Gender, City).
