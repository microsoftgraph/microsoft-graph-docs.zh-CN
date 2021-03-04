---
title: 更新 governanceRoleAssignmentRequests
description: 使管理员能够更新其 (`AdminApproved` 或) `AdminDenied` 状态为 governanceRoleAssignmentRequests 的决策 `PendingAdminDecision` 。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 59080cf19cf96d82f029d3ba9513cd16a042157a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435852"
---
# <a name="update-governanceroleassignmentrequests"></a>更新 governanceRoleAssignmentRequests

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使管理员能够更新其 (`AdminApproved` 或) `AdminDenied` 状态为 [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) 的决策 `PendingAdminDecision` 。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。

>**注意：** 此 API 还要求请求者至少具有一个管理员角色分配 (或) `Active` `owner` `user access administrator` [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 所属的资源分配权限。 

### <a name="azure-resources"></a>Azure 资源

| 权限类型 | 权限 |
|:--------------- |:----------- |
| 委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureResources |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application | 不支持。 |

### <a name="azure-ad"></a>Azure AD

| 权限类型 | 权限 |
|:--------------- |:----------- |
| 委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureAD |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application | 不支持。 |

### <a name="groups"></a>组

|权限类型 | 权限 |
|:-------------- |:----------- |
| 委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureADGroups |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application | 不支持。 |

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
|reason        |String                 |✓        |管理员提供其决策的原因。|
|决策        |String                 |✓        |请求的管理员角色分配决定。 值应更新为 `AdminApproved` 或 `AdminDenied` 。|
|schedule      |[governanceSchedule](../resources/governanceschedule.md)|        | 请求角色分配计划。 对于状态 `AdminApproved` ，此为必需项。|
|assignmentState      |String|         | 工作分配的状态，值可以是 `Eligible` 或 `Active` 。 要做出 `AdminApproved` 决策，必须执行。 |
### <a name="response"></a>响应
此方法只能应用于状态为 `PendingAdminDecision` .

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

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/updaterequest-governanceroleassignmentrequest-java-snippets.md)]
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


