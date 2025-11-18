# Segment 4: Agents and Exam Prep - Official Resources

## Official Microsoft Documentation

### Agents Overview
- **Microsoft 365 Copilot Agents**
  - https://learn.microsoft.com/en-us/microsoft-365-copilot/microsoft-365-copilot-overview
  - **Definition:** "Agents are scoped or focused versions of Microsoft 365 Copilot that act as AI assistants and can automate business processes"
  - Customized implementations for specific organizational needs
  - Integration with organizational data sources

### Agent Types

#### Declarative Agents
- **Simple, instruction-based agents**
- No-code or low-code creation
- Defined by instructions, knowledge, and actions
- Built using Microsoft 365 Agents Toolkit or Copilot Studio

#### Agent Use Cases
- **Help desk automation:** Create tickets, track issues
- **Employee information lookup:** Query HR systems
- **Research assistants:** Gather and synthesize information
- **Data analysts:** Analyze data and generate insights
- **Custom business processes:** Organization-specific workflows

### Building Declarative Agents
- **Build Declarative Agents Guide**
  - https://learn.microsoft.com/en-us/microsoft-365-copilot/extensibility/build-declarative-agents
  - Comprehensive guide for creating agents

- **Prerequisites:**
  - Sandbox M365 organization with Copilot (TAP membership) OR production with Copilot license
  - Visual Studio Code installed
  - Microsoft 365 Agents Toolkit extension (v6.0+)
  - Familiarity with Teams Store validation guidelines

- **Creation Process:**
  1. **Initialize:** Open Agents Toolkit in VS Code → "Create a New Agent/App"
  2. **Select Template:** Choose "Declarative Agent" → "No Action" for basic
  3. **Configure:** Name project and select storage location
  4. **Provision:** Use Lifecycle pane to provision agent

- **Testing:**
  - Access via m365.cloud.microsoft/chat
  - Select agent from conversation drawer
  - Verify functionality and responses

### Agent Components

#### Instructions and Persona
- Define agent purpose and behavior
- Set tone and communication style
- Specify capabilities and limitations
- Create clear boundaries

#### Knowledge Configuration
- Connect to data sources
- SharePoint sites and libraries
- OneDrive files
- Web content (if enabled)
- Custom knowledge bases

#### Actions and Skills
- Power Automate flows
- Microsoft Graph API calls
- Custom connectors
- Pre-built certified connectors (Salesforce, ServiceNow, Zendesk, etc.)

#### Conversation Starters
- Pre-defined prompts to guide users
- Common questions and tasks
- Help users discover capabilities

### Agent Extensibility
- **Business Applications Overview**
  - https://learn.microsoft.com/en-us/microsoft-365-copilot/extensibility/overview-business-applications
  - Actions creation through Power Platform
  - Built-in actions (Power Automate, connectors)
  - Development paths for custom actions

### Agent Governance and Management

#### Lifecycle Management
- Creation and development
- Testing and validation
- Approval and publication
- Monitoring and maintenance
- Version control and updates

#### Access Control
- User permissions for creation
- Agent publication policies
- Distribution controls
- External sharing restrictions

#### Approval Workflows
- Submit for approval process
- Admin review and testing
- Publication to organization
- Distribution to specific users or groups

#### Monitoring
- Agent usage analytics
- Conversation metrics
- Success vs. escalation rates
- User satisfaction scores

### Copilot Studio
- **Copilot Studio Portal**
  - https://copilotstudio.microsoft.com/
  - Web-based agent development environment
  - Visual builder for agents
  - Integration with Power Platform

- **Relationship to Power Virtual Agents:**
  - Copilot Studio is evolution of Power Virtual Agents
  - Enhanced AI capabilities
  - Deeper M365 integration

## Microsoft Learn Training Modules

### Agent Development
- **Microsoft 365 Copilot Extensibility**
  - Documentation on extending Copilot with agents
  - Plugin development
  - Integration patterns

### Power Platform Training
- **Power Platform Fundamentals (PL-900)**
  - https://learn.microsoft.com/en-us/certifications/power-platform-fundamentals/
  - Foundation for understanding Power Platform integration

- **Power Platform Functional Consultant (PL-200)**
  - https://learn.microsoft.com/en-us/certifications/power-platform-functional-consultant-associate/
  - Advanced Power Platform skills for agent development

## AB-900 Exam Preparation

### About the AB-900 Exam

**IMPORTANT:** AB-900 is a REAL Microsoft certification exam!

