 Windows 10 Security Hardening & Audit

**Submitted by:** Innocentia Mbalenhle Jiwa  

**Course:** IT Security – Defense Against the Digital Dark Arts  

**Submission Date:** 13 February 2026

---

##Project Overview
This repository documents a manual security audit and system hardening exercise. The project focuses on evaluating a Windows 10 workstation’s defensive posture across three critical domains: **Authentication**, **Network Security (Firewalls)**, and **Patch Management**.

## Security Audit Checklist & Findings

### 1. Identity & Access Management (IAM)
* **Objective:** Enforce credential integrity and local security.
* **Action:** Implemented a new password policy including mandatory hint requirements.
* **Security Outcome:** Mitigates the risk of unauthorized local access and ensures account recovery protocols are established.

<img width="1137" height="746" alt="image" src="https://github.com/user-attachments/assets/305050bc-2fd2-4a55-a237-62e0bd9c2325" />


### 2. Network Perimeter Defense
* **Objective:** Minimize the attack surface via the Windows Defender Firewall.
* **Action:** Verified firewall status for **Domain**, **Private**, and **Public** networks. 
* **Observation:** Confirmed active protection on the private network profile (`CAPACITI Candidates 2.4GHz`).
* **Configuration:** The firewall is set to "Block all connections" for apps not explicitly whitelisted, adhering to the **Principle of Least Privilege**.

<img width="1591" height="851" alt="image" src="https://github.com/user-attachments/assets/7890b9f8-1211-498e-9bf0-9a12bfa4d373" />

<img width="890" height="494" alt="image" src="https://github.com/user-attachments/assets/714305be-5316-4a16-8363-06b0e5835673" />


### 3. Vulnerability Assessment & Patch Management
* **Observation:** System audit revealed the OS has reached **End of Support**.
* **Risk Factor:**  **CRITICAL**. The system is no longer receiving security intelligence updates or quality fixes from the vendor.
* **Improvement Suggestion:** For a secure posture, immediate migration to a supported OS (Windows 11) is required to defend against modern exploits and zero-day vulnerabilities.

<img width="1363" height="793" alt="image" src="https://github.com/user-attachments/assets/38cfe8bb-b6d5-4e1a-8a9b-f9985b52c81e" />


---

## 🛠️ Technical Summary
| Category | Component | Status |
| :--- | :--- | :--- |
| **Authentication** | Password/Hint Creation | ✅ Configured |
| **Network Security** | Windows Defender Firewall | ✅ Active |
| **System Health** | Update & Security Status | ⚠️ End-of-Life |

##  Conclusion
While local authentication and firewall policies are correctly configured, the **End-of-Life (EOL)** status of the operating system remains a significant security gap. This audit highlights that robust firewall rules cannot fully protect an unpatched OS from modern digital threats.

---

### About the Author
**Innocentia Mbalenhle Jiwa** *Technical Support Specialist & Aspiring AI/ML Engineer*
