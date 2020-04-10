---
title: 更新 governanceRoleAssignmentRequests
description: 使管理员能够更新状态为的`AdminApproved` `PendingAdminDecision`governanceRoleAssignmentRequests `AdminDenied`上的决策（或）。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: b726903082d8a3302e2be386206b76d741d89928
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218862"
---
# <a name="update-governanceroleassignmentrequests"></a>更新 governanceRoleAssignmentRequests

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使管理员能够更新状态为的`AdminApproved` `AdminDenied` `PendingAdminDecision` [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)上的决策（或）。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

>**注意：** 此 API 还要求请求者在[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)所属的资源`Active`中至少有一个`owner`管理员`user access administrator`角色分配（或）。 

|权限类型      | Permissions              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureResources  |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a>请求标头
| 名称           | 说明|
|:---------------|:----------|
| Authorization  | Bearer {code}|
| Content-type  | application/json|

## <a name="request-body"></a>请求正文

|参数      |类型                   |必需 |说明|
|:-------------|:----------------------|:--------|:----------|
|reason        |字符串                 |✓        |管理员为自己的决定提供的原因。|
|权        |字符串                 |✓        |角色分配请求的管理员决定。 应将值更新为`AdminApproved`或。 `AdminDenied`|
|schedule      |[governanceSchedule](../resources/governanceschedule.md)|        | 角色分配请求的日程安排。 对于的状态`AdminApproved`，是必需的。|
|assignmentState      |字符串|         | 工作分配的状态，值可以是`Eligible`或。 `Active` 有关的决策`AdminApproved`，则是必需的。 |
### <a name="response"></a>响应
此方法仅适用于状态为的`PendingAdminDecision`请求。

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例
##### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updaterequest-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updaterequest-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updaterequest-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="request-body"></a>请求正文
```json
{
  "reason":"approve the request to extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-02-20T07:31:13.451Z",
    "stopDateTime":"2018-05-21T07:31:13.451Z",
    },
  "decision":"AdminApproved",
  "assignmentState": "Eligible"
}
```

##### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "UpdateRequest governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
