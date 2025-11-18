# Segment 2: Data Protection and Governance - Official Resources

## Official Microsoft Documentation

### Microsoft Purview Overview
- **Microsoft Purview Main Page**
  - https://learn.microsoft.com/en-us/purview/
  - Comprehensive data governance, security, and compliance portfolio
  - Unified platform for information protection, DLP, insider risk, and more

- **Microsoft Purview Compliance Portal**
  - https://compliance.microsoft.com/
  - Central hub for all compliance and governance activities

### Information Protection
- **Sensitivity Labels Overview**
  - Create and apply classification labels to data
  - Configure encryption and access controls
  - Implement automatic labeling rules
  - Label inheritance and propagation

- **Data Classification**
  - **Content Explorer:** View labeled content
  - **Activity Explorer:** Monitor labeling activities
  - **Trainable Classifiers:** ML-based content classification
  - **Sensitive Information Types:** Pre-built and custom patterns

### Data Loss Prevention (DLP)
- **Microsoft Purview DLP Overview**
  - Monitor and prevent accidental data leaks
  - Cross-platform protection (M365, endpoints, cloud apps)
  - Policy-based prevention and alerting

- **Microsoft Learn DLP Module**
  - https://learn.microsoft.com/en-us/training/modules/m365-compliance-information-prevent-data-loss/
  - Comprehensive DLP training covering:
    - DLP policy creation and deployment
    - Adaptive Protection for risk-aware safeguards
    - DLP analytics for performance optimization
    - Alert management and activity monitoring

- **DLP Components:**
  - **Locations:** Where to apply policies (Exchange, SharePoint, Teams, OneDrive, endpoints)
  - **Conditions:** What triggers the policy (sensitive info types, labels)
  - **Actions:** What happens (block, notify, override, quarantine)
  - **Exceptions:** When to skip the policy
  - **User notifications:** Policy tips and email alerts
  - **Incident reports:** Admin notifications

### Insider Risk Management
- **Detect and Mitigate Internal Threats**
  - Monitor user activities for risky behavior
  - Data theft prevention
  - Departing employee monitoring
  - Security policy violation detection
  - Machine learning-based risk scoring

- **Risk Indicators:**
  - Unusual file activity
  - Data exfiltration patterns
  - After-hours access
  - Risky browsing behavior

### Communication Compliance
- **Monitor Organizational Communications**
  - Scan emails, Teams messages, Yammer posts
  - Detect policy violations (harassment, inappropriate content)
  - Regulatory compliance (SEC, FINRA)
  - Built-in and custom policies

### Data Security Posture Management
- **Assess and Improve Security Stance**
  - Discover sensitive data across environments
  - Identify security gaps and misconfigurations
  - Implement security recommendations
  - Monitor posture improvements

### Compliance Manager
- **Microsoft Purview Compliance Manager**
  - https://learn.microsoft.com/en-us/purview/compliance-manager
  - Automated compliance assessment and management
  - 360+ regulatory templates (GDPR, HIPAA, SOX, ISO, etc.)
  - Risk-based compliance score
  - Improvement actions with step-by-step guidance

- **Key Components:**
  - **Controls:** Requirements for system configuration and processes
  - **Assessments:** Groupings of controls from regulations
  - **Regulations:** Pre-built templates for standards
  - **Improvement Actions:** Recommended tasks to improve compliance

- **Compliance Score:**
  - Measures progress in completing improvement actions
  - Points awarded for implementing controls
  - Baseline score from M365 data protection defaults

### Copilot Data Protection
- **How Copilot Accesses Data**
  - Copilot respects existing permissions (no elevation)
  - Users only see data they already have access to
  - Semantic Index for enhanced retrieval
  - Real-time permission checks

- **Copilot and Governance**
  - DLP policies apply to Copilot interactions
  - Sensitivity labels honored in responses
  - No data used for foundation model training
  - Tenant boundary protection
  - Data grounding within your organization

## Microsoft Learn Training Modules

### Data Governance and Compliance
- **Microsoft 365 Compliance Information Governance**
  - https://learn.microsoft.com/en-us/training/modules/m365-compliance-information-governance/
  - Learning objectives:
    - Understand importance of data security and compliance
    - How Microsoft Purview addresses protection and management
    - Key concepts in data protection and lifecycle management
    - Identify Purview tools and solutions

