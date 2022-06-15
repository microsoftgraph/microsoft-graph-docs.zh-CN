---
title: 下载 driveItemVersion 资源的内容
description: 检索 driveItem 的特定版本的内容。
ms.localizationpriority: medium
ms.prod: sharepoint
author: JeremyKelley
doc_type: apiPageType
ms.openlocfilehash: c8f080ab1893ea520f4e2094e914356ce71010b6
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094658"
---
# <a name="download-contents-of-a-driveitemversion-resource"></a>下载 driveItemVersion 资源的内容

命名空间：microsoft.graph

检索 [driveItem](../resources/driveitem.md) 的特定版本的内容。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All    |
|应用程序 | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All |


## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/items/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a>响应

返回 `302 Found` 响应，重定向到文件字节已预先验证的下载 URL。

应用必须遵循响应中的 `Location` 头，才能下载文件内容。许多 HTTP 客户端库将自动遵循 302 重定向并立即开始下载文件。

已预先验证的下载 URL 仅在短期（几分钟）内有效，无需 `Authorization` 头即可下载。

## <a name="example"></a>示例

本示例检索当前用户驱动器中的文件版本。

### <a name="http-request"></a>HTTP 请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/versions/{version-id}/content
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-version-contents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-version-contents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-version-contents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-version-contents-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

会返回一个重定向链接，可以在其中下载版本的内容。

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Found
Location: https://onedrive.com/34FF49D6...
```


## <a name="remarks"></a>注解

OneDrive 不保留文件以前版本的完整元数据。

当你的应用检索文件的可用版本列表时，将返回 [一个 driveItemVersion](../resources/driveitemversion.md) 资源，该资源提供有关特定版本的可用信息。

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
} -->

