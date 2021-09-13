---
author: JeremyKelley
ms.date: 09/10/2017
title: 删除文件或文件夹
ms.localizationpriority: medium
ms.prod: sharepoint
description: 通过使用其 ID 或路径删除 DriveItem。
doc_type: apiPageType
ms.openlocfilehash: 9e08bd7510c57b011e33acd36c022e5476841173
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59140863"
---
# <a name="delete-a-driveitem"></a>删除 DriveItem

命名空间：microsoft.graph

通过使用其 ID 或路径删除 [DriveItem](../resources/driveitem.md)。注意，使用此方法删除项将把项移动到回收站中，而不是永久删除该项。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Files.ReadWrite、Files.ReadWrite.All    |
|应用程序 | Files.ReadWrite.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a>可选的请求标头

| 名称          | 类型   | 说明                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-match      | String | 如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。 |

## <a name="example"></a>示例

下面是一个如何调用此 API 的示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "delete-drive-item", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
DELETE /me/drive/items/{item-id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-drive-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-drive-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-drive-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-drive-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a>响应

如果成功，此调用将返回 `204 No Content` 响应，以指明资源已被删除，没有可返回的内容。

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

### <a name="error-responses"></a>错误响应

请参阅[错误响应][error-response]，详细了解错误返回方式。

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a DriveItem from a drive",
  "keywords": "delete,existing item,onedrive",
  "section": "documentation",
  "tocPath": "Items/Delete",
  "suppressions": [
  ]
} -->

