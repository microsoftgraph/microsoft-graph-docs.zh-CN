---
title: 在 Microsoft Graph 中使用 Microsoft 365 的使用情况报表
description: 使用 Microsoft Graph，可以访问 Microsoft 365 使用情况报告资源，以获取有关企业中的人员如何使用Microsoft 365服务的信息。例如，你可以确定谁经常使用服务并达到配额，或者谁根本不需要 Microsoft 365 许可证。
ms.localizationpriority: high
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 123c3e12837528890950a6afa2788d58ee7cf887
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390904"
---
# <a name="working-with-microsoft-365-usage-reports-in-microsoft-graph"></a>在 Microsoft Graph 中使用 Microsoft 365 的使用情况报表

使用 Microsoft Graph，可以访问 Microsoft 365 使用情况报告资源，以获取有关企业中的人员如何使用 Microsoft 365 服务的信息。例如，你可以确定谁经常使用服务并达到配额，或者谁可能根本不需要 Microsoft 365 许可证。 

有关控制 Microsoft 365 使用情况报告数据中信息标识/取消标识设置的详细信息，请参阅 [管理中心内的 Microsoft 365报表](/microsoft-365/admin/activity-reports/activity-reports)。

## <a name="authorization"></a>Authorization

Microsoft Graph 通过权限控制对资源的访问。 必须指定访问报表资源所需的权限。 通常是在 Azure Active Directory (Azure AD) 门户中指定权限。 有关详细信息，请参阅 [Microsoft Graph 权限参考](/graph/permissions-reference)和[报表权限](/graph/permissions-reference#reports-permissions)。

## <a name="cloud-deployments"></a>云部署

下表显示了所有云部署中每个 API 的可用性。

| API                                                         | Microsoft Graph 全局服务 | **Microsoft Cloud for US Government** | **由世纪互联运营的 Microsoft Cloud 中国** | **Microsoft 云德国** |
| ------------------------------------------------------------ | ------------------------------ | ------------------------------------- | ---------------------------------------------- | --------------------------- |
| [Microsoft 365 激活](/graph/api/resources/office-365-activations-reports?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Microsoft 365 活动用户](/graph/api/resources/office-365-active-users-reports?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Microsoft 365 组活动](/graph/api/resources/office-365-groups-activity-reports?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Microsoft Teams 设备使用情况](/graph/api/resources/microsoft-teams-device-usage-reports?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Microsoft Teams 用户活动](/graph/api/resources/microsoft-teams-user-activity-reports?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Outlook 活动](/graph/api/resources/email-activity-reports?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Outlook 应用使用情况](/graph/api/resources/email-app-usage-reports?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Outlook 邮箱使用情况](/graph/api/resources/mailbox-usage-reports?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [OneDrive 活动](/graph/api/resources/onedrive-activity-reports?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [OneDrive 使用情况](/graph/api/resources/onedrive-usage-reports?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [SharePoint 活动](/graph/api/resources/sharepoint-activity-reports?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [SharePoint 网站使用情况](/graph/api/resources/sharepoint-site-usage-reports?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Skype for Business 活动](/graph/api/resources/skype-for-business-activity-reports?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Skype for Business 设备使用情况](/graph/api/resources/skype-for-business-device-usage-reports?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Skype for Business 组织者活动](/graph/api/resources/skype-for-business-organizer-activity-reports?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Skype for Business 参与者活动](/graph/api/resources/skype-for-business-participant-activity-reports?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Skype for Business 点对点活动](/graph/api/resources/skype-for-business-peer-to-peer-activity?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Yammer 活动](/graph/api/resources/yammer-activity-reports?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Yammer 设备使用情况](/graph/api/resources/yammer-device-usage-reports?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |
| [Yammer 组活动](/graph/api/resources/yammer-groups-activity-reports?view=graph-rest-1.0&preserve-view=true) | ✔                              | ➖                                     | ➖                                              | ➖                           |

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

## <a name="next-steps"></a>后续步骤

报表资源和 API 提供了使用 Microsoft Graph 与用户交互及管理用户体验的新方式。要了解详细信息，请：

- 深入了解对方案最有帮助的资源的方法和属性。
- 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。

需要更多灵感？请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/partners)。

