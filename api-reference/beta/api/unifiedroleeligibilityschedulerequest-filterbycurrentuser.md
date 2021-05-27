---
title: unifiedRoleEligibilityScheduleRequest： filterByCurrentUser
description: 获取 unifiedRoleEligibilityScheduleRequest 对象及其属性的列表，这些对象按特定用户主体进行筛选
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c86e57ad48e239d6a77b6cf992163bd513bd1c0c
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679510"
---
# <a name="unifiedroleeligibilityschedulerequest-filterbycurrentuser"></a>unifiedRoleEligibilityScheduleRequest： filterByCurrentUser
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取与特定主体对象关联的 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedRoleEligibilityScheduleRequest.md) 对象及其属性的列表。

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
GET /roleManagement/directory/RoleEligibilityScheduleRequests/filterByCurrentUser
```

## <a name="function-parameters"></a>函数参数
在请求 URL 中，提供以下查询参数（含值）。
下表显示了可用于此函数的参数。

|参数|类型|说明|
|:---|:---|:---|
|on|RoleEligibilityScheduleRequestFilterByCurrentUserOptions|主体对象的 ID|


## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [unifiedRoleEligibilityScheduleRequest](../resources/unifiedRoleEligibilityScheduleRequest.md) 集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "unifiedRoleEligibilityScheduleRequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/RoleEligibilityScheduleRequests/filterByCurrentUser(on='parameterValue')
```


### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleEligibilityScheduleRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "String (identifier)",
      "action": "String",
      "principalId": "String",
      "roleDefinitionId": "String",
      "directoryScopeId": "String",
      "appScopeId": "String",
      "isValidationOnly": "Boolean",
      "targetScheduleId": "String",
      "justification": "String",
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

