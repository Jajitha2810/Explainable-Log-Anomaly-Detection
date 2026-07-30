# Chapter 1: Introduction

## 1.1 Background

Distributed computing systems such as Hadoop generate massive volumes of log messages during their normal operation. These logs record system events, resource usage, warnings, failures, and communication between distributed components. As organisations increasingly rely on distributed computing platforms to process large datasets, analysing these log files has become an important task for maintaining system reliability and detecting abnormal behaviour.
## 1.2 Problem Statement

Modern distributed systems continuously generate enormous volumes of log data that are difficult to analyse manually. Traditional monitoring approaches rely heavily on predefined rules and expert knowledge, which often fail to detect previously unseen anomalies.

Although machine learning techniques improve anomaly detection performance, many models provide little insight into the reasoning behind their predictions. This lack of transparency reduces user trust and limits the practical adoption of machine learning models in real-world system monitoring.

Therefore, there is a need for an explainable anomaly detection framework capable of automatically identifying abnormal log events while providing meaningful explanations for its decisions.
## 1.3 Aim

The aim of this research is to develop an explainable machine learning framework for detecting anomalies in HDFS log data using Isolation Forest and SHAP explainability.
## 1.4 Objectives

The objectives of this research are:

- To analyse the HDFS log dataset.
- To perform feature engineering on structured log data.
- To implement an Isolation Forest model for unsupervised anomaly detection.
- To evaluate anomaly detection results.
- To apply SHAP explainability for interpreting anomaly predictions.
- To develop an explainable anomaly detection pipeline suitable for distributed system logs.
## 1.5 Research Contributions

The contributions of this research include:

- Development of an explainable log anomaly detection framework.
- Integration of Isolation Forest with SHAP explainability.
- Feature engineering techniques for HDFS log data.
- A reproducible machine learning workflow implemented using Python and Jupyter Notebook.
## 1.6 Research Questions

This research aims to answer the following questions:

1. Can machine learning techniques effectively detect anomalies in HDFS log data without labelled training data?

2. Which log features contribute most significantly to anomaly detection decisions?

3. Can SHAP explanations improve the interpretability of Isolation Forest anomaly detection results?

4. How can explainable artificial intelligence improve trust in automated log monitoring systems?
## 1.7 Dissertation Structure

This dissertation is organised into five chapters.

Chapter 1 introduces the research background, problem statement, aim, objectives, and contributions of the study.

Chapter 2 presents the literature review covering log anomaly detection, machine learning approaches, Isolation Forest, and explainable artificial intelligence techniques.

Chapter 3 describes the methodology used in this research, including dataset preparation, feature engineering, anomaly detection, model evaluation, and SHAP-based explanations.

Chapter 4 presents the experimental results and analysis of the proposed framework.

Chapter 5 concludes the research and discusses limitations and possible future improvements.