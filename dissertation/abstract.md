# Abstract

Log anomaly detection plays an important role in maintaining the reliability and security of distributed computing systems. Traditional manual analysis of system logs is time-consuming and becomes increasingly difficult as the volume of generated log data grows.

This research proposes an explainable anomaly detection framework using the Isolation Forest algorithm combined with SHAP (SHapley Additive Explanations). The Hadoop Distributed File System (HDFS) log dataset was preprocessed and transformed through feature engineering before applying the anomaly detection model. Experimental results demonstrated that the proposed framework successfully identified anomalous log entries while providing interpretable explanations for model predictions.

The explainability analysis highlighted message length, log level, and system components as key factors influencing anomaly detection. The integration of SHAP improved the transparency of the machine learning model, making the framework more useful for system administrators investigating abnormal log events.

Overall, the proposed approach demonstrates that combining unsupervised anomaly detection with explainable artificial intelligence provides an effective solution for distributed system log analysis.

**Keywords:** Explainable Artificial Intelligence, Isolation Forest, SHAP, Log Anomaly Detection, Machine Learning, Hadoop.