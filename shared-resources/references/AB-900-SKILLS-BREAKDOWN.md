# AB-900 Exam Skills - Complete Breakdown

## Exam Structure Overview

**Total Duration:** 45 minutes
**Passing Score:** 700/1000
**Question Types:** Multiple choice, multiple response, interactive scenarios, drag-and-drop, case studies

### Domain Weights
| Domain | Weight | Focus |
|--------|--------|-------|
| Domain 1: Core M365 Features & Objects | 30-35% | Foundation services and security |
| Domain 2: Data Protection & Governance | 35-40% | **LARGEST** - Purview, Copilot data security |
| Domain 3: Copilot & Agent Administration | 25-30% | Copilot/agent deployment and management |

---

# Domain 1: Identify Core Features and Objects of Microsoft 365 Services (30-35%)

## Section 1.1: Identify the Core Objects of Microsoft 365 Services

### Skill: Explain how license types assigned to users and groups affect access to Microsoft 365 features

**What You Need to Know:**
- Different license tiers provide different feature access
- License assignment can be individual or group-based
- Some features require specific licenses (e.g., Copilot requires base M365 license + add-on)

**Key Concepts:**

#### License Types and Feature Access

| License | Key Features | Copilot Eligible |
|---------|--------------|------------------|
| **Microsoft 365 E3** | Office apps, Teams, Exchange, SharePoint, OneDrive, basic security | ✅ Yes |
| **Microsoft 365 E5** | All E3 + advanced security, analytics, compliance, phone system | ✅ Yes |
| **Microsoft 365 Business Basic** | Web/mobile Office, Teams, Exchange, OneDrive, SharePoint | ✅ Yes (Business tiers) |
| **Microsoft 365 Business Standard** | All Basic + desktop Office apps | ✅ Yes |
| **Microsoft 365 Business Premium** | All Standard + advanced security, device management | ✅ Yes |
| **Office 365 E1** | Online Office apps only, Exchange, SharePoint, Teams | ✅ Yes |
| **Office 365 E3** | Desktop Office apps + online, Exchange, SharePoint, Teams | ✅ Yes |
| **Office 365 E5** | All E3 + advanced features | ✅ Yes |

#### License Assignment Impact Examples:
- **No Exchange Online license** → Cannot access email or mailbox
- **No Teams license** → Cannot use Teams chat or meetings
- **No SharePoint license** → Cannot access SharePoint sites or OneDrive
- **No Copilot add-on** → Cannot use Copilot features even with base M365 license
- **Group-based licensing** → Automatic assignment based on group membership
- **Direct licensing** → Manual assignment to individual users

**Hands-On:**
- Navigate to M365 Admin Center → Billing → Licenses
- View available licenses and assigned users
- Assign license to user: Users → Active users → Select user → Licenses and apps
- Create security group and assign licenses to group
- Understand 24-hour delay for Copilot license activation

**Documentation:** https://learn.microsoft.com/en-us/microsoft-365/admin/manage/assign-licenses-to-users

---

### Skill: Explore the organization configurations by using the Microsoft 365 admin center (domain names and org settings)

**What You Need to Know:**
- Microsoft 365 admin center is the central hub for M365 administration
- Domain names determine email addresses and service URLs
- Organizational settings control tenant-wide configurations

**Key Concepts:**

#### Domain Names
- **Primary domain:** Default domain for new users (e.g., contoso.onmicrosoft.com)
- **Custom domains:** Add your own domains (e.g., contoso.com)
- **Domain verification:** Prove ownership via DNS TXT or MX records
- **Domain services:** Email, Teams, SharePoint use domains
- **Domain federation:** Connect to on-premises Active Directory

#### Organization Settings (Settings → Org settings)
- **Organization profile:**
  - Organization name
  - Contact information
  - Preferred language and time zone
  - Data location

- **Services & add-ins:**
  - Calendar
  - Cortana
  - Microsoft 365 groups
  - SharePoint
  - User owned apps and services
  - Microsoft 365 installation options

- **Security & privacy:**
  - Password expiration policy
  - Customer Lockbox
  - Sharing settings
  - Privacy profile

**Hands-On:**
- Navigate to Setup → Domains
- View domain details and DNS records
- Add custom domain (if available)
- Navigate to Settings → Org settings
- Review organization profile
- Check services configuration

**Admin Center URL:** https://admin.microsoft.com

---

### Skill: Identify the appropriate objects to configure by using the Exchange Online admin center (mailboxes and distribution lists)

**What You Need to Know:**
- Exchange Admin Center (EAC) manages email and calendar services
- Different mailbox types serve different purposes
- Distribution lists enable email to groups of users

**Key Concepts:**

#### Mailbox Types

1. **User Mailboxes**
   - Primary mailbox for individual users
   - Includes email, calendar, contacts, tasks
   - Assigned via license
   - Default 50 GB storage (varies by license)

2. **Shared Mailboxes**
   - Shared email address (e.g., info@contoso.com, support@contoso.com)
   - Multiple users can access
   - No separate license required (up to 50 GB)
   - Users need "Full Access" and "Send As" permissions
   - Use cases: Team email, departmental email, service accounts

3. **Resource Mailboxes**
   - **Room mailboxes:** Conference rooms, meeting spaces
   - **Equipment mailboxes:** Projectors, vehicles, laptops
   - Integrated with calendar for booking
   - Automatic accept/decline rules

4. **Archive Mailboxes**
   - Additional storage for compliance
   - In-place archiving
   - Requires E3/E5 or archive add-on license

#### Distribution Lists

1. **Distribution Groups**
   - Email to multiple recipients
   - Static membership (manually managed)
   - Use cases: Department lists, project teams

2. **Microsoft 365 Groups**
   - Modern replacement for distribution groups
   - Includes shared mailbox, calendar, files, OneNote, Planner
   - Dynamic membership options
   - Integration with Teams

3. **Mail-Enabled Security Groups**
   - Combine email capability with security permissions
   - Use for both distribution and access control

