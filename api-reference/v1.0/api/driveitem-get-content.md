---
author: JeremyKelley
title: 下载文件
ms.localizationpriority: high
ms.prod: sharepoint
description: 下载 DriveItem 的主要流 (文件) 的内容。 只能下载具有 file 属性的 driveItem。
doc_type: apiPageType
ms.openlocfilehash: 5e5e3a2b9d174957b80c0a74e96d3a658279e44d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336331"
---
# <a name="download-the-contents-of-a-driveitem"></a>下载 DriveItem 的内容

命名空间：microsoft.graph

[!INCLUDE [tls-1.2-required](../../includes/tls-1.2-required.md)]

下载 [DriveItem](../resources/driveitem.md) 的主要流 (文件) 的内容。 仅能下载具有 **文件** 属性的 **DriveItems**。

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
GET /drives/{drive-id}/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /shares/{shareIdOrEncodedSharingUrl}/driveItem/content
GET /sites/{siteId}/drive/items/{item-id}/content
GET /users/{userId}/drive/items/{item-id}/content
```

## <a name="optional-request-headers"></a>可选的请求标头

| 名称          | 值  | 说明                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-none-match | String | 如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。 |

## <a name="example"></a>示例

下面是下载整个文件的示例。

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "download-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/content
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/download-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/download-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/download-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/download-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

返回 `302 Found` 响应，该响应重定向到文件的预先身份验证的下载 URL。这是可通过 DriveItem 上的 `@microsoft.graph.downloadUrl` 属性获得的同一个 URL。

应用必须遵循响应中的 `Location` 头，才能下载文件内容。许多 HTTP 客户端库将自动遵循 302 重定向并立即开始下载文件。

已预先验证的下载 URL 仅在短期（几分钟）内有效，无需 `Authorization` 头即可下载。

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="downloading-files-in-javascript-apps"></a>在 JavaScript 应用中下载文件
若要在 JavaScript 应用中下载文件，不能使用 `/content` API，因为这会以 `302` 重定向响应。当需要 [跨源资源共享 (CORS)](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS) _预检_ 时 (例如，在提供 **授权** 标头时)，明确禁止使用 `302` 重定向。

相反，应用需要选择 `@microsoft.graph.downloadUrl` 属性，该属性返回 `/content` 指向的相同 URL。
然后，便可以使用 XMLHttpRequest 直接向此 URL 发出请求。
由于这些 URL 已预先验证，因此可以在没有 CORS 预检请求的情况下检索它们。

### <a name="example"></a>示例

若要检索文件的下载 URL，请先发出包含 `@microsoft.graph.downloadUrl` 属性的请求：

```http
GET /drive/items/{item-ID}?select=id,@microsoft.graph.downloadUrl
```

这会返回文件 ID 和下载 URL:

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "12319191!11919",
  "@microsoft.graph.downloadUrl": "https://..."
}
```

然后，可以使用 XMLHttpRequest 向 `@microsoft.graph.downloadUrl` 中提供的 URL 发出请求，从而检索文件。

## <a name="partial-range-downloads"></a>部分范围下载

若要从文件中下载部分范围的字节，应用程序可以使用 [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt) 中指定的 `Range` 标头。请注意，必须将 `Range` 标头附加到实际 `@microsoft.graph.downloadUrl` URL，而不是 `/content` 的请求。

<!-- { "blockType": "request", "opaqueUrl": true, "name": "download-item-partial", "scopes": "files.read" } -->

```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

此方法将返回 `HTTP 206 Partial Content` 响应和文件中字节的请求区域。如果无法生成此范围，可能会忽略 Range 标头，并会返回包含文件完整内容的 `HTTP 200` 响应。

<!-- { "blockType": "response", "name": "download-item-partial", "@odata.type": "stream" } -->

```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048
Content-Type: application/octet-stream

<first 1024 bytes of file>
```

### <a name="error-responses"></a>错误响应

请参阅[错误响应][error-response]，详细了解错误返回方式。

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Download the contents of a DriveItem.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Items/Download",
  "suppressions": [
  ]
} -->

