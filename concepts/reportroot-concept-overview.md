---
title: Microsoft Graph 报告 API 概述
description: 使用报告 API 将 Microsoft 365 使用情况数据并入组织的报告解决方案中，以便所有 IT 服务报告均位于统一位置。
ms.localizationpriority: high
ms.prod: reports
author: sarahwxy
ms.custom: scenarios:getting-started
ms.openlocfilehash: 84718f4a6fb1b0046387e6338980c99e5d91b881
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446124"
---
# <a name="microsoft-graph-reports-api-overview"></a>Microsoft Graph 报告 API 概述

Microsoft Graph 中的报告 API 可帮助你了解 Azure Active Directory (Azure AD) 租户中的应用程序和资源活动。

> [!VIDEO https://www.youtube-nocookie.com/embed/P6HneRXYdx8]

## <a name="why-use-the-reports-api"></a>为什么使用报告 API？

### <a name="integrate-microsoft-365-usage-reporting-into-your-organizations-existing-reporting-solution"></a>将 Microsoft 365 使用情况报告集成到组织的现有报告解决方案中
很多公司都有使用报告应用程序或 Web 门户的现有报告解决方案。 你可以使用报告 API 将 Microsoft 365 使用情况数据并入组织的现有报告解决方案中，以便所有 IT 服务报告均位于统一位置。

### <a name="retain-usage-reports-for-historical-analysis"></a>保留使用情况报告以供历史分析
你可以使用报告 API 获取所有使用情况报告中可用的数据，包括每个服务的组织级别的摘要、过去 7/30/90/180 天的实体级别（用户、网站和帐户）的使用情况信息和每日活动聚合。这样可允许你按照要求的时间保存历史使用信息。

### <a name="analyze-ad-fs-application-activity-and-configuration"></a>分析 AD FS 应用程序活动和配置
提供与使用 Active Directory 联合身份验证服务（以下简称“AD FS”）配置的信赖方相关的信息、其聚合的使用情况，以及是否可以将信赖方配置迁移到 Azure Active Directory。

### <a name="monitor-application-sign-ins"></a>监控应用程序登录

监控应用程序的使用情况以及与使用情况模式相关的决策。

### <a name="determine-who-is-using-your-applications-and-how-are-they-using-them"></a>确定使用您应用程序的人员及其使用方式

身份验证方法使用情况报告可帮助你了解组织中的用户如何使用 Azure Active Directory (Azure AD) 功能，如自助密码重置和多重身份验证 (MFA)。 这些报告可帮助你确定对组织而言最有效的身份验证方法、最终用户遇到的错误类型，以及帮助最终用户接受使用自动密码重置和 MFA 所需要的市场活动。

### <a name="monitor-activity-on-an-azure-ad-tenant"></a>监控 Azure AD 租户上的活动

更好地了解用户如何访问和使用 Azure AD 服务。 可以通过分析数据，创建满足组织特定需求的自定义解决方案。

## <a name="what-data-can-i-access-by-using-the-reports-api"></a>使用报告 API 可以访问哪些数据？

你可以使用报告 API 访问下表中列出的数据集。

| 报告 API | 数据集 |
|:------------ |:-------- |
| 活动 | [目录审核](/graph/api/resources/directoryaudit)<br/>[登录](/graph/api/resources/signin)<br/>[Provisioning](/graph/api/resources/provisioningobjectsummary) |
| AD FS 应用程序 | [信赖方详细摘要（预览版）](/graph/api/resources/relyingpartydetailedsummary) |
| 应用程序注册 | [凭据用户注册计数（预览版）](/graph/api/resources/credentialuserregistrationcount)<br/>[凭据用户注册详细信息（预览版）](/graph/api/resources/credentialuserregistrationdetails) <br/>[用户凭据使用情况详细信息（预览版）](/graph/api/resources/usercredentialusagedetails) <br/>[凭据使用情况摘要（预览版）](/graph/api/resources/credentialusagesummary)|
| 应用程序登录 | [登录摘要（预览版）](/graph/api/resources/applicationsigninsummary) <br/>[登录详细信息（预览版）](/graph/api/resources/applicationsignindetailedsummary)|
| Microsoft Teams | [设备使用情况](/graph/api/resources/microsoft-teams-device-usage-reports)<br/>[团队使用情况](/graph/api/resources/microsoft-teams-team-usage-reports)<br/>[用户活动](/graph/api/resources/microsoft-teams-user-activity-reports)|
| Microsoft 365（常规） | [激活](/graph/api/resources/office-365-activations-reports)<br/>[活动用户](/graph/api/resources/office-365-active-users-reports)<br/>[组活动](/graph/api/resources/office-365-groups-activity-reports) |
| OneDrive | [活动](/graph/api/resources/onedrive-activity-reports)<br/>[使用情况](/graph/api/resources/onedrive-usage-reports) |
| Outlook | [活动](/graph/api/resources/email-activity-reports)<br/>[应用使用情况](/graph/api/resources/email-app-usage-reports)<br/>[邮箱使用情况](/graph/api/resources/mailbox-usage-reports) |
| SharePoint | [活动](/graph/api/resources/sharepoint-activity-reports)<br/>[网站使用情况](/graph/api/resources/sharepoint-site-usage-reports) |
| Skype for Business | [活动](/graph/api/resources/skype-for-business-activity-reports)<br/>[设备使用情况](/graph/api/resources/skype-for-business-device-usage-reports)<br/>[设备使用情况](/graph/api/resources/skype-for-business-device-usage-reports)<br/>[参与者活动](/graph/api/resources/skype-for-business-participant-activity-reports)<br/>[对等活动](/graph/api/resources/skype-for-business-peer-to-peer-activity) |
| Yammer | [活动](/graph/api/resources/yammer-activity-reports)<br/>[设备使用情况](/graph/api/resources/yammer-device-usage-reports)<br/>[组活动](/graph/api/resources/yammer-groups-activity-reports) |

## <a name="api-reference"></a>API 参考

在查找此服务的 API 参考？

- [Microsoft Graph beta 中的身份和访问报告 API](/graph/api/resources/report-identity-access?view=graph-rest-beta&preserve-view=true)
- [Microsoft Graph v1.0 中的 Microsoft 365 使用情况报告 API](/graph/api/resources/report?view=graph-rest-1.0&preserve-view=true)
- [Microsoft Graph beta 中的 Microsoft 365 使用情况报告 API](/graph/api/resources/report?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a>后续步骤

* 请在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中浏览 API。