4. **Dynamic Distribution Groups**
   - Membership based on filter rules (e.g., department=Sales)
   - Automatically updated

**Hands-On:**
- Open Exchange Admin Center: https://admin.exchange.microsoft.com
- Create shared mailbox: Recipients → Mailboxes → Add shared mailbox
- Assign permissions to shared mailbox
- Create distribution list: Recipients → Groups → Add group
- Add members to distribution list
- Test sending email to distribution list

**Common Tasks:**
- Grant "Send As" permission on shared mailbox
- Set mailbox storage quotas
- Enable/disable automatic replies
- Configure mailbox delegation
- Export mailbox to PST

**Documentation:** https://learn.microsoft.com/en-us/exchange/exchange-online

---

### Skill: Identify the appropriate objects to configure by using the SharePoint in Microsoft 365 admin center (sites, libraries, and folders)

**What You Need to Know:**
- SharePoint organizes content into sites, libraries, and folders
- Sites are containers for content and collaboration
- Libraries store documents, media, and other files
- Folders organize files within libraries

**Key Concepts:**

#### SharePoint Sites

1. **Team Sites**
   - Collaboration workspace for teams
   - Automatically created with Microsoft 365 Groups and Teams
   - Includes document library, lists, pages
   - Private by default (members only)

2. **Communication Sites**
   - Broadcast information to broad audience
   - News, announcements, policies
   - One-to-many communication
   - Modern, mobile-friendly design

3. **Hub Sites**
   - Connect related sites
   - Shared navigation and branding
   - Aggregate content across sites
   - Organizational structure

#### Document Libraries
- **Default library:** "Documents" created with every site
- **Custom libraries:** Create for specific content types
- **File storage:** Office docs, PDFs, images, videos
- **Features:**
  - Version history
  - Check-in/check-out
  - Metadata columns
  - Views and filters
  - Content types

#### Folders
- **Traditional organization:** Hierarchical structure
- **Modern alternative:** Metadata and views (preferred)
- **Use cases:** Organize related files
- **Limitations:** Can complicate permissions and search

**SharePoint Structure:**
```
Tenant
└── Site Collection (root)
    ├── Site
    │   ├── Document Library
    │   │   ├── Folder
    │   │   │   └── Files
    │   │   └── Files
    │   └── Lists
    └── Subsites
```

**Hands-On:**
- Open SharePoint Admin Center: https://admin.microsoft.com/sharepoint
- View active sites: Sites → Active sites
- Create site: Create → Team site or Communication site
- Navigate to site
- Create document library: New → Document library
- Create folder within library
- Upload files

**Common Objects:**
- **Lists:** Structured data (tasks, issues, contacts)
- **Pages:** Web pages with web parts
- **Apps:** Extend site functionality

**Documentation:** https://learn.microsoft.com/en-us/sharepoint/

---

### Skill: Identify the appropriate roles and permissions for sites in SharePoint in Microsoft 365

**What You Need to Know:**
- SharePoint uses permission levels assigned to users/groups
- Permission inheritance flows from site to library to folder to file
- Breaking inheritance creates unique permissions

**Key Concepts:**

#### Default Permission Levels

| Permission Level | Capabilities | Typical Use |
|-----------------|--------------|-------------|
| **Full Control** | Complete control, change permissions, delete | Site owners, administrators |
| **Design** | View, add, update, delete, approve, customize | Designers, power users |
| **Edit** | View, add, update, delete items | Team members, contributors |
| **Contribute** | View, add, update, delete own items | Standard users |
| **Read** | View only, download | Read-only users, guests |
| **View Only** | View, cannot download | Highly restricted access |

#### Default SharePoint Groups

1. **[Site Name] Owners**
   - Permission Level: Full Control
   - Can change site settings, permissions
   - Manage site features

2. **[Site Name] Members**
   - Permission Level: Edit
   - Can add/edit/delete content
   - Standard contributors

3. **[Site Name] Visitors**
   - Permission Level: Read
   - Can view content
   - No editing capability

#### Permission Inheritance

```
Site (Full Control)
└── Library (Inherited)
    ├── Folder (Inherited)
    │   └── File (Inherited)
    └── Folder (Unique - Broken inheritance)
        └── File (Inherited from parent folder)
```

**Breaking Inheritance:**
- Site, library, folder, or file can have unique permissions
- "Stop inheriting permissions" breaks link to parent
- Use cases: Confidential folders, HR documents, executive content

**Best Practices:**
- Use groups instead of individual users
- Minimize broken inheritance (complicates management)
- Regular permission audits
- Document permission structure

**Hands-On:**
- Navigate to SharePoint site
- Site Settings → Site permissions
- View permission levels and groups
- Add user to group
- Navigate to library → Library settings → Permissions
- Check if inheriting or unique
- Break inheritance on folder (for testing only)
- Restore inheritance

**Common Scenarios:**
- **Team collaboration:** Members (Edit), Visitors (Read)
- **Department site:** Dept members (Edit), Others (Read)
- **Confidential:** Select users (Contribute), Others (No access)
- **Public news:** Everyone (Read)

**Documentation:** https://learn.microsoft.com/en-us/sharepoint/modern-experience-sharing-permissions

---

### Skill: Identify the appropriate objects to configure by using the Teams admin center (teams, channels, and policies)

**What You Need to Know:**
- Teams Admin Center manages Microsoft Teams environment
- Teams contain channels for organized conversations
- Policies control user capabilities and settings

**Key Concepts:**

#### Teams Structure

**Team:**
- Collaboration workspace for group of people
- Automatically creates Microsoft 365 Group
- Includes:
  - SharePoint site
  - Shared mailbox
  - OneNote notebook
  - Planner board

**Team Types:**
- **Private:** Invitation required to join
- **Public:** Anyone in org can join
- **Org-wide:** Automatic membership for everyone (max 10,000 users)

