---
title: 更新 governanceRoleAssignmentRequests
description: 使管理员能够更新其决策 (`AdminApproved`或`AdminDenied`) 中的状态的 governanceRoleAssignmentRequests 上`PendingAdminDecision`。
localization_priority: Normal
ms.openlocfilehash: 870cd685aade9bb722660b550ae210c6e10d1fe8
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643260"
---
# <a name="update-governanceroleassignmentrequests"></a>更新 governanceRoleAssignmentRequests

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使管理员能够更新其决策 (`AdminApproved`或`AdminDenied`) 上[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)中的状态的`PendingAdminDecision`。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

>**注意：** 此 API 还需要请求者必须至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)所属的资源。 

|权限类型      | 权限              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureResources  |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | PrivilegedAccess.ReadWrite.AzureResources |

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
|原因        |String                 |✓        |提供由管理员为其决策的原因。|
|决策        |String                 |✓        |角色分配请求的管理员决策。 值应更新为`AdminApproved`或`AdminDenied`。|
|计划      |[governanceSchedule](../resources/governanceschedule.md)|        | 角色分配请求的时间表。 状态的`AdminApproved`，需要。|
|assignmentState      |String|         | 状态的工作分配，以及的值可以是`Eligible`或`Active`。 为决策的`AdminApproved`，需要。 |
### <a name="response"></a>响应
此方法可以仅适用于请求的状态中的`PendingAdminDecision`。

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
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
