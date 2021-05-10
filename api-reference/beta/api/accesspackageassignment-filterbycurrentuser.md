---
title: accessPackageAssignment：filterByCurrentUser
description: 检索在登录用户上筛选的 accesspackageassignment 对象列表。
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 72164fb7f9567d1a1c1b79316f19bbd304fabae3
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299138"
---
# <a name="accesspackageassignment-filterbycurrentuser"></a>accessPackageAssignment：filterByCurrentUser
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [Azure AD 权利管理](../resources/entitlementmanagement-root.md)中，检索已登录用户筛选的 [accessPackageAssignment](../resources/accesspackageassignment.md) 对象列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackageAssignments/filterByCurrentUser
```

## <a name="function-parameters"></a>函数参数
下表显示了可用于此函数的参数。

|参数|类型|说明|
|:---|:---|:---|
|on|[accessPackageAssignmentFilterByCurrentUserOptions](../resources/accesspackageassignment-accesspackageassignmentfilterbycurrentuseroptions.md)|可用于在访问包分配列表上进行筛选的当前用户选项的列表。|

- `target` 用于获取 `accessPackageAssignment` 已登录用户作为目标的对象。 生成的列表包括所有目录和访问包中调用方的所有分配（当前分配和过期分配）。

- `createdBy` 用于获取 `accessPackageAssignment` 已登录用户创建的对象。 结果列表包括所有目录和访问包中调用方为自己或代表其他人创建的所有分配，例如管理员直接分配。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessPackageAssignment](../resources/accesspackageassignment.md) 集合。

当结果集跨多个页面时，Microsoft Graph 返回该页面，该页面在响应中包含指向下一 `@odata.nextLink` 页结果的 URL 中的属性。 如果存在该属性，请继续使用每个响应中的 URL 提出其他请求， `@odata.nextLink` 直到返回所有结果。 有关详细信息，请参阅分页[Microsoft Graph应用中的数据](/graph/paging.md)。

## <a name="examples"></a>示例

以下示例获取针对已登录用户的访问包分配的状态。

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "accesspackageassignment_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments/filterByCurrentUser(on='target')
```


### <a name="response"></a>响应
> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
        {
            "@odata.type": "#microsoft.graph.accessPackageAssignment",
            "id": "5521fb4f-6a6c-410a-9191-461a65fd39d4",
            "catalogId": "34cfe9a8-88bc-4c82-b3d8-6b77d7035c33",
            "accessPackageId": "ca6992f8-e413-49a1-9619-c9819f4f73e0",
            "assignmentPolicyId": "7c6e6874-789e-4f11-b351-cc7b5883deef",
            "targetId": "2cb14f51-0108-41d8-89da-cd0e05e2c988",
            "assignmentStatus": "Delivered",
            "assignmentState": "Delivered",
            "isExtended": false,
            "expiredDateTime": null,
            "schedule": {
                "startDateTime": "2021-01-19T20:02:36.013Z",
                "recurrence": null,
                "expiration": {
                    "endDateTime": "2022-01-19T20:02:36.013Z",
                    "duration": null,
                    "type": "afterDateTime"
                }
            }
        }
  ]
}

```