**Channels:**
- Dedicated sections within a team
- **Standard channels:** Conversations and files
- **Private channels:** Subset of team members, separate SharePoint site
- **Shared channels:** Collaborate with people outside team (even external orgs)

**Example Structure:**
```
Marketing Team (Private)
├── General (default channel)
├── Campaigns (standard channel)
├── Budget (private channel - Finance access only)
└── Agency Collaboration (shared channel - external partners)
```

#### Teams Admin Center Objects

**Teams:**
- View and manage all teams
- Team membership
- Channels within teams
- Settings and policies applied

**Channels:**
- Standard, private, shared channels
- Channel membership (for private/shared)
- Channel moderation settings

**Policies:**

1. **Messaging Policies**
   - Delete sent messages
   - Edit sent messages
   - Use Giphy, stickers, memes
   - Chat permissions

2. **Meeting Policies**
   - Allow Meet Now
   - Allow channel meeting scheduling
   - Allow private meeting scheduling
   - Recording permissions
   - Transcription settings
   - Copilot in meetings

3. **App Policies**
   - Installed apps
   - Pinned apps
   - Custom apps
   - Third-party apps

4. **Calling Policies**
   - Make private calls
   - Call forwarding
   - Voicemail
   - Call groups

5. **Live Events Policies**
   - Schedule live events
   - Recording settings
   - Attendee controls

**Hands-On:**
- Open Teams Admin Center: https://admin.teams.microsoft.com
- Navigate to Teams → Manage teams
- View team details, members, channels
- Navigate to Messaging policies
- Review "Global (Org-wide default)" policy
- Create custom messaging policy
- Assign policy to user or group
- Navigate to Meetings → Meeting policies
- Configure Copilot in Teams meetings setting

**Common Admin Tasks:**
- Create org-wide team
- Configure guest access
- Enable/disable apps
- Set meeting recording permissions
- Control who can create teams

**Documentation:** https://learn.microsoft.com/en-us/microsoftteams/

---

## Section 1.2: Understand the Microsoft 365 Security Principles

### Skill: Explain the core Zero Trust principles

**What You Need to Know:**
- Zero Trust assumes breach and verifies each request
- Replaces "trust but verify" with "never trust, always verify"
- Essential security model for modern cloud environments

**Key Concepts:**

#### Three Core Zero Trust Principles

1. **Verify Explicitly**
   - Always authenticate and authorize
   - Use all available data points: identity, location, device, data classification, anomalies
   - Context-aware access decisions
   - Examples:
     - MFA for all users
     - Conditional Access policies
     - Device compliance checks
     - Risk-based authentication

2. **Use Least Privilege Access**
   - Just-in-time (JIT) access
   - Just-enough-access (JEA)
   - Time-bound permissions
   - Minimize user permissions to only what's needed
   - Examples:
     - Privileged Identity Management (PIM)
     - Role-based access control (RBAC)
     - Regularly review permissions
     - Remove standing admin access

3. **Assume Breach**
   - Minimize blast radius
   - Segment access
   - End-to-end encryption
   - Analytics for threat detection
   - Examples:
     - Network segmentation
     - Micro-segmentation
     - Threat intelligence
     - Continuous monitoring and logging
     - Incident response readiness

#### Zero Trust in Microsoft 365

**Identity:**
- Microsoft Entra ID for identity verification
- Conditional Access for policy enforcement
- MFA for strong authentication
- Risk-based access controls

**Devices:**
- Intune for device management
- Compliance policies
- Conditional Access device controls
- App protection policies

**Applications:**
- Cloud App Security (Defender for Cloud Apps)
- OAuth app governance
- App-based Conditional Access

**Data:**
- Sensitivity labels
- Data Loss Prevention (DLP)
- Information Protection
- Encryption

**Infrastructure:**
- Defender for Endpoint
- Defender for Cloud
- Threat protection

**Network:**
- Private Access
- Internet Access
- Security Service Edge (SSE)

**Zero Trust Maturity Model:**
```
Traditional → Initial → Advanced → Optimal
```

**Hands-On Verification:**
- Review Conditional Access policies: Entra Admin → Protection → Conditional Access
- Check MFA enforcement: Entra Admin → Users → Per-user MFA
- Review device compliance: Intune Admin → Devices → Compliance policies
- Verify least privilege: Entra Admin → Roles and administrators

**Documentation:** https://learn.microsoft.com/en-us/security/zero-trust/zero-trust-overview

---

### Skill: Understand authorization

**What You Need to Know:**
- Authorization determines what authenticated users can access
- Different from authentication (who you are) vs authorization (what you can do)
- Role-Based Access Control (RBAC) is primary authorization model

**Key Concepts:**

#### Authorization vs Authentication

| Authentication | Authorization |
|----------------|---------------|
| **Who** you are | **What** you can do |
| Login, password, MFA | Permissions, roles, policies |
| First step | Second step |
| Identity verification | Access control |

#### Authorization Models in M365

**1. Role-Based Access Control (RBAC)**
- Assign roles to users
- Roles define permissions
- Examples:
  - Global Administrator
  - SharePoint Administrator
  - Exchange Administrator
  - User Administrator

**2. Permission-Based**
- Direct permissions on resources
- SharePoint: Full Control, Edit, Read
- Exchange: Full Access, Send As, Send on Behalf

**3. Attribute-Based Access Control (ABAC)**
- Access based on attributes
- User attributes: Department, Location, Job Title
- Resource attributes: Classification, Sensitivity
- Examples:
  - Conditional Access policies
  - Sensitivity label policies

#### Microsoft Entra Roles (Admin Roles)

**Global Administrator:**
- Full access to all features
- Can reset any user password
- Assign any admin role
- Limit number of Global Admins

**Exchange Administrator:**
- Manage Exchange Online
- Mailboxes, groups, transport rules
- Cannot manage other M365 services

**SharePoint Administrator:**
- Manage SharePoint and OneDrive
- Create/delete sites, manage settings
- Cannot manage Exchange or Teams

