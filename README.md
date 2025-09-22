#  SOC Analyst Simulator  – Firewall and Phishing ticket


---

## Description
This lab simulates a Security Operations Center (SOC) workflow using **two representative tickets**.  
- **Ticket 1:** A firewall alert, where users investigate blocked external connections, confirm potential threats, and record the incident response.  
- **Ticket 2:** A phishing alert, where users practice analyzing suspicious emails and URLs, verifying threats, and documenting their findings.  


The lab emphasizes practical SOC skills, threat analysis, and proper incident documentation for real-world cybersecurity scenarios.

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
3. Action Taken: Opened the SIEM (Splunk) and looked up the URL associated with the alert.

Purpose: To verify if the URL was flagged in the threat intelligence feeds and confirm the firewall correctly blocked it.

Outcome: Verified that the URL matched a known malicious or blacklisted domain and that the threat was successfully blocked.

![Threat Analysis](https://i.imgur.com/JWCfNEE.png)

4. Here is the final step and write up for this ticket.
    ![Firewall Alert](https://i.imgur.com/hh3zBlH.png)
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

