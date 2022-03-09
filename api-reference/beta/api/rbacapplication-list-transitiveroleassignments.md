---
title: 列出 transitiveRoleAssignment
description: 列出特定主体的直接和可传递角色分配。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 8bcd70fc0c6e57b4f069f40428a25a308a50f67b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63396306"
---
# <a name="list-transitiveroleassignment"></a>列出 transitiveRoleAssignment

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取特定主体的直接和可传递 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象列表。 例如，如果用户通过组成员身份Azure AD角色，角色分配是可传递的，并且此请求将组 ID 作为 **principalId 列出**。 也可以按 **roleDefinitionId** 和 **directoryScopeId 筛选结果**。 仅支持目录 (Azure AD) 提供程序。

有关详细信息，请参阅使用[Azure AD组管理角色分配](/azure/active-directory/roles/groups-concept)。

> [!NOTE]
> 对于最近创建、更新或删除的角色分配，此请求可能有复制延迟。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

列出目录提供程序的可传递角色分配：

<!-- {
  "blockType": "ignored"
}
-->
```http
GET /roleManagement/directory/transitiveRoleAssignments?$filter=principalId eq '{principalId}'
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 `$count`、 `$filter` (`eq`) `$select` 和 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。 可以按 **principalId**、 **roleDefinitionId** 和 **directoryScopeId** 进行筛选，以检索主体的直接和可传递角色分配。

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | Bearer {token} 必填。 |
| ConsistencyLevel | 最终。 此标头 、 `$count`和 `$filter` 是必需的。 有关使用 **ConsistencyLevel**`$count``$filter`、和 有关详细信息，请参阅对 Azure AD [对象的高级查询功能](/graph/aad-advanced-queries)。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象集合。

## <a name="examples"></a>示例
对于本节中的示例，请考虑以下角色分配方案。 名为 Alice 的用户具有直接角色分配和可传递角色分配，如下所示：

| 用户 | 组 | Role | 范围 | 角色分配 ID |
| :---: | :---: | :---: | :---: | :---: |
| Alice<br/>`2c7936bc-3517-40f3-8eda-4806637b6516` |  | 用户管理员<br/>`fe930be7-5e62-47db-91af-98c3a49a38b1` | 租户 | RA1<br/>`857708a7-b5e0-44f9-bfd7-53531d72a739` |
|  | G1<br/>`ae2fc327-4c71-48ed-b6ca-f48632186510`<br/> (Alice 是成员)  | 用户管理员<br/>`fe930be7-5e62-47db-91af-98c3a49a38b1` | 租户 | RA2<br/>`8a021d5f-7351-4713-aab4-b088504d476e` |
|  | G2<br/>`6ffb34b8-5e6d-4727-a7f9-93245e7f6ea8`<br/> (Alice 是成员)  | 帮助台管理员<br/>`729827e3-9c14-49f7-bb1b-9608f156bbb8` | AU1 (管理) <br/>`26e79164-0c5c-4281-8c5b-be7bc7809fb2` | RA3<br/>`6cc86637-13c8-473f-afdc-e0e65c9734d2` |

+ Alice 直接在租户范围内分配有 RA1 的用户角色分配角色。 
+ Alice 是组 G1 的成员，G1 在租户范围内分配了具有 RA2 的用户角色分配角色。
+ Alice 还是组 G2 的成员，G2 在管理单元 AU1 作用域中分配有支持管理员角色，角色分配 RA3。

### <a name="example-1--get-direct-and-transitive-role-assignments-of-a-principal"></a>示例 1：获取主体的直接和可传递角色分配

#### <a name="request"></a>请求

下面展示了示例请求。 此请求需要 **将 ConsistencyLevel** 标头设置为 和 `eventual` `$count=true` 查询 `$filter` 参数。 有关使用 **ConsistencyLevel**`$count``$filter`、和 有关详细信息，请参阅对 Azure AD [对象的高级查询功能](/graph/aad-advanced-queries)。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_all"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/transitiveRoleAssignments?$count=true&$filter=principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516'
ConsistencyLevel: eventual
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-all-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-all-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-all-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-all-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-unifiedroleassignment-all-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-unifiedroleassignment-all-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


#### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/transitiveRoleAssignments",
    "value": [
        {
            "id": "857708a7-b5e0-44f9-bfd7-53531d72a739",
            "principalId": "2c7936bc-3517-40f3-8eda-4806637b6516",
            "directoryScopeId": "/",
            "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1"
        },
        {
            "id": "8a021d5f-7351-4713-aab4-b088504d476e",
            "principalId": "ae2fc327-4c71-48ed-b6ca-f48632186510",
            "directoryScopeId": "/",
            "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1"
        },
        {
            "id": "6cc86637-13c8-473f-afdc-e0e65c9734d2",
            "principalId": "6ffb34b8-5e6d-4727-a7f9-93245e7f6ea8",
            "directoryScopeId": "/administrativeUnits/26e79164-0c5c-4281-8c5b-be7bc7809fb2",
            "roleDefinitionId": "729827e3-9c14-49f7-bb1b-9608f156bbb8"
        }
    ]
}
```

