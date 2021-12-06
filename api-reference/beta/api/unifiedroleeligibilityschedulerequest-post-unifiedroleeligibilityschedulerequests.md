---
title: 创建 unifiedRoleEligibilityScheduleRequest
description: 创建新的 unifiedRoleEligibilityScheduleRequest 对象。
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 4e88dbaf2c29b08471e9f17167fbec4559ed4868
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60976895"
---
# <a name="create-unifiedroleeligibilityschedulerequest"></a>创建 unifiedRoleEligibilityScheduleRequest
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 对象。 此操作允许管理员和符合条件的用户添加、撤销或扩展符合条件的分配。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|RoleEligibilitySchedule.ReadWrite.Directory|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|不支持|

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

下表显示创建 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)时可选的和必需的属性。

|属性|类型|说明|
|:---|:---|:---|
|action|String|表示角色资格分配上的操作类型。 可能的值有： <ul><li>`AdminAssign`：供管理员向用户或组分配角色资格。</li><li>`AdminExtend`：供管理员扩展即将过期的工作分配。</li><li>`AdminUpdate`：供管理员更改现有角色分配。</li><li>`AdminRenew`：供管理员续订已过期的工作分配。</li><li>`AdminRemove`：供管理员从符合条件的角色中删除用户或组。</li><li>`UserAdd`：供用户激活其符合条件的工作分配。</li><li>`UserExtend`：用户请求延长其即将到期的合格分配。</li><li>`UserRemove`：让用户停用其活动符合条件的分配。</li><li>`UserRenew`：用户请求续订其已过期的合格分配。</li></ul>|
|appScopeId|String|当分配范围特定于应用时，特定于应用的范围的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 应用程序作用域是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将作用域限制为特定的目录对象，例如管理单元或所有用户。|
|directoryScopeId|String|表示工作分配范围的目录对象的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 用于 `/` 租户范围范围。 使用 **appScopeId** 将作用域限制为仅应用程序。|
|isValidationOnly|布尔|确定调用是验证还是实际调用的布尔值。 仅在要检查激活是否受 MFA 等其他规则限制，然后再实际提交请求时设置此属性。|
|justification|String|创建请求时由用户和管理员提供的消息，说明为什么需要该请求。 操作为时可选 `AdminRemove` 。|
|principalId|String|要向其中授予工作分配的主体的标识符。 例如，用户或组。 对于组，它们必须可分配给角色，即组属性设置为 的 **isAssignableToRole。** `true`|
|roleDefinitionId|String|分配所针对的 unifiedRoleDefinition 的标识符。 必需。 只读。|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|请求的计划角色分配对象。 当操作为 时，此属性 **不** 是必需的 `AdminRemove` 。|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|附加到请求的 ticketInfo 角色分配，其中包含票证编号和票证系统的详细信息。 可选。|



## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-admin-to-assign-a-role-eligibility-schedule-request"></a>示例 1：分配角色资格计划请求的管理员

在下面的请求中，管理员创建一个请求，将标识的角色资格分配给 id `fdd7a751-b60b-444a-984c-02652fe8fa1c` 标识的主体 `07706ff1-46c7-4847-ae33-3003830675a1` 。 资格的范围是租户中所有目录对象，直到 2022 年 6 月 30 日午夜 UTC 时间。

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleeligibilityschedulerequest_from_unifiedroleeligibilityschedulerequests"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests
Content-Type: application/json

{
  "action": "AdminAssign",
  "justification": "Assign User Admin eligibility to IT Helpdesk (User) group",
  "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
  "directoryScopeId": "/",
  "principalId": "07706ff1-46c7-4847-ae33-3003830675a1",
  "scheduleInfo": {
    "startDateTime": "2021-07-01T00:00:00Z",
    "expiration": {
      "endDateTime": "2022-06-30T00:00:00Z",
      "type": "AfterDateTime"
    }
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应

下面展示了示例响应。
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "672c03bf-226a-42ec-a8b7-3bfab96064a1",
    "status": "Provisioned",
    "createdDateTime": "2021-07-26T18:08:03.1299669Z",
    "completedDateTime": "2021-07-26T18:08:06.2081758Z",
    "approvalId": null,
    "customData": null,
    "action": "AdminAssign",
    "principalId": "07706ff1-46c7-4847-ae33-3003830675a1",
    "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "directoryScopeId": "/",
    "appScopeId": null,
    "isValidationOnly": false,
    "targetScheduleId": "672c03bf-226a-42ec-a8b7-3bfab96064a1",
    "justification": "Assign User Admin eligibility to IT Helpdesk (User) group",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "displayName": null,
            "id": "fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2021-07-26T18:08:06.2081758Z",
        "recurrence": null,
        "expiration": {
            "type": "afterDateTime",
            "endDateTime": "2022-06-30T00:00:00Z",
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

在下面的请求中，管理员创建一个请求，撤消标识为 id 的主体的角色 `fdd7a751-b60b-444a-984c-02652fe8fa1c` **资格** `07706ff1-46c7-4847-ae33-3003830675a1` 。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleeligibilityschedulerequest_from_unifiedroleeligibilityschedulerequests_AdminRemove"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests
Content-Type: application/json

{
    "action": "AdminRemove",
    "justification": "Assign User Admin eligibility to IT Helpdesk (User) group",
    "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "directoryScopeId": "/",
    "principalId": "07706ff1-46c7-4847-ae33-3003830675a1",
    "scheduleInfo": {
        "startDateTime": "2021-07-26T18:08:06.2081758Z",
        "expiration": {
            "endDateTime": "2022-06-30T00:00:00Z",
            "type": "AfterDateTime"
        }
    }
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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedroleeligibilityschedulerequest-from-unifiedroleeligibilityschedulerequests-adminremove-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




#### <a name="response"></a>响应

下面展示了示例响应。 请求返回响应对象，该对象将以前符合条件的工作分配更改的状态显示为 `Revoked` 。 主体将不再看到其以前符合条件的角色。

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "7f88a144-f9a9-4f8c-9623-39c321ae93c2",
    "status": "Revoked",
    "createdDateTime": "2021-08-06T17:59:12.4263499Z",
    "completedDateTime": null,
    "approvalId": null,
    "customData": null,
    "action": "AdminRemove",
    "principalId": "07706ff1-46c7-4847-ae33-3003830675a1",
    "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "directoryScopeId": "/",
    "appScopeId": null,
    "isValidationOnly": false,
    "targetScheduleId": null,
    "justification": "Assign User Admin eligibility to IT Helpdesk (User) group",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "displayName": null,
            "id": "fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2021-07-26T18:08:06.2081758Z",
        "recurrence": null,
        "expiration": {
            "type": "afterDateTime",
            "endDateTime": "2022-06-30T00:00:00Z",
            "duration": null
        }
    },
    "ticketInfo": {
        "ticketNumber": null,
        "ticketSystem": null
    }
}
```
