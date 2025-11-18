# Segment 3: Copilot Administration - Official Resources

## Official Microsoft Documentation

### Microsoft 365 Copilot Overview
- **Main Copilot Documentation Hub**
  - https://learn.microsoft.com/en-us/copilot/microsoft-365/
  - Comprehensive resource for Copilot features, setup, and administration
  - Described as "Your AI assistant for work and school"
  - Embedded in apps you use daily, connected to work data
  - Enterprise-grade security, privacy, and compliance

- **Microsoft 365 Copilot Product Page**
  - https://www.microsoft.com/microsoft-365-copilot
  - Product overview, pricing, and plans

### Copilot Setup and Deployment
- **Microsoft 365 Copilot Setup Guide**
  - https://learn.microsoft.com/en-us/copilot/microsoft-365/microsoft-365-copilot-setup
  - Complete deployment framework with three phases:
    - **Get ready:** Deploying Copilot
    - **Drive adoption:** Workforce preparation
    - **Deliver impact:** Measuring usage and performance

- **Deployment Components:**
  1. **Prerequisites and Roles**
     - Access to M365 admin center, SharePoint admin center, Purview portal
     - Required admin roles vary by task

  2. **Pre-Deployment Readiness**
     - Test environment establishment
     - Pilot testing with selected users
     - Communication strategy development
     - Conditional access policy review
     - SharePoint Advanced Management implementation
     - Network requirements validation

  3. **Security Implementation**
     - **MFA:** Enable for all users through admin center
     - **Conditional Access:** Configure based on user risk and device compliance
     - **Audit Logging:** Enable unified audit logging in Purview
     - **Data Protection:** Identify high-risk sites, restrict access, implement controls

  4. **Deployment Steps:**
     - **Update Channels:** Use Current or Monthly Enterprise Channel (not Semi-Annual)
     - **License Assignment:** Via M365 admin center (individual or groups)
     - **Configuration:** Copilot Control System in admin center
     - **Phased Rollout:**
       - Pilot: High-engagement early adopters
       - Deployment: Org-wide with oversharing prevention
       - Operations: Monitor via Copilot Dashboard

### Licensing
- **Microsoft 365 Copilot Licensing**
  - https://learn.microsoft.com/en-us/copilot/microsoft-365/microsoft-365-copilot-licensing
  - **Add-on License:** Copilot requires base M365 subscription
  - **Prerequisites:**
    - Microsoft 365 E3, E5
    - Microsoft 365 Business Standard, Business Premium
    - Office 365 E1, E3, E5
    - Various Teams, Exchange, SharePoint, OneDrive plans
    - Government and Education tiers

- **License Assignment:**
  - Through Microsoft 365 admin center
  - Individual assignment: Users → Active users → Select → Licenses
  - Group-based assignment for bulk deployment
  - 24-hour activation time after assignment

- **Licensing Models:**
  - **Monthly subscription:** Traditional per-user monthly fee
  - **Pay-as-you-go:** Usage-based billing (Azure-backed)

### Copilot Product Options
- **Copilot Chat**
  - Secure AI chat experience
  - Grounded in web data and work files
  - Available via M365.cloud.microsoft/chat

- **Microsoft 365 Copilot**
  - Productivity tool with organizational data
  - Embedded in Word, Excel, PowerPoint, Outlook, Teams, Loop
  - Microsoft 365 Chat (cross-app assistant)

- **Agents**
  - Customizable extensions
  - Perform tasks and use tools
  - Integration with external systems

### Copilot Administration Settings
- **Copilot Control Center** (in M365 Admin Center)
  - License status management
  - Security controls configuration
  - Plugin governance
  - Data grounding settings
  - Feature enablement/disablement

- **Admin Controls:**
  - **Copilot Toggle:** Enable/disable Copilot for tenant or users
  - **Web Search:** Control internet access in Copilot
  - **Plugins:** Manage Copilot extensibility
  - **Data Sharing:** Control optional data sharing settings

- **Policy Configuration Methods:**
  - Cloud Policy for Microsoft 365
  - Group Policy (on-premises AD)
  - Intune policies (mobile devices)
  - Conditional Access policies