- **Official Title:** Microsoft 365 Certified: Copilot and Agent Administration Fundamentals (beta)
- **Exam Code:** AB-900
- **Status:** Beta (as of January 2025)
- **Duration:** 45 minutes
- **Passing Score:** 700 out of 1000
- **Format:** Proctored with potential interactive components

### Exam Registration
- **Microsoft Exam Registration**
  - https://examregistration.microsoft.com/
  - Register for AB-900
  - Schedule at Pearson VUE testing centers or online proctored

- **Exam Details Page**
  - https://learn.microsoft.com/en-us/credentials/certifications/exams/ab-900/
  - Official exam information
  - Skills measured
  - Registration links

### Official Study Resources

#### Study Guide
- **AB-900 Study Guide**
  - https://learn.microsoft.com/credentials/certifications/resources/study-guides/ab-900
  - Detailed skill breakdown with percentages:
    - Core Microsoft 365 Features and Objects (30-35%)
    - Data Protection and Governance (35-40%)
    - Copilot and Agent Administration (25-30%)

#### Certification Page
- **M365 Copilot and Agent Administration Fundamentals Certification**
  - https://learn.microsoft.com/en-us/credentials/certifications/m365-copilot-agent-administration-fundamentals/
  - Certification overview and benefits

#### Practice Assessments
- **Status:** Not yet available (typically launches within 8 weeks of GA)
- Check Microsoft Learn regularly for updates

#### Exam Sandbox
- Available through exam registration page
- Familiarize yourself with exam interface
- Practice with demo questions

### Study Plan for AB-900

#### Week 1-2: Core M365 Services (Domain 1: 30-35%)
- [ ] Microsoft 365 architecture
- [ ] Exchange Online administration
- [ ] SharePoint management and Advanced Management
- [ ] Teams administration
- [ ] License management
- [ ] Microsoft Entra ID and authentication
- [ ] Conditional access
- [ ] Privileged Identity Management
- [ ] Zero Trust principles

#### Week 3-4: Data Protection (Domain 2: 35-40%)
- [ ] Microsoft Purview overview
- [ ] Information Protection and sensitivity labels
- [ ] Data Loss Prevention policies
- [ ] Insider Risk Management
- [ ] Communication Compliance
- [ ] Data Security Posture Management
- [ ] Compliance Manager
- [ ] SharePoint oversharing remediation
- [ ] Copilot data access mechanisms

#### Week 5-6: Copilot Administration (Domain 3: 25-30%)
- [ ] Copilot architecture
- [ ] Licensing models (monthly, pay-as-you-go)
- [ ] License assignment
- [ ] Feature management
- [ ] Billing policies
- [ ] Usage monitoring (Viva Insights dashboard)
- [ ] Prompt management
- [ ] Copilot security and governance

#### Week 7: Agents
- [ ] Agent types (Researcher, Analyst, Custom)
- [ ] Declarative agent creation
- [ ] Agent configuration
- [ ] Agent approval processes
- [ ] Agent governance
- [ ] Hands-on agent building

#### Week 8: Review and Practice
- [ ] Review all domains
- [ ] Take practice assessments (when available)
- [ ] Hands-on labs in test tenant
- [ ] Review weak areas
- [ ] Exam strategies

### Hands-On Labs for Agents

#### Lab 1: Create First Declarative Agent
1. Install Visual Studio Code
2. Install Microsoft 365 Agents Toolkit extension
3. Create new declarative agent project
4. Define agent instructions and persona
5. Add conversation starters
6. Configure knowledge sources (upload FAQs)
7. Test in development environment
8. Provision to M365 tenant
9. Test via m365.cloud.microsoft/chat

#### Lab 2: Agent with Actions
1. Create new agent in Copilot Studio
2. Define agent purpose and capabilities
3. Create Power Automate flow
4. Add flow as agent action
5. Configure action parameters
6. Test action invocation
7. Handle action responses
8. Add error handling
9. Deploy to organization

#### Lab 3: Agent Governance
1. Access Power Platform admin center
2. Review agent creation policies
3. Configure user permissions for agent building
4. Set up approval workflows
5. Enable audit logging for agents
6. Create DLP policy that includes agents
7. Monitor agent usage
8. Review compliance reports

#### Lab 4: Agent Analytics
1. Access agent analytics dashboard
2. Review conversation metrics
3. Identify common queries
4. Analyze success vs. escalation rate
5. Review user satisfaction scores
6. Identify improvement areas
7. Update agent knowledge based on findings

