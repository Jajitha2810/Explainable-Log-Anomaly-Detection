# Explainable Machine Learning for System Log Anomaly Detection

## 📌 Overview

This repository contains my research project on explainable machine learning for detecting anomalies in system log data. The goal is to compare traditional machine learning and deep learning approaches while improving the interpretability of anomaly detection models using Explainable AI (XAI) techniques.

---
## 📢 Latest Progress

- ✅ Structured HDFS dataset created
- ✅ Initial exploratory data analysis completed
- ✅ Two visualization figures generated
- 🔄 Preparing data for anomaly detection modelling
---
## 📁 Project Structure

```text
AI_Research/
├── datasets/
├── figures/
├── notebooks/
├── papers/
├── results/
```
---

## 🎯 Research Objectives

- Compare traditional anomaly detection algorithms.
- Implement deep learning-based anomaly detection models.
- Apply Explainable AI techniques such as SHAP and LIME.
- Evaluate model performance on public system log datasets.
- Develop a reproducible research framework.

---

## 📂 Dataset

- ✅ HDFS Log Dataset (HDFS_2k)

---

## 🤖 Planned Models

- Isolation Forest
- One-Class SVM
- Local Outlier Factor (LOF)
- Autoencoder Neural Network

---

## 📊 Evaluation Metrics

- Precision
- Recall
- F1 Score
- ROC-AUC
- Inference Time
---
🚀 Current Status

✅ Research topic finalized
✅ GitHub repository created
✅ Literature review completed
✅ HDFS dataset collected
✅ Initial dataset exploration completed
✅ Feature engineering completed
✅ Isolation Forest implemented
✅ Model evaluation completed
✅ SHAP explainability completed
🔄 Paper writing in progress
  

---
| Stage                     | Status         |
| ------------------------- | -------------- |
| Literature Review         | ✅ Completed    |
| Dataset Preparation       | ✅ Completed    |
| Exploratory Data Analysis | ✅ Completed    |
| Model Development         | ✅ Completed    |
| Explainability Analysis   | ✅ Completed    |
| Paper Writing             | 🔄 In Progress |


---

- ## Progress Log

### Day 1 – Environment Setup
---
* Installed Python 3.14
* Installed Git
* Installed Visual Studio Code
* Configured Jupyter Notebook
* Created the research project structure
* Downloaded the HDFS_2k dataset
---
### Day 2 – Initial Dataset Exploration
---
* Successfully loaded the HDFS_2k log dataset using Python.
* Verified that the dataset contains 2,000 log entries.
* Explored the structure of HDFS log messages.
* Identified key components such as timestamps, log levels, Block IDs, DataNode, PacketResponder, and FSNamesystem.
* Recorded initial observations about the dataset for future analysis.
---
### Day 3 – Data Structuring and Exploratory Data Analysis
---
* Parsed raw HDFS log entries into a structured pandas DataFrame.
* Saved the processed dataset as `HDFS_2k_structured.csv`.
* Performed exploratory data analysis (EDA).
* Visualized the distribution of log levels.
* Analyzed Hadoop component frequency.
* Documented observations within the research notebook.
* Generated the first research figures for the project.
* Initialized Git version control and created the first project commit.
----
### Day 4 – Feature Engineering

* Created a dedicated feature engineering notebook.
* Engineered numerical and binary features from HDFS log messages.
* Generated a machine-learning-ready feature matrix.
* Documented observations about engineered features.

---

### Day 5 – Isolation Forest & Initial Model Evaluation

* Implemented the Isolation Forest anomaly detection model.
* Successfully trained the model using engineered HDFS log features.
* Generated anomaly predictions for all 2,000 log entries.
* Detected 88 anomalous log entries (approximately 4.4% of the dataset).
* Created the initial model evaluation notebook.
* Visualized the distribution of normal and anomalous log entries.
* Identified dfs.DataNode$DataXceiver as the component with the highest number of detected anomalies.
* Documented initial observations for future Explainable AI analysis.
---
### Completed

- Development environment setup
- GitHub repository creation
- HDFS dataset download
- Initial HDFS log exploration
- Parsed raw HDFS logs into a structured pandas DataFrame
- Exploratory Data Analysis (EDA)
- Feature engineering
- Machine learning feature matrix preparation
- Isolation Forest anomaly detection model
- Initial model evaluation
----
### Currently Working On

- Evaluating Isolation Forest results.
- Preparing Explainable AI (SHAP) analysis.

   ## 👩‍💻 Author

**Jajitha Kumbakonam**

Research Interests:
- Artificial Intelligence
- Machine Learning
- Anomaly Detection
- Explainable AI (XAI)
- Natural Language Processing
- Large Language Models



GitHub: https://github.com/jajitha2810

---

> This repository is part of an ongoing research project that aims to contribute to trustworthy and explainable AI for anomaly detection.
