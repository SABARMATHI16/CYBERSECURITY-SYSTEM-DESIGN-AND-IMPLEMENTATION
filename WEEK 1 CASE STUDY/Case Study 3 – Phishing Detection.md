**Case Study 3 – Phishing Detection**



**AI-Based Multi-Layer Phishing Email and URL Detection System**



**1. Introduction**



**Phishing remains a major social-engineering threat in which attackers attempt to deceive users through malicious emails and URLs. Traditional detection approaches may focus primarily on either email content or URL characteristics. A more comprehensive approach can analyze both sources of information before making a final decision.**



**2. Core Problem**



**A phishing email may contain convincing content while directing the victim to a malicious URL. Similarly, a suspicious URL may appear without enough email context to make an accurate decision.**



**The problem is:**



**How can a system jointly analyze email content and URL characteristics to identify phishing attempts more effectively?**



**3. Proposed Solution**



**An AI-Based Multi-Layer Phishing Email and URL Detection System is proposed to analyze both email and URL information.**



**The system performs two separate analyses.**



**Email Analysis:**



**Subject**

**Email body**

**Keywords**

**Urgency**

**Suspicious language**



**URL Analysis:**



**URL length**

**Special characters**

**Domain structure**

**Subdomains**

**HTTPS usage**



**Separate machine-learning models generate email and URL risk scores. A risk engine combines these results into a final phishing score.**



**The system classifies the input as:**



**Legitimate, Suspicious or Phishing.**



**4. Proposed Technical Innovation**



**The project will investigate a Multi-Layer Phishing Risk Model.**



**Instead of depending on a single phishing indicator, the system maintains two analysis layers:**



**Email Content → NLP/ML Analysis**



**URL Structure → ML Analysis**



**The results are then combined by a risk engine to produce an overall phishing risk score.**



**This approach allows the final decision to consider both the message content and the destination URL.**



**5. Cloud Deployment**



**Cloud deployment is not required for the proposed system. The application can operate as a standalone web-based or local cybersecurity application with separate email-analysis and URL-analysis modules.**



**6. Expected Impact**



**The system could help identify phishing attempts by considering multiple indicators instead of relying on a single characteristic. Providing a risk score and classification can also help users understand the severity of a detected phishing attempt.**



**7. Case Study Takeaway**



**The project investigates a security requirement:**



**“A phishing detection system should not judge an email or URL using a single indicator; it should combine content and URL evidence before making a security decision.”**

