# phishing_incident_investigation_lab
simulated SOC investigation of a phishing email incident, documenting validation, and response steps

## Scenario
A user reported clicking a suspicious link in an email. This lab simulates the investigation process a SOC analyst would follow to determine whether the incident posed a security risk

## Objectives
- Validate whether the email was malicious
- Determine potential system impact
- Identify inducators of compromise
- Document response actions

## Investigation Steps
1. Reviewed the reported email for phisihing indicators
2. Analyzed the embedded URL using an online reputation service
3. checked system logs for unusual activity following the click
4. reviewed DNS and proxy logs for connections to suspicious domains

## Findings 
- The URL redirected to a known malicious domain
- No evidence of malware execution was observed
- No additional outbound connections detected

## Screenshot Evidence - Phishing Incident
![Phisihing Email Screensot](phising-email-screenshot.png)

Observations:
- Email found in Gmail spam folder
- Suspicious URL clearly visable and highlighted
- obvious phishing characteristics (sender mismatch, typos, urgent request)

## Response Actions
- User workstation isolated as a precaution
- Malicious domain blocked at network level
- User advised to reset credentails
- Incident documented for future reference

## Lessons Learned
- Early reporting by users reduces risk
- URL analysis is critical for phishing investigations
- Containment actions sholud be taken even when imapct is uncertain
