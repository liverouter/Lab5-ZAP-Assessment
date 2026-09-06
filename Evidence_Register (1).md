# Cyber Security Assessment Evidence Register

**Project / Scope:** Web Application Penetration Test (DVWA & Mutillidae)  
**Date captured:** September 6, 2026  
**Total Evidence Artifacts:** 14  

---

## Master Evidence Inventory

| Evidence ID | File Name | Timestamp | Target App | Category / Vulnerability | Description / Context |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **E-01** | `E-01-ZAP-Protected-Mode.png` | 09:43 AM | Environment | Scope Control | Proof of OWASP ZAP configured in Protected Mode to prevent unauthorized scanning. |
| **E-02** | `E-02-ZAP-Context&Scope.png` | 09:43 AM | Environment | Target Scoping | Screenshot of defined scope contexts and target URL inclusion/exclusion rules. |
| **E-03** | `E-03-DVWA-Site-Tree.png` | 10:05 AM | DVWA | Reconnaissance | Site tree mapping showing discovered paths, directories, and endpoints on DVWA. |
| **E-04** | `E-04-Mutillidae-Site-Tree.png` | 10:04 AM | Mutillidae | Reconnaissance | Site tree structure and path enumeration results for OWASP Mutillidae. |
| **E-05** | `E-05-ZAP-Passive-Alerts.png` | 10:06 AM | Environment | Passive Analysis | Summary of passive scanner findings, missing flags, and informational alerts. |
| **E-06** | `E-06-Baseline-Environment.png` | 10:34 AM | Environment | Setup Verification | Screenshot documenting testing workstation setup, proxy routing, and tool states. |
| **E-07** | `E-07-Overal-ZAP-AutoScan.png` | 11:08 AM | Target Scope | Automated Scan | High-level overview and progress/results of the full-scope automated ZAP scan. |
| **E-08** | `E-08-DVWA-Reduced-Active-Scan.png` | 11:27 AM | DVWA | Active Scan | Results of scoped active scanning targeting DVWA endpoints. |
| **E-09** | `E-09-Mutillidae-Reduced-Active-Scan.png` | 11:40 AM | Mutillidae | Active Scan | Active scan progress and alert output specifically focused on Mutillidae paths. |
| **E-10** | `E-10-DVWA-X-Content-Type-Proof.png` | 01:47 PM | DVWA | Security Headers | Proof of missing/misconfigured `X-Content-Type-Options` response header in DVWA. |
| **E-11** | `E-11-Mutillidae-Path-Tranversal-Proof.png` | 01:03 PM | Mutillidae | Path Traversal | Primary screenshot demonstrating successful Path Traversal / Arbitrary File Read. |
| **E-11b** | `E-11b-Mutillidae-Path-Tranversal-Proof.png` | 01:04 PM | Mutillidae | Path Traversal | Secondary/extended proof payload execution for Path Traversal in Mutillidae. |
| **E-12** | `E-12-Mutillidae-Cross-Site-Scripting-Proof.png` | 02:14 PM | Mutillidae | Cross-Site Scripting (XSS) | Proof-of-concept execution showing successful script injection and execution in browser. |
| **E-13** | `E-13-DVWA-Anti-Clickjacking-Proof.png` | 03:42 PM | DVWA | Clickjacking | Demonstration of missing `X-Frame-Options` / `Content-Security-Policy` framing protections. |

---
