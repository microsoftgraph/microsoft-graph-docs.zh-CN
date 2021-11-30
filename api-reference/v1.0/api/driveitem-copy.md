---
author：一个 Author：一个用户，作者：一个 Author：driveItem：copy ms.localizationpriority： medium ms.prod： "sharepoint" description： "Asynchronously creates a copy of an driveItem (including any children) ， under a new parent item or with a new name."
doc_type： apiPageType
---
# <a name="driveitem-copy"></a>driveItem：copy

命名空间：microsoft.graph

以异步方式在新父项下或使用新名称创建一个 [driveItem][item-resource] 副本（包括任何子项）。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Files.ReadWrite、Files.ReadWrite.All    |
|应用程序 | Files.ReadWrite.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 `@microsoft.graph.conflictBehavior` 查询参数在发生冲突时自定义行为。

| 值           | 说明                                    |
|:----------------|:---------------------------------------------- |
| 失败            | 默认行为是报告失败。     |
| replace         | 覆盖目标网站中的现有项目。    |
| rename          | 重命名该项目。                               |

**注意：**_conflictBehavior_ 不受 OneDrive 支持。

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。


| 名称            | 值                                          | 说明                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| parentReference | [ItemReference](../resources/itemreference.md) | 可选。引用在其中创建副本的父项。                                         |
| name            | string                                         | 可选。副本的新名称。如果未提供新名称，将同一名称用作原始名称。    |

**注意：**_parentReference_ 应包括目标文件夹的 `driveId` 和 `id` 参数。

## <a name="response"></a>响应

返回有关如何在接受请求时[监视复制操作进度](/graph/long-running-actions-overview)的详细信息。

## <a name="example"></a>示例

本示例将由 `{item-id}` 标识的文件复制到使用 `driveId` 和 `id` 值标识的文件夹。
该文件的新副本将被命名为 `contoso plan (copy).txt`。


### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite", "tags": "service.graph", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "driveId": "6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B",
    "id": "DCD0D3AD-8989-4F23-A5A2-2C086050513F"
  },
  "name": "contoso plan (copy).txt"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/copy-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/copy-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/copy-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/copy-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>响应

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

`Location` 头值提供的服务 URL 将返回复制操作的最新状态。
可以使用此信息来确定 [复制何时完成](/graph/long-running-actions-overview)。

### <a name="remarks"></a>注解

在许多情况下，异步执行复制操作。
来自 API 的响应将仅指示复制操作已接受或拒绝;例如，由于目标文件名已在使用中。

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
} -->

