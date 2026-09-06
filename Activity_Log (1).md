# Penetration Testing & Vulnerability Assessment Activity Log

**Date:** September 6, 2026  
**Target Environments:** DVWA (Damn Vulnerable Web Application), Mutillidae  
**Tools Used:** OWASP ZAP (Zed Attack Proxy), Web Browser  

---

## Chronological Activity Timeline

| Time (WAT) | Activity ID | Target / Focus Area | Description / Action Taken | Associated Evidence |
| :--- | :--- | :--- | :--- | :--- |
| **09:43 AM** | ACT-001 | OWASP ZAP Setup | Configured ZAP Protected Mode to restrict active scanning outside designated scope. | `E-01-ZAP-Protected-Mode.png` |
| **09:43 AM** | ACT-002 | OWASP ZAP Setup | Defined target contexts, inclusion/exclusion rules, and operational scope within ZAP. | `E-02-ZAP-Context&Scope.png` |
| **10:04 AM** | ACT-003 | Mutillidae | Performed initial application mapping and manual crawling to map Mutillidae site tree. | `E-04-Mutillidae-Site-Tree.png` |
| **10:05 AM** | ACT-004 | DVWA | Explored and mapped target endpoints to populate the DVWA site tree in ZAP. | `E-03-DVWA-Site-Tree.png` |
| **10:06 AM** | ACT-005 | ZAP Scanner | Reviewed passive scanning alerts and preliminary HTTP header configurations. | `E-05-ZAP-Passive-Alerts.png` |
| **10:34 AM** | ACT-006 | Testing Environment | Verified and documented the baseline testing environment, proxy rules, and setup. | `E-06-Baseline-Environment.png` |
| **11:08 AM** | ACT-007 | Broad Assessment | Executed overall automated scan across mapped target applications. | `E-07-Overal-ZAP-AutoScan.png` |
| **11:27 AM** | ACT-008 | DVWA | Ran targeted reduced active scan on specific DVWA modules to identify key vulnerabilities. | `E-08-DVWA-Reduced-Active-Scan.png` |
| **11:40 AM** | ACT-009 | Mutillidae | Executed reduced active scan policy against targeted Mutillidae endpoints. | `E-09-Mutillidae-Reduced-Active-Scan.png` |
| **01:03 PM** | ACT-010 | Mutillidae | Conducted manual testing for Path Traversal / Local File Inclusion (LFI). Initial proof capture. | `E-11-Mutillidae-Path-Tranversal-Proof.png` |
| **01:04 PM** | ACT-011 | Mutillidae | Validated Path Traversal vulnerability with refined payload and supplementary screenshot. | `E-11b-Mutillidae-Path-Tranversal-Proof.png` |
| **01:47 PM** | ACT-012 | DVWA | Tested HTTP security headers; verified missing or misconfigured `X-Content-Type-Options`. | `E-10-DVWA-X-Content-Type-Proof.png` |
| **02:14 PM** | ACT-013 | Mutillidae | Tested for Reflected/Stored Cross-Site Scripting (XSS) and captured successful execution. | `E-12-Mutillidae-Cross-Site-Scripting-Proof.png` |
| **03:42 PM** | ACT-014 | DVWA | Assessed Anti-Clickjacking protections; verified missing `X-Frame-Options` / CSP directives. | `E-13-DVWA-Anti-Clickjacking-Proof.png` |

---