### Copilot Security and Governance
- **Data Protection:**
  - Copilot operates within existing security boundaries
  - Respects user permissions (no privilege elevation)
  - Honors sensitivity labels
  - Subject to DLP policies
  - No data used for foundation model training
  - Tenant boundary enforcement

- **Audit Logging:**
  - Unified audit log captures Copilot activities
  - eDiscovery support
  - Legal hold capabilities
  - Data retention controls

- **Ethical AI Principles:**
  - Fairness, reliability, safety
  - Privacy and security
  - Inclusiveness
  - Transparency
  - Accountability

### Usage Monitoring and Analytics
- **Copilot Dashboard in Viva Insights**
  - https://learn.microsoft.com/en-us/viva/insights/org-team-insights/copilot-dashboard
  - Available to all M365 customers with Exchange Online
  - No Viva Insights or Copilot license required for viewing
  - Full capabilities require 50+ licenses

- **Four Metric Categories:**
  1. **Readiness**
     - Total licenses purchased
     - Assigned licenses
     - Active users

  2. **Adoption**
     - User engagement across M365 apps
     - Active users: "Completed at least one Copilot action in previous 28 days"
     - App-specific usage (Teams, Outlook, Word, Excel, PowerPoint)

  3. **Impact**
     - Copilot assisted hours
     - Value generated through AI assistance
     - Time savings metrics

  4. **Sentiment**
     - User satisfaction surveys
     - Feedback collection

- **Data Refresh:**
  - Previous 28 days with up to 6-day delay
  - Filter by organizational attributes (department, function, hierarchy)
  - Access controls via Entra ID roles

- **Microsoft 365 Usage Reports:**
  - Admin center → Reports → Usage
  - Copilot activity reports
  - User activity insights
  - App-specific metrics

### Copilot Experiences by Application

#### Copilot in Word
- Document drafting and writing assistance
- Content rewriting and tone adjustment
- Summarization of long documents
- Content generation from prompts

#### Copilot in Excel
- Data analysis and insights
- Formula generation and explanation
- Pivot table creation
- Chart and visualization suggestions
- Natural language queries

#### Copilot in PowerPoint
- Presentation creation from prompts
- Slide design and layout suggestions
- Content generation from documents
- Image and visual recommendations

#### Copilot in Outlook
- Email drafting and composition
- Email thread summarization
- Meeting preparation and briefs
- Action item extraction

#### Copilot in Teams
- Meeting recap and summaries
- Key decisions and action items
- Chat thread summarization
- Call summaries and notes
- Follow-up task generation

#### Microsoft 365 Chat (Business Chat)
- Cross-application AI assistant
- Query across emails, documents, meetings, chats
- Project status summaries
- Information synthesis from multiple sources

#### Copilot in Loop
- Collaborative workspace assistance
- Content generation in Loop pages
- Team collaboration support

## Microsoft Learn Training Modules

### Core Copilot Training
- **Introduction to Microsoft 365 Copilot**
  - https://learn.microsoft.com/en-us/training/modules/introduction-microsoft-365-copilot/
  - **Learning Objectives:**
    - Describe purpose and functionalities
    - Outline working principles
    - Identify core components
    - Understand responsible AI commitment

  - **Module Units (7 total):**
    1. Introduction
    2. What is Microsoft 365 Copilot?
    3. Explore how Microsoft 365 Copilot works
    4. Explore the core components
    5. Examine Microsoft's responsible AI commitment
    6. Module assessment
    7. Summary

  - **Target Audience:** Administrators, business owners, users
  - **Level:** Beginner
  - **Prerequisites:** None

### Adoption and Training
- **Microsoft 365 Copilot Adoption Resources**
  - https://adoption.microsoft.com/copilot/
  - User training materials
  - Admin guidance
  - Champions program resources

## Hands-On Practice

### Lab Scenarios

#### Lab 1: Verify Copilot Prerequisites
1. Check Microsoft 365 app versions (Current or Monthly Enterprise Channel)
2. Verify base license assignments (E3/E5 or Business)
3. Confirm OneDrive provisioning for all users
4. Review network connectivity requirements
5. Validate security and compliance settings
6. Check conditional access policies