### <a name="example-2-get-direct-and-transitive-assignments-of-a-principal-but-only-specific-role-definitions"></a>示例 2：获取主体的直接和可传递分配，但仅获取特定角色定义

#### <a name="request"></a>请求

下面展示了示例请求。 此请求需要 **将 ConsistencyLevel** 标头设置为 和 `eventual` `$count=true` 查询 `$filter` 参数。 有关使用 **ConsistencyLevel**`$count``$filter`、和 有关详细信息，请参阅对 Azure AD [对象的高级查询功能](/graph/aad-advanced-queries)。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_transitive"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/transitiveRoleAssignments?$count=true&$filter=principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516' and roleDefinitionId eq 'fe930be7-5e62-47db-91af-98c3a49a38b1'
ConsistencyLevel: eventual
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-transitive-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-transitive-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-transitive-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-transitive-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-unifiedroleassignment-transitive-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-unifiedroleassignment-transitive-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/transitiveRoleAssignments",
    "value": [
        {
            "id": "857708a7-b5e0-44f9-bfd7-53531d72a739",
            "principalId": "2c7936bc-3517-40f3-8eda-4806637b6516",
            "directoryScopeId": "/",
            "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1"
        },
        {
            "id": "8a021d5f-7351-4713-aab4-b088504d476e",
            "principalId": "6ffb34b8-5e6d-4727-a7f9-93245e7f6ea8",
            "directoryScopeId": "/",
            "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1"
        }
    ]
}
```

### <a name="example-3-get-direct-and-transitive-role-assignments-of-a-principal-but-only-administrative-unit-scoped"></a>示例 3：获取主体的直接和可传递角色分配，但仅作用域为管理单元

#### <a name="request"></a>请求

下面展示了示例请求。 此请求需要 **将 ConsistencyLevel** 标头设置为 和 `eventual` `$count=true` 查询 `$filter` 参数。 有关使用 **ConsistencyLevel**`$count``$filter`、和 有关详细信息，请参阅对 Azure AD [对象的高级查询功能](/graph/aad-advanced-queries)。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_tenantscoped"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/transitiveRoleAssignments?$count=true&$filter=principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516' and directoryScopeId eq '/administrativeUnits/26e79164-0c5c-4281-8c5b-be7bc7809fb2'
ConsistencyLevel: eventual
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-tenantscoped-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-tenantscoped-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-tenantscoped-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-tenantscoped-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-unifiedroleassignment-tenantscoped-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-unifiedroleassignment-tenantscoped-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


#### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/transitiveRoleAssignments",
    "value": [
        {
            "id": "6cc86637-13c8-473f-afdc-e0e65c9734d2",
            "principalId": "6ffb34b8-5e6d-4727-a7f9-93245e7f6ea8",
            "directoryScopeId": "/administrativeUnits/26e79164-0c5c-4281-8c5b-be7bc7809fb2",
            "roleDefinitionId": "729827e3-9c14-49f7-bb1b-9608f156bbb8"
        }
    ]
}
```
