# Phishing Analysis Report — sim_001

## Overview
| Field | Details |
|---|---|
| Sample ID | sim_001 |
| Type | Simulated |
| Date Analyzed | 2026-03-14 |
| Verdict | Phishing |
| Severity | High |

## Email Header Analysis
| Field | Value |
|---|---|
| From | security-alert@micros0ft-verify.com |
| Reply-To | noreply@micros0ft-verify.com |
| Return-Path | bounce@malicious-relay.ru |
| SPF | Fail |
| DKIM | Not Present |
| DMARC | Not Found |
| Originating IP | 185.220.101.45 |
| Mail Server | malicious-relay.ru |

## Sender Analysis
- `micros0ft-verify.com` is a typosquat — letter O replaced with zero (0)
- Real Microsoft domain is `microsoft.com`
- Return-Path uses `.ru` Russian domain — mismatch with sender

## IOC Analysis

### Domain Investigation

*Domain:* micros0ft-verify.com

*VirusTotal Result:* 0/91 security vendors flagged the domain as malicious.

*Analysis:*  
Although VirusTotal did not detect the domain as malicious, the domain is suspicious because it impersonates Microsoft by replacing the letter "o" with the number "0". The email also contains authentication and sender inconsistencies.

*Verdict:* Suspicious / Potential phishing domain

### IP Address Investigation

*IP Address:* 185.220.101.45

*VirusTotal Result:* 16/91 security vendors flagged the IP address as malicious.

*Analysis:*  
The originating IP address has a negative reputation on VirusTotal. Multiple security vendors classify the IP as malicious, phishing, or malware-related. This provides additional evidence that the email may have originated from suspicious infrastructure.

*Verdict:* Malicious / High-risk IP address

## Final Assessment

*Verdict:* Phishing  
*Severity:* High

The email was determined to be a phishing attempt impersonating Microsoft. The sender used a lookalike domain, the email failed SPF authentication, and the Return-Path did not match the sender domain. The originating IP address was also flagged as malicious by 16/91 security vendors on VirusTotal.

## Recommended Actions

•⁠  ⁠Block the suspicious sender domain.
•⁠  ⁠Block the malicious IP address.
•⁠  ⁠Quarantine and remove the phishing email from affected mailboxes.
•⁠  ⁠Check whether the recipient clicked the link or entered credentials.
•⁠  ⁠Reset the user's password if credentials may have been exposed.
•⁠  ⁠Review authentication logs for suspicious sign-in activity.
•⁠  ⁠Monitor for similar phishing emails targeting other users.
