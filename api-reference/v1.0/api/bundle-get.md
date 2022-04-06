---
author: JeremyKelley
title: 获取捆绑包
description: 获取 driveItems 捆绑包
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 41d8c613095e9a3b167f25f457167ca3393fb207
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/17/2022
ms.locfileid: "63561582"
---
# <a name="get-bundle"></a>获取捆绑包

命名空间：microsoft.graph

根据捆绑 [包的唯一][] ID 检索捆绑包的元数据。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 不支持。                             |
|委派（个人 Microsoft 帐户） | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All    |
|应用程序          | 不支持。                                           |

## <a name="http-request"></a>HTTP 请求

```http
GET /drive/bundles/{bundle-id}
GET /drive/items/{bundle-id}
```

由于捆绑包是项，因此可以使用 **items** 集合返回有关捆绑包的元数据。
您还可以使用 **bundles 集合** 作为方便，以确保收到响应中的捆绑包。

## <a name="optional-query-parameters"></a>可选的查询参数

可以使用 [OData查询参数][odata-parameters]限制通过此调用返回的对象的形状。

## <a name="request-headers"></a>请求标头
| 名称          | 说明  |
|:------------- |:------------ |
| Authorization | 持有者 \{token\}。必需。 |
| if-none-match | eTag。 可选。 如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。

## <a name="request-body"></a>请求正文

请勿为此方法提供请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 [driveItem][driveItem]resource with the [bundle][bundle]。

有关错误响应的信息，请参阅 [错误响应][error-response]。

## <a name="examples"></a>示例

### <a name="example-1-get-a-bundle"></a>示例 1：获取捆绑包

#### <a name="request"></a>请求

<!-- { "blockType": "request", "name": "get-bundle-metadata" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles/{bundle-id}
```

#### <a name="response"></a>响应

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "My Photo Album Bundle",
  "eTag": "etag",
  "cTag": "etag",
  "createdBy": { "user": { "id": "1234", "displayName": "Ryan Gregg" } },
  "createdDateTime": "datetime",
  "lastModifiedBy": { "user": { "id": "1234", "displayName": "Ryan Gregg" } },
  "lastModifiedDateTime": "datetime",
  "size": 1234,
  "webUrl": "http://onedrive.com/...",
  "bundle": {
    "childCount": 4,
     "album": { }
  }
}
```

为了提高可读性，可能缩短了此处显示的响应对象。

### <a name="example-2-get-a-bundle-and-its-children-in-a-single-call"></a>示例 2：在单个调用中获取捆绑包及其子项

可以使用查询 [`expand`](/graph/query-parameters) 字符串参数在检索捆绑包元数据的同一调用中包括捆绑包的子项。

#### <a name="request"></a>请求

<!-- { "blockType": "request", "name": "get-bundle-and-children" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/items/{bundle-id}?expand=children
```

#### <a name="response"></a>响应

此调用将返回捆绑包元数据和捆绑包的子项列表。
如果捆绑包没有子项，它将返回空集合。

如果捆绑包中的子项数量大于默认页面大小， **children@odata.nextLink** 属性将返回一个 URL，该 URL 可用于请求捆绑包中的下一页子项。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "101230100alkc",
  "name": "My Cool Day at the Beach",
  "children": [
    { "id": "120100abab", "name": "image1.jpg", "file": {} },
    { "id": "120100abo1", "name": "image2.jpg", "file": {} }
  ],
  "children@odata.nextLink": "https://api.onedrive.com/v1.0/..."
}
```

为了提高可读性，可能缩短了此处显示的响应对象。


[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters


<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about a bundle and its children in OneDrive",
  "keywords": "retrieve,item,bundle,metadata",
  "section": "documentation",
  "tocPath&quot;: &quot;Bundles/Get Bundle Metadata"
} -->


