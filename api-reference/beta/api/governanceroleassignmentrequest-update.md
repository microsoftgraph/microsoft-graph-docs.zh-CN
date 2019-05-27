---
title: 更新 governanceRoleAssignmentRequests
description: 使管理员能够更新状态为的`AdminApproved` `PendingAdminDecision`governanceRoleAssignmentRequests `AdminDenied`上的决策 (或)。
localization_priority: Normal
ms.openlocfilehash: b123345ed14bfe3f12471f70a24df5e02aca0f11
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/23/2019
ms.locfileid: "34422337"
---
# <a name="update-governanceroleassignmentrequests"></a>更新 governanceRoleAssignmentRequests

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使管理员能够更新状态为的`AdminApproved` `AdminDenied` `PendingAdminDecision` [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)上的决策 (或)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

>**注意:** 此 API 还要求请求者在[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)所属的资源`Active`中至少有一个`owner`管理员`user access administrator`角色分配 (或)。 

|权限类型      | 权限              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | PrivilegedAccess AzureResources  |
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
|在于        |String                 |✓        |管理员为自己的决定提供的原因。|
|权        |String                 |✓        |角色分配请求的管理员决定。 应将值更新为`AdminApproved`或。 `AdminDenied`|
|schedule      |[governanceSchedule](../resources/governanceschedule.md)|        | 角色分配请求的日程安排。 对于的状态`AdminApproved`, 是必需的。|
|assignmentState      |String|         | 工作分配的状态, 值可以是`Eligible`或。 `Active` 有关的决策`AdminApproved`, 则是必需的。 |
### <a name="response"></a>响应
此方法仅适用于状态为的`PendingAdminDecision`请求。

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例
##### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
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
#### <a name="sdk-sample-code"></a>SDK 示例代码
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/updaterequest_governanceroleassignmentrequest-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/updaterequest_governanceroleassignmentrequest-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
