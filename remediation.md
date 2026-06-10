# REMEDIATION

To mitigate the identified vulnerabilities and strengthen the security of the Active Directory environment, the following recommendations are proposed:

## 1. Enforce Strong Password Policies

Implement complex password requirements including minimum length, special characters, and regular password changes to prevent weak credential usage.

## 2. Enable Account Lockout Policy

Configure account lockout thresholds to prevent unlimited login attempts, reducing the effectiveness of password spraying attacks.

## 3. Secure Service Accounts

Avoid using regular user accounts as service accounts. Implement Managed Service Accounts (gMSA) to automatically manage strong passwords and reduce Kerberoasting risks.

## 4. Monitor Kerberos Activity

Enable logging and monitoring of Kerberos ticket requests to detect unusual patterns that may indicate Kerberoasting attempts.

## 5. Apply Least Privilege Principle

Ensure that service accounts and users have only the minimum privileges required for their tasks to prevent privilege escalation.

## 6. Implement Security Monitoring

Deploy SIEM solutions to monitor authentication events, detect anomalies, and respond to suspicious activities in real time.

