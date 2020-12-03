---
title: 在 Microsoft Graph 中使用 Microsoft Search API 搜索自定义类型
description: 您可以使用 Microsoft 搜索 API 通过 [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) 资源导入外部数据，并对此外部内容运行搜索查询。
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: ba08eeb2aeaf4aa13e6b5bc686143e9b4293c0d8
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49523761"
---
# <a name="use-the-microsoft-search-api-to-search-custom-types-imported-using-microsoft-graph-connectors-preview"></a>使用 Microsoft 搜索 API 搜索使用 Microsoft Graph 连接器导入的自定义类型 (预览)  

使用 Microsoft 搜索 API 跨内容引入进行搜索，并按 [Microsoft Graph 连接器](/microsoftsearch/connectors-overview)编制索引。 内容可以通过 Microsoft 提供的 [内置连接器](/microsoftsearch/connectors-gallery) 或通过使用 [microsoft GRAPH 连接器摄取 API](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)实现的自定义连接器导入。

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

导入并编制内容索引后，您可以使用搜索 API 来查询内容。

若要搜索自定义类型，请在 [查询](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) 方法的请求正文中指定以下属性：

- **ContentSources** 属性，以包含在连接器安装过程中分配的连接 ID。 可以在多个连接之间传递多个连接 Id 以进行搜索。 结果在单个列表中返回，并在多个连接中排名。

<!--
TODOSEARCHAPI - Bug 1653398 
-->

- **EntityTypes** 属性为 `externalItem` 。

- **Fields** 属性，用于包含要检索的外部项中的字段。 请注意，如果未在请求中包含任何 **字段**，则响应将包含在为 **contentSources** 属性中的指定连接指定的数据架构中标记为可 *检索* 的所有字段。

此外，您还可以根据 [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) 中的属性聚合搜索结果，这些属性是数字或字符串类型，并且在 [架构](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true)中设置为可精简。 有关详细信息，请参阅 [使用聚合优化搜索结果](search-concept-aggregation.md)。

## <a name="example"></a>示例

在此示例中，使用 Azure SQL 内置连接器引入了 [AdventureWorks](/sql/samples/adventureworks-install-configure) 数据库的内容。

### <a name="request"></a>请求

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "externalItem"
      ],
      "contentSources": [
          "/external/connections/azuresqlconnector",
          "/external/connections/azuresqlconnector2"
      ],
      "query": {
        "queryString": "yang"
      },
      "from": 0,
      "size": 25,
      "fields": [
        "BusinessEntityID",
        "firstName",
        "lastName"
      ]
    }
  ]
}
```

### <a name="response"></a>响应

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
  "value": [
    {
      "searchTerms": ["ya"],
      "hitsContainers": [
        {
          "total": 2,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "AAMkADc0NDNlNTE0",
              "rank": 1,
              "summary": "<ddd/>",
              "contentSource": "/external/connections/azuresqlconnector",
              "resource": {
                "@odata.type": "#microsoft.graph.externalItem",
                "properties": {
                  "businessEntityID": 20704,
                  "firstName": "Amy",
                  "lastName": "Yang"
                }
              }
            },
           {
              "hitId": "AQMkADg3M2I3YWMyLTEwZ",
              "rank": 2,
              "summary": "<ddd/>",
              "contentSource": "/external/connections/azuresqlconnector2",
              "resource": {
                "@odata.type": "#microsoft.graph.externalItem",
                "properties": {
                  "businessEntityID": 20704,
                  "shortdescription": "Contoso maintenance guidelines",
                  "firstName": "Amy",
                  "lastName": "Yang"
                }
              }
            },
          ]
        }
      ]
    }
  ]
}
```

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)