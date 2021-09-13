---
title: 使用 Microsoft Microsoft 搜索 中的 Graph API 搜索自定义类型
description: 可以使用 Microsoft 搜索 API 通过[externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)资源导入外部数据，并针对此外部内容运行搜索查询。
author: nmoreau
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: 53716d886f586207fce607234d3cae993fc38794
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127904"
---
# <a name="use-the-microsoft-search-api-to-search-custom-types-imported-using-microsoft-graph-connectors-preview"></a>使用 Microsoft 搜索 API 搜索使用 Microsoft Graph 连接器导入的自定义 (预览)  

使用 Microsoft 搜索 API 跨 Microsoft Graph 连接器进行检索[和索引的内容](/microsoftsearch/connectors-overview)。 内容通过 Microsoft 提供的内置[](/microsoftsearch/connectors-gallery)连接器或通过使用[Microsoft](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)Graph连接器 API 实现的自定义连接器导入。

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

导入内容并编制索引后，可以使用搜索 API 查询内容。

若要搜索自定义类型，在查询方法的请求正文中指定 [以下](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) 属性：

- 要包括在连接器设置过程中分配的连接 ID 的 **contentSources** 属性。 你可以传递多个连接 ID 以跨多个连接进行搜索。 结果在单个列表中返回，并跨多个连接进行排名。

<!--
TODOSEARCHAPI - Bug 1653398 
-->

- **entityTypes** 属性为 `externalItem` 。

- 要 **包含** 要检索的外部项中的字段的 fields 属性。 请注意，如果请求中不包含任何字段，响应将包含 **contentSources** 属性中为指定连接指定的数据架构中标记为可检索的所有字段。

此外，您可以基于 [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) 中的属性聚合搜索结果，这些属性是数值或字符串类型，且在架构中设置为可 [精简](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true)。 有关详细信息，请参阅使用聚合 [优化搜索结果](search-concept-aggregation.md)。

## <a name="example-1-retrieve-items-using-azure-sql-built-in-connector"></a>示例 1：使用 Azure SQL内置连接器检索项目

本示例中[，AdventureWorks](/sql/samples/adventureworks-install-configure)数据库的内容已使用 Azure SQL内置连接器进行采用。

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

## <a name="example-2-retrieve-items-using-semantic-labels"></a>示例 2：使用语义标签检索项目

### <a name="request"></a>请求

```HTTP
POST https://graph.microsoft.com/beta/search/query
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
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

有关详细信息，请参阅分配 [属性标签](/microsoftsearch/configure-connector#step-5-assign-property-labels)。

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
