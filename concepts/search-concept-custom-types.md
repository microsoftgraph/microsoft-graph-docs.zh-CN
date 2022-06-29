---
title: 使用 Microsoft 搜索 API 搜索使用连接器导入的自定义类型
description: 使用 Microsoft Graph 中的 Microsoft 搜索 API 在 Microsoft Graph 连接器引入和索引的外部内容之间进行搜索。
author: nmoreau
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: 64a1733722afee9de1e5970389c275062b574e9d
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437630"
---
# <a name="use-the-microsoft-search-api-to-search-custom-types-imported-using-microsoft-graph-connectors"></a>使用 Microsoft 搜索 API 搜索使用 Microsoft Graph 连接器导入的自定义类型

使用 Microsoft Graph 中的 Microsoft 搜索 API 在 [Microsoft Graph 连接器](/microsoftsearch/connectors-overview)引入和索引的外部内容之间进行搜索。 内容通过 Microsoft 提供的 [内置连接器](https://www.microsoft.com/microsoft-search/connectors) 或通过使用 [Microsoft Graph 连接器引入 API 实现的自定义连接器导入](/graph/api/resources/indexing-api-overview)。

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

导入内容并编制索引后，可以使用搜索 API 查询内容。

若要搜索自定义类型，请在 [查询](/graph/api/search-query) 方法的请求正文中指定以下属性：

- 要包含在连接器设置期间分配的连接 ID 的 **contentSources** 属性。 可以传递多个连接 ID 以跨多个连接进行搜索。 结果在单个列表中返回，在多个连接之间进行排名。

<!--
TODOSEARCHAPI - Bug 1653398 
-->

- **entityTypes** 属性为 `externalItem`.

- 要在要检索的外部项中包含字段的 **fields** 属性。 请注意，如果请求中不包含任何 **字段**，响应将包含在为 **contentSources** 属性中的指定连接指定的数据架构中标记为 *可检索* 的所有字段。

此外，可以根据 [外部Item](/graph/api/resources/externalitem) 中的属性聚合搜索结果，这些属性是数值或字符串类型，并且在 [架构](/graph/api/resources/schema)中设置为可再定义的。 有关详细信息，请参阅 [使用聚合优化搜索结果](search-concept-aggregation.md)。

## <a name="example-1-retrieve-items-using-azure-sql-built-in-connector"></a>示例 1：使用Azure SQL内置连接器检索项

在此示例中，已使用Azure SQL内置连接器引入 [AdventureWorks](/sql/samples/adventureworks-install-configure) 数据库的内容。

### <a name="request"></a>请求

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.searchResponse)",
  "value": [
    {
      "searchTerms": ["yang"],
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
                  "shortDescription": "Contoso maintenance guidelines",
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

## <a name="example-2-retrieve-items-using-semantic-labels"></a>示例 2：使用语义标签检索项

### <a name="request"></a>请求

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
Content-Type: application/json

{
    "requests": [
      {
        "entityTypes": [
          "microsoft.graph.externalItem"
        ],
        "contentSources": [
          "/external/connections/FileAsUdt"
        ],
        "query": {
          "query_string": {
            "query": "test"
          }
        },
        "stored_fields": [
          "label_Title",
          "label_URL",
          "label_LastModifiedBy",
          "label_LastModifiedDateTime"
        ],
        "from": 0,
        "size": 25
      }
    ]
}
```

### <a name="response"></a>响应

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.searchResponse)",
"value": [
      {
        "searchTerms": [
          "test"
        ],
        "hitsContainers": [
          {
            "hits": [
              {
                "_id": "AQMkAGRjZWJjZTFkLTkzYWItNDhlOC1iODA2LTgwMTNjNjEzYzI2YwBGAAADOx0/YV2JckefuDmJtUO7mwcAHNjGq33S50uXSFeU/U9mogAAAgEWAAAAHNjGq33S50uXSFeU/U9mogAAAgleAAAA",
                "_contentSource": "FileAsUdt",
                "_score": 1,
                "_summary": "<c0>Test</c0> component to move data files and messages between the gateway and internal <ddd/>",
                "_source": {
                  "@odata.type": "#microsoft.graph.externalItem",
                  "properties": {
                    "label_Title": "SONIC Operations support and test Guide for the month of March",
                    "label_URL": "D:\\\\ConnectorsEcho\\\\New\\\\MSW06SecondSet\\\\teams\\\\Enterprise_Platforms\\\\CCO\\\\Projects\\\\BTSi Modernization\\\\SONIC Retirement\\\\SONIC_Operations_Support_Guide.docx",
                    "label_LastModifiedBy": [
                      "Bob",
                      "Scott"
                    ],
                    "label_LastModifiedDateTime": "2020-01-30T12:44:19Z"
                  }
                }
              },
              {
                "_id": "AQMkAGRjZWJjZTFkLTkzYWItNDhlOC1iODA2LTgwMTNjNjEzYzI2YwBGAAADOx0/YV2JckefuDmJtUO7mwcAHNjGq33S50uXSFeU/U9mogAAAgEWAAAAHNjGq33S50uXSFeU/U9mogAAAgldAAAA",
                "_contentSource": "FileAsUdt",
                "_score": 2,
                "_summary": "File Transfer Workbench A <c0>test</c0> File transfer Management Solution File Transfer the number <ddd/>",
                "_source": {
                  "@odata.type": "#microsoft.graph.externalItem",
                  "properties": {
                    "label_Title": "Test File Transfer Workbench for the month of January",
                    "label_URL": "D:\\\\ConnectorsEcho\\\\New\\\\MSW06SecondSet\\\\teams\\\\IssueLog\\\\FCAGA Organisation\\\\NSN CO CCA Infra YBCFTPAR entry\\\\File Transfer Workbench.ppt",
                    "label_LastModifiedBy": [
                      "Alice",
                      "Scott"
                    ],
                    "label_LastModifiedDateTime": "2020-01-31T11:44:19Z"
                  }
                }
              },
              {
                "_id": "AQMkAGRjZWJjZTFkLTkzYWItNDhlOC1iODA2LTgwMTNjNjEzYzI2YwBGAAADOx0/YV2JckefuDmJtUO7mwcAHNjGq33S50uXSFeU/U9mogAAAgEWAAAAHNjGq33S50uXSFeU/U9mogAAAglgAAAA",
                "_contentSource": "FileAsUdt",
                "_score": 3,
                "_summary": "document and the associated <c0>test</c0> software are the sole property of Express Logic.<ddd/>",
                "_source": {
                  "@odata.type": "#microsoft.graph.externalItem",
                  "properties": {
                    "label_Title": "System User Guide Express Logic 858.613.6640",
                    "label_URL": "D:\\\\ConnectorsEcho\\\\New\\\\MSW06FirstSet\\\\teams\\\\AzureIoTMarketing\\\\Shared Documents\\\\Whitepapers\\\\RTOS Whitepapers\\\\User Guides\\\\Azure_RTOS_FileX_User_Guide.pdf",
                    "label_LastModifiedBy": [
                      "Alice",
                      "Bob"
                    ],
                    "label_LastModifiedDateTime": "2020-05-25T10:20:19Z"
                  }
                }
              }
            ],
            "total": 3,
            "moreResultsAvailable": false
          }
        ]
      }
    ]
}
```

有关详细信息，请参阅 [分配属性标签](/microsoftsearch/configure-connector#step-6-assign-property-labels)。

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview)
