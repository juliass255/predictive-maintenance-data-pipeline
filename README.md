# Predictive Maintenance Data Pipeline

##  Overview
[PT]
Este projeto simula um pipeline completo de engenharia de dados e aprendizado de máquina para manutenção preditiva usando dados de sensores de IoT industrial, graças à minha paixão ao chão de fábrica e às maquinas.

O objetivo é processar medições de sensores brutas, realizar limpeza de dados e engenharia de features, armazenar os dados processados em um banco de dados SQLite, fazer análise em SQL e treinar um modelo de aprendizado de máquina capaz de prever falhas de máquinas.

Este projeto foi desenvolvido usando apenas ferramentas gratuitas (Google Colab, GitHub e SQLite).

[EN]
This project simulates a complete data engineering and machine learning pipeline for predictive maintenance using industrial IoT sensor data, thanks to my passion for the factory floor and machines.

The goal is to process raw sensor measurements, perform data cleaning and feature engineering, store the processed data in a SQLite database, do analysis in SQL, and train a machine learning model capable of predicting machine failures.

This project was developed using only free tools (Google Colab, GitHub, and SQLite).
---

##  Dataset

- Source: AI4I 2020 Predictive Maintenance Dataset
- Records: 10,000
- Features:
  - Air Temperature
  - Process Temperature
  - Rotational Speed
  - Torque
  - Tool Wear
  - Machine Type
  - Target:
  - Machine Failure

---

##  Pipeline

```
Raw CSV
     │
     ▼
Data Validation
     │
     ▼
Data Cleaning
     │
     ▼
Feature Engineering
     │
     ▼
SQLite Database
     │
     ▼
SQL Queries
     │
     ▼
Exploratory Data Analysis
     │
     ▼
Random Forest Model
     │
     ▼
Failure Prediction
```

---

##  Technologies

- Python
- Pandas
- NumPy
- SQLite
- SQL
- Matplotlib
- Scikit-learn
- Google Colab
- Git
- GitHub

---

##  Feature Engineering

The following features were created during preprocessing:

- Temperature Difference
- Power Index
- Wear Level

The project also removes unnecessary identifiers and prevents data leakage by excluding failure-specific columns.

---

##  Machine Learning

Algorithm:

- Random Forest Classifier

Train/Test Split:

- 80% Training
- 20% Testing

---

##  Model Performance

| Metric | Value |
|---------|-------|
| Accuracy | 99% |
| Precision | 93% |
| Recall | 79% |
| F1-score | 86% |

The dataset is highly imbalanced (approximately 3.4% failures), therefore Precision, Recall and F1-score are more informative than Accuracy alone.

---

##  Dataset Distribution

![Failure Distribution](images/failure_distribution.png)

---

##  Failure Rate by Wear Level

![Wear Level](Saídas/imagens/wear_level.png)

---

##  Failure Rate by Machine Type

![Machine Type](images/failure_rate_machine_type.png)

---

##  Feature Importance

![Feature Importance](Saídas/imagens/feature_importance.png)
---

##  Repository Structure

```
predictive-maintenance-data-pipeline/

│
├── README.md
├── 01_predictive_maintenance.ipynb
├── predictive_maintenance_clean.csv
├── maintenance.db
├── random_forest_model.pkl
├── feature_importance.png
```

---

##  Future Improvements

- Airflow orchestration
- PostgreSQL
- Docker
- MLflow
- Streamlit Dashboard
- Power BI Dashboard
- Cloud deployment (AWS)

---

##  Author

Julia Souza Borges
