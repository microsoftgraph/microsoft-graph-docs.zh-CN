---
title: 创建 unifiedRoleAssignmentScheduleRequest
description: 创建新的 unifiedRoleAssignmentScheduleRequest 对象。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7ec7a150b413b79590b304b63d2a37a0b918b2a4
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397577"
---
# <a name="create-unifiedroleassignmentschedulerequest"></a>创建 unifiedRoleAssignmentScheduleRequest
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象。 此操作允许管理员和用户添加、删除、扩展或续订分配。 若要运行此请求，调用用户必须实施多重身份验证 (MFA) 并在请求 MFA 的会话中运行查询。 请参阅 [“启用每用户 Azure AD 多重身份验证”来保护登录事件](/azure/active-directory/authentication/howto-mfa-userstates)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|RoleAssignmentSchedule.ReadWrite.Directory|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|不支持|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleAssignmentScheduleRequests
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象的 JSON 表示形式。

下表显示了创建 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|unifiedRoleAssignmentScheduleRequest 的唯一标识符。 键，不可为 null，只读。|
|action|字符串|表示角色分配上的操作类型。 可能的值有： <ul><li>`AdminAssign`：让管理员将角色分配给用户或组。</li><li>`AdminRemove`：让管理员从角色中删除用户或组。</li><li> `AdminUpdate`：让管理员更改现有角色分配。</li><li>`AdminExtend`：让管理员延长即将过期的分配。</li><li>`AdminRenew`：让管理员续订过期的分配。</li><li>`SelfActivate`：让用户激活其分配。</li><li>`SelfDeactivate`：让用户停用其活动分配。</li><li>`SelfExtend`：让用户请求延长其即将到期的分配。</li><li>`SelfRenew`：用户请求续订其过期的分配。</li></ul>
|principalId|String|要向其授予分配的主体的标识符。|
|roleDefinitionId|字符串|工作分配所用于的 unifiedRoleDefinition 的标识符。 只读。|
|directoryScopeId|String|表示分配范围的目录对象的标识符。 分配的范围确定已授予主体访问权限的资源集。 目录范围是存储在多个应用程序理解的目录中的共享范围。 用于 `/` 租户范围。 使用 **appScopeId** 将范围限制为仅限应用程序。 |
|appScopeId|String|分配范围特定于应用时特定于应用的范围的标识符。 分配的范围确定已授予主体访问权限的资源集。 应用范围是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将范围限制为特定目录对象，例如管理单元。|
|isValidationOnly|Boolean|指定调用是验证还是实际调用。 仅当要在实际提交请求之前检查激活是否受 MFA 等其他规则约束时，才设置此属性。|
|targetScheduleId|String|附加到分配的计划对象的 ID。|
|理由|字符串|用户和管理员在创建有关为何需要它的请求时提供的消息。|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|角色分配请求的计划对象。|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|附加到角色分配请求的 ticketInfo 对象，其中包括票证编号和票证系统的详细信息。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象。

当调用用户在登录会话期间未对多重身份验证提出质询时，使用 SelfActivate 操作的请求将失败并返回 `400 Bad request` 响应代码。

## <a name="examples"></a>示例

### <a name="example-1-admin-assigning-a-directory-role-to-a-principal"></a>示例 1：管理员将目录角色分配给主体

#### <a name="request"></a>请求

在以下请求中，管理员创建一个请求，以将标 `fdd7a751-b60b-444a-984c-02652fe8fa1c` 识的角色分配 **给 ID 标** 识的 `07706ff1-46c7-4847-ae33-3003830675a1`主体。 其角色的范围是租户中的所有目录对象，并且分配是永久性的，即不会过期。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentschedulerequest_from_unifiedroleassignmentschedulerequests"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/
Content-Type: application/json

