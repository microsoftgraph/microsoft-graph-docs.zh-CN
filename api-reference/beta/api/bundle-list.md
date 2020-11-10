---
author: JeremyKelley
ms.author: jeremyke
title: 列出捆绑包
description: 列出用户驱动器中的捆绑包
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4704017f135f4ed30928d6c7b2736e51190819e3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960244"
---
# <a name="list-bundles"></a>列出捆绑包

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取用户驱动器中 [所有捆绑][包] 的列表。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 不支持。                             |
|委派（个人 Microsoft 帐户） | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All    |
|应用程序          | 不支持。                                           |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /drive/bundles
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 [OData 查询参数][]筛选响应和生成响应形状。

`expand=children`枚举绑定时不能使用查询参数。

## <a name="request-headers"></a>请求标头

| 名称          | 说明  |
|:------------- |:------------ |
| Authorization | 持有者 \{token\}。 必填。 |

## <a name="request-body"></a>请求正文

请勿为此方法提供请求正文。

## <a name="response"></a>响应

如果成功，此请求将返回为驱动器定义的捆绑包项的列表。

阅读 " [错误响应][error-response] " 主题，了解有关如何返回错误的详细信息。

## <a name="examples"></a>示例

### <a name="example-1-list-all-bundles-in-a-drive"></a>示例1：列出驱动器中的所有捆绑包

若要请求对驱动器中定义的所有绑定的枚举，可以向不带任何参数的 **束** 集合发出请求。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "list-all-bundles", "tags": "service.onedrive" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-all-bundles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-all-bundles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-all-bundles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-all-bundles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true, "isCollection": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0123456789abc",
      "name": "Vacation photo album",
      "bundle": {
        "childCount": 1,
        "album": { }
      }
    },
    {
      "id": "0120310201abd",
      "name": "Family shared files",
      "bundle": {
        "childCount": 1
      }
    }
  ],
  "@odata.nextLink": "https://..."
}
```

为了提高可读性，可能缩短了此处显示的响应对象。 所有属性都是从实际调用返回。


### <a name="example-2-list-all-photo-albums-in-a-drive"></a>示例2：列出驱动器中的所有相册

若要筛选从请求返回到捆绑包集合的捆绑包列表，可以使用 `filter` 查询字符串参数指定要返回的捆绑包的类型，方法是检查捆绑包中是否存在某一 facet：

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {"blockType": "request", "name": "list-album-bundles", "tags": "service.onedrive" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles?filter=bundle/album%20ne%20null
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-album-bundles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-album-bundles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-album-bundles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-album-bundles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

对绑定终结点的 GET 响应是具有[捆绑包][]的[driveItem][]资源的数组。
由于所有捆绑包都是项目，因此可以对其使用所有的标准项操作。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true, "isCollection": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0123456789abc",
      "name": "Vacation photo album",
      "bundle": {
        "childCount": 1,
        "album": { }
      }
    },
    {
      "id": "120301010abcd",
      "name": "Seattle Center event",
      "bundle": {
        "childCount": 4,
        "album": { }
      },
      "tags": [
        {
          "name": "outside",
          "autoTagged": { }
        }
      ]
    }
  ]
}
```

为了提高可读性，可能缩短了此处显示的响应对象。 所有属性都是从实际调用返回。


[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors
[OData 查询参数]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "List the bundles in a drive.",
  "keywords": "list,bundle,collection",
  "section": "documentation",
  "tocPath": "Bundles/List"
} -->


