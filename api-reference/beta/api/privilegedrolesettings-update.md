---
title: 更新 privilegedRoleSettings
description: 更新给定角色设置的角色设置。 将返回一个 privilegedRoleSettings 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 01737dd7ffbb15e3fd96cad6b9c9c3aa55cc981d
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633655"
---
# <a name="update-privilegedrolesettings"></a>更新 privilegedRoleSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新给定角色设置的角色设置。 将返回一个[privilegedRoleSettings](../resources/privilegedrolesettings.md)对象。
## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

>**注意:** 请求者必须具有特权角色管理员角色才能更新角色设置。 

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | PrivilegedAccess 的 AzureAD、Directory.accessasuser.all    |
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
在请求正文中, 提供[privilegedRoleSettings](../resources/privilegedrolesettings.md)对象的 JSON 表示形式。

下表列出了在更新角色设置时可以提供的属性。

|属性|类型|说明|
|:---------------|:--------|:----------|
|elevationDuration|duration|激活角色的持续时间。 必需。|
|id|string|角色设置的唯一标识符。 只读。 必需。|
|isMfaOnElevationConfigurable|boolean|如果 mfaOnElevation 是可配置的,**则为 true** 。 **假**如果 mfaOnElevation 不可配置。 必需。|
|lastGlobalAdmin|Boolean|仅供内部使用。|
|maxElavationDuration|duration|已激活角色的最长持续时间。 必需。|
|mfaOnElevation|Boolean|如果需要 MFA 以激活角色,**则为 true** 。 **假**如果无需进行 MFA 即可激活角色。 必需。|
|minElevationDuration|duration|已激活角色的最小持续时间。 必需。|
|notificationToUserOnElevation|Boolean|如果激活角色时向最终用户发送通知,**则为 true** 。 **假**如果在角色激活时不发送通知。 必需。|
|ticketingInfoOnElevation|Boolean|如果激活角色时需要票证信息,**则为 true** 。 **假**如果激活角色时不需要票证信息。 必需。|
|approvalOnElevation|Boolean|如果激活角色时需要进行审批,**则为 true** 。 **假**如果激活该角色时不需要审批。 必需。|
|approverIds|字符串集合|审批 Id 的列表 (如果激活需要审批)。|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

请注意, 需要将租户注册到 PIM。 否则, 将返回 HTTP 403 禁止的状态代码。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。

# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
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
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-privilegedrolesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-privilegedrolesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-privilegedrolesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应
下面是一个响应示例。
<!-- {
  "blockType": "response",
  "truncated": true
}-->
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
  ]
}
-->