{
  "action": "AdminAssign",
  "justification": "Assign User Admin to IT Helpdesk (User) group",
  "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
  "directoryScopeId": "/",
  "principalId": "07706ff1-46c7-4847-ae33-3003830675a1",
  "scheduleInfo": {
    "startDateTime": "2021-07-01T00:00:00Z",
    "expiration": {
      "type": "NoExpiration"
    }
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应

下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignmentScheduleRequests/$entity",
  "id": "b5a22921-656a-4429-9c4e-59a5f576614d",
  "status": "Provisioned",
  "createdDateTime": "2021-07-27T09:18:40.2029365Z",
  "completedDateTime": "2021-07-27T09:18:42.7811184Z",
  "approvalId": null,
  "customData": null,
  "action": "AdminAssign",
  "principalId": "07706ff1-46c7-4847-ae33-3003830675a1",
  "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
  "directoryScopeId": "/",
  "appScopeId": null,
  "isValidationOnly": false,
  "targetScheduleId": "b5a22921-656a-4429-9c4e-59a5f576614d",
  "justification": "Assign User Admin to IT Helpdesk (User) group",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": null,
      "id": "fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f"
    }
  },
  "scheduleInfo": {
    "startDateTime": "2021-07-27T09:18:42.7811184Z",
    "recurrence": null,
    "expiration": {
      "type": "noExpiration",
      "endDateTime": null,
      "duration": null
    }
  },
  "ticketInfo": {
    "ticketNumber": null,
    "ticketSystem": null
  }
}
```

### <a name="example-2-user-activating-their-eligible-role"></a>示例 2：用户激活其符合条件的角色

#### <a name="request"></a>请求

在以下请求中， **由 principalId** `c6ad1942-4afa-47f8-8d48-afb5d8d69d2f` 标识的用户激活其自己的符合条件的角色 `9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3`。 其角色的范围是租户中的所有目录对象，分配为 5 小时。 若要运行此请求，调用用户必须实施多重身份验证 (MFA) 并在请求 MFA 的会话中运行查询。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentschedulerequest_from_unifiedroleassignmentschedulerequests_SelfActivate"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/
Content-Type: application/json

{
    "action": "SelfActivate",
    "principalId": "c6ad1942-4afa-47f8-8d48-afb5d8d69d2f",
    "roleDefinitionId": "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    "directoryScopeId": "/",
    "justification": "Need to update app roles for selected apps.",
    "scheduleInfo": {
        "startDateTime": "2021-08-17T17:40:00.000Z",
        "expiration": {
            "type": "AfterDuration",
            "duration": "PT5H"
        }
    },
    "ticketInfo": {
        "ticketNumber": "CONTOSO:Normal-67890",
        "ticketSystem": "MS Project"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-selfactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-selfactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-selfactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-selfactivate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-selfactivate-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-unifiedroleassignmentschedulerequest-from-unifiedroleassignmentschedulerequests-selfactivate-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应

下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignmentScheduleRequests/$entity",
    "id": "163daf73-8746-4996-87de-ab71dc624bf9",
    "status": "Granted",
    "createdDateTime": "2021-08-17T17:39:36.7040696Z",
    "completedDateTime": "2021-08-17T17:40:00Z",
    "approvalId": null,
    "customData": null,
    "action": "SelfActivate",
    "principalId": "c6ad1942-4afa-47f8-8d48-afb5d8d69d2f",
    "roleDefinitionId": "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    "directoryScopeId": "/",
    "appScopeId": null,
    "isValidationOnly": false,
    "targetScheduleId": "163daf73-8746-4996-87de-ab71dc624bf9",
    "justification": "Need to update app roles for selected apps.",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "displayName": null,
            "id": "c6ad1942-4afa-47f8-8d48-afb5d8d69d2f"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2021-08-17T17:40:00Z",
        "recurrence": null,
        "expiration": {
            "type": "afterDuration",
            "endDateTime": null,
            "duration": "PT5H"
        }
    },
    "ticketInfo": {
        "ticketNumber": "CONTOSO:Normal-67890",
        "ticketSystem": "MS Project"
    }
}
```
