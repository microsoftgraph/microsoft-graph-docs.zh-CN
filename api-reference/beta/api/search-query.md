---
title: 搜索：查询
description: 在此处提供说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b5da13640d2c62eb8258ca1a154ddcb8c2e1b353
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703705"
---
# <a name="search-query"></a>搜索：查询

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

执行请求正文中指定的查询。 搜索结果在响应中提供。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 阅读文章、文件、读取、ExternalItem、阅读、全部 |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

```HTTP
POST /search/query
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | 持有者 {token} |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型        | 说明 |
|:-------------|:------------|:------------|
|requests|[searchRequest](../resources/searchrequest.md)集合|要发送到 JSON blob 中格式化的查询终结点的搜索请求。 它包含响应中的预期实体类型、基础源、分页参数、请求的字段和实际搜索查询。|

## <a name="response"></a>响应

如果成功，此方法在`HTTP 200 OK`响应正文中返回响应代码和[searchResponse](../resources/searchresponse.md)集合对象。

## <a name="common-use-cases"></a>常见用例

- 搜索[邮件消息](/graph/search-concept-messages)
- 搜索[日历事件](/graph/search-concept-events)
- 搜索[文件](/graph/search-concept-files)
- 搜索[自定义类型（连接器）](/graph/search-concept-custom-types)数据

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "search_query"
}-->

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "microsoft.graph.externalItem"
      ],
      "contentSources": [
        "/external/connections/connectionfriendlyname"
      ],
      "query": {
        "query_string": {
          "query": "contoso product"
        }
      },
      "from": 0,
      "size": 25,
      "stored_fields": [
        "title",
        "description"
      ]
    }
  ]
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-query-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-query-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-query-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.searchResponse",
  "isCollection": true
} -->

```HTTP
HTTP/1.1 200 OK
Content-type: application/json
```

```json
{
  "value": [
    {
      "searchTerms": [
        "searchTerms-value"
      ],
      "hitsContainers": [
        {
          "hits": [
            {
              "_id": "1",
              "_score": 1,
              "_sortField": "Relevance",
              "_summary": "_summary-value",
              "_source": "The source field will contain the underlying graph entity part of the response"
            }
          ],
          "total": 47,
          "moreResultsAvailable": true
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "search: query",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
