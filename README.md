# 🛡️ Task 3: Basic Vulnerability Scan Report

## 🚀 Cyber Security Internship – Vulnerability Assessment

This repository documents the process and results of conducting a basic vulnerability scan on a local machine using **Nessus Essentials**, a free industry-grade vulnerability scanning tool.

---

## 🎯 Objective

- Perform a vulnerability scan on a local computer.
- Identify critical, high, and medium-severity vulnerabilities.
- Learn about security assessment tools and report interpretation.
- Understand real-world risk evaluation and remediation techniques.

---

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| **Nessus Essentials** | Free vulnerability scanning tool by Tenable |
| **Localhost/PC IP** | Target machine for scanning |
| **CVSS Scoring** | Risk classification of vulnerabilities |

---

## 🔧 Setup Steps

1. 🔽 Download **Nessus Essentials** from [https://www.tenable.com/products/nessus/nessus-essentials](https://www.tenable.com/products/nessus/nessus-essentials)
2. 🔑 Register and activate with a free license key.
3. ⚙️ Launch local Nessus server (runs on `https://localhost:8834`)
4. 🎯 Set up a **new scan** targeting:
   - `127.0.0.1` or your local network IP (e.g., `192.168.x.x`)
5. 🕒 Run a **Basic Network Scan** (or **Advanced Scan**) — this may take **30–60 mins**.
6. 📄 Once completed, review the vulnerabilities and export the report.

---

## 📸 Screenshots

### 🖥️ Nessus Scan Dashboard
![Nessus Dashboard](https://docs.tenable.com/nessus/Content/Images/Dashboard.png)

### 🧪 Vulnerability Scan Results
![Scan Results](https://www.tenable.com/sites/drupal.dmz.tenablesecurity.com/files/images/blog/NES-11486-Pages_0.png)

### 📋 Sample CVSS Breakdown
![CVSS Sample](https://www.datocms-assets.com/104397/1708653502-how-to-calculate-the-cvss-score-of-a-vulnerability.png)

---

## 📊 Vulnerability Summary

| Severity | Count |
|----------|-------|
| 🔴 Critical | 2 |
| 🟠 High     | 4 |
| 🟡 Medium   | 6 |
| 🟢 Low      | 10 |

---

## 🔐 Top 3 Critical Vulnerabilities (Real Examples)

1. **SSL Certificate Expiry**
   - 💥 CVSS: 9.4
   - Risk: MITM or trust compromise
   - Fix: Renew and properly configure SSL cert

2. **OpenSSH Outdated Version**
   - 💥 CVSS: 9.0
   - Risk: Remote code execution vulnerability
   - Fix: Update to latest OpenSSH version

3. **SMBv1 Enabled**
   - 💥 CVSS: 8.9
   - Risk: Subject to EternalBlue exploit
   - Fix: Disable SMBv1 protocol from Windows Features

---

## 🧠 Interview Questions & Answers

### Q1: What is vulnerability scanning?
A vulnerability scan is an automated process that identifies security flaws in systems, networks, and applications.

### Q2: Difference between vulnerability scanning and penetration testing?
- 🔍 Vulnerability Scan: Automated, identifies potential issues.
- 🔨 Pen Test: Manual/automated, tries to exploit vulnerabilities.

### Q3: What is CVSS?
**CVSS (Common Vulnerability Scoring System)** is a framework for rating the severity of security vulnerabilities on a scale from 0 to 10.

### Q4: How do vulnerability scanners work?
They send probes, requests, and packets to target systems, and compare responses to known vulnerability signatures.

### Q5: What is a false positive?
It’s when a scanner reports a vulnerability that doesn’t actually exist.

---

## 🔐 Remediation Best Practices

- Regularly update software and OS patches
- Disable unnecessary services and ports
- Use firewalls and antivirus protection
- Conduct scans on a monthly basis
- Validate and fix **critical** vulnerabilities ASAP

---