### Exam Tips

#### Question Types
- **Multiple choice:** Single correct answer
- **Multiple response:** Select all that apply
- **Interactive scenarios:** Hands-on simulations
- **Drag and drop:** Ordering or matching
- **Case studies:** Multi-question scenarios

#### Strategies
1. **Read Carefully:** Watch for "EXCEPT," "NOT," "LEAST"
2. **Manage Time:** 45 minutes for all questions
3. **Eliminate Wrong Answers:** Narrow choices
4. **Mark for Review:** Come back to uncertain questions
5. **Trust First Instinct:** Don't overthink
6. **Use Process of Elimination:** Remove clearly wrong options
7. **Look for Specifics:** Scenario details matter

#### Common Pitfalls
- Confusing licensing models
- Mixing up agent types
- Forgetting 24-hour license activation delay
- Not understanding Copilot's permission model
- Mixing up DLP and sensitivity labels
- Overlooking SharePoint Advanced Management features
- Not knowing Compliance Manager's role

### What to Memorize

#### Key Numbers
- **Passing score:** 700
- **Exam duration:** 45 minutes
- **License activation:** Up to 24 hours
- **Copilot Dashboard data:** Previous 28 days
- **Dashboard delay:** Up to 6 days
- **Practice assessment:** Typically within 8 weeks of GA

#### Admin Centers and URLs
- M365 Admin: admin.microsoft.com
- Entra Admin: entra.microsoft.com
- Purview Compliance: compliance.microsoft.com
- SharePoint Admin: admin.microsoft.com/sharepoint
- Teams Admin: admin.teams.microsoft.com
- Exchange Admin: admin.exchange.microsoft.com
- Copilot Studio: copilotstudio.microsoft.com
- M365 Chat: m365.cloud.microsoft/chat

#### Domain Percentages
- Domain 1 (Core M365): 30-35%
- Domain 2 (Data Protection): 35-40%
- Domain 3 (Copilot & Agents): 25-30%

#### License Prerequisites for Copilot
- M365 E3 or E5
- M365 Business Standard or Premium
- Office 365 E1, E3, or E5
- Plus Copilot add-on license

#### Purview Features (Know all 5)
1. Information Protection
2. Data Loss Prevention
3. Insider Risk Management
4. Communication Compliance
5. Data Security Posture Management

#### Agent Types (Know all 3 use cases)
1. **Researcher:** Information gathering, research
2. **Analyst:** Data analysis, insights
3. **Custom:** Organization-specific scenarios

## Real-World Scenarios

### Scenario 1: IT Helpdesk Agent
**Business Need:** Reduce helpdesk ticket volume for common issues

**Solution:**
1. Create declarative agent with IT knowledge base
2. Add instructions for friendly, helpful persona
3. Configure actions:
   - Password reset via Power Automate + Graph API
   - Ticket creation via ServiceNow connector
4. Add conversation starters:
   - "How do I reset my password?"
   - "I can't access my email"
   - "How do I set up MFA?"
5. Publish to organization via Teams
6. Monitor usage and satisfaction
7. Iterate based on analytics

### Scenario 2: HR Onboarding Agent
**Business Need:** Streamline employee onboarding

**Solution:**
1. Create agent with onboarding knowledge
2. Connect to SharePoint onboarding site
3. Configure actions:
   - Document checklist tracking
   - Meeting scheduling
   - Benefits enrollment guidance
4. Add personalized greetings
5. Implement approval workflow for manager review
6. Deploy to new hires on day 1
7. Track completion metrics

### Scenario 3: Sales Intelligence Agent
**Business Need:** Help sales team access customer data quickly

**Solution:**
1. Create analyst agent
2. Connect to CRM (Dynamics 365/Salesforce)
3. Configure data analysis actions
4. Implement security (sales team only)
5. Add conversation starters:
   - "Show me accounts at risk"
   - "What's the pipeline for Q2?"
   - "Find opportunities closing this month"
6. Test with pilot sales users
7. Gather feedback and refine
8. Roll out to entire sales org

## Additional Certifications

### Related Certifications to Consider

#### Microsoft 365 Track
- **MS-900:** Microsoft 365 Fundamentals
  - Foundation certification for M365
- **MS-102:** Microsoft 365 Administrator
  - Advanced M365 administration

#### Security and Compliance Track
- **SC-300:** Microsoft Identity and Access Administrator
  - Deep dive into Entra ID