**Teams Administrator:**
- Manage Teams service
- Policies, settings, team creation
- Cannot manage underlying SharePoint

**Security Administrator:**
- Manage security features
- Security policies, threat management
- Cannot manage non-security features

**Compliance Administrator:**
- Manage compliance features
- DLP, retention, eDiscovery
- Cannot manage security policies

**Best Practices:**
- Principle of least privilege
- Use specific admin roles (not Global Admin)
- Limit number of Global Admins (max 3-5)
- Use Privileged Identity Management (PIM) for JIT access
- Regular access reviews
- Document role assignments

**Hands-On:**
- Navigate to Entra Admin → Roles and administrators
- View all admin roles
- Click role to see members
- Assign role to user (test environment)
- Check user's permissions in target service

**Documentation:** https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/

---

### Skill: Understand authentication methods

**What You Need to Know:**
- Authentication proves user identity
- Multiple methods available with varying security levels
- Multi-factor authentication (MFA) is critical for security

**Key Concepts:**

#### Authentication Methods in Microsoft 365

**1. Password**
- Traditional username + password
- Weakest method alone
- Vulnerable to phishing, brute force
- Should always combine with MFA

**2. Multi-Factor Authentication (MFA)**
- Requires 2+ verification factors:
  - Something you know (password)
  - Something you have (phone, security key)
  - Something you are (biometrics)

**MFA Methods:**

| Method | Security Level | User Experience | Use Case |
|--------|---------------|-----------------|----------|
| **Microsoft Authenticator App** | High | Push notification or code | Recommended for most users |
| **SMS Text Message** | Medium | Code via text | Fallback option |
| **Phone Call** | Medium | Automated call | Users without smartphones |
| **OATH Hardware Token** | High | Physical device generates code | High-security environments |
| **FIDO2 Security Key** | Highest | Physical USB/NFC key | Passwordless, most secure |
| **Windows Hello** | High | Biometrics or PIN | Windows devices |

**3. Windows Hello for Business**
- Biometric authentication (face, fingerprint)
- Device-based PIN
- Replaces passwords
- Public/private key cryptography

**4. Certificate-Based Authentication**
- X.509 certificates
- Smart cards
- High-security scenarios
- Requires PKI infrastructure

**5. Passwordless Authentication**
- No password needed
- Methods:
  - Microsoft Authenticator (passwordless)
  - FIDO2 security keys
  - Windows Hello for Business
  - Certificate-based

**6. Single Sign-On (SSO)**
- Authenticate once, access multiple apps
- Seamless user experience
- Based on token-based authentication
- Reduces password fatigue

#### Authentication Protocols

**Modern Authentication:**
- OAuth 2.0 and OpenID Connect
- Token-based
- Supports MFA and Conditional Access
- Required for Microsoft 365

**Legacy Authentication:**
- Basic authentication (deprecated)
- No MFA support
- Security risk
- Blocked by default in new tenants

**Hands-On:**
- Entra Admin → Users → Per-user MFA
- View MFA status for users
- Entra Admin → Protection → Authentication methods
- Configure available methods (Authenticator, SMS, FIDO2)
- Set default method
- Enable passwordless authentication
- User self-service: https://mysignins.microsoft.com/security-info

**Common Configurations:**
- Enable Microsoft Authenticator for all users
- Disable SMS (less secure)
- Enable FIDO2 security keys for admins
- Block legacy authentication

**Documentation:** https://learn.microsoft.com/en-us/entra/identity/authentication/concept-authentication-methods

---

### Skill: Understand threat protection and intelligence

**What You Need to Know:**
- Threat protection defends against attacks targeting M365
- Threat intelligence provides insights into attack patterns
- Multiple layers of protection across email, identities, endpoints, data

**Key Concepts:**

#### Microsoft Defender XDR (Extended Detection and Response)

**Integrated Protection:**
- Defender for Office 365 (Email & collaboration)
- Defender for Identity (Identity-based attacks)
- Defender for Endpoint (Devices)
- Defender for Cloud Apps (Cloud applications)
- Unified portal: https://security.microsoft.com

#### Threat Protection Layers

**1. Email Protection (Defender for Office 365)**
- **Anti-phishing:** Detect impersonation and spoofing
- **Anti-spam:** Block unwanted email
- **Anti-malware:** Scan attachments for viruses
- **Safe Attachments:** Detonate files in sandbox
- **Safe Links:** Check URLs at click time
- **Zero-hour auto purge (ZAP):** Remove malicious emails after delivery

**2. Identity Protection (Defender for Identity)**
- Monitor on-premises AD for attacks
- Detect compromised identities
- Lateral movement detection
- Suspicious activities
- Integration with Entra ID Protection

**3. Endpoint Protection (Defender for Endpoint)**
- Antivirus and anti-malware
- Attack surface reduction
- Endpoint detection and response (EDR)
- Automated investigation and remediation
- Threat & vulnerability management

**4. Cloud App Protection (Defender for Cloud Apps)**
- Cloud Access Security Broker (CASB)
- Shadow IT discovery
- OAuth app governance
- App-to-app protection
- Data protection for SaaS apps

#### Threat Intelligence

**Microsoft Threat Intelligence:**
- **Global insights:** 65+ trillion signals per day
- **Research:** Microsoft Security Response Center
- **Threat actors:** Track known threat groups
- **Indicators of Compromise (IoCs):** IPs, domains, file hashes
- **Threat analytics:** Actionable reports

**Threat Intelligence Features:**
- Threat Explorer (Defender for Office 365)
- Threat analytics (Microsoft 365 Defender)
- Advanced hunting (KQL queries)
- Incident investigation
- Threat tracking

**Security Capabilities:**

| Feature | Purpose | Location |
|---------|---------|----------|
| **Attack Simulation** | Train users to recognize phishing | Microsoft 365 Defender → Attack simulation training |
| **Secure Score** | Measure security posture | Microsoft 365 Defender → Secure Score |
| **Incidents** | Correlated alerts | Microsoft 365 Defender → Incidents |
| **Threat Analytics** | Intelligence reports | Microsoft 365 Defender → Threat analytics |
| **Hunting** | Proactive threat search | Microsoft 365 Defender → Hunting |