#### Lab 2: Assign Copilot Licenses
1. Access Microsoft 365 admin center
2. Navigate to Billing → Licenses
3. Select Copilot for Microsoft 365
4. Assign to pilot users (individual or group)
5. Verify assignment in user properties
6. Document 24-hour activation wait time
7. Communicate to pilot users

#### Lab 3: Configure Copilot Settings
1. Access Copilot Control Center in admin center
2. Review tenant-wide Copilot settings
3. Configure web search (enable/disable)
4. Manage plugin permissions
5. Set data sharing preferences
6. Apply Cloud Policy for user-specific controls
7. Test setting inheritance

#### Lab 4: Test Copilot Across Apps
1. **Word:** Draft document from prompt
2. **Excel:** Analyze sample data, create formulas
3. **PowerPoint:** Generate presentation
4. **Outlook:** Compose email, summarize thread
5. **Teams:** Test meeting recap, chat summary
6. **Microsoft 365 Chat:** Cross-app query
7. Document user experience and feedback

#### Lab 5: Monitor Copilot Usage
1. Navigate to Viva Insights Copilot Dashboard
2. Review readiness metrics
3. Analyze adoption across apps
4. Measure impact (assisted hours)
5. Check sentiment scores
6. Export usage data
7. Create adoption report for leadership

#### Lab 6: Implement Copilot Security
1. Enable MFA for all users
2. Configure conditional access for Copilot
3. Enable audit logging in Purview
4. Review Copilot audit events
5. Test DLP policies with Copilot
6. Verify sensitivity label respect
7. Document security posture

#### Lab 7: Phased Rollout
1. Identify pilot users (champions, power users)
2. Assign initial licenses (10-50 users)
3. Provide pilot user training
4. Collect feedback (surveys, interviews)
5. Adjust policies based on learnings
6. Expand to department (100-500 users)
7. Monitor adoption and iterate
8. Plan organization-wide rollout

## AB-900 Exam Focus Areas

### Domain 3: Copilot and Agent Administration (25-30%)

**Critical Topics:**

- [ ] **Licensing Models**
  - Monthly subscription vs. pay-as-you-go
  - License prerequisites (M365 E3/E5, Business)
  - License assignment procedures (individual, group, PowerShell)
  - 24-hour activation delay

- [ ] **Feature Management**
  - Enable/disable Copilot features
  - Configure web search capabilities
  - Manage plugins
  - Set data sharing preferences

- [ ] **Agent Use Cases**
  - **Researcher agents:** Information gathering, research tasks
  - **Analyst agents:** Data analysis, insights generation
  - **Custom agents:** Organization-specific scenarios

- [ ] **Billing Policy Management**
  - Configure pay-as-you-go billing
  - Set spending limits
  - Monitor usage and costs

- [ ] **Usage Monitoring**
  - Copilot Dashboard in Viva Insights
  - Readiness metrics (licenses, active users)
  - Adoption tracking (app-specific usage)
  - Impact measurement (assisted hours)
  - Sentiment collection

- [ ] **Prompt Management**
  - Effective prompt engineering
  - Create prompt libraries
  - Share prompt examples

- [ ] **Agent Administration**
  - Agent creation and configuration
  - Agent approval processes
  - Agent governance

**Key Concepts to Master:**

1. **Copilot Architecture**
   - LLM + Microsoft Graph + Semantic Index + Data
   - Real-time orchestration
   - Permission-based data access

2. **Deployment Phases**
   - Readiness → Pilot → Phased → Organization-wide

3. **Licensing Requirements**
   - Base license (M365 E3/E5 or Business)
   - + Copilot add-on
   - + OneDrive provisioned

4. **Admin Centers**
   - M365 Admin: License assignment, Copilot settings
   - Purview: Security and compliance
   - SharePoint Admin: Content governance
   - Viva Insights: Usage dashboard

5. **Security Model**
   - Copilot = User permissions (no elevation)
   - Respects labels and DLP
   - No training on your data
   - Tenant isolation

## Prompt Engineering Best Practices

### Effective Prompt Principles
1. **Be Specific:** Provide clear, detailed requests
2. **Give Context:** Include background information
3. **Set Expectations:** Specify format, length, tone
4. **Iterate:** Refine based on results
5. **Break Down:** Split complex tasks into steps

