# Phishing Email Investigation
## BTLO Phishing Analysis 2

**Analyst:** Melanie Aljabari  
**Platform:** Blue Team Labs Online  
**Category:** Security Operations  
**Status:** Completed  
**Investigation Type:** Phishing Email Analysis

---

## 1. Executive Summary

This investigation involved analyzing a suspicious email impersonating Amazon and attempting to convince the recipient that their account had been locked.

The objective was to examine the email's structure, identify suspicious indicators, investigate embedded URLs, and determine the potential security risks associated with the message.

The investigation identified indicators consistent with a credential-phishing attempt, including brand impersonation, a suspicious sender domain, and an account-verification link directing the recipient to an unrelated domain.

**Assessment:** Suspected credential phishing.

---

## 2. Investigation Objectives

- Examine email headers and metadata.
- Identify potential sender impersonation.
- Analyze suspicious URLs and redirects.
- Decode encoded email content.
- Examine HTML structure and external resources.
- Identify potential indicators of compromise.
- Recommend appropriate defensive actions.

---

## 3. Tools and Technologies

| Tool | Purpose |
|------|---------|
| Text Editor | Examine raw email headers and MIME structure |
| CyberChef | Decode Base64-encoded email content |
| VirusTotal | Review URL reputation and security detections |
| URLScan.io | Investigate URL history and available scan information |
| URL2PNG | Attempt to preview the suspicious destination |
| HTML Analysis | Identify embedded links and external resources |

---

## 4. Investigation Methodology

### Step 1: Email Header Analysis

Opened the supplied `.eml` file in a text editor to examine the raw email headers.

Reviewed:

- Sender and recipient information
- Subject line
- Date and time
- Email routing information
- MIME structure
- Content-transfer encoding

The message claimed to originate from Amazon, but the sender's domain was unrelated to the legitimate company.

This discrepancy was a significant phishing indicator.

### Step 2: Email Encoding Analysis

Identified the following MIME header:

`Content-Transfer-Encoding: base64`

The email body contained encoded content that was not immediately readable in the text editor.

Used CyberChef's **From Base64** operation to decode the content into readable HTML.

This allowed further examination of the email's structure and embedded links.

### Step 3: HTML and URL Analysis

Inspected the decoded HTML to identify:

- The primary call-to-action link
- External image resources
- Embedded third-party URLs
- Suspicious destination domains

The email contained a Microsoft Safe Links-wrapped URL.

Further inspection revealed that the underlying destination was unrelated to Amazon.

This demonstrated why analysts should examine the actual destination of embedded links rather than relying solely on their visible appearance.

### Step 4: URL Reputation Investigation

Reviewed the suspicious destination using VirusTotal and URLScan.io.

VirusTotal did not show widespread malicious detections at the time of analysis.

However, the absence of detections does not establish that a URL is safe.

URLScan.io was used to investigate available historical information without submitting a new public scan containing recipient-specific information.

### Step 5: Website Preview

Attempted to examine the destination using URL2PNG.

The destination did not render successfully.

Because the website could not be loaded, its current content and functionality could not be independently verified.

The email's suspicious characteristics nevertheless supported a phishing assessment.

---

## 5. Key Findings

### Finding 1: Brand Impersonation

The email used Amazon branding and account-security language to create a sense of urgency.

### Finding 2: Suspicious Sender Domain

The sender address used a domain unrelated to Amazon.

This was inconsistent with the claimed sender identity.

### Finding 3: Suspicious Account Verification Link

The primary call-to-action directed the recipient toward an unrelated domain.

The link included recipient-specific information in its URL parameters.

### Finding 4: Encoded HTML Content

The message used Base64 content-transfer encoding.

Although Base64 is common in legitimate email, decoding was necessary to inspect the message's underlying HTML.

### Finding 5: External Resources

The HTML referenced externally hosted images and third-party URLs.

These resources were identified by examining HTML attributes, including image source references.

---

## 6. Security Risk Assessment

**Threat Type:** Suspected Credential Phishing

**Potential Impact:**

- Credential theft
- Unauthorized account access
- Exposure of personal information
- Further phishing or account takeover attempts

**Confidence:** Moderate to High

The assessment is based on email impersonation indicators and suspicious link destinations. Credential collection was not directly confirmed because the destination website could not be loaded.

---

## 7. Recommended SOC Response

1. Preserve the original email as evidence.
2. Extract and document relevant indicators.
3. Check email security logs for similar messages.
4. Search for additional recipients within the organization.
5. Block confirmed malicious domains and URLs according to organizational policy.
6. Determine whether recipients clicked the suspicious link.
7. Investigate potential credential exposure if interaction occurred.
8. Educate affected users about phishing indicators.
9. Document findings and escalate when appropriate.

---

## 8. Lessons Learned

This investigation strengthened my understanding of:

- Email header analysis
- MIME structure and content encoding
- Base64 decoding with CyberChef
- HTML source inspection
- URL analysis and redirect identification
- Threat intelligence enrichment
- Phishing indicators and credential-theft risks
- Evidence-based security assessments

A key takeaway was that a URL receiving few or no malicious detections should not automatically be considered safe.

Multiple indicators must be evaluated together before reaching a conclusion.

---

## 9. Conclusion

The investigation identified several indicators consistent with a phishing attempt targeting account credentials.

Although the destination website was unavailable during analysis, the suspicious sender domain, brand impersonation, and unrelated account-verification destination supported the assessment.

This exercise provided practical experience in email investigation, threat analysis, and documenting security findings using a structured SOC workflow.

---

**Analyst:** Melanie Aljabari  
**Portfolio:** Blue Team Security Investigations

*This report documents investigative methodology and findings from an authorized cybersecurity training exercise. Challenge answer keys and recipient-specific information have been intentionally excluded.*
