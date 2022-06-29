---
author: JeremyKelley
ms.date: 09/10/2017
title: 列出文件夹的内容
ms.localizationpriority: high
ms.prod: sharepoint
description: 在 DriveItem 的子项关系中返回 DriveItems 集合。
doc_type: apiPageType
ms.openlocfilehash: 38834367de258bf7f9a5758945f211fd0f28a6be
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443494"
---
# <a name="list-children-of-a-driveitem"></a>列出 DriveItem 的子项

命名空间：microsoft.graph

在 DriveItem 的 **children** 关系中返回 [DriveItems](../resources/driveitem.md) 集合。

具有非 null **folder** 或 **package** facet 的 DriveItem 可以拥有一个或多个子 DriveItem。


## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All    |
|应用程序 | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/items/{item-id}/children
GET /me/drive/items/{item-id}/children
GET /sites/{site-id}/drive/items/{item-id}/children
GET /users/{user-id}/drive/items/{item-id}/children
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 `$expand`、`$select`、`$skipToken`、`$top` 和 `$orderby` [OData 查询参数](/graph/query-parameters)自定义响应。

### <a name="optional-request-headers"></a>可选的请求标头

| 名称     | 值 | 说明                                                                                                                                              |
|:----------------|:------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| _if-none-match_ | etag  | 如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。 |

## <a name="examples"></a>示例

### <a name="list-children-in-the-root-of-the-current-users-drive"></a>列出当前用户的驱动器根目录中的子项

若要检索驱动器根目录中的文件，请使用驱动器上的 `root` 关系，然后访问子项关系。


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "list-children-root", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/root/children
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-children-root-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-children-root-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-children-root-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-children-root-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="list-children-of-a-driveitem-with-a-known-id"></a>列出带已知 ID 的 DriveItem 子项

若要检索驱动器根目录中的文件，请使用驱动器上的 `root` 关系，然后访问子项关系。


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "list-children-files", "scopes": "files.read" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/children
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-children-files-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-children-files-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-children-files-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-children-files-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-children-files-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-children-files-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="list-children-of-a-driveitem-with-a-known-path"></a>列出带已知路径的 DriveItem 子项

<!-- { "blockType": "request", "name": "list-children-from-path", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/root:/{path-relative-to-root}:/children
```

## <a name="response"></a>响应

如果成功，此方法将返回目标项的子项集合列表。 子项集合由 [driveItem][item-resource] 资源组成。

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.driveItem)", 
       "truncated": true,
       "name": [ "list-children-root", "list-children-files", "list-children-from-path" ] } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048, "file": {} },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ],
  "@odata.nextLink": "https://..."
}
```

**注意：** 如果集合超出默认页面大小（200 项），则在响应中返回 **\@odata.nextLink** 属性以指示有更多项可用，并提供下一页项目的请求 URL。

可以通过[可选的查询字符串参数](/graph/query-parameters)控制页面大小

### <a name="error-responses"></a>错误响应

请参阅[错误响应][error-response]，详细了解错误返回方式。

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "Items/List children",
  "suppressions": [
  ]
} -->
