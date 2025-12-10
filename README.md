# Airline Data Engineering Pipeline on Azure Databricks

## 📌 Overview
This project is an end-to-end data engineering pipeline built on Azure Databricks.  
It processes multiple airline datasets including:

- Bookings  
- Flights  
- Airports  
- Passengers  

The pipeline demonstrates scalable ingestion, transformation, Delta Lake optimization, and workflow automation commonly used in modern data engineering systems.

---

## 🚀 Features
- **Raw to curated multi-layer architecture (Bronze → Silver → Gold)**
- **Auto-ingestion of multiple datasets with schema enforcement**
- **Complex PySpark transformations**
  - Window functions  
  - Advanced joins  
  - Aggregations  
  - Filtering + cleaning logic  
- **Delta Lake features**
  - Time travel  
  - Optimize + Z-order  
  - Partitioning  
  - Merge operations  
- **Workflow automation using Databricks Jobs**
- **Parameter-driven notebook execution**
- **Validated data outputs for reporting/analytics**

---

## 🏗️ Architecture

### **Bronze Layer (Raw Ingestion)**
- Loads raw CSV/Parquet datasets  
- Applies schema validation  
- Stores raw data in Delta format  

### **Silver Layer (Cleaned)**
- Removes duplicates  
- Cleans and standardizes columns  
- Adds derived fields (dates, durations, categories)  

### **Gold Layer (Curated)**
- Creates aggregated datasets  
- Passenger-level metrics  
- Flight performance insights  
- Airport-level analytics  

---

## ⚙️ Tech Stack
- **Azure Databricks**
- **PySpark**
- **Delta Lake**
- **Azure Data Lake Storage**
- **Databricks Jobs**
- **Notebook Workflows**

---

## 📂 Datasets Used
- Airlines dataset (flights)
- Bookings dataset
- Airports dataset
- Passenger dataset

*(Add file names if you want.)*

---

## 🧩 Pipeline Workflow

1. **Ingest raw datasets into Bronze tables**
2. **Transform and clean data into the Silver layer**
3. **Build business-ready Gold tables**
4. **Optimize Delta tables for query performance**
5. **Automate end-to-end execution using Databricks Jobs**

---

## 🔧 How to Run the Project

1. Import the notebook folder into Databricks  
2. Upload the dataset files to DBFS / ADLS  
3. Update file paths in the configuration cell  
4. Run the notebook series in this order:
    - `01_bronze_ingestion`
    - `02_silver_transformation`
    - `03_gold_aggregation`
5. (Optional) Create a Databricks Job to automate execution  
6. Validate output tables in the Gold layer  

---

## 📊 Sample Outputs
- Flight route performance  
- Delay patterns  
- Passenger booking statistics  
- Airport-level traffic analysis  

*(Add screenshots when you upload the notebook.)*

---

## 📈 Future Enhancements
- Add Airflow orchestration  
- Add unit tests with pytest  
- Add automated data quality checks using expectations  
- Add CI/CD integration with Databricks Repos  

---

## 📬 Contact
For any questions or discussion, feel free to reach out via LinkedIn or email.