### Prompt Examples by App

**Word:**
- "Create a 2-page proposal for remote work expansion including benefits, challenges, and implementation timeline"
- "Summarize this 10-page document in bullet points, focusing on action items"
- "Rewrite this section in a more formal tone suitable for executives"

**Excel:**
- "Analyze Q4 sales data and identify top 5 performing products"
- "Create a pivot table showing revenue by region and product category"
- "Explain what this VLOOKUP formula does and suggest improvements"

**PowerPoint:**
- "Create a 10-slide presentation about our Q1 results using a professional theme"
- "Add relevant images to slides about sustainability initiatives"
- "Summarize this Word document into a 5-slide presentation"

**Outlook:**
- "Draft a polite response declining the meeting due to scheduling conflict"
- "Summarize this email thread and identify action items assigned to me"
- "Prepare me for tomorrow's budget meeting by summarizing relevant emails"

**Teams:**
- "Summarize key decisions from today's project meeting"
- "What were the action items assigned to me this week?"
- "Create a recap of yesterday's standup meeting"

**Microsoft 365 Chat:**
- "What are the latest updates on Project Phoenix across all my emails and Teams chats?"
- "Create a status report on customer requests from the past week"
- "Find all documents related to the Q4 budget review"

## Copilot Readiness Checklist

### Technical Prerequisites
- [ ] Base licenses assigned (M365 E3/E5 or Business Standard/Premium)
- [ ] Copilot licenses acquired
- [ ] Users have OneDrive provisioned
- [ ] Microsoft 365 apps updated to Current or Monthly Enterprise Channel
- [ ] Browser compatibility verified
- [ ] Network requirements validated

### Security and Compliance
- [ ] Data governance policies in place
- [ ] DLP policies configured
- [ ] Sensitivity labels deployed
- [ ] Audit logging enabled
- [ ] MFA enabled for all users
- [ ] Conditional access policies reviewed
- [ ] Security baseline established

### Deployment Planning
- [ ] Pilot users identified
- [ ] Success metrics defined
- [ ] Training materials prepared
- [ ] Communication plan ready
- [ ] Support process established
- [ ] Feedback mechanism created
- [ ] Timeline developed

### Post-Deployment
- [ ] Monitor Copilot Dashboard regularly
- [ ] Collect user feedback
- [ ] Track adoption metrics
- [ ] Measure impact and ROI
- [ ] Iterate on policies and training
- [ ] Expand to additional users
- [ ] Share best practices

## Tools and Portals

| Tool | URL | Purpose |
|------|-----|---------|
| M365 Admin Center | https://admin.microsoft.com/ | License assignment, settings |
| Copilot Dashboard | admin.microsoft.com/Adminportal/Home#/copilot | Usage analytics |
| Microsoft 365 Chat | https://m365.cloud.microsoft/chat | Cross-app Copilot |
| Cloud Policy | https://config.office.com/ | Policy management |
| Viva Insights | insights.viva.office.com | Adoption metrics |
| Adoption Resources | https://adoption.microsoft.com/copilot/ | Training materials |

## Additional Resources

### Community
- **Microsoft 365 Copilot Tech Community**
  - https://techcommunity.microsoft.com/t5/microsoft-365-copilot/bd-p/Microsoft365Copilot
  - Forums, discussions, announcements

- **Microsoft 365 Community (PnP)**
  - https://aka.ms/m365pnp
  - Community resources and samples

### Blogs
- **Microsoft 365 Blog - Copilot**
  - https://techcommunity.microsoft.com/t5/microsoft-365-blog/bg-p/microsoft_365blog
  - Product updates and best practices

### Videos
- **Microsoft Mechanics**
  - https://www.youtube.com/c/MicrosoftMechanics
  - Technical demos and deep dives

---

**Related Segments:**
- [Segment 1: Core M365 Services](../../segment-01-core-m365-services/)
- [Segment 2: Data Protection and Governance](../../segment-02-data-protection-governance/)
- [Segment 4: Agents and Exam Prep](../../segment-04-agents-exam-prep/)
