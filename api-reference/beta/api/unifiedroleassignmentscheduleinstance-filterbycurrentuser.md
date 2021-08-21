---
title: unifiedRoleAssignmentScheduleInstance：filterByCurrentUser
description: 获取 unifiedRoleAssignmentScheduleInstance 对象及其属性的列表，这些对象按特定用户主体进行筛选
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d60f9f31e23dfd28ee41b526a525c05b8fdeca0e
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453602"
---
# <a name="unifiedroleassignmentscheduleinstance-filterbycurrentuser"></a>unifiedRoleAssignmentScheduleInstance：filterByCurrentUser
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [unifiedRoleAssignmentScheduleInstance](../resources/unifiedRoleAssignmentScheduleInstance.md) 对象及其与特定主体对象关联的属性的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|RoleAssignmentSchedule.Read.Directory、RoleManagement.Read.Directory、RoleManagement.Read.All、RoleAssignmentSchedule.ReadWrite.Directory、RoleManagement.ReadWrite.Directory|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|RoleManagement.Read.All、RoleManagement.Read.Directory、RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleInstances/filterByCurrentUser(on='principal')
```

## <a name="function-parameters"></a>函数参数
下表显示了可用于此方法的参数。

|参数|类型|说明|
|:---|:---|:---|
|on|roleAssignmentScheduleInstanceFilterByCurrentUserOptions|筛选以查询当前用户作为主体的对象。 允许的值为 `principal` 。 必需。|


## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$select` OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。


## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentscheduleinstance_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleInstances/filterByCurrentUser(on='principal')
```


### <a name="response"></a>响应

下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentScheduleInstance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(unifiedRoleAssignmentScheduleInstance)",
  "value": [
    {
      "@odata.type": "#microsoft.graph.unifiedRoleAssignmentScheduleInstance",
      "id": "lAPpYvVpN0KRkAEhdxReECssmvzcHW1IohFf6Mp3-h8-1",
      "principalId": "fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f",
      "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
      "directoryScopeId": "/",
      "appScopeId": null,
      "startDateTime": null,
      "endDateTime": null,
      "assignmentType": "Assigned",
      "memberType": "Direct",
      "roleAssignmentOriginId": "lAPpYvVpN0KRkAEhdxReECssmvzcHW1IohFf6Mp3-h8-1",
      "roleAssignmentScheduleId": "lAPpYvVpN0KRkAEhdxReECssmvzcHW1IohFf6Mp3-h8-1"
    }
  ]
}
```

