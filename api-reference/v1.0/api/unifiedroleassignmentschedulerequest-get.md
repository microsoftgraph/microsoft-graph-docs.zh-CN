---
title: 获取 unifiedRoleAssignmentScheduleRequest
description: 在 PIM 中，阅读通过 unifiedRoleAssignmentScheduleRequest 对象进行的主动和持久角色分配请求的详细信息。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e8e66bc6e7c0238e52283e301487532e6b20c3dc
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134090"
---
# <a name="get-unifiedroleassignmentschedulerequest"></a>获取 unifiedRoleAssignmentScheduleRequest
命名空间：microsoft.graph

在 PIM 中，阅读通过 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象进行的主动和持久角色分配请求的详细信息。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|RoleAssignmentSchedule.Read.Directory、RoleManagement.Read.Directory、RoleManagement.Read.All、RoleAssignmentSchedule.ReadWrite.Directory、RoleManagement.ReadWrite.Directory|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|RoleManagement.Read.Directory、RoleManagement.Read.All、RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestId}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$select` OData 查询参数， `$expand` 以帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentschedulerequest"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests/95c690fb-3eb3-4942-a03f-4524aed6f31e
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignmentScheduleRequests/$entity",
    "id": "95c690fb-3eb3-4942-a03f-4524aed6f31e",
    "status": "Provisioned",
    "createdDateTime": "2022-04-11T11:50:05.95Z",
    "completedDateTime": "2022-04-11T11:50:06Z",
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

### <a name="example-2-retrieve-specified-properties-of-a-role-assignment-request-and-expand-the-relationships"></a>示例 2：检索角色分配请求的指定属性并展开关系

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentschedulerequest_expand_relationships"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests/95c690fb-3eb3-4942-a03f-4524aed6f31e?$select=principalId,action,roleDefinitionId&$expand=roleDefinition,activatedUsing,principal,targetSchedule
```


#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignmentScheduleRequests(principalId,action,roleDefinitionId,roleDefinition(),activatedUsing(),principal(),targetSchedule())/$entity",
    "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
    "action": "adminAssign",
    "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "roleDefinition": {
        "id": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
        "description": "",
        "displayName": "Groups Administrator",
        "isBuiltIn": true,
        "isEnabled": true,
        "templateId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
        "version": null,
        "resourceScopes": [],
        "rolePermissions": []
    },
    "activatedUsing": null,
    "principal": {
        "@odata.type": "#microsoft.graph.user",
        "id": "071cc716-8147-4397-a5ba-b2105951cc0b",
        "displayName": "Conf Room Adams",
        "userPrincipalName": "Adams@Contoso.com",
        "mail": "Adams@Contoso.com",
        "businessPhones": [],
        "givenName": null,
        "jobTitle": null,
        "mobilePhone": null,
        "officeLocation": null,
        "preferredLanguage": null,
        "surname": null
    },
    "targetSchedule": {
        "id": "95c690fb-3eb3-4942-a03f-4524aed6f31e",
        "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
        "roleDefinitionId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
        "directoryScopeId": "/",
        "appScopeId": null,
        "createdUsing": "95c690fb-3eb3-4942-a03f-4524aed6f31e",
        "createdDateTime": "2022-04-11T11:50:05.95Z",
        "modifiedDateTime": "2022-04-11T11:50:05.95Z",
        "status": "Provisioned",
        "assignmentType": "Assigned",
        "memberType": "Direct",
        "scheduleInfo": {
            "startDateTime": "2022-04-11T11:50:05.9999343Z",
            "recurrence": null,
            "expiration": {
                "type": "noExpiration",
                "endDateTime": null,
                "duration": null
            }
        }
    }
}
```