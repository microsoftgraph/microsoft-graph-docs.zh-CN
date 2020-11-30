---
title: 在 Microsoft Graph 中使用 Microsoft Search API 优化包含聚合的查询
description: 您可以使用 Microsoft 搜索 API 检索 aggreations
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 1a8e8cf17995adceadb9f426d1824d85505e806e
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377941"
---
# <a name="refine-search-results-using-aggregations-preview"></a><span data-ttu-id="1615d-103">使用聚合 (预览优化搜索结果) </span><span class="sxs-lookup"><span data-stu-id="1615d-103">Refine search results using aggregations (preview)</span></span>

<span data-ttu-id="1615d-104">优化搜索结果并在索引中显示其分布。</span><span class="sxs-lookup"><span data-stu-id="1615d-104">Refine search results and show their distribution in the index.</span></span>

## <a name="example-1-request-aggregations-by-string-fields"></a><span data-ttu-id="1615d-105">示例1：请求聚合（按字符串字段）</span><span class="sxs-lookup"><span data-stu-id="1615d-105">Example 1: Request aggregations by string fields</span></span>

<span data-ttu-id="1615d-106">下面的 **示例搜索 "** 列表中的资源"，并按其文件类型和内容类聚合结果，这两者都是字符串值。</span><span class="sxs-lookup"><span data-stu-id="1615d-106">The following example searches **listItem** resources and aggregates results by their file type and content class, both of which are string values.</span></span>

<span data-ttu-id="1615d-107">响应包含两个 [searchBucket](/graph/api/resources/searchbucket?view=graph-rest-beta&preserve-view=true) 对象的两个聚合：</span><span class="sxs-lookup"><span data-stu-id="1615d-107">The response includes two [searchBucket](/graph/api/resources/searchbucket?view=graph-rest-beta&preserve-view=true) objects for the two aggregations:</span></span>
- <span data-ttu-id="1615d-108">**Key** 属性指定由 `FileType` `contentclass` 值在同一存储桶中聚合的匹配的 **listItem** 匹配项对象的实际值 (或) 。</span><span class="sxs-lookup"><span data-stu-id="1615d-108">The **key** property specifies the actual value (by `FileType` or `contentclass`) for those matching **listItem** objects that are aggregated in the same bucket by that value.</span></span>
- <span data-ttu-id="1615d-109">**Count** 属性指定在同一存储桶中聚合的此类对象的数目。</span><span class="sxs-lookup"><span data-stu-id="1615d-109">The **count** property specifies the number of such objects aggregated in the same bucket.</span></span> <span data-ttu-id="1615d-110">请注意，此数字是匹配项数的近似值，不会提供精确的匹配数。</span><span class="sxs-lookup"><span data-stu-id="1615d-110">Note that this number is an approximation of the number of matches and will not provide an exact number of matches.</span></span>
- <span data-ttu-id="1615d-111">按文件类型汇总的结果的存储桶按计数以降序排列。</span><span class="sxs-lookup"><span data-stu-id="1615d-111">Buckets of results aggregated by file type are sorted by count in descending order.</span></span> <span data-ttu-id="1615d-112">在此示例中，有3个存储桶，共3个文件类型： `docx` 、 `xlsx` 和 `pptx` 。</span><span class="sxs-lookup"><span data-stu-id="1615d-112">In this example, there are 3 buckets for 3 file types: `docx`, `xlsx`, and `pptx`.</span></span>
- <span data-ttu-id="1615d-113">按内容类汇总的结果桶按内容类的字符串值以降序排序。</span><span class="sxs-lookup"><span data-stu-id="1615d-113">Buckets of results aggregated by content class are sorted by the string value of the content class in descending order.</span></span> <span data-ttu-id="1615d-114">在此示例中，只有一个存储桶和所有匹配的对象共享同一个内容类 `STS_ListItem_DocumentLibrary` 。</span><span class="sxs-lookup"><span data-stu-id="1615d-114">In this example, there is only one bucket with all the matching objects sharing the same content class, `STS_ListItem_DocumentLibrary`.</span></span>

