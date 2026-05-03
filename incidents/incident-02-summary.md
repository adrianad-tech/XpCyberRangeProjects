# Incident 02: Active Directory Access Control & Privilege Misconfiguration

## 🆔 Incident Information
- Submission ID: 147643  
- Challenge ID: 129  
- Timestamp: 1/29/2026 3:09 AM UTC  
- Environment: Domain Controller (Active Directory)  
- Role: Cyber IT System Administrator  
- Scenario Source: XP Cyber Range (HR & Intern Access Control)

---

## 🧠 Scenario Summary
Following the completion of an intern program at DASWebs, it was discovered that a user (Rob) with basic domain credentials had excessive access to critical systems. A review of the domain environment revealed that multiple users had improper access to servers and shared resources, creating a significant security and access control risk.

The objective was to correct misconfigured permissions, enforce least privilege principles, and secure domain account access.

---

## ⚠️ Issues Identified
- HR share accessible beyond intended users  
- Accounting share improperly exposed  
- Intern account (Rob) had excessive domain access  
- User logon restrictions not properly enforced  
- Weak segregation of duties across security groups  

---

## 🛠️ Actions Taken
- Restricted HR share access to **HRSec security group only**
- Limited HR share access from Domain Admins group appropriately
- Restricted Accounting share access to **AccountingSec security group only**
- Disabled intern account (Rob)
- Enforced workstation login restrictions:
  - Brimlock Stones → Workstation-Desk only  
  - Sergio Chanel → Workstation-Desk only  
- Applied access control corrections using domain security groups

---

## ✅ Results
All system checks passed successfully (7/7):

- ✔ HR share access secured  
- ✔ Accounting share access secured  
- ✔ Intern account disabled  
- ✔ Workstation login restrictions enforced  
- ✔ Security group permissions corrected  

Final completion time: 0:55

---

## 🧠 Skills Demonstrated
- Active Directory user and group management  
- Access control and least privilege enforcement  
- Security group configuration  
- Account lifecycle management (disable/limit access)  
- System administration and privilege auditing  
- Enterprise security policy enforcement  

---

## 🎯 SOC / Security Relevance
This scenario demonstrates real-world system administration and SOC-adjacent responsibilities including:
- Identity and access management (IAM)
- Privilege escalation prevention
- Security group configuration
- Organizational access control enforcement
- Risk mitigation in enterprise environments
