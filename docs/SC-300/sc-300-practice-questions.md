# SC-300 Practice Questions

← **Back to:** [SC-300 Index](index.md)

!!! warning Practice Questions
    Use these questions to test yourself. Answers are hidden below each question using a callout.

---

## Domain 1 — User Identities

**Q1.** An organisation wants to allow a Helpdesk Administrator to reset passwords only for users in the Marketing department, without granting tenant-wide permissions. What feature should they use?

??? success "Answer"
    **Administrative Units (AUs).** Scope the Helpdesk Admin role to an AU containing only Marketing users. → [Administrative Units](sc-300-user-identities.md#administrative-units-aus)

---

**Q2.** A company has on-premises AD and wants to sync users to Entra ID. They require that passwords are validated against on-prem AD in real time and that no password hashes are stored in the cloud. Which hybrid authentication method should they use?

??? success "Answer"
    **Pass-through Authentication (PTA).** → [Hybrid Identity](sc-300-user-identities.md#microsoft-entra-connect-sync)

---

**Q3.** A global company has two separate Entra ID tenants due to an acquisition. They need to automatically synchronise user accounts from one tenant to the other. What feature should they use?

??? success "Answer"
    **Cross-Tenant Synchronisation.** → [External Identities](sc-300-user-identities.md#cross-tenant-access-settings)

---

**Q4.** An organisation wants users in a dynamic group to automatically include all users where the department attribute equals "Finance". What group type enables this?

??? success "Answer"
    **Dynamic group** with a dynamic membership rule based on the department attribute. → [Groups](sc-300-user-identities.md#groups)

---

**Q5.** A company is migrating from AD FS to a cloud-native authentication model. Which method should they choose if they want the highest resilience and are comfortable with cloud-based authentication?

??? success "Answer"
    **Password Hash Synchronisation (PHS).** It is the most resilient option — cloud sign-in continues even if on-premises infrastructure is unavailable. → [Hybrid Identity](sc-300-user-identities.md#microsoft-entra-connect-sync)

---

**Q6.** What is the purpose of Microsoft Entra Connect Health?

??? success "Answer"
    It monitors the health of hybrid identity infrastructure (Entra Connect Sync, AD FS, AD DS), alerting on sync errors, latency, and service health issues. → [Connect Health](sc-300-user-identities.md#microsoft-entra-connect-health)

---

## Domain 2 — Authentication and Access Management

**Q7.** A new employee cannot register their MFA methods because they don't have a phone yet. What temporary credential can an admin issue to let them sign in and complete registration?

??? success "Answer"
    A **Temporary Access Pass (TAP).** It is a time-limited passcode used to bootstrap passwordless registration or for account recovery. → [TAP](sc-300-authentication-and-access.md#temporary-access-pass-tap)

---

**Q8.** An administrator wants to deploy a Conditional Access policy but is unsure of the impact. What mode should they use first?

??? success "Answer"
    **Report-only mode.** It logs the impact of the policy without enforcing it, allowing safe testing. → [Conditional Access](sc-300-authentication-and-access.md#conditional-access)

---

**Q9.** Which Conditional Access control ensures users are re-prompted to authenticate every 8 hours when accessing a sensitive application?

??? success "Answer"
    **Sign-in frequency** (a Session Control). → [Session Controls](sc-300-authentication-and-access.md#session-controls)

---

**Q10.** An Entra ID admin needs to require extra MFA when deleting a tenant, regardless of the user's existing session. Which feature enables this?

??? success "Answer"
    **Protected Actions** — step-up authentication for specific high-risk Entra operations. → [Protected Actions](sc-300-authentication-and-access.md#protected-actions)

---

**Q11.** A user's credentials were found in a dark web breach. Entra ID Protection marks the account as high user risk. What remediation actions are available?

??? success "Answer"
    Block access, require a **secure password reset** (via SSPR with MFA), or an admin can manually remediate and dismiss the risk. → [ID Protection](sc-300-authentication-and-access.md#remediation-actions)

---

**Q12.** An organisation wants to give remote employees access to an internal intranet site without deploying a VPN. Which two Microsoft solutions could achieve this?

??? success "Answer"
    1. **Microsoft Entra Application Proxy** — publishes the on-prem web app securely via Entra ID.
    2. **Microsoft Entra Private Access** (Global Secure Access) — ZTNA-based access without a VPN. → [Application Proxy](sc-300-workload-identities.md#application-proxy) | [Global Secure Access](sc-300-authentication-and-access.md#global-secure-access)

---

**Q13.** What is Continuous Access Evaluation (CAE) and when does it trigger?

??? success "Answer"
    CAE enables near-real-time token revocation. It triggers on critical events like account disable, password change, high-risk detection, or a significant IP address change — without waiting for token expiry. → [CAE](sc-300-authentication-and-access.md#session-controls)

---

## Domain 3 — Workload Identities

**Q14.** An Azure Function App needs to access an Azure Key Vault to retrieve secrets. What is the recommended approach to authenticate without storing credentials in code?

??? success "Answer"
    Assign a **Managed Identity** (system-assigned or user-assigned) to the Function App, then grant it the **Key Vault Secrets User** role on the Key Vault. → [Managed Identities](sc-300-workload-identities.md#managed-identities)

---

**Q15.** What is the difference between a system-assigned and a user-assigned managed identity?

??? success "Answer"
    A **system-assigned** identity is tied to a single resource and deleted with it. A **user-assigned** identity has an independent lifecycle and can be assigned to multiple resources. → [Managed Identities](sc-300-workload-identities.md#types)

---

**Q16.** A developer registers an app in Entra ID. The app needs to read all users' mailboxes without any user being signed in. What permission type is required, and who must grant it?

??? success "Answer"
    **Application permission** (e.g., Mail.Read for the Graph API). It requires **admin consent** since the app acts as itself without a signed-in user. → [App Registrations](sc-300-workload-identities.md#permission-types)

---

**Q17.** An organisation discovers that employees have granted OAuth permissions to many third-party apps, some of which are risky. Which feature helps detect and manage these?

??? success "Answer"
    **OAuth App Policies** in Microsoft Defender for Cloud Apps. → [OAuth App Policies](sc-300-workload-identities.md#oauth-app-policies)

---

**Q18.** What is the difference between an App Registration and a Service Principal?

??? success "Answer"
    The **App Registration** is the global definition of the application (in the home tenant). A **Service Principal** is the local representation of that app in each tenant where it is used — it is the object that is granted permissions and used for access control. → [Workload Identities](sc-300-workload-identities.md#enterprise-applications-and-service-principals)

---

**Q19.** A company wants to allow users on unmanaged devices to access SharePoint Online but prevent them from downloading files. Which feature enables this?

??? success "Answer"
    **Conditional Access App Control** (via Defender for Cloud Apps) with a **session policy** that blocks downloads. → [App Control](sc-300-workload-identities.md#conditional-access-app-control)

---

## Domain 4 — Identity Governance

**Q20.** What is an Access Package in Entitlement Management?

??? success "Answer"
    A bundled set of resources (groups, apps, SharePoint sites) that users can request access to through a defined approval workflow, with a configured duration and expiry. → [Entitlement Management](sc-300-identity-governance.md#entitlement-management)

---

**Q21.** A company wants guest users to automatically lose access when they no longer have any active access packages. Which feature enables this?

??? success "Answer"
    The **external user lifecycle management** setting in Entitlement Management — guests are automatically removed when their last access package expires. → [External User Lifecycle](sc-300-identity-governance.md#external-user-lifecycle)

---

**Q22.** What is the difference between an Eligible and an Active PIM assignment?

??? success "Answer"
    An **Eligible** assignment means the user must explicitly activate the role when needed (JIT). An **Active** assignment means the user has the role active at all times. Eligible is preferred for privileged roles to reduce standing access. → [PIM](sc-300-identity-governance.md#role-assignment-types)

---

**Q23.** A Global Administrator gets locked out due to a misconfigured Conditional Access policy. What should the organisation have prepared for this situation?

??? success "Answer"
    A **break-glass account** — a highly privileged emergency account excluded from all CA policies, with credentials stored offline. → [Break-Glass Accounts](sc-300-identity-governance.md#break-glass-accounts)

---

**Q24.** An access review is configured for a group but reviewers are not responding. The organisation wants access to be removed automatically when no response is received. What setting enables this?

??? success "Answer"
    **Auto-apply results** with a setting to remove access when reviewers do not respond (treat non-response as denial). → [Access Reviews](sc-300-identity-governance.md#review-settings)

---

**Q25.** A security team wants to be alerted any time a break-glass account signs in. How should they implement this?

??? success "Answer"
    Configure a **diagnostic setting** to send Sign-in Logs to a **Log Analytics Workspace**, then create a **KQL-based alert rule** that triggers when the break-glass account UPN appears in sign-in events. → [Monitoring](sc-300-identity-governance.md#diagnostic-settings)

---

**Q26.** What does the Identity Secure Score measure?

??? success "Answer"
    The security posture of an organisation's Entra ID configuration. A higher score indicates fewer identity security risks. It provides improvement actions with guidance. → [Identity Secure Score](sc-300-identity-governance.md#identity-secure-score)

---

**Q27.** An organisation wants to require that external partners accept a terms-of-use document before accessing a partner portal application. How is this implemented?

??? success "Answer"
    Create a **Terms of Use (ToU)** document in Microsoft Entra ID, then enforce it via a **Conditional Access policy** targeting the partner portal application. → [Terms of Use](sc-300-identity-governance.md#terms-of-use-tou)

---

## Mixed / Scenario Questions

**Q28.** A company wants to ensure that only users who are members of a specific group, on compliant devices, and in a named location can access their financial reporting app — and only during business hours. Which feature handles all of these conditions?

??? success "Answer"
    **Conditional Access** — using group assignment, device compliance, named location, and time-based conditions as signals, with a Grant control requiring access. → [Conditional Access](sc-300-authentication-and-access.md#conditional-access)

---

**Q29.** An admin notices a PIM activation request from a Global Administrator role at 3am from an unusual location. Which logs should they check, and what action might they take?

??? success "Answer"
    Check the **PIM audit history** for the activation request details, and the **Sign-in logs** and **Risky sign-ins** report in Entra ID Protection. If suspicious, they may **dismiss / remediate** the user risk and **revoke all sessions**. → [PIM Audit](sc-300-identity-governance.md#pim-audit-history) | [ID Protection](sc-300-authentication-and-access.md#microsoft-entra-id-protection)

---

**Q30.** A developer wants to build an app that accesses the Microsoft Graph API on behalf of the signed-in user. What permission type should they request?

??? success "Answer"
    **Delegated permissions** — the app acts on behalf of the user, limited to what the user themselves can access. → [App Registrations](sc-300-workload-identities.md#permission-types)