**Hands-On:**
- Navigate to https://security.microsoft.com
- Review Secure Score
- Check recent incidents and alerts
- Explore Threat analytics
- Email & collaboration → Policies & rules → Threat policies
- Review anti-phishing, anti-spam, anti-malware policies
- Launch Attack simulation training

**Common Threat Scenarios:**
- **Phishing:** Fake emails to steal credentials
- **Business Email Compromise (BEC):** CEO fraud, invoice scams
- **Ransomware:** Encrypt files, demand payment
- **Account takeover:** Compromised credentials
- **Insider threat:** Malicious or negligent insiders
- **Data exfiltration:** Stealing sensitive data

**Documentation:** https://learn.microsoft.com/en-us/microsoft-365/security/

---

### Skill: Understand features and capabilities of Microsoft Defender XDR

**What You Need to Know:**
- Microsoft Defender XDR (Extended Detection and Response) unifies security across M365
- Provides coordinated defense and automated response
- Central portal for all security operations

**Key Concepts:**

#### Microsoft Defender XDR Components

**1. Microsoft Defender for Office 365**
- Plans: Plan 1 (protection), Plan 2 (investigation + response)
- **Protection:**
  - Safe Attachments
  - Safe Links
  - Anti-phishing (impersonation protection)
  - Spoof intelligence
- **Investigation:**
  - Threat Explorer
  - Email entity page
  - Campaign views
- **Response:**
  - Automated Investigation and Response (AIR)
  - Threat remediation

**2. Microsoft Defender for Identity**
- Monitors on-premises Active Directory
- Detects:
  - Compromised credentials
  - Lateral movement attempts
  - Domain dominance attacks (Golden Ticket, etc.)
- Sensor deployment on domain controllers
- Integration with Entra ID Protection

**3. Microsoft Defender for Endpoint**
- Endpoint detection and response (EDR)
- **Features:**
  - Next-gen antivirus
  - Attack surface reduction rules
  - Device isolation
  - Live response (remote shell)
  - Threat & vulnerability management
- Supported platforms: Windows, macOS, Linux, iOS, Android

**4. Microsoft Defender for Cloud Apps**
- Cloud Access Security Broker (CASB)
- **Capabilities:**
  - Discover and control shadow IT
  - Protect sensitive information
  - Protect against cyberthreats
  - Assess compliance
- App connectors for SaaS apps
- OAuth app governance

#### Unified Capabilities

**Incidents:**
- Correlated alerts across products
- Single incident for multi-stage attack
- Attack story visualization
- Automated investigation
- Response actions

**Advanced Hunting:**
- Kusto Query Language (KQL)
- Query across 30 days of data
- Create custom detections
- Proactive threat hunting

**Threat Analytics:**
- Real-time reports on emerging threats
- Analyst reports with mitigations
- Impacted devices and users
- Exposure and recommendations

**Secure Score:**
- Numerical score (0-100%) representing security posture
- Improvement actions with points
- Comparison to benchmarks
- Track progress over time

**Automated Investigation and Response (AIR):**
- Triggered by alerts
- Investigates entities (users, devices, emails, files)
- Determines verdict (malicious, suspicious, clean)
- Recommends or automatically applies remediation
- Action center for approval

**Action Center:**
- Pending actions requiring approval
- History of completed actions
- Unified view across all Defender products

**Microsoft Defender Portal:**
- Unified URL: https://security.microsoft.com
- Single pane of glass
- Role-based access control
- Customizable dashboards

#### Key Features by Plan

| Feature | Defender for Office 365 P1 | Defender for Office 365 P2 |
|---------|---------------------------|---------------------------|
| Safe Attachments | ✅ | ✅ |
| Safe Links | ✅ | ✅ |
| Anti-phishing | ✅ | ✅ |
| Threat Explorer | ❌ | ✅ |
| Automated Investigation | ❌ | ✅ |
| Attack Simulation Training | ❌ | ✅ |
| Threat Trackers | ❌ | ✅ |

**Hands-On:**
- Navigate to https://security.microsoft.com
- Explore Home dashboard
- View Incidents & alerts
- Check Secure Score and improvement actions
- Email & collaboration → Threat Explorer (if P2)
- Assets → Devices (Defender for Endpoint)
- Assets → Identities (Defender for Identity)
- Cloud apps (Defender for Cloud Apps)
- Advanced hunting → Run query
- Action center → Pending actions

**Common Use Cases:**
- Investigate phishing email: Threat Explorer → Email entity page
- Respond to ransomware: Incident → Automated investigation → Device isolation
- Hunt for threats: Advanced hunting → Query for suspicious PowerShell
- Improve posture: Secure Score → Implement actions
- Test security: Attack simulation training → Launch phishing simulation

**Documentation:** https://learn.microsoft.com/en-us/microsoft-365/security/defender/

---

## Section 1.3: Identify the Core Security Features of Microsoft 365 Services

### Skill: Understand features and capabilities of Microsoft Entra

**What You Need to Know:**
- Microsoft Entra (formerly Azure AD) is the identity and access management service
- Central to all M365 security
- Provides authentication, authorization, and identity protection

**Key Concepts:**

#### Microsoft Entra ID Core Features

**1. Identity Management**
- **Users:** Individual identities with credentials
- **Groups:**
  - Security groups (access control)
  - Microsoft 365 Groups (collaboration)
  - Dynamic groups (rule-based membership)
  - Assigned groups (manual membership)
- **Service principals:** Application identities
- **Managed identities:** For Azure resources

**2. Authentication Services**
- User authentication
- Multi-factor authentication (MFA)
- Self-service password reset (SSPR)
- Password protection (banned passwords)
- Smart lockout (brute force protection)

