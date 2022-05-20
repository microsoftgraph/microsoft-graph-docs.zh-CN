---
title: 获取书签
description: 读取书签对象的属性和关系。
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 2b02bfc05e0fc1e993942c7002287a62edc19947
ms.sourcegitcommit: 995056279c2151d7ce4a0fcff067fbc6edced728
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2022
ms.locfileid: "65602789"
---
# <a name="get-bookmark"></a>获取书签
命名空间：microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取 [书签](../resources/search-bookmark.md) 对象的属性和关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）| SearchConfiguration.Read.All、SearchConfiguration.ReadWrite.All |
|委派（个人 Microsoft 帐户）| 不支持。 |
|应用程序| SearchConfiguration.Read.All、SearchConfiguration.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /search/bookmarks/{bookmarksId}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `select`[OData](/graph/query-parameters) `expand``orderBy``filter`查询参数，`maxTop``count`以帮助自定义响应。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [书签](../resources/search-bookmark.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookmark"
}
-->
``` http
GET https://graph.microsoft.com/beta/search/bookmarks/{bookmarksId}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookmark-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookmark-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookmark-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookmark-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-bookmark-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-bookmark-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.search.bookmark"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "733b26d5-af76-4eea-ac69-1a0ce8716897",
  "displayName": "Italy Holiday",
  "webUrl": "http://www.margiestravel.com/",
  "description": "Book a fancy vacation in Tuscany or browse museums in Florence.",
  "lastModifiedDateTime": "2016-03-21T20:01:37Z",
  "lastModifiedBy": {
    "user": {
        "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
        "displayName": "Amalie Larsen"
    }
  },
  "keywords":  {
    "keywords": ["Vacation in Europe", "Holiday in Europe"],
    "reservedKeywords": ["Vacation in Italy"],
    "matchSimilarKeywords": true
  },
  "categories": ["HR"],
  "availabilityStartDateTime": "2020-09-21T20:01:37Z",
  "availabilityEndDateTime": "2020-11-21T20:01:37Z",
  "languageTags": ["en-us"],
  "platforms": ["ios"],
  "groupIds": ["groupId"],
  "targetedVariations": null,
  "powerAppIds": ["powerAppId"],
  "state": "published",
  "isSuggested": false
}
```

