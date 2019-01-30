---
title: 更新 privilegedRoleSettings
description: 更新给定的角色设置的角色设置。 将返回一个 privilegedRoleSettings 对象。
localization_priority: Normal
ms.openlocfilehash: 09464c878c76ed557f30d0eac21e0572fae05062
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641118"
---
# <a name="update-privilegedrolesettings"></a>更新 privilegedRoleSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新给定的角色设置的角色设置。 将返回一个[privilegedRoleSettings](../resources/privilegedrolesettings.md)对象。
## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

>**注意：** 请求者必须具有以下角色之一： 具有权限的角色管理员、 全局管理员、 安全管理员或安全读取器。 

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供[privilegedRoleSettings](../resources/privilegedrolesettings.md)对象的 JSON 表示形式。

下表列出更新角色设置时可以提供的属性。

|属性|类型|说明|
|:---------------|:--------|:----------|
|elevationDuration|duration|当激活角色持续时间。 必需。|
|id|string|角色设置唯一标识符。 只读。 必需。|
|isMfaOnElevationConfigurable|boolean|**true**如果 mfaOnElevation 可配置。 **false**如果 mfaOnElevation 不可配置。 必需。|
|lastGlobalAdmin|布尔值|仅供内部使用。|
|maxElavationDuration|duration|激活角色的最长持续时间。 必需。|
|mfaOnElevation|布尔值|如果为**true** MFA 需要激活角色。 **false**如果 MFA 不需要激活角色。 必需。|
|minElevationDuration|duration|激活角色的最低持续时间。 必需。|
|notificationToUserOnElevation|布尔值|**true**如果角色激活时向最终用户发送通知。 **false**如果角色被激活时不发送通知。 必需。|
|ticketingInfoOnElevation|布尔值|如果为**true**时，票证信息是必需激活角色。 **false**如果票证信息不需要激活角色。 必需。|
|approvalOnElevation|布尔值|**true**如果情况下审批，需要激活角色。 **false**如果审批不需要激活角色。 必需。|
|approverIds|array|审批 Id，如果需要激活审核的列表。|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

请注意，需要将其注册到 PIM 租户。 否则，将返回的 HTTP 403 禁止访问状态代码。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "put_privilegedrolesettings"
}-->
```http
PUT https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
Content-type: application/json

{
    "id": "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    "elevationDuration": "PT8H",
    "notificationToUserOnElevation": false,
    "ticketingInfoOnElevation": true,
    "mfaOnElevation": false,
    "maxElavationDuration": "PT0S",
    "minElevationDuration": "PT0S",
    "lastGlobalAdmin": false,
    "isMfaOnElevationConfigurable": true,
    "approvalOnElevation": false,
    "approverIds": ["e2b2a2fb-13d7-495c-adc9-941fe966793f", "22770e3f-b9b4-418e-9dea-d0e3d2f275dd"]
}
```
##### <a name="response"></a>响应
下面是一个响应示例。

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrolesettings-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
