---
title: "Tenant Isolation in Office 365"
ms.author: robmazz
author: robmazz
manager: laurawi
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
localization_priority: Normal
search.appverid:
- MET150
ms.collection:
- Strat_O365_IP
- M365-security-compliance
description: "A summary of how Microsoft enforces tenant isolation for Office 365."
---

# Tenant Isolation in Office 365

One of the primary benefits of cloud computing is concept of a shared, common infrastructure across numerous customers simultaneously, leading to economies of scale. This concept is called *multi-tenancy*. Microsoft works continuously to ensure that the multi-tenant architectures of our cloud services support enterprise-level security, confidentiality, privacy, integrity, and availability standards.

Based upon the significant investments and experience gathered from [Trustworthy Computing](https://www.microsoft.com/en-us/twc/default.aspx) and the [Security Development Lifecycle](http://www.microsoft.com/security/sdl/default.aspx), Microsoft cloud services were designed with the assumption that all tenants are potentially hostile to all other tenants, and we have implemented security measures to prevent the actions of one tenant from affecting the security or service of another tenant, or accessing the content of another tenant.

The two primary goals of maintaining tenant isolation in a multi-tenant environment are:
1.	Preventing leakage of, or unauthorized access to, customer content across tenants; and
2.	Preventing the actions of one tenant from adversely affecting the service for another tenant

Multiple forms of protection have been implemented throughout Office 365 to prevent customers from compromising Office 365 services or applications or gaining unauthorized access to the information of other tenants or the Office 365 system itself, including:
- Logical isolation of customer content within each tenant for Office 365 services is achieved through Azure Active Directory authorization and role-based access control.
- SharePoint Online provides data isolation mechanisms at the storage level.
- Microsoft uses rigorous physical security, background screening, and a multi-layered encryption strategy to protect the confidentiality and integrity of customer content. All Office 365 datacenters have biometric access controls, with most requiring palm prints to gain physical access. In addition, all U.S.-based Microsoft employees are required to successfully complete a standard background check as part of the hiring process. For more information on the controls used for administrative access in Office 365, see [Office 365 Administrative Access Controls](office-365-administrative-access-controls-overview.md).
- Office 365 uses service-side technologies that encrypt customer content at rest and in transit, including BitLocker, per-file encryption, Transport Layer Security (TLS) and Internet Protocol Security (IPsec). For specific details about encryption in Office 365, see [Data Encryption Technologies in Office 365](/microsoft-365/compliance/office-365-encryption-in-the-microsoft-cloud-overview.md).

Together, the above-listed protections provide robust logical isolation controls that provide threat protection and mitigation equivalent to that provided by physical isolation alone.

## Related Links
- [Isolation and Access Control in Azure Active Directory](office-365-isolation-in-azure-active-directory.md)
- [Tenant Isolation in the Office Graph and Delve](office-365-isolation-in-graph-and-delve.md)
- [Tenant Isolation in Office 365 Search](office-365-isolation-in-office-365-search.md)
- [Tenant Isolation in Office 365 Video](office-365-isolation-in-office-365-video.md)
- [Resource Limits](office-365-resource-limits.md)
- [Monitoring and Testing Tenant Boundaries](office-365-monitoring-and-testing.md)
- [Isolation and Access Control in Office 365](office-365-isolation-in-office-365.md)