# Risk Register

---

## 📘 Overview

A risk register helps analysts track and prioritise risks by evaluating:

- **Asset** – what needs protection  
- **Threat** – what could cause harm  
- **Vulnerability** – why the threat is possible  
- **Likelihood** – probability of exploitation  
- **Impact** – severity of damage  
- **Risk Score** – likelihood × impact  
- **Recommended Controls** – mitigation steps

---

## 📊 Example Risk Register

| Asset | Threat | Vulnerability | Likelihood (1–3) | Impact (1–3) | Risk Score | Recommended Controls |
|-------|---------|----------------|------------------|--------------|-------------|------------------------|
| Customer Database | External attacker exfiltrates PII | Weak access controls, excessive permissions | 3 | 3 | 9 | MFA, least privilege, encrypt data at rest + in transit |
| HR System | Insider modifies payroll entries | No separation of duties | 2 | 3 | 6 | RBAC, audit logs, approval workflows |
| File Server | Ransomware encrypts files | Phishing exposure, outdated endpoint protection | 2 | 3 | 6 | EDR, security awareness training, strong email filtering |
| Marketing Website | DDoS attack | No rate limiting | 1 | 2 | 2 | WAF, traffic throttling |

---

## 🎯 Reflection

- Risks become critical when **high likelihood** meets **high impact**  
- Many issues stem from **access mismanagement**  
- Controls must be *targeted*—not every system needs maximum lockdown  
- The register forms the foundation of incident planning and mitigation

