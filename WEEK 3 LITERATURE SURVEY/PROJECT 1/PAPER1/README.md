Paper 01
Paper Title

A Deep Learning/Machine Learning Approach for Anomaly Based Network Intrusion Detection

Authors

Reem Almuhanna, Samia Dardouri

Year

2025

Journal

Frontiers in Artificial Intelligence

DOI

10.3389/frai.2025.1625891

Paper Link

Official Open-Access Paper / Free Full Text

1. Project / Paper Overview

This research presents a hybrid network intrusion detection approach that combines several machine-learning and deep-learning techniques. The main objective is to improve the detection of both known and emerging network attacks by using multiple models rather than depending on one algorithm.

2. Problem Statement

Traditional IDS solutions can struggle with new attack patterns because signature-based methods mainly recognize previously known threats. The research also considers challenges such as imbalanced network-traffic data and the difficulty of maintaining reliable detection across different attack categories.

3. Existing System

The paper proposes a hybrid anomaly-based NIDS. Instead of using only one classifier, it combines several ML and DL models and uses their outputs together for intrusion classification.

4. Technologies / Methods Used
XGBoost
Random Forest
Graph Neural Networks (GNN)
Long Short-Term Memory (LSTM)
Autoencoders
SMOTE
Weighted soft-voting ensemble
Feature engineering
CICIDS2017 dataset

The study used more than 5.6 million network-traffic records for its main training/evaluation process.

5. Main Advantages
Combines different ML and DL techniques.
Can identify different categories of network attacks.
Uses an ensemble mechanism rather than relying on a single model.
Addresses class imbalance using SMOTE.
Evaluates the approach using cross-validation.
Tests generalization using an independent benchmark dataset.
6. Main Disadvantages / Limitations
The approach is primarily focused on detection and classification.
It does not provide the complete threat-intelligence and automated-response pipeline proposed in your project.
High-complexity models can increase computational requirements.
Dataset-based evaluation does not automatically guarantee real-time performance in every production environment.
7. Component Relevant to Our Project

The most relevant part is the hybrid ML/DL intrusion-detection layer.

Your project can use this concept for:

Network Traffic → Feature Extraction → ML/DL Detection → Attack/Anomaly Result

8. Research Gap

The paper concentrates mainly on improving intrusion-detection accuracy through hybrid ML/DL models. Your proposed system can extend this idea by combining detection results with threat intelligence, risk scoring and automated response.

9. Relevance to Our Project

Very High.

This is one of the strongest base papers for your Project 1 because your proposed IDS also uses multiple detection techniques and an anomaly-detection layer.

10. How We Can Extend This Paper

Your project can build an additional security-decision layer:

Hybrid Detection → Threat Intelligence → Risk Score (0–100) → Allow/Monitor/Alert/Block → Cloud Dashboard
