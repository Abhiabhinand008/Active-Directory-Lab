# FINDINGS

The assessment identified multiple critical security weaknesses within the Active Directory environment that allowed an attacker to progress from initial access to full domain compromise.

## 1. Weak Password Policy

Users were configured with weak and easily guessable passwords such as "Password123" and "SQL123". This enabled successful password spraying attacks, allowing unauthorized access to valid user accounts.

**Severity:** High\
**Impact:** Initial access gained

## 2. Absence of Account Lockout Policy

The domain lacked an account lockout mechanism, allowing unlimited login attempts. This made password spraying attacks highly effective without triggering any defensive response.

**Severity:** High\
**Impact:** Increased attack success rate

## 3. Kerberoasting Vulnerability

The svc\_sql service account was configured with a Service Principal Name (SPN), making it vulnerable to Kerberoasting. An attacker was able to request a Kerberos ticket and extract a crackable hash.

**Severity:** Critical\
**Impact:** Credential exposure

## 4. Weak Service Account Credentials

The service account (svc\_sql) used a weak password, allowing the attacker to successfully authenticate after extracting the Kerberos hash.

**Severity:** Critical\
**Impact:** Privilege escalation

## 5. Excessive Privileges

The svc\_sql account had elevated privileges within the domain, allowing the attacker to perform administrative actions and access sensitive resources.

**Severity:** Critical\
**Impact:** Full domain compromise

## 6. Lack of Monitoring and Detection

No logging or monitoring mechanisms were in place to detect suspicious activities such as password spraying or Kerberos ticket requests.

**Severity:** High\
**Impact:** Attack remained undetected



