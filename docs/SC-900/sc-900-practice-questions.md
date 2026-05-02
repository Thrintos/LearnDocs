# SC-900 Practice Questions

← **Back to:** [SC-900 Index](index.md)

!!! warning Practice Questions
    Use these questions to test yourself. Answers are hidden below each question using a callout.

---

## Domain 1 — Security Concepts

**Q1.** Which principle of the Zero Trust model states that access should be limited to only what is needed?

??? success "Answer"
    **Least privilege access** (Use least privilege access / JIT-JEA). → [Zero Trust Model](sc-900-security-concepts.md#zero-trust-model)

---

**Q2.** In the Shared Responsibility Model, which responsibility always remains with the customer, regardless of the service model?

??? success "Answer"
    **Data, accounts, and access management.** Customers always own their data. → [Shared Responsibility Model](sc-900-security-concepts.md#shared-responsibility-model)

---

**Q3.** A hospital's patient records are encrypted so that only authorised doctors can read them. Which component of the CIA triad does this represent?

??? success "Answer"
    **Confidentiality.** → [CIA Triad](sc-900-security-concepts.md#cia-triad)

---

**Q4.** What type of attack overwhelms a server to make it unavailable?

??? success "Answer"
    **DDoS (Distributed Denial of Service).** → [Common Threats](sc-900-security-concepts.md#common-threats)

---

**Q5.** Which encryption type uses a public/private key pair?

??? success "Answer"
    **Asymmetric encryption.** Used in TLS and digital certificates. → [Encryption](sc-900-security-concepts.md#encryption)

---

## Domain 2 — Identity and Access

**Q6.** What is the difference between authentication and authorisation?

??? success "Answer"
    **Authentication** verifies *who* you are. **Authorisation** determines *what* you can do. → [Authentication vs. Authorisation](sc-900-identity-and-access.md#authentication-vs-authorisation)

---

**Q7.** Which Entra ID feature uses signals like IP location, device compliance, and user risk to grant or block access?

??? success "Answer"
    **Conditional Access.** → [Conditional Access](sc-900-identity-and-access.md#conditional-access)

---

**Q8.** A company wants its administrators to request temporary elevated access that is logged and approved. Which feature should they use?

??? success "Answer"
    **Privileged Identity Management (PIM).** Requires Entra ID P2. → [Privileged Identity Management (PIM)](sc-900-identity-and-access.md#privileged-identity-management-pim)

---

**Q9.** Which Entra ID feature detects leaked credentials on the dark web and marks user accounts as high risk?

??? success "Answer"
    **Microsoft Entra ID Protection.** → [Identity Protection](sc-900-identity-and-access.md#identity-protection)

---

**Q10.** What is the purpose of Microsoft Entra Connect?

??? success "Answer"
    It synchronises on-premises Active Directory with Microsoft Entra ID (cloud). → [Hybrid Identity — Microsoft Entra Connect](sc-900-identity-and-access.md#hybrid-identity-microsoft-entra-connect)

---

**Q11.** Which MFA factor category does a fingerprint scan belong to?

??? success "Answer"
    **Something you are** (biometric factor). → [MFA Factors](sc-900-identity-and-access.md#mfa-factors)

---

**Q12.** Which Entra ID edition is required for Conditional Access?

??? success "Answer"
    **Entra ID P1** (or higher). → [Editions](sc-900-identity-and-access.md#editions)

---

## Domain 3 — Security Solutions

**Q13.** What is the purpose of Microsoft Sentinel?

??? success "Answer"
    Microsoft Sentinel is a cloud-native **SIEM and SOAR** solution that collects, detects, investigates, and responds to threats. → [Microsoft Sentinel](sc-900-security-solutions.md#microsoft-sentinel)

---

**Q14.** Which Microsoft Defender product protects against phishing and malicious attachments in email?

??? success "Answer"
    **Microsoft Defender for Office 365.** Features include Safe Attachments and Safe Links. → [Microsoft Defender for Office 365](sc-900-security-solutions.md#microsoft-defender-for-office-365)

---

**Q15.** What score does Microsoft Defender for Cloud provide to measure security posture?

??? success "Answer"
    **Secure Score.** → [Microsoft Defender for Cloud](sc-900-security-solutions.md#microsoft-defender-for-cloud)

---

**Q16.** An organisation wants to discover all unsanctioned cloud apps used by employees. Which tool should they use?

??? success "Answer"
    **Microsoft Defender for Cloud Apps** (CASB) — provides Shadow IT discovery. → [Microsoft Defender for Cloud Apps (CASB)](sc-900-security-solutions.md#microsoft-defender-for-cloud-apps-casb)

---

**Q17.** What does Azure Bastion provide?

??? success "Answer"
    Secure RDP/SSH access to Azure VMs over TLS directly from the Azure Portal, without exposing VMs to the public internet. → [Azure Bastion](sc-900-security-solutions.md#azure-bastion)

---

**Q18.** What are the two main capabilities of Microsoft Defender for Cloud?

??? success "Answer"
    1. **Cloud Security Posture Management (CSPM)** — assesses and recommends improvements.
    2. **Cloud Workload Protection (CWP)** — detects and responds to threats. → [Microsoft Defender for Cloud](sc-900-security-solutions.md#microsoft-defender-for-cloud)

---

**Q19.** Which layer of the WAF deployment operates at Layer 7?

??? success "Answer"
    **Web Application Firewall (WAF)** operates at Layer 7 (HTTP/HTTPS). → [Web Application Firewall (WAF)](sc-900-security-solutions.md#web-application-firewall-waf)

---

## Domain 4 — Compliance Solutions

**Q20.** What is Microsoft Purview?

??? success "Answer"
    Microsoft Purview is the unified **data governance and compliance** platform covering information protection, DLP, eDiscovery, audit, and more. → [Microsoft Purview Overview](sc-900-compliance-solutions.md#microsoft-purview-overview)

---

**Q21.** What does the Compliance Score in Compliance Manager indicate?

??? success "Answer"
    It measures an organisation's compliance posture — a higher score means fewer compliance risks. → [Compliance Manager](sc-900-compliance-solutions.md#compliance-manager)

---

**Q22.** An employee is about to email a file containing credit card numbers to an external address. Which feature can detect and block this action?

??? success "Answer"
    **Data Loss Prevention (DLP)** policies. → [Data Loss Prevention (DLP)](sc-900-compliance-solutions.md#data-loss-prevention-dlp)

---

**Q23.** What is the difference between a retention policy and a retention label?

??? success "Answer"
    A **retention policy** applies broadly to locations (e.g., all Exchange mailboxes). A **retention label** is applied to specific items for more granular control. → [Data Lifecycle Management (Retention)](sc-900-compliance-solutions.md#data-lifecycle-management-retention)

---

**Q24.** A legal team needs to preserve all emails from a specific employee for a lawsuit. What feature should they use?

??? success "Answer"
    **Legal Hold** (part of eDiscovery). → [eDiscovery](sc-900-compliance-solutions.md#ediscovery)

---

**Q25.** Where can customers access Microsoft's audit reports (SOC, ISO) and compliance documentation?

??? success "Answer"
    The **Service Trust Portal** at https://servicetrust.microsoft.com. → [Service Trust Portal](sc-900-compliance-solutions.md#service-trust-portal)

---

**Q26.** Which Microsoft Purview feature monitors employee communications for insider trading or regulatory violations?

??? success "Answer"
    **Communication Compliance.** → [Communication Compliance](sc-900-compliance-solutions.md#communication-compliance)

---

**Q27.** An employee downloads a large volume of sensitive data two weeks before their resignation. Which feature would detect this?

??? success "Answer"
    **Insider Risk Management.** → [Insider Risk Management](sc-900-compliance-solutions.md#insider-risk-management)

---

## Mixed / Scenario Questions

**Q28.** A company needs to ensure that only users with compliant devices can access their CRM application. Which feature makes this possible?

??? success "Answer"
    **Conditional Access** with a device compliance requirement. → [Conditional Access](sc-900-identity-and-access.md#conditional-access)

---

**Q29.** A security analyst wants to write custom queries to hunt for suspicious activity across all data sources. Which Sentinel feature enables this?

??? success "Answer"
    **Threat Hunting** with KQL queries. → [Microsoft Sentinel](sc-900-security-solutions.md#microsoft-sentinel)

---

**Q30.** What model does Microsoft use to describe the division of security responsibilities between Microsoft and its customers?

??? success "Answer"
    The **Shared Responsibility Model.** → [Shared Responsibility Model](sc-900-security-concepts.md#shared-responsibility-model)