- **SC-400:** Microsoft Information Protection Administrator
  - Advanced Purview and data protection

#### Power Platform Track
- **PL-900:** Power Platform Fundamentals
  - Foundation for agent development
- **PL-200:** Power Platform Functional Consultant
  - Advanced Power Platform skills

#### AI Track
- **AI-900:** Microsoft Azure AI Fundamentals
  - Understanding AI concepts

## Post-Certification

### Maintain Your Skills
- Stay updated on Copilot features (monthly releases)
- Join Microsoft 365 community events
- Follow Tech Community blogs
- Attend Microsoft Ignite
- Participate in user groups

### Career Opportunities
- Microsoft 365 Administrator
- Copilot Administrator
- AI Governance Specialist
- Digital Workplace Consultant
- Modern Work Specialist

### Share Your Achievement
- Add to LinkedIn profile
- Update resume and CV
- Join Microsoft Certified community
- Mentor others studying for AB-900

## Tools and Resources

### Development Tools
| Tool | URL | Purpose |
|------|-----|---------|
| Visual Studio Code | https://code.visualstudio.com/ | Agent development |
| M365 Agents Toolkit | VS Code Extensions | Agent creation |
| Copilot Studio | https://copilotstudio.microsoft.com/ | Web-based agent builder |
| Power Automate | https://make.powerautomate.com/ | Create agent actions |

### Learning Resources
| Resource | URL | Purpose |
|----------|-----|---------|
| Microsoft Learn | https://learn.microsoft.com/ | Official training |
| Tech Community | https://techcommunity.microsoft.com/ | Forums and blogs |
| M365 PnP | https://aka.ms/m365pnp | Community resources |
| Microsoft Mechanics | https://youtube.com/c/MicrosoftMechanics | Video training |

### Exam Resources
| Resource | URL | Purpose |
|----------|-----|---------|
| Exam Registration | https://examregistration.microsoft.com/ | Schedule exam |
| AB-900 Exam Page | https://learn.microsoft.com/credentials/certifications/exams/ab-900/ | Official info |
| Practice Assessments | Microsoft Learn | Practice questions |
| Certification Profile | https://learn.microsoft.com/users/me/credentials | Track certifications |

## Community and Support

### Forums
- **Microsoft Tech Community - Copilot**
  - https://techcommunity.microsoft.com/t5/microsoft-365-copilot/bd-p/Microsoft365Copilot

- **Copilot Studio Community**
  - https://powerusers.microsoft.com/t5/Microsoft-Copilot-Studio/ct-p/PVACommunity

- **Power Platform Community**
  - https://powerusers.microsoft.com/

### Social Media
- Follow @Microsoft365 on Twitter/X
- Join Microsoft 365 LinkedIn groups
- Subscribe to Microsoft 365 YouTube channels

### Blogs to Follow
- Microsoft 365 Blog
- Tech Community Copilot Blog
- Microsoft Mechanics
- Copilot adoption blog

---

## Quick Reference: AB-900 at a Glance

### What It Certifies
✅ Support, secure, and protect AI-enabled M365 environments
✅ Manage M365 core services
✅ Implement security features
✅ Administer Copilot and agents

### Who Should Take It
- Microsoft 365 Administrators
- Copilot Administrators
- IT Professionals implementing AI
- Digital Workplace Specialists

### How to Prepare
1. Study all 3 domains (focus on Domain 2 - largest)
2. Get hands-on practice in M365 tenant
3. Use official Microsoft Learn modules
4. Review AB-900 Study Guide
5. Take practice assessments (when available)

### Exam Day
- 45 minutes
- Proctored (online or testing center)
- Interactive + multiple choice
- 700 to pass
- Results: Immediate (or 2-4 weeks for beta)

---

**Good luck with your AB-900 exam and agent development journey!**

For the latest information, visit:
- **Exam Page:** https://learn.microsoft.com/credentials/certifications/exams/ab-900/
- **Study Guide:** https://learn.microsoft.com/credentials/certifications/resources/study-guides/ab-900

---

**Related Segments:**
- [Segment 1: Core M365 Services](../../segment-01-core-m365-services/)
- [Segment 2: Data Protection and Governance](../../segment-02-data-protection-governance/)
- [Segment 3: Copilot Administration](../../segment-03-copilot-administration/)
- [Complete AB-900 Exam Guide](../../shared-resources/references/AB-900-EXAM-GUIDE.md)
