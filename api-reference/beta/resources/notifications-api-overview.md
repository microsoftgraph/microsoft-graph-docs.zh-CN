---
title: 使用 Microsoft Graph 的通知 REST API
description: 你可以使用 Microsoft Graph 中的通知 API 向用户发送推送通知。 只需定位要向其发送通知的用户帐户，平台即可向所有设备终结点发送通知。 将通过委派权限和[通知权限]( /graph/permissions_reference)代表用户执行通知 API 请求，这两种权限可与 Microsoft 帐户或工作或学校帐户结合使用。
localization_priority: Priority
ms.prod: project-rome
ms.openlocfilehash: 2a4c23955e348159d2e17514d6041260f13cffba
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513982"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a>使用 Microsoft Graph 的通知 REST API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

你可以使用 Microsoft Graph 中的通知 API 向用户发送推送通知。 只需定位要向其发送通知的用户帐户，平台即可向所有设备终结点发送通知。 将通过[委派权限](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions)和[通知权限]( /graph/permissions_reference)代表用户执行通知 API 请求，这两种权限可与 Microsoft 帐户或工作或学校帐户结合使用。
此类以用户为中心的通知通过[通知](../resources/projectrome-notification.md)资源标识，存储在 Microsoft Graph 中。 随后可由发布应用程序通过 [Project Rome SDK API](https://github.com/Microsoft/project-rome) 访问和管理。 

## <a name="next-steps"></a>后续步骤
- 请参阅[通知资源](../resources/projectrome-notification.md)并创建通知，以与用户交互。 
- 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/notifications-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
