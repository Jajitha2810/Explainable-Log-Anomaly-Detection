# Chapter 2: Literature Review

## 2.1 Introduction

This chapter reviews previous research related to log anomaly detection, machine learning approaches, Isolation Forest, and Explainable Artificial Intelligence (XAI). The purpose of this review is to identify current research trends, existing limitations, and the research gap addressed by this study.
## 2.2 Log Anomaly Detection

System logs provide valuable information about the operational behaviour of distributed computing systems. They record normal activities, warnings, failures, and communication between system components. Detecting anomalous log events is essential for identifying failures, security threats, and abnormal system behaviour.

Traditional log analysis methods rely on manual inspection or predefined rule-based systems. Although effective for known events, these approaches struggle to detect new or previously unseen anomalies and do not scale well with the increasing volume of modern log data.
## 2.3 Machine Learning for Log Analysis

Machine learning has become an important technique for analysing large-scale system logs. Unlike traditional rule-based approaches, machine learning algorithms are capable of discovering hidden patterns and identifying abnormal system behaviour without requiring manually defined rules.

Machine learning methods used in log anomaly detection can generally be divided into supervised, semi-supervised, and unsupervised approaches. Supervised learning requires labelled datasets containing both normal and anomalous log entries. However, obtaining accurately labelled log data is expensive and time-consuming.

Unsupervised learning has therefore gained considerable attention because it can identify anomalies without requiring labelled training data. These methods assume that anomalous events are rare and significantly different from normal observations. Isolation Forest is one of the most widely used unsupervised anomaly detection algorithms due to its efficiency and scalability for large datasets.
## 2.4 Isolation Forest

Isolation Forest is an unsupervised machine learning algorithm specifically designed for anomaly detection. Unlike distance-based or density-based methods, Isolation Forest identifies anomalies by isolating observations rather than profiling normal data.

The algorithm constructs multiple random decision trees, known as isolation trees. During tree construction, features and split values are selected randomly. Since anomalous observations are typically rare and different from the majority of the data, they require fewer splits to become isolated. Consequently, anomalies tend to have shorter average path lengths than normal observations.

Isolation Forest offers several advantages for large-scale log analysis. It is computationally efficient, scalable to high-dimensional datasets, and does not require labelled training data. These characteristics make it particularly suitable for analysing large system log datasets such as the Hadoop Distributed File System (HDFS) logs used in this research.

Due to these advantages, Isolation Forest was selected as the primary anomaly detection model in this study.
## 2.5 Explainable Artificial Intelligence (XAI)

Explainable Artificial Intelligence (XAI) refers to techniques that enable humans to understand and interpret the decisions made by machine learning models. As machine learning algorithms become increasingly complex, many models operate as black-box systems, producing accurate predictions without providing explanations for how those predictions were generated.

The lack of interpretability presents significant challenges in critical application domains such as healthcare, cybersecurity, finance, and system monitoring. Users often require explanations to build trust, verify model behaviour, identify potential biases, and support decision-making.

XAI techniques improve transparency by identifying the factors that contribute most significantly to a model's predictions. Rather than replacing machine learning models, XAI complements them by making their decisions understandable to human users.

In the context of log anomaly detection, explainability allows system administrators to understand why a specific log entry has been classified as anomalous, enabling more informed system maintenance and troubleshooting.
## 2.6 SHAP (SHapley Additive Explanations)

SHAP (SHapley Additive Explanations) is a widely used explainability technique based on concepts from cooperative game theory. It assigns a contribution value, known as the SHAP value, to each feature involved in a machine learning prediction. These values indicate how much each feature increases or decreases the model's output.

One of the key advantages of SHAP is that it provides both global and local explanations. Global explanations identify the most influential features across the entire dataset, while local explanations describe the contribution of each feature for an individual prediction.

SHAP has become popular because it offers consistent, mathematically grounded explanations that can be applied to a wide range of machine learning models, including tree-based algorithms such as Isolation Forest.

In this research, SHAP is employed to explain the anomaly predictions generated by the Isolation Forest model, thereby improving the transparency and interpretability of the proposed anomaly detection framework.
## 2.7 Research Gap

Previous studies have demonstrated that machine learning techniques are effective for detecting anomalies in large-scale system logs. Numerous approaches have focused on improving anomaly detection accuracy using supervised and unsupervised learning algorithms.

However, many existing studies primarily concentrate on prediction performance while providing limited insight into the reasoning behind anomaly classifications. As a result, system administrators often struggle to understand why particular log entries are identified as anomalous, reducing trust in automated monitoring systems.

Although Explainable Artificial Intelligence (XAI) techniques have recently gained attention, their application to log anomaly detection remains relatively limited. In particular, the integration of Isolation Forest with SHAP explainability for HDFS log analysis has not been extensively explored.

This research addresses this gap by combining efficient unsupervised anomaly detection using Isolation Forest with SHAP-based explainability. The proposed framework not only detects anomalous log events but also provides interpretable explanations that improve transparency, trust, and practical usability in distributed system monitoring.
## 2.8 Chapter Summary

This chapter reviewed previous research related to log anomaly detection, machine learning approaches, Isolation Forest, Explainable Artificial Intelligence, and SHAP explainability. The literature highlights the effectiveness of machine learning for anomaly detection while identifying the lack of model interpretability as an important limitation. The identified research gap provides the motivation for the explainable anomaly detection framework proposed in this dissertation.
