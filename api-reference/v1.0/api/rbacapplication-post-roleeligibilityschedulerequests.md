---
title: 创建 unifiedRoleEligibilityScheduleRequest
description: 在 PIM 中，通过 unifiedRoleEligibilityScheduleRequest 对象请求主体的角色资格。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c778b6bf713bafd3199d7fa2fe8743ecdca4bf19
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206681"
---
# <a name="create-unifiedroleeligibilityschedulerequest"></a>创建 unifiedRoleEligibilityScheduleRequest
命名空间：microsoft.graph

在 PIM 中，通过 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 对象请求主体的角色资格。 此操作允许管理员和符合条件的用户添加、撤销或扩展符合条件的分配。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|RoleEligibilitySchedule.ReadWrite.Directory|
|委派（个人 Microsoft 帐户）|不支持|
|Application|RoleAssignmentSchedule.ReadWrite.Directory|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleEligibilityScheduleRequests
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 对象的 JSON 表示形式。

创建 **unifiedRoleEligibilityScheduleRequest** 时，可以指定以下属性。

|属性|类型|说明|
|:---|:---|:---|
|action|unifiedRoleScheduleRequestActions|表示角色资格请求的操作类型。可能的值是：`adminAssign`、、`adminUpdate`、`adminRemove`、`selfActivate`、`adminExtend``selfDeactivate`、`adminRenew`、`selfExtend`。 `selfRenew``unknownFutureValue` <br/><ul><li>`adminAssign`：让管理员将符合条件的角色分配给主体。</li><li>`adminRemove`：让管理员从主体中删除符合条件的角色。</li><li> `adminUpdate`：让管理员更改现有角色可变性。</li><li>`adminExtend`：让管理员延长即将过期的角色可质性。</li><li>`adminRenew`：让管理员续订过期的可质性。</li><li>`selfActivate`：让用户激活其分配。</li><li>`selfDeactivate`：让用户停用其活动分配。</li><li>`selfExtend`：让用户请求延长其即将到期的分配。</li><li>`SelfRenew`：用户请求续订其过期的分配。</li></ul>|
|appScopeId|String|当角色资格限定到应用时，特定于应用的范围的标识符。 角色资格的范围决定了主体有资格访问的资源集。 应用范围是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将范围限制为特定目录对象，例如管理单元。 需要 **directoryScopeId** 或 **appScopeId** 。|
|directoryScopeId|String|表示角色资格范围的目录对象的标识符。 角色资格的范围决定了向主体授予访问权限的资源集。 目录范围是存储在多个应用程序理解的目录中的共享范围。 用于 `/` 租户范围。 使用 **appScopeId** 将范围限制为仅限应用程序。 需要 **directoryScopeId** 或 **appScopeId** 。|
|isValidationOnly|Boolean|确定调用是验证还是实际调用。 仅当要在实际提交请求之前检查激活是否受 MFA 等其他规则约束时，才设置此属性。 可选。|
|理由|String|用户和管理员在创建 **统一RoleEligibilityScheduleRequest** 对象时提供的消息。 操作 **为 {** a0 时为 `adminRemove`可选。|
|principalId|字符串|已授予角色资格的主体的标识符。 必填。|
|roleDefinitionId|字符串|分配给主体的 [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象的标识符。 必填。|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|角色资格的期限。 当前不支持定期计划。 操作 **为 {** a0 时为 `adminRemove`可选。|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|与角色资格请求链接的票证详细信息，包括票证编号和票证系统的详细信息。 可选|


## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-admin-to-assign-a-role-eligibility-schedule-request"></a>示例 1：管理员分配角色资格计划请求

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleeligibilityschedulerequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/roleManagement/directory/roleEligibilityScheduleRequests
Content-Type: application/json

{
    "action": "adminAssign",
    "justification": "Assign Attribute Assignment Admin eligibility to restricted user",
    "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    "directoryScopeId": "/",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "scheduleInfo": {
        "startDateTime": "2022-04-10T00:00:00Z",
        "expiration": {
            "type": "afterDateTime",
            "endDateTime": "2024-04-10T00:00:00Z"
        }
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleeligibilityschedulerequest-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleeligibilityschedulerequest-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleeligibilityschedulerequest-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleeligibilityschedulerequest-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedroleeligibilityschedulerequest-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "50877283-9d40-433c-bab8-7986dc10458a",
    "status": "Provisioned",
    "createdDateTime": "2022-04-12T09:05:39.7594064Z",
    "completedDateTime": "2022-04-12T09:05:41.8532931Z",
    "approvalId": null,
    "customData": null,
    "action": "adminAssign",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    "directoryScopeId": "/",
    "appScopeId": null,
    "isValidationOnly": false,
    "targetScheduleId": "50877283-9d40-433c-bab8-7986dc10458a",
    "justification": "Assign Attribute Assignment Admin eligibility to restricted user",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "displayName": null,
            "id": "3fbd929d-8c56-4462-851e-0eb9a7b3a2a5"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2022-04-12T09:05:41.8532931Z",
        "recurrence": null,
        "expiration": {
            "type": "afterDateTime",
            "endDateTime": "2024-04-10T00:00:00Z",
            "duration": null
        }
    },
    "ticketInfo": {
        "ticketNumber": null,
        "ticketSystem": null
    }
}
```

### <a name="example-2-admin-to-remove-an-existing-role-eligibility-schedule-request"></a>示例 2：管理员删除现有角色资格计划请求

在以下请求中，管理员会创建一个请求，以撤销 ID 为 ID `071cc716-8147-4397-a5ba-b2105951cc0b` 角色 `8424c6f0-a189-499e-bbd0-26c1753c96d4`的主体的资格。

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleeligibilityschedulerequest_from_unifiedroleeligibilityschedulerequests_adminRemove"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests
Content-Type: application/json

{
    "action": "adminRemove",
    "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    "directoryScopeId": "/",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-adminremove-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-adminremove-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-adminremove-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-adminremove-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-adminremove-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-adminremove-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应

下面介绍响应示例。 响应对象显示主体的先前角色资格。`Revoked` 主体将不再看到其以前符合条件的角色。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "f341269e-c926-41fa-a905-cef3b01b2a67",
    "status": "Revoked",
    "createdDateTime": "2022-04-12T09:12:15.6859992Z",
    "completedDateTime": null,
    "approvalId": null,
    "customData": null,
    "action": "adminRemove",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    "directoryScopeId": "/",
    "appScopeId": null,
    "isValidationOnly": false,
    "targetScheduleId": null,
    "justification": null,
    "scheduleInfo": null,
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "displayName": null,
            "id": "3fbd929d-8c56-4462-851e-0eb9a7b3a2a5"
        }
    },
    "ticketInfo": {
        "ticketNumber": null,
        "ticketSystem": null
    }
}
```
