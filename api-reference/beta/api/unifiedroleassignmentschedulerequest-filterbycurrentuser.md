---
title: unifiedRoleAssignmentScheduleRequest： filterByCurrentUser
description: 获取由特定用户主体筛选的 unifiedRoleAssignmentScheduleRequest 对象及其属性的列表
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f30a2e8a7c1ac1440291d4e9e7849637c20e3be3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680274"
---
# <a name="unifiedroleassignmentschedulerequest-filterbycurrentuser"></a>unifiedRoleAssignmentScheduleRequest： filterByCurrentUser
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


获取与特定主体对象关联的 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象及其属性的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|PrivilegedAccess.ReadWrite.AzureAD|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|PrivilegedAccess.Read.AzureAD|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleRequests/filterByCurrentUser
```

## <a name="query-parameters"></a>查询参数
下表显示了可用于此方法的查询参数。

|参数|类型|说明|
|:---|:---|:---|
|on|RoleAssignmentScheduleRequestFilterByCurrentUserOptions|主体对象的 ID。|


## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleAssignmentScheduleRequest](../resources/unifiedRoleAssignmentScheduleRequest.md) 集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentschedulerequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/RoleAssignmentScheduleRequests/filterByCurrentUser(on='d6e4112f-112f-d6e4-2f11-e4d62f11e4d6')
```


### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentScheduleRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "action": "AdminAssign",
      "principalId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "roleDefinitionId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "directoryScopeId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "appScopeId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "isValidationOnly": false,
      "targetScheduleId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "justification": "this is a justification",
      "scheduleInfo": {
        "@odata.type": "microsoft.graph.requestSchedule"
      },
      "ticketInfo": {
        "@odata.type": "microsoft.graph.ticketInfo"
      }
    }
  ]
}
```

