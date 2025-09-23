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
- - **Alert Queue**  
 

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








   5. Here is the second ticket which is a Phishing type. An inbound email alert was triggered due to suspicious characteristics, including the presence of external links. This type of alert is commonly associated with phishing attempts, where malicious actors try to trick users into clicking unsafe URLs.
   ![SIEM Ticket Details](https://i.imgur.com/uW5m5Io.png)

6. Reviewed the alert details in the SIEM.

Confirmed the email was received by the user.

Verified that the user did not click on any of the links, and no endpoints attempted to access the suspicious URLs.
![TryDetectThis Analysis](https://i.imgur.com/fdQ9MB9.png)

7. To further investigate the phishing alert, I opened a secure virtual machine and tested the URL using TryDetectThis to check for malicious behavior. It came back clean.
![Phishing Email in SIEM](https://i.imgur.com/swI4Y4R.png)

8. Here is the write up for ticket 2.
 ![Final Ticket Verification](https://i.imgur.com/WU1EFSb.png)

## Key Takeaways

Through this lab, I reinforced essential SOC skills, including alert triage, prioritization, and investigation. I learned how to efficiently analyze phishing emails, URLs, and firewall alerts using a SIEM, verify threats safely in a virtual environment, and document incident response procedures accurately. The lab emphasized the importance of distinguishing true positives from false positives, escalating critical alerts when necessary, and maintaining proper documentation for compliance and auditing purposes. Overall, it provided hands-on experience in applying SOC workflows to real-world cybersecurity scenarios.

---



---

