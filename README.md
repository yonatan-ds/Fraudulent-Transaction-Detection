#  Financial Fraud & Money Laundering Detection Pipeline

###  PySpark + DuckDB Big Data Project

---

##  Overview

A scalable ETL pipeline for detecting **fraudulent and money laundering transactions** using large-scale financial data.
Combines data engineering and analytics to generate **risk-based insights**.

---

## 📊 Dataset

* **PaySim:** 6.3M transactions (fraud simulation)
* **AML Data:** 5.0M banking transactions
* **Currency Data:** 286 mappings

---

## ⚙️ Tech Stack

* Python
* PySpark
* DuckDB
* Pandas

---

## 🔄 Pipeline

* **Ingestion:** Parquet, CSV, JSON
* **Cleaning:** Standardized schema, fixed timestamps, no missing values
* **Enrichment:** Added currency codes
* **Feature Engineering:**

  * Time (hour, day)
  * Transaction size (Small / Medium / Large)
  * Bank activity metrics
* **Risk Logic:**

  * High-value + night transactions
  * Fraud signals from PaySim
  * Final flag → `aml_flag`

---

## 📈 Results

* **5,078,345 transactions processed**
* **5,177 fraud cases (~0.1%)**
* High-value & night transactions show higher risk

---

## 🗄️ Output

Final dataset stored in **DuckDB** for fast analytics.

---

## ▶️ Run

```bash
git clone https://github.com/YOUR_USERNAME/fraud-detection-pipeline.git
cd fraud-detection-pipeline
pip install pyspark pandas duckdb
jupyter notebook
```

---

## 👤 Author

Your Name

Yonatan kiross

 *A practical big data project for real-world fraud detection*
