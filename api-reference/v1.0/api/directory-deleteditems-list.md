---
title: '列出 deletedItems (目录对象) '
description: 从已删除的项目中检索最近删除的项目列表。
author: keylimesoda
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6ed39739978d7d72427e32f01445d9bcac36c930
ms.sourcegitcommit: 033e779ba738b61b03e2760f39554a2fd0ab65b4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2022
ms.locfileid: "66788771"
---
# <a name="list-deleteditems-directory-objects"></a>列出 deletedItems (目录对象) 

命名空间：microsoft.graph

检索最近删除的目录对象的列表。 目前，仅[应用程序、](../resources/application.md)[组](../resources/group.md)和[用户](../resources/user.md)资源支持此功能。

目前，删除的项目功能仅支持 [应用程序](../resources/application.md)、 [servicePrincipal](../resources/serviceprincipal.md)、 [组](../resources/group.md)和 [用户](../resources/user.md) 资源。

>**注意：** 已删除的安全组将被永久删除，无法通过此 API 检索。

## <a name="permissions"></a>权限

[!INCLUDE [limited-info](../../includes/limited-info.md)]

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

### <a name="for-applications-and-service-principals"></a>对于应用程序和服务主体：

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Application.Read.All、Application.ReadWrite.All、Directory.Read.All |

### <a name="for-users"></a>对于用户：

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序 | User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All |

### <a name="for-groups"></a>对于组：

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Group.Read.All、Group.ReadWrite.All、Directory.Read.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Group.Read.All、Group.ReadWrite.All、Directory.Read.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.application
GET /directory/deleteditems/microsoft.graph.servicePrincipal
GET /directory/deletedItems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
GET /directory/deletedItems/microsoft.graph.device
```

此 API 目前支持检索 () 、servicePrincipals (`microsoft.graph.application`) 、组 (`microsoft.graph.serviceprincipal`) `microsoft.graph.group` 或从已删除项 (`microsoft.graph.user`) 的用户的对象类型。 OData 强制转换类型是 URI 的必需部分，**不** 支持不使用类型调用`GET /directory/deleteditems`。

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持由 OData 强制转换指定的资源支持的查询参数。 即、、`$count``$expand`、`$filter`、`$orderBy`、`$search``$select`和`$top`查询参数。 只有将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count` 时，才支持某些查询。 例如：

```msgraph-interactive
https://graph.microsoft.com/beta/directory/deletedItems/microsoft.graph.group?&$count=true&$orderBy=deletedDateTime desc&$select=id,displayName,deletedDateTime
ConsistencyLevel: eventual
```

此示例需要 **ConsistencyLevel** 标头， `$orderBy` 因为查询中使用了查询参数和 `$count` 查询参数。

### <a name="examples-using-the-orderby-odata-query-parameter"></a>使用 $orderBy OData 查询参数的示例

已 `$orderBy` 删除对象类型的 **deletedDateTime**、 **displayName** 和 **userPrincipalName** 属性支持 OData 查询参数。 在 **deletedDateTime** 属性上，查询需要添加 [高级查询参数](/graph/aad-advanced-queries) (将 **ConsistencyLevel** 标头设置为`true``$count=true`查询字符串) 。

| OData 强制转换 | 支持$orderBy的属性 | 示例 |
| :--- | :--- | :--- |
| microsoft.graph.user | deletedDateTime、displayName、userPrincipalName | /directory/deletedItems/microsoft.graph.user？$orderBy=userPrincipalName |
| microsoft.graph.group | deletedDateTime、displayName | /directory/deletedItems/microsoft.graph.group？$orderBy=deletedDateTime asc&$count=true |
| microsoft.graph.application | deletedDateTime、displayName | /directory/deletedItems/microsoft.graph.application？$orderBy=displayName |
| microsoft.graph.device | deletedDateTime、displayName | /directory/deletedItems/microsoft.graph.device？$orderBy=deletedDateTime&$count=true |

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer &lt;code&gt;。*必需*|
| 接受  | application/json |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。
## <a name="examples"></a>示例

### <a name="example-1-retrieve-deleted-groups"></a>示例 1：检索已删除的组

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group
```

#### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "value": [
    {
      "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
      "displayName":"SampleGroup",
      "groupTypes":["Unified"],
      "mail":"example@contoso.com",
      "mailEnabled":true,
      "mailNickname":"Example",
      "securityEnabled":false,
      "visibility":"Public"
    }
  ]
}
```

### <a name="example-2-retrieve-the-count-of-deleted-user-objects-and-order-the-results-by-the-deleteddatetime-property"></a>示例 2：检索已删除用户对象的计数，并按 deletedDateTime 属性对结果进行排序

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group?$count=true&$orderBy=deletedDateTime asc&$select=id,DisplayName,deletedDateTime
ConsistencyLevel: eventual
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deleteditems-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deleteditems-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deleteditems-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-deleteditems-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-deleteditems-count-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-deleteditems-count-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups(id,displayName,deletedDateTime)",
    "@odata.count": 2,
    "value": [
        {
            "id": "c31799b8-0683-4d70-9e91-e032c89d3035",
            "displayName": "Role assignable group",
            "deletedDateTime": "2021-10-26T16:56:36Z"
        },
        {
            "id": "74e45ce0-a52a-4766-976c-7201b0f99370",
            "displayName": "Role assignable group",
            "deletedDateTime": "2021-10-26T16:58:37Z"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
