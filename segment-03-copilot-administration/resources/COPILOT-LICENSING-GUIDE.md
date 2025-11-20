# Microsoft 365 Copilot Licensing Guide

A straightforward guide to understanding what you can and can't do with Microsoft 365 Copilot licensing.

---

## Quick Overview

| Feature | Without Copilot License | With Copilot License |
|---------|------------------------|---------------------|
| Microsoft 365 apps (Word, Excel, etc.) | Yes | Yes |
| AI-powered assistance in apps | No | Yes |
| Copilot chat in Teams | No | Yes |
| Business Chat (work content) | No | Yes |
| Microsoft Graph integration | Limited | Full |

---

## License Types

### Microsoft 365 Copilot (Enterprise/Business)

**Subscription Model** - Per user, per month

- **Prerequisites**: Requires an eligible Microsoft 365 or Office 365 base license
  - Microsoft 365 E3/E5, Business Standard, or Business Premium
  - Office 365 E3/E5

- **What's Included**:
  - Copilot in Word, Excel, PowerPoint, Outlook, Teams
  - Business Chat (Microsoft365.com, Teams, Bing)
  - Microsoft Graph grounding (access to your organizational data)
  - Enterprise-grade security and compliance

### Copilot Pro (Individual)

**Subscription Model** - Per user, per month (lower cost than enterprise)

- **For**: Individuals and families
- **Prerequisites**: Microsoft 365 Personal or Family subscription
- **What's Included**:
  - Copilot in Word, Excel, PowerPoint, Outlook, OneNote
  - Priority access to latest models
  - 100 boosts per day for image creation

---

## Pay-As-You-Go vs Subscription

### Subscription Licensing

| Aspect | Details |
|--------|---------|
| **Billing** | Fixed monthly/annual cost per user |
| **Commitment** | Usually annual commitment for best pricing |
| **Best For** | Organizations with predictable usage |
| **Cost Control** | Predictable budgeting |
| **Assignment** | Licenses assigned to specific users |

### Pay-As-You-Go (Consumption-Based)

| Aspect | Details |
|--------|---------|
| **Billing** | Pay for what you use (metered) |
| **Commitment** | No long-term commitment |
| **Best For** | Variable usage, testing, specific scenarios |
| **Cost Control** | Can be harder to predict costs |
| **Availability** | Available through Azure for specific Copilot services |

**Note**: As of 2024, Microsoft 365 Copilot primarily uses subscription licensing. Pay-as-you-go options are more common for:
- Copilot Studio (agent building)
- Azure OpenAI Service
- Power Platform connectors

---

## What You CAN Do Without a Copilot License

- Use all standard Microsoft 365 applications
- Access free Copilot features at copilot.microsoft.com (consumer version)
- Use basic AI features in some apps (like Editor in Word)
- Benefit from some organizational Copilot deployments as a guest (limited scenarios)

## What You CANNOT Do Without a Copilot License

- Access Copilot features embedded in Microsoft 365 apps
- Use Business Chat to query organizational data
- Generate content with AI in Word, Excel, PowerPoint
- Have Copilot summarize meetings in Teams
- Use Copilot to draft emails in Outlook

---

## License Assignment Best Practices

### Who Should Get a License?

**High Priority**:
- Knowledge workers who create documents frequently
- Executives needing meeting summaries
- Teams that handle large volumes of email
- Employees who analyze data in Excel

**Consider Carefully**:
- Frontline workers with limited desktop app usage
- Users who primarily use mobile devices
- Temporary or seasonal employees

### How to Assign Licenses

1. **Microsoft 365 Admin Center** - Individual or bulk assignment
2. **Group-Based Licensing** - Assign via Azure AD groups
3. **PowerShell** - Automated assignment at scale

---

## Compliance and Data Considerations

| Concern | How Copilot Handles It |
|---------|------------------------|
| **Data residency** | Respects Microsoft 365 data boundaries |
| **Data access** | Only accesses data user already has permission to view |
| **Audit logging** | Activities logged in Microsoft 365 compliance center |
| **Retention** | Follows existing retention policies |

---

## Cost Optimization Tips

1. **Start with a pilot** - Test with a subset of users before broad rollout
2. **Monitor adoption** - Use Copilot Dashboard to track actual usage
3. **Reallocate unused licenses** - Review and reassign from low-usage users
4. **Consider mixed licensing** - Not everyone needs Copilot Pro or Enterprise
5. **Annual commitment** - Usually provides better per-user pricing

---

## Common Licensing Questions

### Can users share a Copilot license?
No. Licenses are assigned per user and cannot be shared or used concurrently.

### What happens when a license is removed?
The user immediately loses access to Copilot features but retains access to all their Microsoft 365 apps and data.

### Can guests use Copilot?
External guests cannot use your organization's Copilot licenses. They need their own.

### Is there a free trial?
Microsoft periodically offers trial licenses. Check with your Microsoft representative or the Admin Center.

### Do I need additional licenses for Copilot Studio?
Copilot Studio has separate licensing (subscription or pay-as-you-go) for building custom agents.

---

## Summary Table

| Scenario | License Needed | Licensing Model |
|----------|---------------|-----------------|
| Individual using Copilot at home | Copilot Pro | Subscription |
| Enterprise employee using Copilot in Teams | Microsoft 365 Copilot | Subscription |
| Building custom agents | Copilot Studio | Subscription or Pay-as-you-go |
| Using Azure OpenAI directly | Azure OpenAI Service | Pay-as-you-go |
| Basic Microsoft 365 usage | Microsoft 365 (no Copilot) | Subscription |

---

## Additional Resources

- [Microsoft 365 Copilot licensing documentation](https://learn.microsoft.com/microsoft-365-copilot/microsoft-365-copilot-licensing)
- [Copilot for Microsoft 365 requirements](https://learn.microsoft.com/microsoft-365-copilot/microsoft-365-copilot-requirements)
- [Copilot Studio licensing](https://learn.microsoft.com/microsoft-copilot-studio/requirements-licensing)

---

*Last updated: November 2024*
