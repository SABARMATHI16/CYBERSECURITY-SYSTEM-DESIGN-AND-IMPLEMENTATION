Case Study 1 – Adaptive Hybrid IDS
Cloud-Based Adaptive Hybrid Intrusion Detection System for IoT/Edge Traffic with Feedback-Weighted Risk Scoring and Explainable Alerts
1. Introduction

IoT and edge devices are now widely used in areas such as smart homes, healthcare, industries, and connected infrastructure. These devices continuously communicate over networks, but many of them have limited processing capabilities and different hardware, software, and communication protocols. Because of this, detecting attacks in IoT and edge environments can be more difficult than detecting attacks in conventional networks. A normal IDS may either miss new types of attacks or generate too many false alerts. To address this issue, this project proposes a cloud-based hybrid IDS designed specifically for IoT/edge network traffic. It combines different detection methods and dynamically adjusts their contribution to the final security decision.

2. Core Problem

Existing IDS solutions are generally effective at identifying previously known attacks, but detecting new or changing attack behavior remains a challenge. This becomes more difficult in IoT/edge networks because different devices can produce very different traffic patterns. A detector that works well for one type of device may not perform equally well for another. Using fixed weights for multiple detection methods can also reduce accuracy when the reliability of a detector changes over time.

Therefore, the main question addressed by this project is:

How can IoT/edge network traffic be continuously monitored to identify both known and unknown attacks, while dynamically adapting detector reliability and providing analysts with an understandable explanation for every security alert?

3. Proposed Solution

The proposed system is a Cloud-Based Adaptive Hybrid Intrusion Detection System that continuously analyzes IoT and edge network traffic.

The system combines several security mechanisms:

Signature-based attack detection
Machine-learning-based detection
Anomaly detection
Threat intelligence
Feedback-based risk scoring
Automated response
Cloud-based monitoring and logging

Network traffic is first collected and converted into useful IoT-related features. These features are then analyzed by multiple detection modules. The system can consider traffic characteristics such as MQTT/CoAP communication patterns and device polling behavior.

The outputs from the different detectors are combined with threat-intelligence information. A risk engine then produces an overall risk score and classifies the activity as low, medium, or high risk.

Depending on the result, the system can:

Monitor → Alert → Block

4. Proposed Technical Innovation

The main technical idea of this project is a Feedback-Weighted Adaptive Hybrid Risk-Based Detection Model.

Instead of giving every detector a permanent or fixed importance, the system keeps track of how reliable each detector has been recently. When previous alerts are confirmed as correct or incorrect, this feedback is used to adjust the detector's contribution to future risk calculations.

For example, if the anomaly detector is currently producing more accurate results than another detector, its influence on the final risk score can be increased.

The overall process is:

Network Traffic → Multiple Detection Methods → Threat Intelligence → Feedback-Weighted Risk Engine → Explainable Alert → Response

Another important feature is explainable alerts. Rather than displaying only a risk score such as 85/100, the system will provide information about why the score was high.

For example:

Signature detector: triggered
Anomaly detector: high anomaly level
Threat intelligence: suspicious source
Final risk score: 85/100
Recommended action: Block

This makes the result easier for a security analyst to understand.

5. Cloud Deployment

The system will be designed using cloud-based services so that traffic analysis and monitoring can be performed centrally.

The proposed cloud architecture can include:

IoT/edge traffic collector
Feature-processing service
ML inference service
Anomaly detection service
Threat-intelligence service
Feedback-weighted risk engine
Event database
Alert and response service
Security monitoring dashboard

This architecture also allows the system to be expanded later when the number of monitored devices increases.

6. Expected Impact

The proposed system is expected to improve intrusion detection for IoT and edge environments by using more than one detection technique. The adaptive weighting mechanism can help the system respond when the performance of individual detectors changes over time.

The explainable alert mechanism can also make security results easier to understand because analysts can see which detection signals contributed to the final decision.

Overall, the project aims to provide a more adaptive, transparent, and practical approach to IoT/edge intrusion detection.

7. Case Study Takeaway

The main idea of this project is that an IoT/edge IDS should not simply combine several detectors and produce a final number. It should also consider which detection methods are currently reliable, why an alert was generated, and what action should be taken.

The project therefore focuses on three important aspects:

Adaptive Detection + Explainable Risk Scoring + Automated Response
