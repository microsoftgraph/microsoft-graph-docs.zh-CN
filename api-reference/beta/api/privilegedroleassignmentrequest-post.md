---
title: 创建 privilegedRoleAssignmentRequest
description: 创建 privilegedroleassignmentrequest 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 8899aa70125809f73e2f247a8cf5b83cad0c7731
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441142"
---
# <a name="create-privilegedroleassignmentrequest"></a>创建 privilegedRoleAssignmentRequest

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建 [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) 对象。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | PrivilegedAccess.ReadWrite.AzureAD、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。 |
|Application                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供 [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) 对象的 JSON 表示形式。 

| 属性     | 类型    |  说明|
|:---------------|:--------|:----------|
|roleId|String|角色的 ID。 此为必需属性。|
|type|String|表示对项目执行的操作角色分配。 值可以是 `AdminAdd` ：管理员将用户添加到角色 `UserAdd` ;：用户添加角色分配。 必需。|
|assignmentState|String|工作分配的状态。 该值可用于符合条件的分配-如果直接由管理员分配，或由用户激活在符合条件的分配 `Eligible` `Active` `Active` 上。 可取值为：``NotStarted``、`Completed`、`RequestedApproval`、`Scheduled`、`Approved`、`ApprovalDenied`、`ApprovalAborted`、`Cancelling`、`Cancelled`、`Revoked`、`RequestExpired`。 必需。|
|reason|String|需要为审核和审核角色分配请求提供原因。|
|schedule|[governanceSchedule](../resources/governanceschedule.md)|请求角色分配计划。|

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回响应代码和 `201 Created` [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) 对象。

### <a name="error-codes"></a>错误代码
此 API 返回该标准 HTTP 错误代码。 此外，它可以返回下表中列出的错误代码。

|错误代码     | 错误消息              | 
|:--------------------| :---------------------|
| 400 BadRequest | RoleAssignmentRequest 属性为 NULL |
| 400 BadRequest | 无法反初始化 roleAssignmentRequest 对象。 |
| 400 BadRequest | RoleId 是必需的。 |
| 400 BadRequest | 必须指定计划开始日期，并且应大于"现在"。 |
| 400 BadRequest | 此用户、角色和计划类型已存在计划。 |
| 400 BadRequest | 此用户、角色和审批类型已存在待审批。 |
| 400 BadRequest | 请求者原因缺失。 |
| 400 BadRequest | 请求者原因应小于 500 个字符。 |
| 400 BadRequest | 提升持续时间必须介于 0.5 和 {from setting}之间。 |
| 400 BadRequest | 计划激活和请求之间存在重叠。 |
| 400 BadRequest | 角色已激活。 |
| 400 BadRequest | GenericElevateUserToRoleAssignments：滴答信息是必需的，在激活过程中不提供。 |
| 400 BadRequest | 计划激活和请求之间存在重叠。 |
| 403 UnAuthorized | 提升需要多重身份验证。 |
| 403 UnAuthorized | 不允许代表提升。 |

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_privilegedroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
Content-type: application/json

{
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "schedule": {
        "startDateTime": "2018-02-08T02:35:17.903Z"
    },
    "type": "UserAdd",
    "assignmentState": "Active",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-privilegedroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应
下面是一个响应示例。 注意：为简洁起见，可能会截断此处显示的响应对象。 将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests/$entity",
    "schedule": {
        "type": "activation",
        "startDateTime": "2018-02-08T02:35:17.903Z",
        "endDateTime": null,
        "duration" : null
    },
    "id": "e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1",
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
    "status": "NotStarted",
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "userId": "Self",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Post privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


