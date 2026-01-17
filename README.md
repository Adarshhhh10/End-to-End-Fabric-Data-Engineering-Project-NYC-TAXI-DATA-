# 🚖 End-to-End Data Engineering Project – NYC Taxi Data (Microsoft Fabric)

## 📌 Project Overview
- Designed and implemented an **end-to-end data engineering pipeline** using **Microsoft Fabric**
- Processed **NYC Yellow Taxi public data** following the **Medallion Architecture (Bronze–Silver–Gold)**
- Built scalable data ingestion, transformation, warehousing, and reporting layers
- Delivered business-ready insights using **Semantic Models and Power BI**

---

## 🏗️ Architecture Summary
- **Source**: NYC Yellow Taxi public dataset (Parquet)
- **Ingestion & Transformation**: Dataflow Gen2
- **Storage**: Fabric Lakehouse (OneLake)
- **Analytics**: Fabric Warehouse
- **Semantic Layer**: Fabric Semantic Model
- **Visualization**: Power BI

---

## 🧱 Medallion Architecture Implementation

### 🟤 Bronze Layer – Raw Data
- Stored raw NYC Taxi parquet files in **Fabric Lakehouse (Files)**
- Preserved source schema and historical data
- Enabled scalable cloud storage using OneLake

### ⚪ Silver Layer – Processed Data
- Used **Dataflow Gen2** for:
  - Data cleansing and validation
  - Column standardization
  - Date and numeric transformations
- Wrote cleaned data back to Lakehouse tables

### 🟡 Gold Layer – Analytics Ready
- Loaded curated datasets into **Fabric Warehouse**
- Designed tables optimized for reporting and analytics
- Supported fast query performance for BI use cases

---

## 🔄 Data Orchestration (Pipelines)
- Built **Fabric Pipelines** to automate:
  - Staging data processing
  - Lookup table handling
  - End-to-end workflow execution
- Ensured dependency-driven and repeatable pipeline runs

---

## 📊 Semantic Model
- Created a **Fabric Semantic Model** on top of the warehouse
- Defined:
  - Table relationships
  - Business measures
  - Aggregations for reporting
- Enabled reusable metrics across reports

---

## 📈 Power BI Reporting
- Developed an interactive **Power BI dashboard**
- Visualized:
  - Trip volume trends
  - Revenue analysis
  - Pickup and drop-off zone insights
  - Time-based demand patterns
- Connected directly to Fabric Semantic Model

---

## 📂 Repository Structure






nyc-taxi-fabric-data-engineering/
│
├── README.md
│
├── workspace/
│ └── workspace_schema.png
│
├── dataflows/
│ └── df_pres_processing_nyctaxi.m.txt
│
├── warehouse/
│ └── nyc_taxi_data_warehouse.zip
│
├── pipelines/
│ ├── pl_pres_processing_nyctaxi.png
│ ├── pl_stg_processing_nyctaxi.png
│ ├── pl_orchestrate_nyctaxi.png
│ └── pl_stg_lookup.png
│
├── semantic_model/
│ └── semantic_model_schema.png
│
└── reports/
└── NYC_Taxi_Data_Presentation.pbix

