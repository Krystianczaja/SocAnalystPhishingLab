# TryHackMe SOC Analyst – Phishing and Firewall ticket

### [YouTube Demonstration / Lab Walkthrough](https://www.youtube.com/placeholder)

---

## Description
This lab simulates phishing attacks and allows the user to respond to alerts using a Security Operations Center (SOC) workflow.  
Users practice analyzing emails, URLs, and alerts in a Splunk environment, escalate critical threats, and document incident response procedures.  
The lab emphasizes practical SOC skills and threat analysis for real-world cybersecurity scenarios.

---

## Tools and Utilities Used

- **Splunk**  
- **Analyst VM / SOC Environment**  
- **Email Analysis Tools**  
- **Python / Bash (optional scripting for analysis)**  

---

## Environment Used

- **Windows 10 / Linux (VMs)**  
- **TryHackMe SOC Lab Environment**  

---

## Lab Walk-through
1. All incoming alerts are triaged in the SOC alert queue. Alerts are prioritized based on severity, potential impact, and likelihood of being malicious
![SOC Alert Queue](https://i.imgur.com/sRDZAFh.png)


2. I start with the highest severity alert because it represents the greatest potential risk to the organization. This ensures critical threats are addressed immediately.  

![Selected Ticket Details](https://i.imgur.com/jc4yxkX.png)
3. Action Taken: Opened the SIEM (Splunk/Chronicle) and looked up the URL associated with the alert.

Purpose: To verify if the URL was flagged in the threat intelligence feeds and confirm the firewall correctly blocked it.

Outcome: Verified that the URL matched a known malicious or blacklisted domain and that the threat was successfully blocked.

![Threat Analysis](https://i.imgur.com/JWCfNEE.png)
## Key Takeaways

- Hands-on experience with SOC alert triage and incident response  
- Practical phishing detection and threat analysis  
- Familiarity with Splunk dashboards and alert queues  
- Documentation of SOC procedures for escalated incidents  

---

## How to Run / Lab Instructions

1. Enroll in TryHackMe SOC Analyst course.  
2. Launch the lab environment (Analyst VM).  
3. Follow lab instructions to identify and respond to phishing alerts.  
4. Document your findings and escalate critical threats.  

---

