# SOC Threat Intelligence Assessment

**Lab:** The Report | Blue Team Labs Online (BTLO)  
**Category:** Threat Intelligence & Security Operations  
**Difficulty:** Easy  
**Status:** Completed

## Investigation Overview

As a SOC analyst in a newly established Security Operations Center, I was tasked with reviewing a 2022 cybersecurity threat intelligence report.

The objective was to identify significant cyber threats, analyze attacker techniques, examine vulnerabilities, and recommend defensive security measures to strengthen SOC operations.

## Investigation Methodology

I analyzed a cybersecurity threat intelligence report published in 2022 to identify threats relevant to a newly established Security Operations Center (SOC).

My investigation focused on:

- Identifying major cybersecurity threats and attack campaigns.
- Researching vulnerabilities affecting enterprise systems.
- Examining attacker tactics, techniques, and procedures (TTPs).
- Mapping malicious activity to the MITRE ATT&CK framework.
- Evaluating ransomware and initial access techniques.
- Identifying opportunities to improve SOC detection and prevention.

## Tools and Frameworks

- MITRE ATT&CK Framework
- CVE and vulnerability research
- Threat intelligence analysis
- Security detection and monitoring concepts
- Blue Team Labs Online (BTLO)

- ## Key Investigation Findings

### 1. Log4Shell Vulnerability

Identified Log4Shell, a critical vulnerability affecting the Apache Log4j Java logging library.

- CVE: CVE-2021-44228
- Impact: Remote code execution (RCE)
- Risk: Attackers could potentially compromise vulnerable systems.
- SOC Priority: Identify vulnerable assets, monitor exploitation attempts, and prioritize remediation.

### 2. Microsoft Exchange Vulnerabilities

Examined security threats involving Microsoft Exchange Server vulnerabilities.

Potential consequences included:

- Unauthorized access to email infrastructure.
- Remote code execution.
- Credential theft.
- Compromise of sensitive organizational information.

### 3. Ransomware Threats

Analyzed ransomware activity, including the use of affiliate-based operations and initial access techniques.

Key risks included:

- Encryption of critical business data.
- Operational disruption.
- Financial losses.
- Data theft and extortion.

### 4. Malicious JavaScript Execution

Investigated detection concepts involving malicious JavaScript files.

SOC analysts should monitor suspicious process execution, unusual parent-child process relationships, and potentially malicious scripts.

### 5. Cryptojacking

Reviewed threats involving unauthorized cryptocurrency mining.

Attackers may exploit outdated software to install cryptocurrency miners, consuming system resources and potentially indicating a broader compromise.
## Defensive Security Recommendations

Based on the threats examined during this investigation, I would recommend the following security improvements for a newly established SOC.

### 1. Vulnerability Management
- Maintain an accurate inventory of organizational assets.
- Prioritize patching critical vulnerabilities, including Log4Shell.
- Monitor CISA's Known Exploited Vulnerabilities (KEV) Catalog.
- Conduct regular vulnerability scans.

### 2. Endpoint Detection and Response
- Deploy endpoint detection and response (EDR) solutions.
- Monitor suspicious process execution and parent-child relationships.
- Investigate unexpected JavaScript execution.
- Alert on unusual PowerShell activity.

### 3. Ransomware Prevention
- Maintain offline or immutable backups.
- Implement multifactor authentication (MFA).
- Apply least-privilege access controls.
- Segment critical networks.
- Monitor for suspicious file encryption activity.

### 4. Remote Access Security
- Restrict unnecessary Remote Desktop Protocol (RDP) access.
- Require MFA for remote connections.
- Monitor unusual authentication attempts.
- Investigate repeated failed login attempts.

### 5. Threat Intelligence Integration
- Use the MITRE ATT&CK framework to map attacker behaviors.
- Incorporate relevant threat intelligence into SOC monitoring.
- Review detection rules against emerging threats.
- Document findings and escalate significant risks.

## SOC Analyst Takeaways

This investigation strengthened my understanding of how threat intelligence supports security operations.

I practiced connecting vulnerability information, attacker techniques, and threat trends to practical defensive recommendations.

The exercise also reinforced the importance of translating technical intelligence into actionable information that helps organizations prioritize security risks.
---

## Conclusion

The BTLO "The Report" challenge provided practical experience analyzing cybersecurity threat intelligence and translating technical findings into actionable security recommendations.

Through this investigation, I examined critical vulnerabilities, ransomware threats, attacker techniques, and defensive security strategies.

The exercise strengthened my ability to:

- Interpret cybersecurity threat intelligence reports.
- Identify vulnerabilities and potential organizational risks.
- Understand attacker tactics using MITRE ATT&CK.
- Recommend appropriate security controls.
- Communicate technical findings in a structured format.

These skills support my continued development toward a SOC Analyst or Threat Intelligence Analyst role.

---

**Analyst:** Melanie Aljabari  
**Platform:** Blue Team Labs Online  
**Challenge:** The Report  
**Status:** Completed

*This report documents an authorized cybersecurity training exercise. The recommendations are based on the threats examined during the challenge.*
