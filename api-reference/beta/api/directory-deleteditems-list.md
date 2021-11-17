---
title: 列出已删除的项目
description: 从已删除的项目中检索最近删除的项目列表。
author: keylimesoda
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b0c5edfe90d551a1db4c709fd26bb8881e78e0e9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987049"
---
# <a name="list-deleted-items"></a>列出已删除项目

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从[已删除的项目](../resources/directory.md)中检索最近删除的项目列表。

目前，仅应用程序、组和用户资源支持[已删除项目功能](../resources/user.md)。 [](../resources/group.md) [](../resources/application.md)

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

### <a name="for-applications"></a>对于应用程序：

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Application.Read.All、Application.ReadWrite.All、Directory.Read.All |

### <a name="for-users"></a>对于用户：

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序 | User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All |

### <a name="for-groups"></a>对于组：

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Group.Read.All、Group.ReadWrite.All、Directory.Read.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.application
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

此 API 当前支持检索应用程序的对象类型 () 、组 `microsoft.graph.application` () 用户 () `microsoft.graph.group` `microsoft.graph.user` 删除的项目。 OData 转换类型是 URI 的必需部分，不支持在没有类型 `GET /directory/deleteditems` 的情况下 **调用** 。

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 OData 转换指定的资源支持的查询参数。 即 `$count` `$expand` `$filter` ，、、、、、、 `$orderBy` `$search` `$select` 和 `$top` 查询参数。 只有将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count` 时，才支持某些查询。 例如：

```msgraph-interactive
https://graph.microsoft.com/beta/directory/deletedItems/microsoft.graph.group?&$count=true&$orderBy=deletedDateTime desc&$select=id,displayName,deletedDateTime
ConsistencyLevel: eventual
```

此示例需要 **ConsistencyLevel** 标头，因为 查询中使用了 和 `$orderBy` `$count` 查询参数。

### <a name="examples-using-the-orderby-odata-query-parameter"></a>使用 OData $orderBy参数的示例

`$orderBy`在已删除的对象类型的 **deletedDateTime** **、displayName** 和 **userPrincipalName** 属性上支持 OData 查询参数。 在 **deletedDateTime** 属性上，查询需要将 [](/graph/aad-advanced-queries)高级查询参数 (**ConsistencyLevel** 标头设置为 ， `true` 并添加 `$count=true` 查询字符串) 。

| OData 转换 | 支持属性$orderBy | 示例 |
| :--- | :--- | :--- |
| microsoft.graph.user | deletedDateTime、displayName、userPrincipalName | /directory/deletedItems/microsoft.graph.user？$orderBy=userPrincipalName |
| microsoft.graph.group | deletedDateTime， displayName | /directory/deletedItems/microsoft.graph.group？$orderBy=deletedDateTime asc&$count=true |
| microsoft.graph.application | deletedDateTime， displayName | /directory/deletedItems/microsoft.graph.application？$orderBy=displayName |
| microsoft.graph.device | deletedDateTime， displayName | /directory/deletedItems/microsoft.graph.device？$orderBy=deletedDateTime&$count=true |

## <a name="request-headers"></a>请求头
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

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deleteditems-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deleteditems-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deleteditems-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-deleteditems-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-deleteditems-go-snippets.md)]
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
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

### <a name="example-2-retrieve-the-count-of-deleted-user-objects-and-order-the-results-by-the-deleteddatetime-property"></a>示例 2：检索已删除用户对象的计数，并按 deletedDateTime 属性对结果排序

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/deletedItems/microsoft.graph.group?$count=true&$orderBy=deletedDateTime asc&$select=id,displayName,deletedDateTime
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

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-deleteditems-count-go-snippets.md)]
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(id,displayName,deletedDateTime)",
    "@odata.count": 3,
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/54c8f8fa-7217-4846-baf9-94af2381864f/Microsoft.DirectoryServices.Group",
            "id": "54c8f8fa-7217-4846-baf9-94af2381864f",
            "displayName": "Digital Initiative Public Relations",
            "deletedDateTime": "2021-09-07T15:41:06Z"
        },
        {
            "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/a7acbd5f-07ec-4b97-9fbf-8fe94d44b044/Microsoft.DirectoryServices.Group",
            "id": "a7acbd5f-07ec-4b97-9fbf-8fe94d44b044",
            "displayName": "GitHub issue #13843",
            "deletedDateTime": "2021-09-07T15:41:57Z"
        },
        {
            "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/1a5999a0-3b42-498e-b408-0c2f9951db1d/Microsoft.DirectoryServices.Group",
            "id": "1a5999a0-3b42-498e-b408-0c2f9951db1d",
            "displayName": "GitHub issue #13843",
            "deletedDateTime": "2021-09-07T15:42:03Z"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
