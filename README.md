# System Vulnerability Checklist — Project 4 (DecodeLabs Internship Cybersecurity Track)

A hands-on security audit of my own primary machine (macOS), performed as the optional
Mastery Phase of the DecodeLabs Cybersecurity Track. The goal: apply a 4-step vulnerability
checklist to a real endpoint, document what's found using CVSS 3.1 scoring, fix it, and
prove the fix with command-line evidence.

## Scope

The audit covers four domains, mirroring the checklist taught in this module:

1. **Identity Front Door** — password policy and MFA strength (NIST 800-63B)
2. **Software Decay & Patch Management** — OS/browser update status, Shadow IT
3. **Human Perimeter** — guest accounts, admin privilege creep, screen lock, credential storage
4. **Network & Endpoint Hygiene** — firewall configuration, full-disk encryption

## Findings summary

| ID | Finding | CVSS 3.1 | Risk |
|----|---------|----------|------|
| F-01 | Legacy MFA reliance (SMS) | 7.4 | High |
| F-02 | Outdated / Beta OS build | 5.3 | Medium |
| F-03 | Insecure local credential storage | 5.5 | Medium |
| F-04 | Firewall stealth mode disabled | 4.3 | Medium |

All four findings were remediated and independently re-verified via Terminal output and
System Settings. Full detail — including CVSS vectors, remediation steps taken, and proof
of the hardened end state — is in the report.

## Report

See [`Vulnerability_Report_OmarBaydoun.docx`](./Vulnerability_Report_OmarBaydoun.docx) for
the full 1-page report (Diagnosis / Treatment / Proof format).

## Methodology note

CVSS 3.1 scores were derived manually using standard vector metrics as a self-assessment of
configuration and process gaps on a personal endpoint — they are not output from an automated
scanner or tied to a published CVE, since these are practice/configuration findings rather
than disclosed software vulnerabilities.

## Author

Omar Baydoun — DecodeLabs Internship Cybersecurity Track, Batch 2026
