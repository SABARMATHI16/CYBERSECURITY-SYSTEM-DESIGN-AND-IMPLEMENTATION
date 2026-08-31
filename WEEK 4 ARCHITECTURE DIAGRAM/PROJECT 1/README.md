# Project 1 – Cloud-Based Intelligent Hybrid Intrusion Detection System

## Overview

The system is designed to monitor network traffic in a cloud environment and identify potential cyberattacks. It combines **known attack detection and anomaly detection** to detect both recognized and unusual network activities.

The detected results are combined and enriched with **threat intelligence** before calculating a risk score. Based on the risk level, the system can monitor, generate alerts, or perform an automated response.

## High-Level Workflow

**Network Traffic → Cloud Traffic Collector → Traffic Preprocessing → Feature Extraction → Known Attack Detection + Anomaly Detection → Hybrid Result Fusion → Threat Intelligence Enrichment → Risk Scoring Engine → Risk Score → Risk-Based Response → Audit & Security Logs → Cloud Database → Cloud Security Dashboard**

## System Modules

**1. Network Traffic**
Provides network activity that needs to be analyzed for possible security threats.

**2. Cloud Traffic Collector**
Collects network traffic and forwards it to the cloud-based detection pipeline.

**3. Traffic Preprocessing**
Cleans and prepares the collected traffic for further analysis.

**4. Feature Extraction**
Extracts relevant characteristics from the network traffic for detection.

**5. Known Attack Detection**
Identifies previously recognized attack patterns using detection models.

**6. Anomaly Detection**
Detects unusual traffic behavior that differs from normal patterns.

**7. Hybrid Result Fusion**
Combines the results from known attack and anomaly detection to improve the overall assessment.

**8. Threat Intelligence Enrichment**
Adds available threat information to provide additional context about detected activity.

**9. Risk Scoring Engine**
Combines the security information and produces a **risk score from 0–100**.

**10. Risk-Based Response**
The system selects an action according to the calculated risk:

* **Low Risk → Monitor**
* **Medium Risk → Alert / Investigate**
* **High Risk → Automated Response / Block**

**11. Audit & Security Logs**
Records detected events, risk scores, alerts, and actions taken by the system.

**12. Cloud Database / Store**
Stores security events and monitoring information for later analysis.

**13. Cloud Security Dashboard**
Displays detected attacks, risk levels, alerts, responses, and security activity.

## Core Concept

**Collect Network Traffic → Preprocess → Extract Features → Detect Attacks → Combine Results → Enrich Threat Information → Calculate Risk → Respond → Log → Monitor**

## Architecture Direction

The architecture connects **network monitoring, hybrid intrusion detection, threat intelligence, risk assessment, and automated response** into one cloud-based security workflow. This allows the system to move from simply detecting an attack to **evaluating its risk and taking an appropriate security action**.

