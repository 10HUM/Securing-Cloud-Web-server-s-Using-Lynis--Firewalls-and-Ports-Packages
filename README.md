# 🛡️ Cloud Security Implementation & Server Hardening Lab

## 📋 Project Overview
As a **Junior Cloud Security Engineer**, this project demonstrates the end-to-end process of securing an Ubuntu 22.04 server hosting a critical Apache web application. The implementation covers automated security auditing, host-based firewall configuration, vulnerability remediation, and a holistic cloud security framework encompassing IAM, compliance, incident response, and training.

---

## 🛠️ Tools & Technologies Used
* **Operating System:** Ubuntu 22.04 LTS (Docker Container)
* **Containerization:** Docker (`nwendlo1/c1w2m6`)
* **Security Auditing:** Lynis
* **Firewall & Network Security:** iptables, UFW
* **Web Services:** Apache HTTP Server
* **Frameworks & Principles:** Least Privilege (IAM), NIST/CIS Benchmarks, Incident Response Lifecycles

---

## 🚀 Key Tasks & Implementation Steps

### Task 1: Assess Current Security Posture
* Deployed and initialized the assessment container.
* Executed **Lynis** security auditing tools to scan the Ubuntu system, identify misconfigurations, outdated packages, and potential vulnerabilities.
* Analyzed the generated audit report to prioritize remediation steps.

### Task 2: Harden the Server
* Updated system packages (`apt update && apt upgrade`) to patch known vulnerabilities.
* Restricted incoming and outgoing network traffic using **iptables** rules.
* Removed unnecessary services and disabled insecure protocols to minimize the attack surface.

### Task 3: Develop a Cloud Security Strategy & IAM
* Applied the **Principle of Least Privilege (PoLP)**.
* Designed role-based access control policies for administrative and service accounts interacting with the cloud environment.

### Task 4: Deploy Security Tools and Technologies
* Configured host-based security mechanisms to continuously monitor system integrity and network traffic.
* Hardened Apache configurations to prevent information disclosure (e.g., hiding version numbers, disabling directory indexing).

### Task 5: Incident Response Plan (IRP)
* Developed a structured 4-phase incident response playbook: **Preparation, Detection & Analysis, Containment/Eradication/Recovery, and Post-Incident Activity**.
* Defined clear escalation pathways for suspected web server compromises or unauthorized access attempts.

### Task 6: Compliance and Governance
* Aligned server configurations with industry-recognized benchmarks (such as CIS Benchmarks and NIST CSF).
* Ensured data privacy and logging standards met organizational governance requirements.

### Task 7: Conduct Training & Awareness
* Outlined security awareness training modules for system administrators and development teams regarding secure coding, SSH key management, and common web attack vectors (OWASP Top 10).

### Task 8: Overall Reflection
* Synthesized technical hardening measures with strategic cloud governance objectives to evaluate overall risk posture improvements.

---

## 💻 Getting Started / Reproduction

To spin up the lab environment locally using Docker:

1. **Pull and run the assessment container:**
   ```bash
   docker run -it nwendlo1/c1w2m6 /bin/bash
