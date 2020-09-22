---
title: 在 Microsoft Graph 中使用 Microsoft Search API 搜索自定义类型
description: 您可以使用 Microsoft 搜索 API 通过 [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) 资源导入外部数据，并对此外部内容运行搜索查询。
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: b125b8f923e941ad73d5c578e99a67fdd9ea9eea
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192600"
---
# <a name="use-the-microsoft-search-api-to-search-custom-types-imported-using-microsoft-graph-connectors"></a><span data-ttu-id="308c8-103">使用 Microsoft 搜索 API 搜索使用 Microsoft Graph 连接器导入的自定义类型</span><span class="sxs-lookup"><span data-stu-id="308c8-103">Use the Microsoft Search API to search custom types imported using Microsoft Graph connectors</span></span>

<span data-ttu-id="308c8-104">使用 Microsoft 搜索 API 跨内容引入进行搜索，并按 [Microsoft Graph 连接器](https://docs.microsoft.com/microsoftsearch/connectors-overview)编制索引。</span><span class="sxs-lookup"><span data-stu-id="308c8-104">Use the Microsoft Search API to search accross content ingested and indexed by [Microsoft Graph connectors](https://docs.microsoft.com/microsoftsearch/connectors-overview).</span></span> <span data-ttu-id="308c8-105">内容可以通过 Microsoft 提供的 [内置连接器](https://docs.microsoft.com/microsoftsearch/connectors-gallery) 或通过使用 [microsoft GRAPH 连接器摄取 API](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)实现的自定义连接器导入。</span><span class="sxs-lookup"><span data-stu-id="308c8-105">The content is imported either via [built-in connectors](https://docs.microsoft.com/microsoftsearch/connectors-gallery) provided by Microsoft, or via custom connectors implemented using the [Microsoft Graph connectors ingestion API](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true).</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

<span data-ttu-id="308c8-106">导入并编制内容索引后，您可以使用搜索 API 来查询内容。</span><span class="sxs-lookup"><span data-stu-id="308c8-106">Once the content has been imported and indexed, you can use the search API to query the content.</span></span>

<span data-ttu-id="308c8-107">若要搜索自定义类型，请在 [查询](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) 方法的请求正文中指定以下属性：</span><span class="sxs-lookup"><span data-stu-id="308c8-107">To search for custom types, specify the following properties in the request body of the [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) method:</span></span>

- <span data-ttu-id="308c8-108">**ContentSources**属性，以包含在连接器安装过程中分配的连接 ID。</span><span class="sxs-lookup"><span data-stu-id="308c8-108">The **contentSources** property to include the connection ID that is assigned during the connector setup.</span></span> <span data-ttu-id="308c8-109">可以在多个连接之间传递多个连接 Id 以进行搜索。</span><span class="sxs-lookup"><span data-stu-id="308c8-109">You can pass multiple connection IDs to search across multiple connections.</span></span> <span data-ttu-id="308c8-110">结果在单个列表中返回，并在多个连接中排名。</span><span class="sxs-lookup"><span data-stu-id="308c8-110">Results are returned in a single list, ranked accross the multiple connections.</span></span>

<!--
TODOSEARCHAPI - Bug 1653398 
-->

- <span data-ttu-id="308c8-111">**EntityTypes**属性为 `externalItem` 。</span><span class="sxs-lookup"><span data-stu-id="308c8-111">The **entityTypes** property as `externalItem`.</span></span>

- <span data-ttu-id="308c8-112">**Fields**属性，用于包含要检索的外部项中的字段。</span><span class="sxs-lookup"><span data-stu-id="308c8-112">The **fields** property to include the fields in the external item to retrieve.</span></span>

## <a name="example"></a><span data-ttu-id="308c8-113">示例</span><span class="sxs-lookup"><span data-stu-id="308c8-113">Example</span></span>

<span data-ttu-id="308c8-114">在此示例中，使用 Azure SQL 内置连接器引入了 [AdventureWorks](https://docs.microsoft.com/sql/samples/adventureworks-install-configure) 数据库的内容。</span><span class="sxs-lookup"><span data-stu-id="308c8-114">In this example, the content of the [AdventureWorks](https://docs.microsoft.com/sql/samples/adventureworks-install-configure) database has been ingested using the Azure SQL built-in connector.</span></span>

### <a name="request"></a><span data-ttu-id="308c8-115">请求</span><span class="sxs-lookup"><span data-stu-id="308c8-115">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="308c8-116">响应</span><span class="sxs-lookup"><span data-stu-id="308c8-116">Response</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="308c8-117">已知限制</span><span class="sxs-lookup"><span data-stu-id="308c8-117">Known limitations</span></span>

- <span data-ttu-id="308c8-118">您必须指定 **fields** 属性，才能在搜索架构中获取可检索的字段。</span><span class="sxs-lookup"><span data-stu-id="308c8-118">You must specify the **fields** property to get retrievable fields in the search schema.</span></span>

## <a name="next-steps"></a><span data-ttu-id="308c8-119">后续步骤</span><span class="sxs-lookup"><span data-stu-id="308c8-119">Next steps</span></span>

- [<span data-ttu-id="308c8-120">使用 Microsoft 搜索 API 查询数据</span><span class="sxs-lookup"><span data-stu-id="308c8-120">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