### <a name="request"></a><span data-ttu-id="1615d-115">请求</span><span class="sxs-lookup"><span data-stu-id="1615d-115">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
          "listItem"
      ],
      "query": {
          "queryString": "test"
      },
      "from": 0,
      "size": 25,
      "aggregations": [
          {
              "field": "FileType",
              "size": 20,
              "bucketDefinition": {
                  "sortBy": "count",
                  "isDescending": "true",
                  "minimumCount": 0
              }
          },
          {
              "field": "contentclass",
              "size": 15,
              "bucketDefinition": {
                  "sortBy": "keyAsString",
                  "isDescending": "true",
                  "minimumCount": 0
              }
          }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1615d-116">响应</span><span class="sxs-lookup"><span data-stu-id="1615d-116">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.searchResponse",
    "hitsContainers": [
        {
            "@odata.type": "#microsoft.graph.searchHitsContainer",
            "hits": [
                "..."
            ],
            "total": 9,
            "moreResultsAvailable": false,
            "aggregations": [
                {
                    "@odata.type": "#microsoft.substrateSearch.searchAggregation",
                    "field": "FileType",
                    "buckets": [
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "docx",
                            "count": 5,
                            "aggregationFilterToken": "\"ǂǂ646f6378\""
                        },
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "xlsx",
                            "count": 3,
                            "aggregationFilterToken": "\"ǂǂ786c7378\""
                        },
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "pptx",
                            "count": 1,
                            "aggregationFilterToken": "\"ǂǂ70707478\""
                        }
                    ]
                },
                {
                    "@odata.type": "#microsoft.substrateSearch.searchAggregation",
                    "field": "contentclass",
                    "buckets": [
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "STS_ListItem_DocumentLibrary",
                            "count": 9,
                            "aggregationFilterToken": "\"ǂǂ5354535f4c6973744974656d5f446f63756d656e744c696272617279\""
                        }
                    ]
                }
            ]
        }
    ]
}
```

## <a name="example-2-apply-an-aggregation-filter-based-on-a-previous-request"></a><span data-ttu-id="1615d-117">示例2：根据之前的请求应用聚合筛选器</span><span class="sxs-lookup"><span data-stu-id="1615d-117">Example 2: Apply an aggregation filter based on a previous request</span></span>

<span data-ttu-id="1615d-118">在此示例中，我们应用基于 **aggregationFilterToken** `docx` 作为 `FileType` 示例1中的字段返回的 aggregationFilterToken 的聚合筛选器。</span><span class="sxs-lookup"><span data-stu-id="1615d-118">In this example, we apply an aggregation filter that is based on the **aggregationFilterToken** returned for `docx` as the `FileType` field in example 1.</span></span>

<span data-ttu-id="1615d-119">分配给 **aggregationFilters** 属性的字符串值采用格式 **"{field}： \\ {aggregationFilterToken} \\ " "**。</span><span class="sxs-lookup"><span data-stu-id="1615d-119">The string value assigned to the **aggregationFilters** property follows the format **"{field}:\\"{aggregationFilterToken}\\""**.</span></span>

### <a name="request"></a><span data-ttu-id="1615d-120">请求</span><span class="sxs-lookup"><span data-stu-id="1615d-120">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
          "driveItem"
      ],
      "query": {
          "queryString": "test"
      },
      "from": 0,
      "size": 20,
      "aggregations": [
          {
              "field": "FileType",
              "size": 10,
              "bucketDefinition": {
                  "sortBy": "count",
                  "isDescending": "true",
                  "minimumCount": 0
              }
          }
      ],
      "aggregationFilters": [
        "FileType:\"ǂǂ68746d6c\""
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1615d-121">响应</span><span class="sxs-lookup"><span data-stu-id="1615d-121">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.searchResponse",
    "hitsContainers": [
        {
            "@odata.type": "#microsoft.graph.searchHitsContainer",
            "hits": [
                "..."
            ],
            "total": 69960,
            "moreResultsAvailable": true,
            "aggregations": [
            {
                "@odata.type": "#microsoft.substrateSearch.searchAggregation",
                "field": "FileType",
                "buckets": [
                    {
                        "@odata.type": "#microsoft.substrateSearch.searchBucket",
                        "key": "html",
                        "count": 69960,
                        "aggregationFilterToken": "\"ǂǂ68746d6c\""
                    }
                ]
            }
        ]
        }
    ]
}
```

## <a name="example-3-request-aggregation-by-a-numeric-field"></a><span data-ttu-id="1615d-122">示例3：请求聚合（按数字字段）</span><span class="sxs-lookup"><span data-stu-id="1615d-122">Example 3: Request aggregation by a numeric field</span></span>

