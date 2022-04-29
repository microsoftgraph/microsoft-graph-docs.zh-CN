---
title: 创建 unifiedRoleAssignmentScheduleRequest
description: 在 PIM 中，通过 unifiedRoleAssignmentScheduleRequest 对象请求活动和持久角色分配。 使用此 API 激活符合条件的角色。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e8295babb10821b9949231bb27ebb20b8570662d
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133916"
---
# <a name="create-unifiedroleassignmentschedulerequest"></a>创建 unifiedRoleAssignmentScheduleRequest
命名空间：microsoft.graph

在 PIM 中，通过 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象执行以下操作：
+ 请求主体的活动和持久角色分配，无论是否过期日期。
+ 激活、停用、扩展或续订主体的合格角色分配。

若要调用此 API 来为自己更新、续订和扩展分配，必须强制执行多重身份验证 (MFA) ，并在对 MFA 提出质询的会话中运行查询。 请参阅[“启用每用户Azure AD多重身份验证来保护登录事件](/azure/active-directory/authentication/howto-mfa-userstates)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|RoleAssignmentSchedule.ReadWrite.Directory|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|RoleAssignmentSchedule.ReadWrite.Directory|

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

创建 **unifiedRoleAssignmentScheduleRequest** 时，可以指定以下属性。

|属性|类型|说明|
|:---|:---|:---|
|action|unifiedRoleScheduleRequestActions|表示角色分配请求上的操作类型。 可取值包括：`adminAssign`、`adminUpdate`、`adminRemove`、`selfActivate`、`selfDeactivate`、`adminExtend`、`adminRenew`、`selfExtend`、`selfRenew`、`unknownFutureValue`。 <br/><ul><li>`adminAssign`：让管理员将角色分配给用户或组。</li><li>`adminRemove`：让管理员从角色中删除用户或组。</li><li> `adminUpdate`：让管理员更改现有角色分配。</li><li>`adminExtend`：让管理员延长即将过期的分配。</li><li>`adminRenew`：让管理员续订过期的分配。</li><li>`selfActivate`：让用户激活其分配。</li><li>`selfDeactivate`：让用户停用其活动分配。</li><li>`selfExtend`：让用户请求延长其即将到期的分配。</li><li>`selfRenew`：用户请求续订其过期的分配。</li></ul>|
|customData|String|用于定义请求的任何自定义数据的免费文本字段。 可选。|
|principalId|String|已授予分配的主体的标识符。 必需。|
|roleDefinitionId|String|正在分配的 [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象的标识符。 必需。|
|directoryScopeId|String|表示分配范围的目录对象的标识符。 分配的范围确定已授予主体访问权限的资源集。 目录范围是存储在多个应用程序理解的目录中的共享范围。 用于 `/` 租户范围。 使用 **appScopeId** 将范围限制为仅限应用程序。 需要 **directoryScopeId** 或 **appScopeId** 。|
|appScopeId|String|分配作用域为应用时特定于应用的范围的标识符。 分配的范围确定已授予主体访问权限的资源集。 应用范围是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将范围限制为特定目录对象，例如管理单元。 需要 **directoryScopeId** 或 **appScopeId** 。|
|理由|String|用户和管理员创建 **unifiedRoleAssignmentScheduleRequest** 对象时提供的消息。 可选。|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|角色分配请求的周期。 当前不支持定期计划。 必需。|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|链接到角色分配请求的票证详细信息，包括票证编号和票证系统的详细信息。 可选。|



## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-admin-assigning-a-directory-role-to-a-principal"></a>示例 1：管理员将目录角色分配给主体

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentschedulerequest_from_"
}
-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests
Content-Type: application/json

{
    "action": "adminAssign",
    "justification": "Assign Groups Admin to IT Helpdesk group",
    "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "directoryScopeId": "/",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "scheduleInfo": {
        "startDateTime": "2022-04-10T00:00:00Z",
        "expiration": {
            "type": "NoExpiration"
        }
    }
}
```


#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest"
}
-->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignmentScheduleRequests/$entity",
    "id": "95c690fb-3eb3-4942-a03f-4524aed6f31e",
    "status": "Provisioned",
    "createdDateTime": "2022-04-11T11:50:03.9014347Z",
    "completedDateTime": "2022-04-11T11:50:05.9999343Z",
    "approvalId": null,
    "customData": null,
    "action": "adminAssign",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "directoryScopeId": "/",
    "appScopeId": null,
    "isValidationOnly": false,
    "targetScheduleId": "95c690fb-3eb3-4942-a03f-4524aed6f31e",
    "justification": "Assign Groups Admin to IT Helpdesk group",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "displayName": null,
            "id": "3fbd929d-8c56-4462-851e-0eb9a7b3a2a5"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2022-04-11T11:50:05.9999343Z",
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

在以下请求中，**principalId** `071cc716-8147-4397-a5ba-b2105951cc0b` 标识的用户将激活自己的 *符合条件的角色*，并将其激活到 ID 标`8424c6f0-a189-499e-bbd0-26c1753c96d4`识的Azure AD角色。 其角色的范围是租户中的所有目录对象，分配为 5 小时。 若要运行此请求，调用用户必须实施多重身份验证 (MFA) 并在请求 MFA 的会话中运行查询。

若要检索其资格请求的详细信息并确定激活资格，用户将调用 [unifiedRoleEligibilitySchedule：filterByCurrentUser](unifiedroleeligibilityschedule-filterbycurrentuser.md) API。

<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentschedulerequest_from_unifiedroleassignmentschedulerequests_selfActivate"
}
-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests/
Content-Type: application/json

{
    "action": "selfActivate",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    "directoryScopeId": "/",
    "justification": "I need access to the Attribute Administrator role to manage attributes to be assigned to restricted AUs",
    "scheduleInfo": {
        "startDateTime": "2022-04-14T00:00:00.000Z",
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignmentScheduleRequests/$entity",
    "id": "911bab8a-6912-4de2-9dc0-2648ede7dd6d",
    "status": "Granted",
    "createdDateTime": "2022-04-13T08:52:32.6485851Z",
    "completedDateTime": "2022-04-14T00:00:00Z",
    "approvalId": null,
    "customData": null,
    "action": "selfActivate",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
    "directoryScopeId": "/",
    "appScopeId": null,
    "isValidationOnly": false,
    "targetScheduleId": "911bab8a-6912-4de2-9dc0-2648ede7dd6d",
    "justification": "I need access to the Attribute Administrator role to manage attributes to be assigned to restricted AUs",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "displayName": null,
            "id": "071cc716-8147-4397-a5ba-b2105951cc0b"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2022-04-14T00:00:00Z",
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