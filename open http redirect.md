
# Open HTTP Redirect Lab

## Description

This project demonstrates an **Open HTTP Redirect** vulnerability in a controlled DVWA lab environment. The objective is to understand how unvalidated user input can redirect users to unintended external websites.

## Objectives

* Identify an Open Redirect vulnerability.
* Understand the security impact of unvalidated redirects.
* Verify the vulnerability using a proof of concept.
* Learn secure mitigation techniques.

## Environment

* DVWA (Damn Vulnerable Web Application)
* Local Lab Environment
* Kali Linux
* Web Browser

## Vulnerability

The application accepts a user-controlled URL parameter without proper validation, allowing an attacker to redirect users to arbitrary external websites.

## Proof of Concept

1. Locate the redirect functionality.
2. Modify the redirect URL parameter.
3. Redirect the browser to an external domain.
4. Confirm the application performs the redirect.

## Security Impact

* Phishing attacks
* User trust abuse
* Credential theft through malicious websites
* Social engineering campaigns

## Mitigation

* Use an allowlist of trusted domains.
* Validate redirect destinations.
* Avoid accepting arbitrary URLs from user input.
* Display confirmation before redirecting to external websites.

###   LAB NAME   ###   

<img width="939" height="403" alt="1" src="https://github.com/user-attachments/assets/70b24e6b-3824-45fc-8167-0198b271550c" />
###  BURP SUITE DEMONSTARTION ON LAB ###
<img width="855" height="459" alt="2" src="https://github.com/user-attachments/assets/237b343a-2e5a-447a-adca-c2f6b1046340" />
<img width="883" height="278" alt="3" src="https://github.com/user-attachments/assets/2fecaf6a-1b78-45f4-84cc-ebaeff3f0176" />
<img width="734" height="292" alt="4" src="https://github.com/user-attachments/assets/ce617c67-4748-457b-83ee-416eeb5f733f" />
