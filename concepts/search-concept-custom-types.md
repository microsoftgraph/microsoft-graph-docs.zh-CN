---
ms.author: yiwenwang
title: 使用 Microsoft Graph 中的 Microsoft 搜索 API 搜索自定义类型
description: 可以使用 Microsoft 搜索 API 通过 [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) 资源导入外部数据，并针对此外部内容运行搜索查询。
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: c4e0b158356d3f26d8a0f36a7d7e86faeba96649
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471836"
---
# <a name="use-the-microsoft-search-api-to-search-custom-types-imported-using-microsoft-graph-connectors-preview"></a><span data-ttu-id="8e1bb-103">使用 Microsoft 搜索 API 搜索使用 Microsoft Graph 连接器导入的自定义类型 (预览) </span><span class="sxs-lookup"><span data-stu-id="8e1bb-103">Use the Microsoft Search API to search custom types imported using Microsoft Graph connectors (preview)</span></span> 

<span data-ttu-id="8e1bb-104">使用 Microsoft 搜索 API 跨 Microsoft Graph 连接器所输入和编制索引 [的内容进行搜索](/microsoftsearch/connectors-overview)。</span><span class="sxs-lookup"><span data-stu-id="8e1bb-104">Use the Microsoft Search API to search accross content ingested and indexed by [Microsoft Graph connectors](/microsoftsearch/connectors-overview).</span></span> <span data-ttu-id="8e1bb-105">内容通过 Microsoft 提供的内置[](/microsoftsearch/connectors-gallery)连接器或通过使用 Microsoft Graph 连接器[导入 API 实现的](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)自定义连接器导入。</span><span class="sxs-lookup"><span data-stu-id="8e1bb-105">The content is imported either via [built-in connectors](/microsoftsearch/connectors-gallery) provided by Microsoft, or via custom connectors implemented using the [Microsoft Graph connectors ingestion API](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true).</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

<span data-ttu-id="8e1bb-106">导入内容并编制索引后，可以使用搜索 API 查询内容。</span><span class="sxs-lookup"><span data-stu-id="8e1bb-106">Once the content has been imported and indexed, you can use the search API to query the content.</span></span>

<span data-ttu-id="8e1bb-107">若要搜索自定义类型，请指定查询方法 [的请求正文中的](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) 以下属性：</span><span class="sxs-lookup"><span data-stu-id="8e1bb-107">To search for custom types, specify the following properties in the request body of the [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) method:</span></span>

- <span data-ttu-id="8e1bb-108">要包括在连接器设置期间分配的连接 ID 的 **contentSources** 属性。</span><span class="sxs-lookup"><span data-stu-id="8e1bb-108">The **contentSources** property to include the connection ID that is assigned during the connector setup.</span></span> <span data-ttu-id="8e1bb-109">可以传递多个连接 ID 以跨多个连接进行搜索。</span><span class="sxs-lookup"><span data-stu-id="8e1bb-109">You can pass multiple connection IDs to search across multiple connections.</span></span> <span data-ttu-id="8e1bb-110">结果在单个列表中返回，跨多个连接进行排名。</span><span class="sxs-lookup"><span data-stu-id="8e1bb-110">Results are returned in a single list, ranked accross the multiple connections.</span></span>

<!--
TODOSEARCHAPI - Bug 1653398 
-->

- <span data-ttu-id="8e1bb-111">**entityTypes** 属性为 `externalItem` 。</span><span class="sxs-lookup"><span data-stu-id="8e1bb-111">The **entityTypes** property as `externalItem`.</span></span>

- <span data-ttu-id="8e1bb-112">要 **包含** 要检索的外部项中的字段的 fields 属性。</span><span class="sxs-lookup"><span data-stu-id="8e1bb-112">The **fields** property to include the fields in the external item to retrieve.</span></span> <span data-ttu-id="8e1bb-113">请注意，如果请求中不包含任何字段，响应将包含为 **contentSources** 属性中指定的连接指定的数据架构中标记为可检索的所有字段。</span><span class="sxs-lookup"><span data-stu-id="8e1bb-113">Note that if you do not include any **fields** in the request, the response will contain all the fields marked as *retrievable* in the data schema specified for the specified connections in the **contentSources** property.</span></span>

<span data-ttu-id="8e1bb-114">此外，您可以基于 [外部](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) 项中的属性聚合搜索结果，这些属性是数字或字符串类型，并且设置为在架构中可 [精简](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="8e1bb-114">In addition, you can aggregate search results based on properties in an [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) that are numeric or string type, and that are set to be refinable in the [schema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="8e1bb-115">有关详细信息，请参阅使用 [聚合优化搜索结果](search-concept-aggregation.md)。</span><span class="sxs-lookup"><span data-stu-id="8e1bb-115">For more information, see [Refine search results using aggregations](search-concept-aggregation.md).</span></span>

## <a name="example-1-retrieve-items-using-azure-sql-built-in-connector"></a><span data-ttu-id="8e1bb-116">示例 1：使用 Azure SQL内置连接器检索项目</span><span class="sxs-lookup"><span data-stu-id="8e1bb-116">Example 1: Retrieve items using Azure SQL built-in connector</span></span>

<span data-ttu-id="8e1bb-117">此示例中 [，AdventureWorks](/sql/samples/adventureworks-install-configure) 数据库的内容已使用 Azure SQL内置连接器进行获取。</span><span class="sxs-lookup"><span data-stu-id="8e1bb-117">In this example, the content of the [AdventureWorks](/sql/samples/adventureworks-install-configure) database has been ingested using the Azure SQL built-in connector.</span></span>

### <a name="request"></a><span data-ttu-id="8e1bb-118">请求</span><span class="sxs-lookup"><span data-stu-id="8e1bb-118">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="8e1bb-119">响应</span><span class="sxs-lookup"><span data-stu-id="8e1bb-119">Response</span></span>

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

## <a name="example-2-retrieve-items-using-semantic-labels"></a><span data-ttu-id="8e1bb-120">示例 2：使用语义标签检索项目</span><span class="sxs-lookup"><span data-stu-id="8e1bb-120">Example 2: Retrieve items using semantic labels</span></span>

### <a name="request"></a><span data-ttu-id="8e1bb-121">请求</span><span class="sxs-lookup"><span data-stu-id="8e1bb-121">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="8e1bb-122">响应</span><span class="sxs-lookup"><span data-stu-id="8e1bb-122">Response</span></span>

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

<span data-ttu-id="8e1bb-123">有关详细信息，请参阅"[分配属性标签"。](/microsoftsearch/configure-connector#step-5-assign-property-labels)</span><span class="sxs-lookup"><span data-stu-id="8e1bb-123">For more details, see [Assign property labels](/microsoftsearch/configure-connector#step-5-assign-property-labels).</span></span>

## <a name="next-steps"></a><span data-ttu-id="8e1bb-124">后续步骤</span><span class="sxs-lookup"><span data-stu-id="8e1bb-124">Next steps</span></span>

- [<span data-ttu-id="8e1bb-125">使用 Microsoft 搜索 API 查询数据</span><span class="sxs-lookup"><span data-stu-id="8e1bb-125">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
