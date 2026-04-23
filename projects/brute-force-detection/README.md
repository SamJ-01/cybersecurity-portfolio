# 🕵️ Brute Force Attack Investigation

## 📌 Scenario
A system showed multiple failed login attempts over a short period. The objective was to determine whether this activity indicated a brute-force attack.

---

## 🛠 Tools & Environment

- Microsoft Azure (Cloud Infrastructure)
- Virtual Networks (VNet) & Network Security Groups (NSG)
- Log Analytics Workspace (Centralised logging)
- Microsoft Sentinel (SIEM)
- Endpoint Detection & Response (EDR)
- Tenable (Vulnerability Scanning)

---

## 🌐 Environment Overview

This investigation was conducted within a cloud-based enterprise SOC environment hosted on Microsoft Azure.

The setup included:

- Multiple virtual networks simulating enterprise infrastructure  
- Network Security Groups (NSGs) controlling traffic flow  
- Virtual machines acting as endpoints within subnets  
- Centralised log collection via Log Analytics  
- SIEM integration using Microsoft Sentinel for event correlation  
- Continuous vulnerability monitoring using Tenable  

The environment was exposed to real-world attack patterns, allowing for realistic detection and response scenarios similar to a live Security Operations Center (SOC).

---

## 🔍 Investigation Steps

1. Reviewed authentication logs  
2. Identified repeated failed login attempts  
3. Observed patterns from a single IP address  
4. Analysed timing between attempts  

---

## 🚨 Findings

- High number of failed login attempts  
- Activity originated from a single IP  
- Pattern consistent with brute-force behaviour  

---

## 🧠 Conclusion

The observed activity strongly indicates a brute-force attack targeting user accounts.

---

## 🛡 Recommendations

- Enable account lockout policies  
- Implement multi-factor authentication (MFA)  
- Block suspicious IP addresses  
- Monitor for continued attack attempts  

---

## 🧩 SOC Workflow Context

This investigation aligns with a real-world SOC workflow:

1. Detection (EDR / Sentinel alert)  
2. Log collection (Log Analytics)  
3. Correlation (SIEM analysis)  
4. Investigation (analyst review)  
5. Containment & response recommendations  