**3. Conditional Access**
- Policy-based access control
- Conditions: User, location, device, app, risk
- Controls: Block, require MFA, require compliant device, etc.

**4. Single Sign-On (SSO)**
- Access multiple apps with one login
- Support for SAML, OAuth, OpenID Connect, WS-Fed
- Enterprise app gallery (thousands of pre-integrated apps)
- Custom app integration

**5. Identity Protection**
- **Risk detections:**
  - User risk: Leaked credentials, unusual behavior
  - Sign-in risk: Atypical travel, anonymous IP, malware-linked IP
- **Risk-based Conditional Access:**
  - Require MFA for medium/high sign-in risk
  - Block or require password change for high user risk
- **Investigation:**
  - Risky users report
  - Risky sign-ins report
  - Risk detections report

**6. Privileged Identity Management (PIM)**
- Just-in-time admin access
- Time-bound role assignments
- Approval workflow for activation
- Access reviews
- Audit trail

**7. Identity Governance**
- **Entitlement Management:**
  - Access packages
  - Automated provisioning/deprovisioning
  - Guest access lifecycle
- **Access Reviews:**
  - Periodic review of group memberships
  - Application assignments
  - Admin role assignments
- **Lifecycle Workflows:**
  - Automate joiner/mover/leaver processes
  - Pre-hire, onboarding, offboarding tasks

**8. B2B Collaboration (Guest Access)**
- Invite external users
- Guest accounts in your directory
- Controlled access to resources
- Cross-tenant collaboration

**9. B2C (Customer Identity)**
- Consumer-facing applications
- Social identity providers
- Custom branding
- Separate from B2B

#### Microsoft Entra ID Editions

| Feature | Free | P1 | P2 |
|---------|------|----|----|
| Users and groups | ✅ | ✅ | ✅ |
| SSO | ✅ | ✅ | ✅ |
| Self-service password reset | Cloud only | ✅ Hybrid | ✅ Hybrid |
| Conditional Access | ❌ | ✅ | ✅ |
| PIM | ❌ | ❌ | ✅ |
| Identity Protection | ❌ | ❌ | ✅ |
| Access Reviews | ❌ | ❌ | ✅ |

**Microsoft Entra Suite:**
- Entra ID P2
- Entra ID Governance
- Entra Private Access
- Entra Internet Access
- Entra Permissions Management
- Entra Verified ID

**Hands-On:**
- Navigate to https://entra.microsoft.com
- Identity → Users → All users
- Identity → Groups → All groups
- Protection → Conditional Access
- Protection → Identity Protection
- Identity Governance → PIM
- Applications → Enterprise applications
- Review sign-in logs: Monitoring → Sign-in logs
- Check audit logs: Monitoring → Audit logs

**Common Admin Tasks:**
- Create user: Identity → Users → New user
- Create group: Identity → Groups → New group
- Assign app to user: Applications → Enterprise apps → Select app → Users and groups
- Configure SSPR: Protection → Password reset
- Review risky sign-ins: Protection → Identity Protection → Risky sign-ins

**Documentation:** https://learn.microsoft.com/en-us/entra/fundamentals/

---

### Skill: Understand conditional access policies

**What You Need to Know:**
- Conditional Access is policy-based access control
- "If-then" statements: IF user tries to access resource, THEN apply controls
- Critical for Zero Trust implementation

**Key Concepts:**

#### Conditional Access Policy Structure

**Assignments (Conditions):**
```
IF User/Group
AND Cloud app/action
AND Conditions:
  - User risk level
  - Sign-in risk level
  - Device platform
  - Location
  - Client apps
  - Device state
```

**Access Controls (Then):**
```
THEN Grant OR Block
  - Require MFA
  - Require compliant device
  - Require hybrid Azure AD joined device
  - Require app protection policy
  - Require password change
  - Block access
```

#### Policy Components in Detail

**1. Users and Groups**
- **Include:**
  - All users
  - Select users and groups
  - Guest and external users
- **Exclude:**
  - Emergency access accounts (break-glass)
  - Service accounts
  - Specific users/groups

**2. Cloud Apps or Actions**
- **All cloud apps** (not recommended for first policy)
- **Select apps:** Office 365, Azure Management, etc.
- **User actions:** Register security information, Join devices

**3. Conditions**

**Sign-in risk (requires Entra ID P2 & Identity Protection):**
- No risk, Low, Medium, High
- Based on real-time and offline detection

**Device platforms:**
- Android, iOS, Windows, macOS, Linux
- Use case: Block Linux devices from accessing finance data

**Locations:**
- Named locations (trusted IPs)
- Countries/regions
- All locations
- Use case: Block access from non-trusted countries

**Client apps:**
- Browser
- Mobile apps and desktop clients
- Exchange ActiveSync
- Other clients (legacy auth)

**Device state:**
- Compliant (Intune)
- Hybrid Azure AD joined
- Use case: Only allow compliant devices

**4. Grant Controls**

**Grant access with requirements:**
- Require MFA
- Require device to be marked as compliant
- Require hybrid Azure AD joined device
- Require approved client app
- Require app protection policy
- Require password change

**Require multiple controls:**
- Require ALL selected (most restrictive)
- Require ONE of selected

**5. Session Controls**
- Use app-enforced restrictions
- Use Conditional Access App Control
- Sign-in frequency
- Persistent browser session
- Customize continuous access evaluation

#### Common Conditional Access Policies

**1. Require MFA for all users:**
- Users: All users (exclude break-glass)
- Apps: All cloud apps
- Grant: Require MFA

**2. Require MFA for admins:**
- Users: Directory roles (Global Admin, etc.)
- Apps: All cloud apps
- Grant: Require MFA

**3. Block legacy authentication:**
- Users: All users
- Apps: All cloud apps
- Conditions: Client apps → Other clients
- Grant: Block access

**4. Require compliant device:**
- Users: All users
- Apps: Office 365
- Grant: Require compliant device OR Require hybrid Azure AD joined

