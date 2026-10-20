# 🛡️ Phishing Analysis | SOC Investigation Report

**Platform:** Blue Team Labs Online (BTLO)  
**Challenge:** Phishing Analysis  
**Category:** Security Operations  
**Difficulty:** Easy  
**Status:** Completed

---

## 1. Executive Summary

This investigation involved analyzing a suspicious email forwarded to a Security Operations Center (SOC).

The objective was to examine the email, investigate its origin, identify suspicious attachments and URLs, and collect information useful for a potential security incident.

The challenge simulated a common SOC Tier 1 responsibility: investigating a reported phishing email and documenting relevant evidence.

---

## 2. Investigation Objectives

The investigation focused on:

- Identifying the email recipient and subject
- Examining email timestamps and headers
- Determining the originating IP address
- Performing reverse DNS analysis
- Identifying the email attachment
- Extracting a URL embedded within the attachment
- Investigating the website hosting service
- Examining webpage content using URL2PNG

---

## 3. Investigation Methodology

### Email Header Analysis

Examined the email's identifying information, including its recipient, subject, timestamp, and originating IP address.

These details help analysts understand where a suspicious message originated and establish an investigation timeline.

### IP Address Investigation

Investigated the originating IP address and performed a reverse DNS lookup to identify its associated hostname.

Reverse DNS information can provide additional context when evaluating suspicious email infrastructure.

### Attachment Analysis

Examined the email attachment to identify embedded URLs.

Extracting URLs from attachments allows analysts to investigate potential phishing destinations without directly interacting with suspicious links.

### Website Investigation

Investigated the extracted URL to identify the service hosting the webpage.

Used URL2PNG to examine the webpage's displayed content.

This approach supports safer preliminary analysis of potentially malicious websites.

---

## 4. Tools and Techniques

| Tool / Technique | Purpose |
|---|---|
| Email Header Analysis | Identify message metadata and originating IP |
| Reverse DNS Lookup | Investigate the hostname associated with an IP |
| DomainTools | Support IP and hostname research |
| Attachment Inspection | Identify suspicious content and embedded URLs |
| URL Analysis | Investigate potential phishing destinations |
| URL2PNG | Examine webpage appearance |

---

## 5. Investigation Results

Successfully completed all nine investigation questions.

The investigation covered:

1. Primary email recipient
2. Email subject
3. Date and time sent
4. Originating IP address
5. Reverse DNS hostname
6. Attachment filename
7. URL embedded in the attachment
8. Website hosting service
9. Webpage heading identified through URL2PNG

**Result:** All investigation questions solved.

---

## 6. SOC Analyst Skills Demonstrated

- Phishing email triage
- Email metadata analysis
- IP address investigation
- Reverse DNS analysis
- Suspicious attachment inspection
- URL extraction and investigation
- Webpage analysis
- Technical documentation

---

## 7. Lessons Learned

This challenge reinforced the importance of investigating suspicious emails systematically.

Email headers, IP addresses, attachments, and embedded URLs can provide valuable information during phishing investigations.

It also demonstrated how security analysts can use multiple investigative techniques to collect evidence before determining appropriate response actions.

---

## 8. Conclusion

Successfully completed the BTLO Phishing Analysis challenge.

This investigation provided practical experience with phishing email analysis, attachment examination, IP investigation, and suspicious URL research.

The techniques practiced are directly applicable to entry-level SOC analyst and cybersecurity incident response responsibilities.

---

**Investigation completed as part of my hands-on cybersecurity training and professional portfolio development.**
