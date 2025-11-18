# Segment 1: Core Microsoft 365 Features and Objects - Official Resources

## Official Microsoft Documentation

### Microsoft 365 Overview
- **Microsoft 365 Enterprise Overview**
  - https://docs.microsoft.com/microsoft-365/enterprise/
  - Comprehensive overview of M365 architecture and services

- **Microsoft 365 Admin Center**
  - https://admin.microsoft.com/
  - Central hub for M365 administration

### Exchange Online
- **Exchange Online Documentation**
  - https://learn.microsoft.com/en-us/exchange/exchange-online
  - Mailbox management, distribution lists, and administrative tasks

- **Exchange Admin Center**
  - https://admin.exchange.microsoft.com
  - Web-based interface for Exchange administration

- **Key Topics:**
  - Mailbox types (user, shared, resource)
  - Distribution groups and Microsoft 365 Groups
  - Mail flow and transport rules
  - Calendar permissions and delegation

### SharePoint Online
- **SharePoint Administrator Role**
  - https://learn.microsoft.com/en-us/sharepoint/sharepoint-admin-role
  - Site management, permissions, and sharing settings

- **SharePoint Advanced Management**
  - https://learn.microsoft.com/en-us/sharepoint/advanced-management
  - Content sprawl prevention, lifecycle management, permissions streamlining
  - Data access governance reports, oversharing remediation
  - Site ownership policies, inactive sites management

- **SharePoint Admin Center**
  - https://admin.microsoft.com/sharepoint
  - Central administration for SharePoint Online

- **Key Topics:**
  - Site collections and sites
  - Permission levels and groups
  - Sharing policies (internal/external)
  - Content organization
  - SharePoint Advanced Management features (included with Copilot licenses)

### Microsoft Teams
- **Teams Administration Overview**
  - https://learn.microsoft.com/en-us/microsoftteams/teams-overview
  - Administrative controls, policies, and management features

- **Teams Admin Center**
  - https://admin.teams.microsoft.com/
  - Manage Teams policies, users, and settings

- **Key Topics:**
  - Teams and channels structure
  - Messaging policies
  - Meeting policies
  - App permissions and governance
  - Guest access policies
  - External access configuration

### Microsoft Entra ID (Azure AD)
- **Microsoft Entra ID Overview**
  - https://learn.microsoft.com/en-us/entra/fundamentals/whatis
  - Cloud-based identity and access management service
  - Authentication, conditional access, and SSO

- **Microsoft Entra Admin Center**
  - https://entra.microsoft.com/
  - Identity and access management hub

- **Conditional Access**
  - Risk-based access policies
  - Multi-factor authentication requirements
  - Device compliance checks
  - Location-based policies

- **Single Sign-On (SSO)**
  - Seamless authentication across M365 apps
  - Integration with Azure and Dynamics CRM
  - Third-party application integration

- **Privileged Identity Management (PIM)**
  - https://learn.microsoft.com/en-us/entra/id-governance/privileged-identity-management/pim-configure
  - Just-in-time access to privileged roles
  - Time-bound role assignments
  - Approval workflows for activation
  - MFA requirements for privileged roles
  - Audit trails and access reviews

- **PIM Role Types:**
  - **Eligible:** Requires activation when needed
  - **Active:** Immediately usable
  - **Permanent:** No expiration date
  - **Time-bound:** Expires on specified dates

### Zero Trust Security
- **Zero Trust Principles**
  - Verify explicitly (authenticate and authorize)
  - Use least privilege access
  - Assume breach (minimize blast radius)

- **Implementation:**
  - Strong identity verification
  - Conditional access policies
  - Device compliance
  - Application protection
  - Data classification and encryption

## Microsoft Learn Training Modules

### Microsoft 365 Fundamentals
- **Microsoft 365 Certified: Fundamentals (MS-900)**
  - https://learn.microsoft.com/en-us/certifications/microsoft-365-fundamentals/
  - Foundation for understanding M365 services

### Microsoft Entra ID (Azure AD)
- **Azure Active Directory Training**
  - https://learn.microsoft.com/en-us/training/modules/azure-active-directory/
  - Identity and access management
  - Authentication and authorization
  - Conditional access configuration
  - Security controls in Microsoft Entra ID

### Exchange, SharePoint, and Teams
- **Microsoft 365 Service Administration**
  - Core service administration concepts
  - User and group management
  - License assignment
  - Service configuration

## Licensing

### Microsoft 365 Licensing Overview
- **Microsoft 365 Service Descriptions**
  - https://docs.microsoft.com/office365/servicedescriptions/
  - Detailed breakdown of what's included in each license

### Copilot Licensing Requirements
- **Microsoft 365 Copilot Licensing**
  - https://learn.microsoft.com/en-us/copilot/microsoft-365/microsoft-365-copilot-licensing
  - Prerequisites: M365 E3/E5 or Business Standard/Premium
  - Copilot add-on license required
  - License assignment methods

