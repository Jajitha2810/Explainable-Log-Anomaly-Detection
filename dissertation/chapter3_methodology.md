# Chapter 3: Methodology

## 3.1 Research Design

This research follows a quantitative experimental methodology for developing an explainable anomaly detection framework for distributed system log data.

The proposed framework consists of data collection, data preprocessing, feature engineering, anomaly detection using Isolation Forest, model evaluation, and explainability analysis using SHAP (SHapley Additive Explanations).

Python programming language together with Jupyter Notebook was used to implement the complete experimental workflow.
## 3.2 Dataset Description

The experiments were conducted using the Hadoop Distributed File System (HDFS) log dataset.

The structured HDFS dataset contains system log entries generated from Hadoop operations. Each log entry includes information such as timestamp, thread identifier, log level, system component, and message content.

Feature engineering was performed to convert textual log information into numerical attributes suitable for machine learning algorithms.
## 3.3 Data Preprocessing

The original HDFS log data was converted into a structured dataset before model development. Missing values and duplicate records were examined to ensure data quality.

Relevant log attributes were selected for anomaly detection. Textual log messages were processed to derive numerical features suitable for machine learning. The preprocessing stage ensured that the dataset was clean, consistent, and ready for feature engineering.
## 3.4 Feature Engineering

Feature engineering was performed to transform raw log information into meaningful numerical attributes. Several features were extracted from each log entry, including message length, presence of block identifiers, occurrence of packet responders, error indicators, warning indicators, and component information.

Categorical variables such as log level and system component were encoded into numerical representations using label encoding techniques. These engineered features provided the Isolation Forest model with meaningful information for distinguishing normal and anomalous log events.
## 3.5 Isolation Forest Model

Isolation Forest was selected as the primary anomaly detection algorithm due to its efficiency and suitability for unsupervised learning. Unlike supervised classification algorithms, Isolation Forest does not require labelled anomaly data during training.

The model was implemented using the Scikit-learn machine learning library in Python. A contamination rate of 5% was selected to estimate the proportion of anomalies within the dataset. Random state 42 was specified to ensure reproducibility of the experimental results.

After training, the model assigned an anomaly score to each log entry. Log records predicted as anomalous were labelled as -1, while normal observations were labelled as 1.
## 3.6 Model Evaluation

The performance of the Isolation Forest model was evaluated by analysing the distribution of detected anomalies and examining their characteristics.

Visualisations were created to compare the number of normal and anomalous log entries. Additional analyses examined the distribution of anomalies across log levels, system components, and message lengths.

The evaluation demonstrated that anomalous log entries generally contained longer messages and were concentrated within specific Hadoop components, supporting the effectiveness of the anomaly detection model.
## 3.7 SHAP Explainability

To improve the interpretability of the anomaly detection model, SHAP (SHapley Additive Explanations) was applied after the Isolation Forest model generated anomaly predictions.

SHAP values were calculated to determine the contribution of each engineered feature to the anomaly detection decisions. Summary plots were generated to visualise feature importance across the dataset.

The explainability analysis identified message length, log level, and Hadoop system components as some of the most influential features affecting anomaly detection. These explanations provide valuable insights for system administrators when investigating abnormal log events.
## 3.8 Research Workflow

The overall research workflow followed a sequential process consisting of dataset collection, preprocessing, feature engineering, anomaly detection, model evaluation, and explainability analysis.

The implementation was organised using Jupyter Notebooks to ensure reproducibility and maintain a structured experimental pipeline. Each stage of the workflow was independently validated before progressing to the next stage, resulting in a complete explainable anomaly detection framework.
## 3.9 Chapter Summary

This chapter described the methodology adopted in this research. It presented the dataset, preprocessing procedures, feature engineering techniques, Isolation Forest implementation, evaluation methods, and SHAP explainability analysis. The next chapter presents the experimental results obtained using the proposed framework and discusses their significance.