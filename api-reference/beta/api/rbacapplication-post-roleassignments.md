---
title: 创建 unifiedRoleAssignment
description: 创建新的 unifiedRoleAssignment 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a7587bf4dea653b86b4f93632e5719bcec4aaaaa
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351102"
---
# <a name="create-unifiedroleassignment"></a>创建 unifiedRoleAssignment

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象。

## <a name="permissions"></a>权限

根据 RBAC 提供程序以及 (或应用程序) 的权限类型，从下表中选择调用此 API 所需的最低特权权限。 若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。

### <a name="for-directory-azure-ad-provider"></a>对于 Azure AD (提供程序) 目录

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  RoleManagement.ReadWrite.Directory   |
|委派（个人 Microsoft 帐户） | 不支持。    |
|Application | RoleManagement.ReadWrite.Directory |

### <a name="for-entitlement-management-provider"></a>对于权利管理提供程序

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  EntitlementManagement.ReadWrite.All   |
|委派（个人 Microsoft 帐户） | 不支持。    |
|Application | 不支持。 |

## <a name="http-request"></a>HTTP 请求

为角色分配创建一个目录提供程序：

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

为角色分配提供程序创建一个权限管理提供程序：

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/entitlementManagement/roleAssignments
```


## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | 持有者 {token} |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象的 JSON 表示形式。 请求必须具有在 Azure AD 中定义的作用域（如 **directoryScopeId）** 或特定于应用程序的范围（如 **appScopeId）。** Azure AD 范围的示例包括租户 ("/") 、管理单元或应用程序。 权利管理使用租户 ("/") 访问包目录范围。 有关详细信息，请参阅 [appScope](../resources/appscope.md)。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和新的 `201 Created` [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-create-a-role-assignment-at-tenant-scope"></a>示例 1：在租户角色分配创建租户

#### <a name="request"></a>请求

下面展示了示例请求。 请注意 roleDefinitionId 的 roleTemplateId 的使用。 roleDefinitionId 可以是服务范围的模板 ID 或特定于目录的 roleDefinitionId。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignment_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments
Content-type: application/json

{ 
    "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScopeId": "/"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "YUb1sHQtUEyvox7IA_Eu_mm3jqnUe4lEhvatluHVi2I-1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScopeId": "/"
}
```

### <a name="example-2--create-a-role-assignment-over-an-administrative-unit-scope"></a>示例 2：创建角色分配管理单元作用域的组

#### <a name="request"></a>请求

以下示例将主要用户管理员角色分配给管理单元。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignment_over_administrativeunit"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1", //template id of User Account Administrator
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScopeId": "/administrativeUnits/5d107bba-d8e2-4e13-b6ae-884be90e5d1a" //object id of an administrative unit
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-over-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-over-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-over-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-over-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "BH21sHQtUEyvox7IA_Eu_mm3jqnUe4lEhvatluHIWb7-1",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScopeId": "/administrativeUnits/5d107bba-d8e2-4e13-b6ae-884be90e5d1a"
}
```


### <a name="example-3-create-a-role-assignment-at-access-package-catalog-scope"></a>示例 3：在角色分配包目录范围创建应用程序

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignment3_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/entitlementManagement/roleAssignments
Content-type: application/json

{
    "principalId": "679a9213-c497-48a4-830a-8d3d25d94ddc",
    "roleDefinitionId": "ae79f266-94d4-4dab-b730-feca7e132178",
    "appScopeId": "/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997"
}
```

#### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/entitlementManagement/roleAssignments/$entity",
    "id": "f3092518-7874-462e-93e9-0cd6c11ffc52",
    "principalId": "679a9213-c497-48a4-830a-8d3d25d94ddc",
    "roleDefinitionId": "ae79f266-94d4-4dab-b730-feca7e132178",
    "appScopeId": "/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997"
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

