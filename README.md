# OWASP ZAP Integrated Assessment, Remediation, and Retest Capstone

An end-to-end web application security assessment, manual vulnerability validation, remediation execution, and retest verification report using **OWASP ZAP** against isolated targets.

---

## 🎯 Project Overview

This capstone project evaluates the security posture of two target environments: **DVWA (Damn Vulnerable Web Application)** and **OWASP Mutillidae II**. The project covers the full assessment lifecycle—from scoped automated scanning and manual finding validation to security remediation and post-fix retesting.

* **Primary Tool:** OWASP ZAP (Zed Attack Proxy)
* **Environment:** Kali Linux / Isolated Virtual Machine

---

## 🔒 Scope & Rules of Engagement

* **In-Scope Targets:**
  * `DVWA` — `http://127.0.0.1:4280`
  * `OWASP Mutillidae II` — `http://127.0.0.1:8888`
* **Operational Mode:** OWASP ZAP configured strictly in **Protected Mode** within a defined target context.
* **Out-of-Scope:** Public endpoints, privilege escalation, lateral movement, credential dumping, or destructive actions.

---

## 📊 Summary of Findings

| Target Application | Vulnerability / Issue | Category | Severity | Remediation Status |
| :--- | :--- | :--- | :--- | :--- |
| **OWASP Mutillidae II** | Path Traversal / Local File Inclusion | Path Traversal | High | Remediation Recommended |
| **OWASP Mutillidae II** | Reflected Cross-Site Scripting (XSS) | Cross-Site Scripting | High | Remediation Recommended |
| **DVWA** | Missing Anti-Clickjacking Header | Security Misconfiguration | Medium | **Remediated & Verified** |
| **DVWA** | Missing `X-Content-Type-Options` Header | Security Misconfiguration | Medium | **Remediated & Verified** |

---

## 🛠️ Key Technical Highlights

### 1. Automated Discovery & Scoped Scanning
* **Site Tree Mapping:** Utilized ZAP Spider to discover endpoints across both targets while maintaining strict context boundaries.
* **Active Scanning:** Executed targeted active scan policies on specific endpoints (`login.php`) to minimize noise and application disruption.

### 2. Manual Finding Validation & PoC
* **Path Traversal:** Validated system file read access (`/etc/passwd`) via input manipulation on the `page` parameter in Mutillidae II.
* **Reflected XSS:** Confirmed client-side execution using DOM event handler payloads (`" onMouseOver="alert(1);`).
* **Security Headers:** Verified missing HTTP headers (`X-Frame-Options`, `X-Content-Type-Options`) using direct `curl` response inspection.

### 3. Remediation & Retesting
* Applied server-level configuration updates on Apache for DVWA to enforce `nosniff` and `SAMEORIGIN` header options.
* Conducted post-remediation verification testing to confirm the successful resolution of identified misconfigurations.

---

## 📁 Repository & Documentation Structure

* **`README.md`**: Executive summary and high-level assessment overview.
* **`Activity_Log.md`**: Complete chronological timeline of commands, scans, and manual checks.
* **`Evidence_Register.md`**: Central inventory mapping evidence artifacts and screenshots to specific test findings.
