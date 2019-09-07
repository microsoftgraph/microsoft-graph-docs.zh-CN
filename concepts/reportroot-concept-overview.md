---
title: Microsoft Graph 报告 API 概述
description: 借助 Microsoft 365 管理中心中的使用情况报告，管理员可以了解其公司各 Office 365 服务的使用情况。 Microsoft Graph 中的报告 API 可用于与 Office 365 使用情况报告集成。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
scenarios: getting-started
ms.openlocfilehash: 1793154262f2c366879d961e768080c35b79759d
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792896"
---
# <a name="microsoft-graph-reports-api-overview"></a>Microsoft Graph 报告 API 概述

借助 Microsoft 365 管理中心中的使用情况报告，管理员可以了解其公司各 Office 365 服务的使用情况。 Microsoft Graph 中的报告 API 可用于与 Office 365 使用情况报告集成。

> [!VIDEO https://www.youtube-nocookie.com/embed/P6HneRXYdx8]

## <a name="why-use-the-reports-api"></a>为什么使用报告 API？

### <a name="integrate-office-365-usage-reporting-into-your-organizations-existing-reporting-solution"></a>将 Office 365 使用情况报告集成到组织的现有报告解决方案中
很多公司都有使用报告应用程序或 Web 门户的现有报告解决方案。 你可以使用报告 API 将 Office 365 使用情况数据并入组织的现有报告解决方案中，以便所有 IT 服务报告均位于统一位置。  

### <a name="retain-usage-reports-for-historical-analysis"></a>保留使用情况报告以供历史分析
你可以使用报告 API 获取所有使用情况报告中可用的数据，包括每个服务的组织级别的摘要、过去 7/30/90/180 天的实体级别（用户、网站和帐户）的使用情况信息和每日活动聚合。 这样，可以根据需要保留历史使用情况信息。

## <a name="what-data-can-i-access-by-using-the-reports-api"></a>使用报告 API 可以访问哪些数据？

你可以使用报告 API 访问下表中列出的数据集。

|Office 365 应用|数据集|
|:--------|:--------|
|Microsoft Teams|[设备使用情况](/graph/api/resources/microsoft-teams-device-usage-reports?view=graph-rest-1.0)<br/>|[用户活动](/graph/api/resources/microsoft-teams-user-activity-reports?view=graph-rest-1.0)|
|Office 365（常规） |[激活](/graph/api/resources/office-365-activations-reports?view=graph-rest-1.0)<br/>[活动用户](/graph/api/resources/office-365-active-users-reports?view=graph-rest-1.0)<br/>[组活动](/graph/api/resources/office-365-groups-activity-reports?view=graph-rest-1.0)|
|OneDrive |[活动](/graph/api/resources/onedrive-activity-reports?view=graph-rest-1.0)<br/>[使用情况](/graph/api/resources/onedrive-usage-reports?view=graph-rest-1.0)|
|Outlook|[活动](/graph/api/resources/email-activity-reports?view=graph-rest-1.0)<br/>[应用使用情况](/graph/api/resources/email-app-usage-reports?view=graph-rest-1.0)<br/>[邮箱使用情况](/graph/api/resources/mailbox-usage-reports?view=graph-rest-1.0)|
|SharePoint |[活动](/graph/api/resources/sharepoint-activity-reports?view=graph-rest-1.0)<br/>[网站使用情况](/graph/api/resources/sharepoint-site-usage-reports?view=graph-rest-1.0)|
|Skype for Business |[活动](/graph/api/resources/skype-for-business-activity-reports?view=graph-rest-1.0)<br/>[设备使用情况](/graph/api/resources/skype-for-business-device-usage-reports?view=graph-rest-1.0)<br/>[设备使用情况](/graph/api/resources/skype-for-business-device-usage-reports?view=graph-rest-1.0)<br/>[参与者活动](/graph/api/resources/skype-for-business-participant-activity-reports?view=graph-rest-1.0)<br/>[对等活动](/graph/api/resources/skype-for-business-peer-to-peer-activity?view=graph-rest-1.0)|
|Yammer |[活动](/graph/api/resources/yammer-activity-reports?view=graph-rest-1.0)<br/>[设备使用情况](/graph/api/resources/yammer-device-usage-reports?view=graph-rest-1.0)<br/>[组活动](/graph/api/resources/yammer-groups-activity-reports?view=graph-rest-1.0)|

## <a name="api-reference"></a>API 参考
在查找此服务的 API 参考？

- [Microsoft Graph v1.0 中的 Office 365 使用情况报告 API](/graph/api/resources/report?view=graph-rest-1.0)
- [Microsoft Graph beta 中的 Office 365 使用情况报告 API](/graph/api/resources/report?view=graph-rest-beta)

## <a name="next-steps"></a>后续步骤

* 请在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中探索 API。
* 了解有关如何[使用报告 REST API](/graph/api/resources/report?view=graph-rest-1.0) 的详细信息。