<span data-ttu-id="1615d-123">下面的示例搜索 **driveItem** 资源，并按其大小为数值来聚合结果。</span><span class="sxs-lookup"><span data-stu-id="1615d-123">The following example searches **driveItem** resources and aggregates results by their size which is a numeric value.</span></span> <span data-ttu-id="1615d-124">请求将聚合按3个大小的范围指定：</span><span class="sxs-lookup"><span data-stu-id="1615d-124">The request specifies aggregation by 3 size ranges:</span></span>
- <span data-ttu-id="1615d-125">小于100的大小</span><span class="sxs-lookup"><span data-stu-id="1615d-125">Size less than 100</span></span>
- <span data-ttu-id="1615d-126">100和1000之间的大小</span><span class="sxs-lookup"><span data-stu-id="1615d-126">Size between 100 and 1000</span></span>
- <span data-ttu-id="1615d-127">调整1000和更高</span><span class="sxs-lookup"><span data-stu-id="1615d-127">Size 1000 and higher</span></span>

<span data-ttu-id="1615d-128">响应包括3个 **searchBucket** 对象，每个对象对应一个大小范围聚合：</span><span class="sxs-lookup"><span data-stu-id="1615d-128">The response includes 3 **searchBucket** objects, one for each size range aggregation:</span></span>
- <span data-ttu-id="1615d-129">较低大小区域中的2个存储桶不包含任何搜索匹配项。</span><span class="sxs-lookup"><span data-stu-id="1615d-129">The 2 buckets of the lower size ranges don't include any search matches.</span></span>
- <span data-ttu-id="1615d-130">所有9个搜索匹配的大小为1000或更高。</span><span class="sxs-lookup"><span data-stu-id="1615d-130">All 9 search matches have sizes 1000 or higher.</span></span>

### <a name="request"></a><span data-ttu-id="1615d-131">请求</span><span class="sxs-lookup"><span data-stu-id="1615d-131">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
    "requests": [
        {
            "entityTypes": [
                "driveItem"
            ],
            "query": {
                "queryString": "test"
            },
            "from": 0,
            "size": 10,
            "aggregations": [
                {
                    "field": "Size",
                    "size": 5,
                    "bucketDefinition": {
                        "sortBy": "keyAsNumber",
                        "isDescending": "true",
                        "minimumCount": 0,
                        "ranges": [
                            {
                                "to": "100"
                            },
                            {
                                "from": "100",
                                "to": "1000"
                            },
                            {
                                "from": "1000"
                            }
                        ]
                    }
                }
            ]
        }
    ]
}
```

### <a name="response"></a><span data-ttu-id="1615d-132">响应</span><span class="sxs-lookup"><span data-stu-id="1615d-132">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.searchResponse",
    "hitsContainers": [
        {
            "@odata.type": "#microsoft.graph.searchHitsContainer",
            "hits": [
                "..."
                    ],
            "total": 9,
            "moreResultsAvailable": false,
            "aggregations": [
                {
                    "@odata.type": "#microsoft.substrateSearch.searchAggregation",
                    "field": "Size",
                    "buckets": [
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "Less than 100",
                            "count": 0,
                            "aggregationFilterToken": "range(min, 100)"
                        },
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "100 up to 1000",
                            "count": 0,
                            "aggregationFilterToken": "range(100, 1000)"
                        },
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "1000 and up",
                            "count": 9,
                            "aggregationFilterToken": "range(1000, max, to=\"le\")"
                        }
                    ]
                }
            ]
        }
    ]
}
```

## <a name="known-limitations"></a><span data-ttu-id="1615d-133">已知限制</span><span class="sxs-lookup"><span data-stu-id="1615d-133">Known limitations</span></span>

<span data-ttu-id="1615d-134">仅 SharePoint 或 OneDrive 项目支持聚合。</span><span class="sxs-lookup"><span data-stu-id="1615d-134">Aggregations are supported only for SharePoint or OneDrive items.</span></span> <span data-ttu-id="1615d-135">**消息**、**事件** 和 **externalItem** 不支持它们。</span><span class="sxs-lookup"><span data-stu-id="1615d-135">They are not supported for **message**, **event**, and **externalItem**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1615d-136">后续步骤</span><span class="sxs-lookup"><span data-stu-id="1615d-136">Next steps</span></span>

- [<span data-ttu-id="1615d-137">使用 Microsoft 搜索 API 查询数据</span><span class="sxs-lookup"><span data-stu-id="1615d-137">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