**5. Require MFA from untrusted locations:**
- Users: All users
- Apps: All cloud apps
- Conditions: Locations → Any location, Exclude trusted locations
- Grant: Require MFA

**6. Block high-risk sign-ins:**
- Users: All users
- Apps: All cloud apps
- Conditions: Sign-in risk → High
- Grant: Block

**Policy Modes:**
- **Report-only:** Test policy without enforcement (see What If results)
- **On:** Policy enforced
- **Off:** Policy disabled

**What If Tool:**
- Test policy impact before enabling
- Entra Admin → Protection → Conditional Access → What If
- Specify user, app, conditions
- See which policies would apply

**Hands-On:**
- Navigate to Entra Admin → Protection → Conditional Access
- Review existing policies
- Click policy to see configuration
- Use "What If" tool: What If → Select user and app → What If
- Create new policy (report-only mode):
  - Conditional Access → New policy
  - Name: Test - Require MFA for executives
  - Users: Select executive group
  - Cloud apps: All cloud apps
  - Grant: Require MFA
  - Enable policy: Report-only mode
  - Create
- Monitor report-only: Sign-in logs → Filter by Conditional Access → Report-only

**Best Practices:**
- Always exclude emergency access (break-glass) accounts
- Start with report-only mode
- Use What If tool before enabling
- Document all policies
- Regular review and cleanup
- Layer policies (e.g., baseline + app-specific)

**Documentation:** https://learn.microsoft.com/en-us/entra/identity/conditional-access/

---

### Skill: Understand the purpose and benefits of SSO

**What You Need to Know:**
- Single Sign-On (SSO) allows users to sign in once and access multiple applications
- Improves user experience and security
- Reduces password fatigue and help desk calls

**Key Concepts:**

#### What is SSO?

**Definition:**
- Authenticate once with identity provider (Microsoft Entra ID)
- Access multiple applications without re-entering credentials
- Based on trust relationship between identity provider and applications

**How SSO Works:**
1. User navigates to application (e.g., Salesforce)
2. App redirects to Microsoft Entra ID
3. User authenticates (if not already)
4. Entra ID issues security token
5. User redirected back to app with token
6. App validates token and grants access
7. Subsequent apps: Token reused, no re-authentication needed

**SSO Flow:**
```
User → App 1 → Entra ID (authenticate) → Token → App 1 (access)
User → App 2 → Entra ID (already authenticated) → Token → App 2 (access)
User → App 3 → Entra ID (already authenticated) → Token → App 3 (access)
```

#### Benefits of SSO

**For Users:**
- **One set of credentials:** Remember one password instead of many
- **Seamless access:** Switch between apps without re-authenticating
- **Faster access:** No repeated login prompts
- **Better security hygiene:** One strong password vs. many weak ones
- **Reduced password fatigue:** Less likely to write down passwords

**For IT/Admins:**
- **Reduced help desk calls:** Fewer password reset requests
- **Centralized access control:** Manage access in one place
- **Better security:** Enforce MFA and policies centrally
- **Audit trail:** Single source for access logs
- **Faster onboarding/offboarding:** Provision/deprovision once
- **Compliance:** Centralized identity governance

**For Organization:**
- **Cost savings:** Reduced IT support costs
- **Improved productivity:** Less time on authentication
- **Enhanced security posture:** Stronger authentication methods
- **Regulatory compliance:** Better access controls and audit logs

#### SSO in Microsoft 365

**Built-in SSO:**
- All Microsoft 365 apps use Entra ID SSO by default:
  - Outlook, Teams, SharePoint, OneDrive, Word, Excel, PowerPoint, etc.
- Sign in once, access all M365 apps

**Third-Party App SSO:**
- **Enterprise App Gallery:** 5,000+ pre-integrated SaaS apps
  - Salesforce, Dropbox, ServiceNow, Workday, SAP, etc.
- **SAML-based SSO**
- **OAuth 2.0 / OpenID Connect**
- **Password-based SSO** (less secure, legacy apps)
- **Linked SSO** (bookmark)

#### SSO Authentication Protocols

**1. SAML 2.0 (Security Assertion Markup Language)**
- XML-based
- Industry standard
- Use case: Enterprise SaaS apps
- Flow: Service Provider-initiated or Identity Provider-initiated

**2. OAuth 2.0 + OpenID Connect (OIDC)**
- Modern, token-based
- JSON Web Tokens (JWT)
- Use case: Modern web and mobile apps
- Microsoft's preferred protocol

**3. WS-Federation**
- Legacy protocol
- Still supported for older apps

**4. Password-based SSO (Password Vaulting)**
- Entra ID stores encrypted credentials
- Auto-fills login forms
- Less secure, use only when SAML/OIDC not available

#### Configuring SSO

**For Gallery Apps:**
1. Entra Admin → Enterprise applications → New application
2. Browse Azure AD Gallery → Search for app (e.g., "Salesforce")
3. Add application
4. Set up single sign-on → Select SAML
5. Follow guided setup:
   - Basic SAML configuration (URLs)
   - User attributes & claims
   - SAML certificate
   - Set up application (app-side config)
6. Assign users/groups
7. Test SSO

**For Custom Apps:**
1. Enterprise applications → New application → Create your own
2. Integrate any other application not in the gallery
3. Configure SSO manually with app's SAML/OIDC settings

#### Seamless SSO (Windows)

**For Domain-Joined Windows Devices:**
- Automatic sign-in to Entra ID using on-prem AD credentials
- No password prompt for Entra ID authentication
- Windows Hello for Business integration
- Primary Refresh Token (PRT)

**Hands-On:**
- Navigate to Entra Admin → Enterprise applications → All applications
- View apps configured for SSO
- Click app → Single sign-on → Review configuration
- View assigned users: Users and groups
- Test SSO: Click "Test" in SSO settings
- User experience: https://myapps.microsoft.com (all SSO apps)

**User Portal:**
- **My Apps:** https://myapps.microsoft.com
- Single portal for all SSO-enabled apps
- Organized collections
- Self-service access request (if enabled)

