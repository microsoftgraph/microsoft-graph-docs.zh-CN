---
title: 更新 unifiedRoleAssignmentMultiple
description: 更新新的 unifiedRoleAssignmentMultiple 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3423c216e9b0c5b6928d0473c1e7db021e1344c9
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334491"
---
# <a name="update-unifiedroleassignmentmultiple"></a>更新 unifiedRoleAssignmentMultiple

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 RBAC [提供程序的现有 unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象。 

目前支持以下 RBAC 提供程序：
- 云电脑 
- Intune (设备) 

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

相比之下 [，unifiedRoleAssignment](../resources/unifiedroleassignment.md) 不支持更新。

## <a name="permissions"></a>权限

根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。 若要了解 [更多信息，包括在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 选择更多特权权限之前保持谨慎，请参阅 [权限](/graph/permissions-reference)。 

### <a name="for-cloud-pc-provider"></a>对于云电脑提供商

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  CloudPC.ReadWrite.All   |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | CloudPC.ReadWrite.All  |

### <a name="for-device-management-intune-provider"></a>对于 Intune (提供程序的设备) 管理

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  DeviceManagementRBAC.ReadWrite.All   |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | DeviceManagementRBAC.ReadWrite.All |


## <a name="http-request"></a>HTTP 请求

若要更新云电脑提供商的现有 unfiedRoleAssignmentMultiple：
<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/cloudPC/roleAssignments
```

若要更新 Intune 提供程序的现有 unfiedRoleAssignmentMultiple：
<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a>请求标头

| 名称 | 说明 |
|:---- |:----------- |
| Authorization | Bearer {token}。必需。 |
| Content-type | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) 对象。

## <a name="example"></a>示例

### <a name="example-1-update-an-existing-unfiedroleassignmentmultiple-in-an-intune-provider"></a>示例 1：更新 Intune 提供程序中的现有 unfiedRoleAssignmentMultiple
### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleassignmentmultiple_from_rbacapplication"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
Content-type: application/json

{ 
    "principalIds": ["0aeec2c1-fee7-4e02-b534-6f920d25b300", "2d5386a7-732f-44db-9cf8-f82dd2a1c0e0"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。
> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 OK

```

## <a name="example-2-update-an-existing-unfiedroleassignmentmultiple-in-a-cloud-pc-provider"></a>示例 2：更新云电脑提供商中的现有 unfiedRoleAssignmentMultiple

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleassignmentmultiple_from_rbacapplication_cloudpc"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments/dbe9d288-fd87-41f4-b33d-b498ed207096
Content-type: application/json

{
    "displayName": "NewName",
    "description": "A new roleAssignment"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments/$entity",
    "id": "dbe9d288-fd87-41f4-b33d-b498ed207096",
    "description": "A new roleAssignment",
    "displayName": "NewName",
    "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
    "principalIds": [
        "0aeec2c1-fee7-4e02-b534-6f920d25b300",
        "2d5386a7-732f-44db-9cf8-f82dd2a1c0e0"
    ],
    "directoryScopeIds": [
        "/"
    ],
    "appScopeIds": []
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


