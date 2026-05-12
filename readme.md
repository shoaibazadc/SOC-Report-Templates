# SOC Report Templates

Structured escalation templates for SOC L1 triage and TryHackMe investigation writeups, covering the most common alert categories. Built for consistent, repeatable documentation.

Templates are tool-agnostic and work alongside any SIEM, EDR, or ticketing platform.

---

## Templates Included

| # | Alert Type |
|---|---|
| 01 | Phishing |
| 02 | Malware / Endpoint Infection |
| 03 | Ransomware |
| 04 | Suspicious Login / Authentication Anomaly |
| 05 | Unauthorised Access / Brute Force |
| 06 | C2 / Beaconing |
| 07 | Suspicious Process Execution |
| 08 | Privilege Escalation |
| 09 | Lateral Movement |
| 10 | Data Exfiltration |
| 11 | Suspicious Network Traffic |
| 12 | Port Scanning |
| 13 | Vulnerability / Exploit Attempt |
| 14 | Denial of Service (DoS / DDoS) |
| 15 | Insider Threat |
| 16 | USB / Removable Media |

---

## Template Structure

Every template follows this layout:

```
Header Fields       — Date/time, severity, ticket ref
Alert Details       — Observables (hashes, IPs, users, endpoints)
Summary             — Alert narrative with correlation context
Impact              — List of potential outcomes
Recommended Actions — List of response steps
```

---

## How to Use

1. Open the relevant template for the alert type you are triaging.
2. Fill in all header metadata before beginning analysis.
3. Write the summary in your own words using the bracketed prompts as a guide.
4. Work through the impact list and delete anything that does not apply.
5. Do the same for recommended actions, then add any steps specific to your environment.
6. Attach or paste the completed report when escalating.

These templates are a starting point, not a ceiling. Add log extracts, IOC tables, or screenshots as needed.

---

*Part of an ongoing SOC homelab and portfolio project. Feedback and contributions welcome.*


*Part of an ongoing SOC homelab and portfolio project. Feedback and contributions welcome.*