**Common Scenarios:**
- **Salesforce SSO:** Sales team accesses Salesforce with M365 credentials
- **ServiceNow SSO:** IT team accesses ServiceNow without separate login
- **Custom LOB app:** Internal HR app uses Entra ID for authentication

**Documentation:** https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/what-is-single-sign-on

---

### Skill: Identify the appropriate security object to use in an organization (users and groups)

**What You Need to Know:**
- Users and groups are fundamental security objects in M365
- Groups simplify permission management
- Different group types serve different purposes

**Key Concepts:**

#### User Types

**1. Member Users (Internal)**
- Employees of organization
- Full user accounts in Entra ID
- Source: Cloud-only or synced from on-prem AD
- User Principal Name (UPN): user@contoso.com
- Licenses assigned directly or via group

**2. Guest Users (External)**
- Partners, vendors, contractors
- B2B collaboration
- User type: Guest
- UPN: externaluser_vendor.com#EXT#@contoso.onmicrosoft.com
- Limited permissions by default
- Invitation required

**3. Service Accounts**
- Non-human identities
- Automation, applications, scripts
- Should NOT use MFA (use managed identities or certificates instead)
- Example: Application accounts, sync accounts

#### Group Types

**1. Security Groups**
- **Purpose:** Access control, permission assignment
- **Members:** Users, devices, service principals, other groups (nested)
- **Membership:**
  - **Assigned:** Manual membership
  - **Dynamic:** Rule-based (e.g., department=Sales)
- **Use cases:**
  - SharePoint site permissions
  - App access
  - Conditional Access policies
  - License assignment
- **Email-enabled:** Optional (mail-enabled security group)

**2. Microsoft 365 Groups (Unified Groups)**
- **Purpose:** Collaboration
- **Includes:**
  - Shared mailbox
  - SharePoint site
  - Planner
  - OneNote
  - Calendar
  - Teams (if Teams-connected)
- **Membership:** Users only (not devices or groups)
- **Visibility:**
  - Public: Anyone can join
  - Private: Invitation required
- **Use cases:**
  - Project teams
  - Department collaboration
  - Community groups

**3. Distribution Groups**
- **Purpose:** Email distribution only
- **Members:** Users, contacts, other distribution groups
- **No security permissions**
- **Use cases:**
  - Department mailing lists
  - Company-wide announcements
  - Legacy email distribution

**4. Mail-Enabled Security Groups**
- **Purpose:** Email + Security
- **Combines:** Distribution group + Security group
- **Use cases:**
  - Email AND resource access (e.g., legal-team@contoso.com has email and SharePoint permissions)

#### Dynamic Groups (Entra ID P1/P2)

**Dynamic User Groups:**
- Membership based on user attributes
- **Rules:**
  ```
  user.department -eq "Sales"
  user.country -eq "United States"
  user.jobTitle -contains "Manager"
  ```
- Automatically add/remove based on rule
- Updates within minutes to hours

**Dynamic Device Groups:**
- Membership based on device attributes
- **Rules:**
  ```
  device.deviceOSType -eq "Windows"
  device.managementType -eq "MDM"
  ```
- Use case: Device management policies

**Rule Builder:**
- Simple or advanced mode
- AND/OR logic
- Validation before saving

#### When to Use Each

| Scenario | Recommended Object |
|----------|-------------------|
| Grant SharePoint site access to team | Security Group (Assigned) |
| Project collaboration workspace | Microsoft 365 Group → Teams |
| All sales department members (auto) | Security Group (Dynamic) |
| Company-wide email announcements | Distribution Group |
| Legal team email + document access | Mail-Enabled Security Group |
| External partner access to specific files | Guest User + Security Group |
| Conditional Access for executives | Security Group (Assigned - critical users) |
| License assignment to department | Security Group (Dynamic) |

#### Best Practices

**Users:**
- Naming convention: firstname.lastname@domain
- Populate all relevant attributes (department, manager, title)
- Use guest access for external users (don't create member accounts)
- Disable accounts immediately when employees leave
- Regular access reviews

**Groups:**
- **Prefer groups over individual permissions**
- Descriptive naming: `SG-SharePoint-Finance-Owners`, `M365-Marketing-Team`
- Document group purpose in description
- Use dynamic groups for department-wide access
- Regular group membership reviews
- Limit number of group owners
- Nested groups sparingly (complicates troubleshooting)

**Security:**
- Principle of least privilege
- Use security groups for permissions
- Use M365 groups for collaboration
- Don't use distribution groups for security
- Monitor guest access

**Hands-On:**
- Entra Admin → Identity → Users → All users
- View user types (filter: User type = Guest)
- Click user → View properties, group memberships
- Create user: New user → Create new user
- Entra Admin → Identity → Groups → All groups
- Filter by group type
- Create security group: New group → Security → Assigned
- Create dynamic security group: New group → Security → Dynamic user → Add dynamic query
- Create M365 group: New group → Microsoft 365
- View group members and owners
- Test adding user to group
- Verify user sees new access (e.g., SharePoint site)

**Common Admin Tasks:**
- Bulk user creation: Users → Bulk operations → Bulk create
- Add guest: Users → New user → Invite external user
- Assign group to app: Enterprise applications → Select app → Users and groups → Add user/group
- License via group: Groups → Select group → Licenses → Assignments

**Documentation:**
- Users: https://learn.microsoft.com/en-us/entra/fundamentals/add-users
- Groups: https://learn.microsoft.com/en-us/entra/fundamentals/concept-learn-about-groups

---

*[Due to length limits, I'll continue with the remaining skills in the next message]*

Would you like me to continue with the remaining skills? I have:
- Remaining Domain 1 skills (troubleshooting, Identity Secure Score, audit logs, PIM, App registrations)
- All of Domain 2 (Data Protection and Governance - 35-40%)
- All of Domain 3 (Copilot and Agent Administration - 25-30%)