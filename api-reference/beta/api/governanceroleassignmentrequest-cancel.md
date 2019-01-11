---
title: 取消 governanceRoleAssignmentRequest
description: 取消 governanceRoleAssignmentRequest。
localization_priority: Normal
ms.openlocfilehash: f155a832a0c29935216dbc740e7db6ae8708f429
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809105"
---
# <a name="cancel-governanceroleassignmentrequest"></a>取消 governanceRoleAssignmentRequest

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

取消[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | Permissions              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureResources  |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | PrivilegedAccess.ReadWrite.AzureResources |

## <a name="optional-query-parameters"></a>可选的查询参数
该方法**不**支持 [OData 查询参数](/graph/query-parameters)。

### <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | 持有者 {code}|
| Content-type  | application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。 

## <a name="error-codes"></a>错误代码
此 API 遵循标准的 HTTP 代码。 此外，如下所示的自定义的错误代码。
|错误代码     | 错误消息              | 详细信息 |
|:--------------------| :---------------------|:--------------------|
| 400 BadRequest | RoleAssignmentRequestNotFound | GovernanceRoleAssignmentRequest 系统中不存在。
| 400 BadRequest | RequestCannotBeCancelled    | 只请求的状态在`Granted`， `PendingApproval`，`PendingApprovalProvisioning`和`PendingAdminDecision`可以取消。

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Cancel governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
