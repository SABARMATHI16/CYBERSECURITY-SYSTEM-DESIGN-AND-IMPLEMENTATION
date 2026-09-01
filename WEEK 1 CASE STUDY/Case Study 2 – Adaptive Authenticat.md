**Case Study 2 – Adaptive Authentication
Cloud-Based Continuous User Behavior Risk Analysis and Adaptive Authentication System with Keystroke Dynamics and Replay-Resistant Scoring
1. Introduction

Most authentication systems verify a user's identity mainly through a username and password at the time of login. Although additional information such as IP address, device and location can improve security, these details may also be available to an attacker who has compromised the user's account or copied the user's login environment.

Because of this, checking the user's identity only once may not be enough for protecting an entire session. This project proposes a cloud-based authentication system that continuously observes user behavior and checks whether the person using the account still behaves like the legitimate user.

2. Core Problem

Consider a situation where an attacker obtains a user's username and password. If the attacker also uses a familiar device, IP address, or location, a conventional adaptive authentication system may consider the login normal.

However, the attacker's actual behavior may be different from the genuine user's behavior.

For example, the attacker may:

Type differently
Navigate through the application differently
Perform actions at an unusual speed
Access pages in an unusual sequence

Therefore, the main problem addressed by this project is:

How can a system continuously determine whether the person using an authenticated account is actually the legitimate user, even when the attacker has access to the user's normal login context?

3. Proposed Solution

The proposed system adds a continuous behavioral-security layer to normal authentication.

During login and throughout the session, the system can collect information such as:

IP address
Device information
Location
Login time
Browser information
Failed login attempts
Keystroke dynamics
In-session navigation behavior

Among these, keystroke dynamics is an important part of the proposed system. The system observes typing characteristics such as the timing between key presses and releases and compares them with the user's established behavioral pattern.

Machine-learning techniques are then used to compare the current activity with the user's behavioral profile.

The system produces a dynamic risk score and applies an adaptive decision:

Low Risk → Continue Session

Medium Risk → Request Step-Up MFA

High Risk → Terminate Session + Alert

4. Proposed Technical Innovation

The main technical idea is a Continuous Behavior-Aware Adaptive Authentication Model.

Traditional authentication mainly asks:

"Are the credentials correct?"

Context-based authentication may additionally ask:

"Is the device, IP address, location and login time normal?"

The proposed system goes one step further by continuously asking:

"Does the current user's behavior still match the behavior expected from this account?"

A behavioral profile is created for each user using information such as typing rhythm and navigation patterns.

The risk score is not calculated only during login. It can be updated during the active session.

For example:

Normal typing + normal navigation → Risk remains low

Unusual typing + unusual navigation → Risk increases

If the risk becomes sufficiently high, the system can require additional authentication or terminate the session.

An important part of the project is testing the system against an attacker who already knows the legitimate user's normal login context. This helps determine whether behavioral analysis can provide additional protection beyond context-based checks.

5. Cloud Deployment

The proposed system can be implemented using a cloud-based architecture containing:

Authentication service
Behavioral-data collection service
User behavioral-profile database
Machine-learning inference service
Device and IP analysis service
Continuous risk engine
MFA service
Session management service
Event logging service
Security monitoring dashboard

The cloud environment allows authentication events and risk information to be centrally processed and monitored.

6. Expected Impact

The proposed system aims to provide additional protection against stolen credentials and session hijacking.

A genuine user with normal behavior should experience minimal interruption. However, if an attacker successfully passes the initial login and later behaves differently, the continuous behavioral analysis can increase the risk score and trigger an appropriate security action.

The use of keystroke dynamics provides an additional behavioral signal that is different from easily observable context such as IP address or device information.

7. Case Study Takeaway

The main idea of this project is that authentication should not necessarily end when login succeeds.

A secure system should continue evaluating the session and determine whether the current behavior is consistent with the legitimate account owner.

The project therefore focuses on:

Continuous Monitoring + Behavioral Analysis + Dynamic Risk Scoring + Adaptive Authentication**
