# 🛡️ Phishing Email Analysis Lab

## 📌 Overview

This project demonstrates my hands-on experience investigating phishing emails from a SOC Analyst perspective.

The lab focuses on analyzing email headers, identifying suspicious indicators, extracting IOCs, using threat intelligence sources, determining severity, and documenting appropriate incident-response actions.

## 🎯 Objectives

•⁠  ⁠Analyze suspicious phishing emails
•⁠  ⁠Investigate email headers
•⁠  ⁠Identify sender spoofing and domain impersonation
•⁠  ⁠Analyze SPF, DKIM, and DMARC results
•⁠  ⁠Extract Indicators of Compromise (IOCs)
•⁠  ⁠Investigate suspicious domains and IP addresses
•⁠  ⁠Use threat intelligence to enrich IOCs
•⁠  ⁠Determine whether an email is benign, suspicious, or malicious
•⁠  ⁠Document SOC findings and recommended actions

## 🛠️ Tools & Technologies

•⁠  ⁠VirusTotal
•⁠  ⁠GitHub
•⁠  ⁠Email Header Analysis
•⁠  ⁠OSINT
•⁠  ⁠Threat Intelligence
•⁠  ⁠SPF / DKIM / DMARC

## 🔍 Investigation Workflow

1.⁠ ⁠Review the suspicious email
2.⁠ ⁠Analyze the sender and Reply-To addresses
3.⁠ ⁠Examine email headers
4.⁠ ⁠Review SPF, DKIM, and DMARC authentication
5.⁠ ⁠Extract domains, URLs, and IP addresses
6.⁠ ⁠Investigate IOCs using threat intelligence
7.⁠ ⁠Determine the email verdict and severity
8.⁠ ⁠Recommend containment and remediation actions
9.⁠ ⁠Document the investigation

## 🚨 Case Study — SIM-001

*Alert Type:* Phishing Email  
*Verdict:* Phishing  
*Severity:* High

### Key Findings

•⁠  ⁠Microsoft impersonation was observed
•⁠  ⁠A lookalike domain was used
•⁠  ⁠SPF authentication failed
•⁠  ⁠Sender infrastructure contained inconsistencies
•⁠  ⁠The originating IP address was investigated using VirusTotal
•⁠  ⁠16/91 security vendors flagged the investigated IP as malicious

### Analyst Conclusion

The email was assessed as a phishing attempt based on multiple indicators, including brand impersonation, email authentication failure, suspicious sender infrastructure, and malicious IP reputation.

### Recommended Actions

•⁠  ⁠Quarantine the phishing email
•⁠  ⁠Block identified malicious indicators
•⁠  ⁠Search other mailboxes for similar messages
•⁠  ⁠Determine whether the recipient clicked the phishing link
•⁠  ⁠Reset credentials if credential exposure is suspected
•⁠  ⁠Review authentication logs for suspicious sign-ins
•⁠  ⁠Continue monitoring for related activity

## 🧠 Skills Demonstrated

•⁠  ⁠Phishing Analysis
•⁠  ⁠SOC Alert Triage
•⁠  ⁠IOC Analysis
•⁠  ⁠Threat Intelligence
•⁠  ⁠Email Security
•⁠  ⁠Incident Response
•⁠  ⁠Security Documentation
•⁠  ⁠Analytical Thinking

## ⚠️ Disclaimer

This project was completed for educational and defensive cybersecurity purposes. Simulated samples are used where appropriate, and suspicious links are not intentionally accessed directly.
