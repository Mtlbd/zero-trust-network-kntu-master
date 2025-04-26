# Zero Trust Network Architecture Implementation

## 🔖 Project Overview
Implementation of a **Zero Trust Network Architecture** using open-source security monitoring and identity management tools.

This project focuses on:
- Deploying **Elastic SIEM** for event monitoring and threat detection.
- Implementing **Keycloak** for centralized authentication, SSO, and access management.
- Simulating attacks to evaluate performance.
- Designing dashboards for real-time monitoring.

---

## 📚 Tools & Technologies

| Tool         | Purpose                                              |
|--------------|------------------------------------------------------|
| Elastic SIEM | Security Information and Event Management (SIEM)     |
| Keycloak     | Identity and Access Management (IAM) with SSO & MFA  |

### Elastic SIEM Features
- Collect logs from multiple sources (servers, firewalls, apps)
- Detect anomalies and potential attacks
- Real-time dashboards using Kibana

### Keycloak Features
- Single Sign-On (SSO) for multiple applications
- User, role, and access control management
- Supports OAuth 2.0, OpenID Connect, and SAML
- LDAP and Active Directory integration

---

## 🔢 Implementation Steps

### 1. Research & Planning
- Compared popular SIEM and IAM solutions.
- Selected Elastic SIEM and Keycloak for their open-source capabilities and strong community support.

### 2. Deployment
- Deployed Elastic Stack components using Docker/Kubernetes.
- Installed and configured Keycloak server.

### 3. Security Monitoring Setup
- Installed **Elastic Agents** on multiple virtual machines.
- Connected agents to the **Fleet Server**.
- Simulated attacks using [revshells.com](https://www.revshells.com) to generate real-world attack scenarios.

### 4. Detection Rules
- Created custom SIEM detection rules to identify suspicious processes and network activities.
- Minimized false positives using strict filtering (e.g., internal IP address whitelisting).

### 5. Authentication Management
- Configured Keycloak clients and roles.
- Enabled login event monitoring.
- Implemented SSO for simulated apps.

### 6. Dashboards and Visualization
- Designed custom dashboards in Kibana for security event visualization.
- Used Keycloak Admin Console for user activity monitoring.

---

## 🔍 Attack Simulation
- Reverse shells and subprocess execution attacks were simulated.
- Detection rules successfully identified unauthorized behaviors.
- Keycloak logs tracked login attempts and impersonation events.

---

## 👨‍💼 Authors
- Mohammad Talebi
- Alireza Karimi
- Ahmad Foroughi

---

## 🎓 License
This project was created for educational purposes within the **Network Management Course - Spring 1404** at Khajeh Nasir Toosi University of Technology.

---

> "Zero Trust is not a product, it’s a strategy."

---
