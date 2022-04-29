---
title: 获取 unifiedRoleEligibilitySchedule
description: 检索角色资格操作的计划。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1fabcd8e003cf954a7893b34412c21b00e4c6e84
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134078"
---
# <a name="get-unifiedroleeligibilityschedule"></a>获取 unifiedRoleEligibilitySchedule
命名空间：microsoft.graph

检索角色资格操作的计划。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|RoleEligibilitySchedule.Read.Directory、RoleManagement.Read.Directory、RoleManagement.Read.All、RoleEligibilitySchedule.ReadWrite.Directory、RoleManagement.ReadWrite.Directory |
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|RoleManagement.Read.All、RoleManagement.Read.Directory、RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilitySchedules/{unifiedRoleEligibilityScheduleId}
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

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleeligibilityschedule"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/roleManagement/directory/roleEligibilitySchedules/1f06eafc-7532-429b-abf1-ab5a5f4a7052
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilitySchedule"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleEligibilitySchedules/$entity",
    "id": "1f06eafc-7532-429b-abf1-ab5a5f4a7052",
    "principalId": "b2af90c6-279b-41f7-8e79-2f55d07af928",
    "roleDefinitionId": "75934031-6c7e-415a-99d7-48dbd49e875e",
    "directoryScopeId": "/",
    "appScopeId": null,
    "createdUsing": "1f06eafc-7532-429b-abf1-ab5a5f4a7052",
    "createdDateTime": "2022-02-18T20:41:37.163Z",
    "modifiedDateTime": null,
    "status": "Provisioned",
    "memberType": "Direct",
    "scheduleInfo": {
        "startDateTime": "2022-02-18T20:41:37.163Z",
        "recurrence": null,
        "expiration": {
            "type": "noExpiration",
            "endDateTime": null,
            "duration": null
        }
    }
}
```

