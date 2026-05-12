# SOC Report Templates

A collection of structured report templates for SOC L1 analyst workflows and TryHackMe investigation writeups, covering the most common alert categories encountered during triage. Built for consistent, repeatable documentation.
Templates are tool-agnostic and intended to work alongside any SIEM, EDR, or ticketing platform.

---

## Templates Included

| # | Alert Type |
|---|---|
| 01 | Phishing |
| 02 | Malware / Endpoint Infection |
| 03 | Suspicious Process Execution |
| 04 | Unauthorised Access / Brute Force |
| 05 | Privilege Escalation |
| 06 | Lateral Movement |
| 07 | Data Exfiltration |
| 08 | C2 / Beaconing |
| 09 | Insider Threat |
| 10 | Vulnerability / Exploit Attempt |
| 11 | Denial of Service (DoS / DDoS) |
| 12 | Suspicious Network Traffic |
| 13 | Suspicious Login / Authentication Anomaly |
| 14 | Ransomware |
| 15 | USB / Removable Media |

---

## Template Structure

Every template follows this layout:

```
Header Fields       — Date/time, analyst, severity, ticket ref
Alert Details       — Tool-specific observables (hashes, IPs, users, endpoints)
Summary             — Guided narrative with correlation context
Impact              — Checkbox list of potential outcomes
Recommended Actions — Prioritised response steps
```

MITRE ATT&CK technique fields are included throughout to support threat intelligence enrichment and reporting.

---

## How to Use

1. Open the relevant template for the alert type you are triaging.
2. Fill in all header metadata before beginning analysis.
3. Write the summary section in your own words, using the bracketed prompts as a guide.
4. Work through the impact checklist and tick every item that applies.
5. Select all the appropriate recommended actions.
6. Attach or paste the completed report when escalating.

> These templates are a starting point, not a ceiling. Add context, screenshots, log extracts, or IOC tables as needed.

---

*Part of an ongoing SOC homelab and portfolio project. Feedback and contributions welcome.*
