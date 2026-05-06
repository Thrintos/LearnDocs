# Glossary — SC-300 Key Terms

← **Back to:** [SC-300 Index](index.md)

---

| Term | Definition | See Also |
|------|------------|----------|
| **Access Package** | A bundle of resources (groups, apps, sites) users can request access to | [Entitlement Management](sc-300-identity-governance.md#entitlement-management) |
| **Access Review** | Periodic review of whether users still need their current access | [Access Reviews](sc-300-identity-governance.md#access-reviews) |
| **Administrative Unit (AU)** | Container that scopes admin permissions to a subset of users/groups | [Administrative Units](sc-300-user-identities.md#administrative-units-aus) |
| **App Registration** | The definition of an application in Entra ID (Client ID, permissions, secrets) | [App Registrations](sc-300-workload-identities.md#app-registrations) |
| **Application Proxy** | Provides secure remote access to on-premises web apps without a VPN | [Application Proxy](sc-300-workload-identities.md#application-proxy) |
| **Application Permission** | Permission granted to an app acting as itself (no user involved); requires admin consent | [App Registrations](sc-300-workload-identities.md#app-registrations) |
| **Audit Logs** | Record of all administrative changes in Entra ID | [Monitoring](sc-300-identity-governance.md#log-types-in-entra-id) |
| **B2B Collaboration** | External partners access your apps using their own organisational identity (guest accounts) | [External Identities](sc-300-user-identities.md#external-identities) |
| **Break-Glass Account** | Emergency access account excluded from MFA/CA; used only when normal admin access fails | [Break-Glass Accounts](sc-300-identity-governance.md#break-glass-accounts) |
| **CAE** | Continuous Access Evaluation — real-time token revocation on critical events | [Session Controls](sc-300-authentication-and-access.md#session-controls) |
| **Catalog** | Container for resources and access packages in Entitlement Management | [Entitlement Management](sc-300-identity-governance.md#entitlement-management) |
| **CBA** | Certificate-Based Authentication — uses X.509 certificates, satisfies MFA | [Authentication Methods](sc-300-authentication-and-access.md#authentication-methods) |
| **Cloud Sync** | Lightweight cloud-managed agent for syncing on-prem AD to Entra ID | [Hybrid Identity](sc-300-user-identities.md#microsoft-entra-cloud-sync) |
| **Conditional Access** | If-then policy engine for access control based on signals | [Conditional Access](sc-300-authentication-and-access.md#conditional-access) |
| **Connected Organisation** | An external Entra tenant whose users can request access packages | [Entitlement Management](sc-300-identity-governance.md#entitlement-management) |
| **Cross-Tenant Access Settings** | Controls for inbound/outbound B2B collaboration between specific tenants | [External Identities](sc-300-user-identities.md#cross-tenant-access-settings) |
| **Custom Role** | Admin role with a specific set of permissions defined by the tenant | [Entra Roles](sc-300-user-identities.md#entra-roles) |
| **Delegated Permission** | App acts on behalf of a signed-in user; bounded by user's own permissions | [App Registrations](sc-300-workload-identities.md#permission-types) |
| **Diagnostic Settings** | Configuration to export Entra logs to Log Analytics, storage, or Event Hub | [Monitoring](sc-300-identity-governance.md#diagnostic-settings) |
| **Dynamic Group** | Group whose membership is automatically managed by attribute rules | [Groups](sc-300-user-identities.md#groups) |
| **Eligible Assignment** | PIM assignment where user must activate the role before use | [PIM](sc-300-identity-governance.md#role-assignment-types) |
| **Entra Cloud Sync** | Lightweight alternative to Entra Connect Sync; cloud-managed | [Hybrid Identity](sc-300-user-identities.md#microsoft-entra-cloud-sync) |
| **Entra Connect Health** | Monitors health of Entra Connect Sync, AD FS, and AD DS | [Hybrid Identity](sc-300-user-identities.md#microsoft-entra-connect-health) |
| **Entra Connect Sync** | On-premises agent that syncs AD identities to Entra ID | [Hybrid Identity](sc-300-user-identities.md#microsoft-entra-connect-sync) |
| **Entra ID** | Microsoft's cloud-based IAM platform (formerly Azure Active Directory) | [Module 1](sc-300-user-identities.md) |
| **Entra ID Protection** | ML-based detection of risky sign-ins and compromised users | [ID Protection](sc-300-authentication-and-access.md#microsoft-entra-id-protection) |
| **Enterprise Application** | Entra ID object representing an app available for use in the tenant (service principal) | [Workload Identities](sc-300-workload-identities.md#enterprise-applications-and-service-principals) |
| **Entitlement Management** | Automates access request, approval, and lifecycle via access packages | [Identity Governance](sc-300-identity-governance.md#entitlement-management) |
| **Federation (ADFS)** | Full sign-in trust delegated to on-premises AD FS infrastructure | [Hybrid Identity](sc-300-user-identities.md#microsoft-entra-connect-sync) |
| **FIDO2** | Passwordless hardware security key standard | [Authentication Methods](sc-300-authentication-and-access.md#authentication-methods) |
| **Global Secure Access** | Microsoft's SSE platform — Private Access (ZTNA) + Internet Access (SWG) | [Global Secure Access](sc-300-authentication-and-access.md#global-secure-access) |
| **gMSA** | Group Managed Service Account — Windows on-prem service identity | [Workload Identities](sc-300-workload-identities.md#what-are-workload-identities) |
| **Identity Governance** | Set of capabilities to manage who has access to what, and for how long | [Module 4](sc-300-identity-governance.md) |
| **Identity Secure Score** | Numeric score measuring Entra ID security posture | [Monitoring](sc-300-identity-governance.md#identity-secure-score) |
| **Internet Access** | Global Secure Access Secure Web Gateway for internet-bound traffic | [Global Secure Access](sc-300-authentication-and-access.md#global-secure-access) |
| **JIT Access** | Just-In-Time — temporary elevated access granted via PIM | [PIM](sc-300-identity-governance.md#privileged-identity-management-pim) |
| **KQL** | Kusto Query Language — used to query Entra logs in Log Analytics | [Monitoring](sc-300-identity-governance.md#kql-queries-in-log-analytics) |
| **Legal Hold** | Preserves data for legal investigations (Purview, not Entra) | — |
| **Managed Identity** | Azure-managed identity for resources; no credentials to store | [Workload Identities](sc-300-workload-identities.md#managed-identities) |
| **MFA** | Multi-Factor Authentication — requires 2+ verification factors | [Authentication Methods](sc-300-authentication-and-access.md#authentication-methods) |
| **Named Location** | Trusted IP ranges or countries used in Conditional Access policies | [Conditional Access](sc-300-authentication-and-access.md#signals-conditions) |
| **OAuth App Policy** | Defender for Cloud Apps policy to detect risky OAuth app consents | [Defender for Cloud Apps](sc-300-workload-identities.md#microsoft-defender-for-cloud-apps-app-monitoring) |
| **Pass-through Authentication (PTA)** | Password validated against on-prem AD in real time; hash never leaves on-prem | [Hybrid Identity](sc-300-user-identities.md#microsoft-entra-connect-sync) |
| **Password Hash Sync (PHS)** | On-prem password hashes synced to Entra ID; most resilient hybrid option | [Hybrid Identity](sc-300-user-identities.md#microsoft-entra-connect-sync) |
| **Password Protection** | Blocks weak/banned passwords in Entra ID and on-prem AD | [Authentication](sc-300-authentication-and-access.md#microsoft-entra-password-protection) |
| **PIM** | Privileged Identity Management — JIT access for admin roles and Azure resources | [Identity Governance](sc-300-identity-governance.md#privileged-identity-management-pim) |
| **PIM for Groups** | Extend JIT access to group membership, not just roles | [PIM](sc-300-identity-governance.md#what-pim-covers) |
| **Private Access** | Global Secure Access ZTNA component — secure access to private apps without VPN | [Global Secure Access](sc-300-authentication-and-access.md#global-secure-access) |
| **Protected Actions** | Step-up MFA required for specific high-risk Entra operations | [Conditional Access](sc-300-authentication-and-access.md#protected-actions) |
| **Provisioning Logs** | Logs of SCIM/HR-driven user provisioning events | [Monitoring](sc-300-identity-governance.md#log-types-in-entra-id) |
| **RBAC** | Role-Based Access Control — controls access to Azure resources | [Workload Identities](sc-300-workload-identities.md) |
| **Registration Campaign** | Nudges users to register for stronger MFA methods | [Authentication](sc-300-authentication-and-access.md#mfa-settings) |
| **Report-Only Mode** | CA policy mode where impact is logged but policy is not enforced | [Conditional Access](sc-300-authentication-and-access.md#conditional-access) |
| **SAML** | Security Assertion Markup Language — federated SSO protocol | [External Identities](sc-300-user-identities.md#external-identity-providers) |
| **Seamless SSO** | Automatically signs in domain-joined users without re-prompting | [Hybrid Identity](sc-300-user-identities.md#microsoft-entra-connect-sync) |
| **Security Defaults** | Microsoft-managed baseline security settings; free tier option for MFA enforcement | [Authentication](sc-300-authentication-and-access.md#mfa-settings) |
| **Service Principal** | The identity of an application in a specific Entra tenant | [Workload Identities](sc-300-workload-identities.md#enterprise-applications-and-service-principals) |
| **Shadow IT** | Unsanctioned cloud apps discovered via Defender for Cloud Apps | [App Monitoring](sc-300-workload-identities.md#cloud-discovery) |
| **Sign-in Logs** | Record of all authentication attempts in Entra ID | [Monitoring](sc-300-identity-governance.md#log-types-in-entra-id) |
| **Sign-in Risk** | ML-assessed risk that a sign-in is not performed by the legitimate user | [ID Protection](sc-300-authentication-and-access.md#risk-types) |
| **SSPR** | Self-Service Password Reset — users reset without admin involvement | [Authentication Methods](sc-300-authentication-and-access.md#authentication-methods) |
| **SSO** | Single Sign-On — one login gives access to multiple apps | [Enterprise Apps](sc-300-workload-identities.md#saas-app-integration) |
| **TAP** | Temporary Access Pass — time-limited passcode for onboarding/recovery | [Authentication Methods](sc-300-authentication-and-access.md#temporary-access-pass-tap) |
| **Terms of Use (ToU)** | Require users to accept terms before accessing a resource | [Entitlement Management](sc-300-identity-governance.md#terms-of-use-tou) |
| **User-Assigned Managed Identity** | Managed identity with its own lifecycle, assignable to multiple resources | [Managed Identities](sc-300-workload-identities.md#types) |
| **User Risk** | ML-assessed risk that a user account is compromised | [ID Protection](sc-300-authentication-and-access.md#risk-types) |
| **Windows Hello for Business** | Device-bound biometric/PIN-based passwordless authentication | [Authentication Methods](sc-300-authentication-and-access.md#authentication-methods) |
| **Workbook** | Azure Monitor visualisation of Entra ID log data | [Monitoring](sc-300-identity-governance.md#workbooks) |
| **Workload Identity** | Non-human identity (app, service, managed identity) used for authentication | [Module 3](sc-300-workload-identities.md) |
| **WS-Federation** | Federated SSO protocol, older alternative to SAML | [External Identities](sc-300-user-identities.md#external-identity-providers) |
| **ZTNA** | Zero Trust Network Access — replaces VPN with identity-aware access | [Global Secure Access](sc-300-authentication-and-access.md#global-secure-access) |
