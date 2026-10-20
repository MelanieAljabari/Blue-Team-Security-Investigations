# MITRE ATT&CK Threat Intelligence Investigation

**Platform:** Blue Team Labs Online (BTLO)  
**Challenge:** ATT&CK  
**Category:** Incident Response / Threat Intelligence  
**Difficulty:** Easy  
**Status:** Completed

---

## 1. Executive Summary

This investigation focused on applying the MITRE ATT&CK framework to security scenarios involving cloud infrastructure, network traffic analysis, initial access, account protection, and credential-based attacks.

The objective was to identify relevant adversary behaviors, understand their potential impact, and determine appropriate defensive strategies.

The challenge consisted of five scenario-based questions, all successfully completed.

---

## 2. Investigation Objectives

- Apply the MITRE ATT&CK framework to realistic security scenarios.
- Identify techniques used by threat actors.
- Investigate unusual network activity.
- Understand initial access methods.
- Examine account protection and access restrictions.
- Explore detection opportunities for Pass-the-Hash attacks.

---

## 3. Investigation Findings

### Finding 1: Cloud Account Discovery

**Scenario:** An organization relies on Microsoft Azure Active Directory and Microsoft 365.

**Analysis:**

Investigated how attackers possessing valid credentials could perform discovery activities within cloud environments.

Evaluated the importance of monitoring identity-related activity and detecting unusual account enumeration behavior.

**Security relevance:**
- Cloud identity security
- Account discovery
- Credential misuse
- Identity monitoring

### Finding 2: Suspicious Network Traffic

**Scenario:** Unusual network traffic was identified on TCP port 4050.

**Analysis:**

Examined how network ports and communication patterns can help analysts identify potentially suspicious activity.

Considered how network indicators can be correlated with known adversary infrastructure and behaviors.

**Security relevance:**
- Network traffic analysis
- Threat actor research
- Command-and-control investigation
- Indicator correlation

**Analyst note:** A port number alone is insufficient to attribute activity to a specific threat actor.

### Finding 3: Initial Access Techniques

**Scenario:** Identify the MITRE ATT&CK tactic associated with techniques used to gain entry into a network.

**Analysis:**

Researched the Initial Access tactic and its relationship to common intrusion methods.

Studied how adversaries establish their first foothold within an organization's environment.

**Security relevance:**
- Initial Access
- Attack surface management
- Threat modeling
- Defensive security controls

### Finding 4: Account Protection and Restrictions

**Scenario:** Identify software that can restrict users from performing account-related activities.

**Analysis:**

Explored defensive technologies and policies designed to restrict unauthorized account modifications and protect access to organizational systems.

**Security relevance:**
- Access control
- Account protection
- Least privilege
- Security policy enforcement

### Finding 5: Pass-the-Hash Detection

**Scenario:** Determine how an organization could detect Pass-the-Hash activity.

**Analysis:**

Investigated how attackers may use stolen password hashes to authenticate to remote systems without knowing the original plaintext passwords.

Reviewed the importance of monitoring authentication activity, investigating unusual lateral movement, and correlating security events.

**Potential detection opportunities:**
- Unusual NTLM authentication activity
- Unexpected remote logins
- Suspicious administrative access
- Authentication patterns inconsistent with normal user behavior

---

## 4. Frameworks and Concepts Applied

- MITRE ATT&CK
- Threat intelligence analysis
- Network security monitoring
- Identity and access management
- Initial access detection
- Credential-based attack detection
- Incident response fundamentals

---

## 5. Recommended Defensive Measures

1. Monitor authentication and cloud identity activity.
2. Investigate unusual network connections and communication patterns.
3. Apply least-privilege access controls.
4. Use multifactor authentication where supported.
5. Centralize security logs for correlation and investigation.
6. Monitor for suspicious lateral movement and credential misuse.
7. Map relevant detections to MITRE ATT&CK techniques.

---

## 6. Skills Demonstrated

- MITRE ATT&CK framework navigation
- Threat intelligence research
- Adversary behavior analysis
- Network indicator investigation
- Cloud identity security awareness
- Credential attack detection concepts
- Security documentation

---

## 7. Investigation Outcome

**Result: Successfully completed all five BTLO ATT&CK challenge questions.**

This exercise strengthened my ability to connect security events with adversary tactics and techniques and evaluate potential detection and mitigation strategies.

The investigation demonstrates foundational skills relevant to Security Operations Center (SOC) analysis, threat intelligence, and incident response.

---

**Portfolio Project | Cybersecurity Analyst**
