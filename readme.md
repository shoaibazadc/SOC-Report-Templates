# SOC Escalation Report Templates

A collection of structured escalation report templates for SOC L1/L2 analysts, covering the most common alert categories encountered during triage. Built to standardise analyst output, reduce escalation errors, and ensure critical fields are captured consistently under pressure.

---

## Background

One of the most common failure points in a SOC is inconsistent escalation quality. Analysts working under alert fatigue miss fields, write vague summaries, or escalate without clear impact assessments, forcing L2 and IR teams to chase down basic context. These templates exist to solve that problem by giving analysts a repeatable, structured starting point for every significant alert type.

Each template follows the same structure: metadata, alert details, a guided summary, an impact checklist, and recommended actions. The `[X]` placeholders and checkbox format are intentional, designed for speed during active triage.

---

## Templates Included

| # | Alert Type |
|---|---|
| 00 | Phishing |
| 01 | Malware / Endpoint Infection |
| 02 | Suspicious Process Execution |
| 03 | Unauthorised Access / Brute Force |
| 04 | Privilege Escalation |
| 05 | Lateral Movement |
| 06 | Data Exfiltration |
| 07 | C2 / Beaconing |
| 08 | Insider Threat |
| 09 | Vulnerability / Exploit Attempt |
| 10 | Denial of Service (DoS / DDoS) |
| 11 | Suspicious Network Traffic |
| 12 | Suspicious Login / Authentication Anomaly |
| 13 | Ransomware |
| 14 | USB / Removable Media |

---

## How to Use

1. Open the relevant template for the alert type you are triaging.
2. Fill in all header metadata fields before beginning analysis.
3. Write the summary section in your own words, using the bracketed prompts as a guide. Replace `[X]` with actual findings.
4. Work through the impact checklist and tick every item that applies. Leave nothing ambiguous.
5. Select all recommended actions appropriate to the confirmed or suspected impact.
6. Attach or paste the completed report into your ticketing system (e.g. Jira, ServiceNow) when escalating.

> These templates are a starting point, not a ceiling. Add context, screenshots, log extracts, or IOC tables as needed.

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

## Notes

- Templates are tool-agnostic and intended to work alongside any SIEM, EDR, or ticketing platform.
- Severity ratings (Low / Medium / High / Critical) should align with your organisation's classification policy.
- The Ransomware template includes IR escalation steps given its potential for rapid, high-impact spread.
- False positive checkboxes are included in every impact section as an explicit triage outcome, not an afterthought.

---

## Repo Structure

```
soc-escalation-report-templates/
├── README.md
└── templates/
    ├── 00-phishing.md
    ├── 01-malware-endpoint-infection.md
    ├── 02-suspicious-process-execution.md
    ├── 03-unauthorised-access-brute-force.md
    ├── 04-privilege-escalation.md
    ├── 05-lateral-movement.md
    ├── 06-data-exfiltration.md
    ├── 07-c2-beaconing.md
    ├── 08-insider-threat.md
    ├── 09-vulnerability-exploit-attempt.md
    ├── 10-dos-ddos.md
    ├── 11-suspicious-network-traffic.md
    ├── 12-suspicious-login-auth-anomaly.md
    ├── 13-ransomware.md
    └── 14-usb-removable-media.md
```

---

*Part of an ongoing SOC homelab and portfolio project. Feedback and contributions welcome.*
