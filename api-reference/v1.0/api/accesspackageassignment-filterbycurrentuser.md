---
title: accessPackageAssignment：filterByCurrentUser
description: 检索在登录用户上筛选的 accesspackageassignment 对象列表。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9ed084f91e84d288ad8ea3d7d07ebaa4b32ffa9e
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242303"
---
# <a name="accesspackageassignment-filterbycurrentuser"></a>accessPackageAssignment：filterByCurrentUser
命名空间：microsoft.graph


在[Azure AD管理](../resources/entitlementmanagement-root.md)中，检索已登录用户筛选的[accessPackageAssignment](../resources/accesspackageassignment.md)对象列表。

## <a name="permissions"></a>Permissions
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
GET /identityGovernance/entitlementManagement/assignments/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a>函数参数
下表显示了可用于此函数的参数。

|参数|类型|说明|
|:---|:---|:---|
|on|accessPackageAssignmentFilterByCurrentUserOptions|可用于筛选访问包分配列表的用户选项列表。|

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

当结果集跨多个页面时，Microsoft Graph 在响应中返回包含指向下一页结果 `@odata.nextLink` 的 URL 的属性的页面。 如果存在该属性，请继续使用每个响应中的 URL 提出其他请求， `@odata.nextLink` 直到返回所有结果。 有关详细信息，请参阅分页[Microsoft Graph应用中的数据](/graph/paging)。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "accesspackageassignment_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignments/filterByCurrentUser(on='target')
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
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
      "id": "5521fb4f-6a6c-410a-9191-461a65fd39d4",
      "state": "delivered",
      "status": "Delivered",
      "expiredDateTime": "null",
      "schedule": {
        "@odata.type": "microsoft.graph.entitlementManagementSchedule"
      }
    }
  ]
}
```