### License Types
| License | Copilot Eligible | Key Features |
|---------|----------------|--------------|
| M365 E3 | ✅ | Enterprise apps, security, compliance |
| M365 E5 | ✅ | All E3 + advanced security, analytics |
| M365 Business Standard | ✅ | Business apps, Teams, Exchange, SharePoint |
| M365 Business Premium | ✅ | All Standard + security, device management |
| Office 365 E1/E3/E5 | ✅ | Office apps only, cloud services |

## Hands-On Labs and Practice

### Microsoft 365 Developer Program
- **Sign up for free M365 tenant**
  - https://developer.microsoft.com/en-us/microsoft-365/dev-program
  - Instant sandbox with sample data
  - 25 user licenses for testing
  - Renewable 90-day subscription

### Practice Tasks
1. **User Management**
   - Create users in Entra ID
   - Assign licenses
   - Configure MFA
   - Set up conditional access

2. **Exchange Online**
   - Create shared mailboxes
   - Configure distribution groups
   - Set calendar permissions
   - Test mail flow

3. **SharePoint**
   - Create site collections
   - Configure sharing settings
   - Set permissions
   - Review SharePoint Advanced Management

4. **Teams**
   - Create teams and channels
   - Configure policies
   - Test guest access
   - Manage apps

5. **Security**
   - Configure conditional access
   - Set up PIM roles
   - Review audit logs
   - Test Zero Trust policies

## AB-900 Exam Focus Areas

### Domain 1: Core Microsoft 365 Features and Objects (30-35%)

**What to Study:**
- [ ] License assignment impacts on feature access
- [ ] Microsoft 365 admin center configuration
- [ ] Exchange Online mailbox and distribution list management
- [ ] SharePoint site management and permissions
- [ ] SharePoint Advanced Management features
- [ ] Teams administrative controls
- [ ] Zero Trust security principles
- [ ] Microsoft Entra authentication features
- [ ] Conditional access policies
- [ ] Single sign-on implementation
- [ ] Privileged Identity Management roles (eligible vs. active)

**Key Concepts:**
- How to assign licenses and impact on features
- Navigating admin centers
- Creating and managing mailboxes
- SharePoint permission inheritance
- SharePoint oversharing remediation
- Teams policies and governance
- Zero Trust "never trust, always verify"
- Conditional access conditions and controls
- PIM just-in-time access
- MFA configuration

## Additional Resources

### Video Training
- **Microsoft Mechanics YouTube Channel**
  - https://www.youtube.com/c/MicrosoftMechanics
  - Technical deep dives and feature demos

### Community
- **Microsoft Tech Community**
  - https://techcommunity.microsoft.com/
  - Forums, blogs, and discussions

- **Microsoft 365 Community (PnP)**
  - https://aka.ms/m365pnp
  - Community samples and best practices

### Blogs
- **Microsoft 365 Blog**
  - https://www.microsoft.com/en-us/microsoft-365/blog/
  - Product announcements and updates

### Tools
- **Microsoft 365 Admin Center:** https://admin.microsoft.com/
- **Entra Admin Center:** https://entra.microsoft.com/
- **Exchange Admin Center:** https://admin.exchange.microsoft.com/
- **SharePoint Admin Center:** https://admin.microsoft.com/sharepoint
- **Teams Admin Center:** https://admin.teams.microsoft.com/

## PowerShell Resources

### Microsoft Graph PowerShell
- **Microsoft Graph PowerShell SDK**
  - https://learn.microsoft.com/en-us/powershell/microsoftgraph/
  - Manage M365 services via PowerShell

### Exchange Online PowerShell
- **Exchange Online PowerShell**
  - https://learn.microsoft.com/en-us/powershell/exchange/exchange-online-powershell
  - Automate Exchange administration

### SharePoint Online PowerShell
- **SharePoint Online Management Shell**
  - https://learn.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online
  - SharePoint automation

## Quick Reference

### Common Administrative Tasks

| Task | Admin Center | Key Steps |
|------|-------------|-----------|
| Assign license | M365 Admin | Users → Active users → Select user → Licenses |
| Create mailbox | Exchange Admin | Recipients → Mailboxes → Add |
| Create SharePoint site | SharePoint Admin | Sites → Active sites → Create |
| Configure Teams policy | Teams Admin | Policy packages or specific policies |
| Set up conditional access | Entra Admin | Protection → Conditional Access → New policy |
| Configure PIM | Entra Admin | Identity Governance → PIM → Assign |

### Service Health Monitoring
- **Message Center:** Stay informed of changes
- **Service Health:** Monitor incidents and advisories
- **Admin App:** Mobile administration via iOS/Android

---

**Related Segments:**
- [Segment 2: Data Protection and Governance](../../segment-02-data-protection-governance/)
- [Segment 3: Copilot Administration](../../segment-03-copilot-administration/)
- [Segment 4: Agents and Exam Prep](../../segment-04-agents-exam-prep/)