- **Microsoft Purview Data Loss Prevention**
  - https://learn.microsoft.com/en-us/training/modules/m365-compliance-information-prevent-data-loss/
  - Comprehensive DLP training (intermediate level, 10 units)
  - Policy planning, deployment, simulation, management
  - Adaptive Protection integration
  - Analytics utilization and alert management

### Security Fundamentals
- **Microsoft Security Copilot Core Features**
  - https://learn.microsoft.com/en-us/training/modules/security-copilot-describe-core-features/
  - Security features and capabilities
  - Integration with Defender, Sentinel, Entra, Intune, Purview
  - Plugins and promptbooks

## Hands-On Practice

### Lab Scenarios

#### Lab 1: Create Sensitivity Labels
1. Access Purview compliance portal
2. Create label taxonomy:
   - Public
   - Internal
   - Confidential
   - Highly Confidential
3. Configure label settings:
   - Encryption (who can access)
   - Content marking (headers, footers, watermarks)
   - Auto-labeling conditions
4. Publish label policy to users
5. Test in Word, Excel, PowerPoint, Outlook

#### Lab 2: Implement DLP Policies
1. Create DLP policy for credit card numbers
2. Configure locations (Exchange, SharePoint, Teams, OneDrive)
3. Set up conditions (sensitive info types)
4. Define actions:
   - Block sharing
   - Notify users with policy tip
   - Send incident report to admin
5. Configure user override options
6. Test policy with sample data
7. Review DLP reports and alerts

#### Lab 3: Configure Adaptive Protection (DLP)
1. Enable insider risk integration
2. Configure risk levels (elevated, moderate, minor)
3. Set up dynamic DLP enforcement based on risk
4. Test with different user risk levels
5. Monitor adaptive policy effectiveness

#### Lab 4: Use Compliance Manager
1. Navigate to Compliance Manager
2. Review compliance score
3. Explore improvement actions
4. Create assessment (e.g., GDPR)
5. Assign improvement actions to team members
6. Track progress and update status
7. Generate compliance reports

#### Lab 5: Discover Sensitive Data
1. Use Content Explorer to find labeled documents
2. Use Activity Explorer to monitor labeling activities
3. Create custom sensitive information type
4. Run sensitive data discovery scan
5. Review findings and remediate

#### Lab 6: Insider Risk Management
1. Configure insider risk settings
2. Create insider risk policy (data theft by departing users)
3. Define risk indicators
4. Specify users in scope
5. Review risk alerts
6. Investigate potential incidents
7. Take action on confirmed risks

#### Lab 7: SharePoint Oversharing Remediation
1. Access SharePoint Advanced Management
2. Review data access governance reports
3. Identify overshared sites and files
4. Implement restricted access controls
5. Configure block download policies
6. Set up site access reviews
7. Monitor oversharing reduction

## AB-900 Exam Focus Areas

### Domain 2: Data Protection and Governance (35-40%)

**Critical Topics:**

- [ ] **Microsoft Purview capabilities**
  - Information Protection
  - Data Loss Prevention
  - Insider Risk Management
  - Communication Compliance
  - Data Security Posture Management

- [ ] **Sensitivity labels**
  - Creating and configuring labels
  - Label policies and scopes
  - Automatic vs. manual labeling
  - Encryption and rights management
  - Label inheritance

- [ ] **Data Loss Prevention**
  - DLP policy creation
  - Conditions, actions, exceptions
  - User notifications and policy tips
  - DLP locations (Exchange, SharePoint, Teams, OneDrive, endpoints)
  - Alert response and investigation

- [ ] **Copilot data access**
  - How Copilot accesses organizational data
  - Permission model (no elevation)
  - Data grounding and semantic index
  - Web search controls
  - Tenant boundary protection

- [ ] **Compliance Manager**
  - Identifying compliance risks
  - Compliance score calculation
  - Improvement actions
  - Assessment creation and management
  - Regulatory templates

- [ ] **Sensitive data discovery**
  - Content Explorer usage
  - Activity Explorer monitoring
  - Sensitive information types
  - Custom classifiers
  - Discovery tools

- [ ] **Insider risk alerts**
  - Risk indicators and scoring
  - Alert investigation
  - Response actions
  - Integration with DLP (Adaptive Protection)

- [ ] **SharePoint oversharing**
  - Data access governance reports
  - Oversharing identification
  - Remediation strategies
  - Restricted access controls
  - Site access reviews
  - SharePoint Advanced Management features

