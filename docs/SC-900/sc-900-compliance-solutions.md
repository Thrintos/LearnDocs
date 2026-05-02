# SC-900 - Compliance Solutions

!!! info "Exam Weight"
    This topic accounts for approximately **25–30%** of the SC-900 exam.

← **Back to:** [SC-900 Index](index.md)

---

## Microsoft Purview Overview

**Microsoft Purview** is the unified data governance and compliance platform. It covers:

- Information Protection
- Data Lifecycle Management
- eDiscovery
- Audit
- Insider Risk Management
- Communication Compliance

---

## Microsoft Purview Compliance Portal

Central location to manage compliance activities across Microsoft 365.

Key sections:

- **Compliance Manager** — Assess and manage compliance posture.
- **Information Protection** — Classify and protect data.
- **Data Lifecycle Management** — Retain and delete data per policy.
- **eDiscovery** — Search and export data for legal/investigative purposes.
- **Audit** — Track user and admin activity.
- **Communication Compliance** — Monitor communications for policy violations.
- **Insider Risk Management** — Detect and act on risky user behaviour.

---

## Compliance Manager

**Compliance Manager** helps organisations manage their compliance posture.

- Provides a **Compliance Score** (higher = fewer risks).
- Maps controls to frameworks (ISO 27001, NIST, GDPR, etc.).
- Gives improvement actions with step-by-step guidance.
- Distinguishes between **Microsoft-managed controls** and **customer-managed controls**.

> Think of it as the compliance equivalent of **Secure Score** from [Microsoft Defender for Cloud](sc-900-security-solutions.md#microsoft-defender-for-cloud).

---

## Information Protection

Classifies and protects sensitive data using **sensitivity labels**.

### Sensitivity Labels

- Applied to documents, emails, and containers (Teams, SharePoint sites).
- Can enforce: encryption, watermarks, access restrictions, visual markings.
- Labels are persistent — they travel with the file.

### Label Flow

```
Identify → Classify → Protect → Monitor
```

### Auto-labelling

Labels can be automatically applied based on sensitive information types (credit card numbers, social security numbers, etc.).

---

## Data Loss Prevention (DLP)

**DLP policies** detect and prevent sensitive data from being shared inappropriately.

- Can apply across: Exchange, SharePoint, OneDrive, Teams, Endpoint, and more.
- Sensitive information types (SITs) define what counts as sensitive (e.g., passport number, IBAN).
- Actions: block, warn, require justification, audit.

---

## Data Lifecycle Management (Retention)

Controls how long data is **kept** and when it is **deleted**.

| Tool | Purpose |
|------|---------|
| **Retention policies** | Apply to broad locations (SharePoint, Exchange, Teams) |
| **Retention labels** | Apply to specific items for more granular control |

### Retention vs. Delete

- **Retain-only** — Keep for minimum period, then let users delete.
- **Delete-only** — Delete after a set period.
- **Retain-then-delete** — Retain for X years, then auto-delete.

### Records Management

Marks content as a **record** or **regulatory record**:

- Records can't be edited or deleted.
- Regulatory records are even stricter (can't be unlabelled).

---

## eDiscovery

Enables searching for and exporting content for legal, regulatory, or investigative purposes.

| Tool | Use Case |
|------|----------|
| **Content Search** | Basic search across M365 services |
| **eDiscovery (Standard)** | Create cases, export content, apply holds |
| **eDiscovery (Premium)** | Advanced analytics, custodian management, review sets, communication threading |

### Legal Hold

Preserves data so it cannot be deleted, even if a retention policy would otherwise delete it.

---

## Audit

Tracks user and administrator activity across Microsoft 365.

| Tier | Features |
|------|----------|
| **Audit (Standard)** | 180-day log retention, available to all M365 plans |
| **Audit (Premium)** | 365-day (or up to 10-year) retention, high-value event logging, faster access |

> Useful for investigations, compliance, and detecting malicious activity.

---

## Communication Compliance

Monitors communications (email, Teams, Yammer) for:

- Inappropriate content
- Insider trading signals
- Regulatory violations (e.g., financial services rules)

Uses machine learning classifiers and keyword policies.

---

## Insider Risk Management

Detects risky user behaviours that could indicate internal threats.

| Signal | Example |
|--------|---------|
| Data exfiltration | Large downloads before resignation |
| Data leakage | Sharing sensitive files externally |
| Security policy violations | Installing unauthorised software |
| Offensive behaviour | Harassment in communications |

Uses a **privacy-by-design** approach — user identities are anonymised until an alert is investigated.

---

## Microsoft Priva

**Microsoft Priva** helps organisations manage **privacy risk** and **data subject requests**.

| Feature | Purpose |
|---------|---------|
| **Privacy Risk Management** | Identifies oversharing, data hoarding, data transfer risks |
| **Subject Rights Requests** | Automates handling of GDPR/CCPA data subject requests |

---

## Service Trust Portal

Microsoft's public portal to access:

- Audit reports (SOC, ISO, PCI, etc.)
- Compliance guides and whitepapers
- Regional compliance information
- Security, privacy, and compliance documentation

URL: [https://servicetrust.microsoft.com](https://servicetrust.microsoft.com)

---

## Key Regulations to Know

| Regulation | Scope |
|------------|-------|
| **GDPR** | EU personal data protection |
| **HIPAA** | US healthcare data |
| **CCPA** | California consumer privacy |
| **ISO 27001** | International information security standard |
| **NIST** | US cybersecurity framework |
| **SOC 1/2** | Service organisation controls reports |

