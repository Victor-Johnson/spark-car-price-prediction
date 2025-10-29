# 🚗 Distributed Car Price Prediction Pipeline using Apache Spark ML

## 📘 Overview
This project predicts used car prices by combining multiple brand datasets (Audi, BMW, Ford, etc.) into a single unified dataset and training a distributed regression model using **Apache Spark ML**.

The goal is to showcase an **end-to-end data engineering and machine learning workflow** — from data cleaning and preprocessing to model training, evaluation, and optional app deployment.

---

## ⚙️ Tech Stack
- **PySpark (Spark MLlib)** – distributed data processing & regression modeling
- **Pandas / NumPy** – lightweight data cleaning
- **Streamlit / FastAPI (optional)** – interactive model demo
- **Matplotlib / Seaborn** – visualization
- **MLflow (optional)** – experiment tracking
- **Docker (optional)** – containerized reproducible environment

---

## 🧩 Project Architecture
Raw CSVs (per car brand)
↓
Pandas cleaning (column alignment, missing values)
↓
Merged dataset (all_cars_clean.csv)
↓
Spark ML Pipeline
├── Feature Engineering
├── VectorAssembler
├── LinearRegression
└── Evaluation (RMSE, R²)
↓
Model Save 


---

## 📁 Folder Breakdown
| Folder | Description |
|--------|--------------|
| `data/` | Raw and cleaned datasets |
| `notebooks/` | Jupyter notebooks for step-by-step exploration |
| `src/` | Core Python scripts for cleaning, training, and evaluation |
| `models/` | Trained Spark model and metadata |
| `app/` | Optional Streamlit app for predictions |
| `scripts/` | Bash scripts for running pipelines |

---

## 🚀 Quick Start

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/Victor-Johnson/spark-car-price-prediction.git
cd spark-car-price-prediction