**Key Concepts to Master:**

1. **Layered Protection Approach**
   - Sensitivity labels → Classify data
   - DLP policies → Prevent leakage
   - Insider risk → Detect threats
   - Compliance Manager → Track posture

2. **How Copilot Respects Governance**
   - Honors existing permissions
   - Respects sensitivity labels
   - Subject to DLP policies
   - No training on your data
   - Audit logging enabled

3. **Compliance Manager Workflow**
   - Baseline assessment
   - Identify gaps via controls
   - Implement improvement actions
   - Track progress via score
   - Generate reports for audits

4. **DLP Policy Structure**
   ```
   Location → Condition → Action → Exception → Notification
   ```

5. **SharePoint Advanced Management**
   - Included with Copilot licenses
   - Site ownership policies
   - Inactive sites detection
   - Data access governance reports
   - Block download controls
   - Site access reviews

## Common Scenarios

### Scenario 1: Protecting Financial Data
**Requirement:** Prevent sharing of credit card and bank account numbers

**Solution:**
1. Create DLP policy with financial sensitive info types
2. Apply to Exchange, SharePoint, Teams, OneDrive
3. Configure action: Block external sharing
4. Enable user notifications
5. Set up admin incident reports
6. Monitor DLP dashboard

### Scenario 2: HIPAA Compliance for Healthcare
**Requirement:** Comply with HIPAA regulations for patient data

**Solution:**
1. Use Compliance Manager HIPAA template
2. Review improvement actions
3. Create sensitivity labels (PHI, ePHI)
4. Implement DLP for health-related info
5. Enable audit logging
6. Set up retention policies
7. Track compliance score

### Scenario 3: Departing Employee Risk
**Requirement:** Detect data theft by employees leaving organization

**Solution:**
1. Enable insider risk management
2. Create "Data theft by departing users" policy
3. Integrate with HR system for departure dates
4. Configure risk indicators (downloads, print, USB)
5. Set up alerts for high-risk activities
6. Investigate and respond to alerts

### Scenario 4: Copilot Data Governance
**Requirement:** Ensure Copilot only accesses appropriate data

**Solution:**
1. Review and clean up SharePoint permissions
2. Apply sensitivity labels to confidential content
3. Create DLP policies for Copilot interactions
4. Configure web search settings
5. Enable audit logging for Copilot activities
6. Use SharePoint Advanced Management to identify overshared content
7. Monitor Copilot usage via Viva Insights dashboard

## Tools and Portals

| Tool | URL | Purpose |
|------|-----|---------|
| Purview Compliance Portal | https://compliance.microsoft.com/ | All compliance activities |
| Information Protection | compliance.microsoft.com/informationprotection | Labels and classification |
| DLP | compliance.microsoft.com/datalossprevention | DLP policies and reports |
| Compliance Manager | compliance.microsoft.com/compliancemanager | Compliance assessments |
| Content Explorer | compliance.microsoft.com/dataclassification/contentexplorer | View labeled content |
| Activity Explorer | compliance.microsoft.com/dataclassification/activityexplorer | Monitor activities |
| Insider Risk | compliance.microsoft.com/insiderrisk | Insider threat management |
| SharePoint Advanced Mgmt | admin.microsoft.com/sharepoint (Settings → Advanced Management) | Governance features |

## Best Practices

### Information Protection
- Start with clear classification taxonomy
- Use auto-labeling where possible
- Train users on label meanings
- Implement least restrictive that meets requirements
- Monitor labeling adoption

### Data Loss Prevention
- Start with test mode, then report-only, then enforce
- Use policy tips to educate users
- Allow user overrides with business justification
- Review false positives regularly
- Tune policies based on reports

### Insider Risk Management
- Define clear policies and communicate
- Focus on risk indicators, not surveillance
- Investigate thoroughly before action
- Ensure privacy and legal compliance
- Regular review of policies

### Compliance Management
- Assess compliance posture regularly
- Assign improvement actions to owners
- Track progress consistently
- Generate reports for stakeholders
- Update assessments when regulations change

---

**Related Segments:**
- [Segment 1: Core M365 Services](../../segment-01-core-m365-services/)
- [Segment 3: Copilot Administration](../../segment-03-copilot-administration/)
- [Segment 4: Agents and Exam Prep](../../segment-04-agents-exam-prep/)
