# Chapter 5: Conclusion

## 5.1 Summary of Research

This research proposed an explainable machine learning framework for detecting anomalies in Hadoop Distributed File System (HDFS) log data.

The study began with dataset collection and preprocessing, followed by feature engineering to transform raw log information into meaningful numerical attributes. An Isolation Forest model was then implemented to detect anomalous log entries without requiring labelled training data.

To improve model transparency, SHAP (SHapley Additive Explanations) was applied to explain the anomaly detection decisions. The results demonstrated that the proposed framework successfully identified anomalous log events while providing interpretable explanations of the factors contributing to those predictions.
## 5.2 Research Contributions

The main contributions of this research include:

- Development of an explainable anomaly detection framework for distributed system logs.

- Successful implementation of Isolation Forest for unsupervised anomaly detection.

- Application of SHAP explainability to improve model transparency.

- Development of a complete machine learning workflow including preprocessing, feature engineering, anomaly detection, evaluation, and interpretation.

- Demonstration that explainable artificial intelligence techniques can improve trust in automated log anomaly detection systems.
## 5.3 Limitations

Although the proposed framework produced promising results, several limitations should be acknowledged.

The experiments were conducted using a single HDFS log dataset, which may limit the generalisability of the findings to other distributed computing environments.

Furthermore, the Isolation Forest contamination parameter was selected manually and may influence the number of detected anomalies. Additional experiments using multiple parameter settings could provide a more comprehensive evaluation.

Finally, the research focused on one anomaly detection algorithm. Other unsupervised machine learning techniques may produce different detection performance.
## 5.4 Future Work

Future research may extend this work by investigating alternative anomaly detection algorithms such as Autoencoders, One-Class Support Vector Machines, and deep learning approaches.

Additional explainability techniques could also be explored to compare their effectiveness with SHAP.

Future studies may evaluate the proposed framework using larger datasets collected from different distributed computing environments and investigate real-time anomaly detection for production systems.
## 5.5 Conclusion

In conclusion, this research successfully developed an explainable log anomaly detection framework using Isolation Forest and SHAP explainability.

The proposed approach effectively identified anomalous HDFS log events while providing meaningful explanations for model predictions. The integration of explainable artificial intelligence improves the transparency and practical applicability of machine learning models for distributed system monitoring.

Overall, this research demonstrates that combining efficient unsupervised anomaly detection with explainability techniques provides a valuable solution for modern log analysis and system reliability.