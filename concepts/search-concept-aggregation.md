---
title: 在 Microsoft Graph 中使用 Microsoft 搜索 API 通过聚合优化查询
description: 可以使用 Microsoft 搜索 API 检索项目
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: fad049649172750cf2e362d2558cfc247467a6ed
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883191"
---
# <a name="refine-search-results-using-aggregations-preview"></a><span data-ttu-id="97268-103">使用聚合和预览 (优化) </span><span class="sxs-lookup"><span data-stu-id="97268-103">Refine search results using aggregations (preview)</span></span>

<span data-ttu-id="97268-104">优化搜索结果，在索引中显示其分布。</span><span class="sxs-lookup"><span data-stu-id="97268-104">Refine search results and show their distribution in the index.</span></span>

## <a name="example-1-request-aggregations-by-string-fields"></a><span data-ttu-id="97268-105">示例 1：按字符串字段请求聚合</span><span class="sxs-lookup"><span data-stu-id="97268-105">Example 1: Request aggregations by string fields</span></span>

<span data-ttu-id="97268-106">以下示例搜索 **listItem** 资源，并按其文件类型和内容类聚合结果，两者都是字符串值。</span><span class="sxs-lookup"><span data-stu-id="97268-106">The following example searches **listItem** resources and aggregates results by their file type and content class, both of which are string values.</span></span>

<span data-ttu-id="97268-107">该响应包括两个聚合的 [searchBucket](/graph/api/resources/searchbucket?view=graph-rest-beta&preserve-view=true) 对象：</span><span class="sxs-lookup"><span data-stu-id="97268-107">The response includes two [searchBucket](/graph/api/resources/searchbucket?view=graph-rest-beta&preserve-view=true) objects for the two aggregations:</span></span>
- <span data-ttu-id="97268-108">键 **属性** 指定实际值 (聚合) 同一存储桶中的 `FileType` `contentclass` **那些匹配的 listItem** 对象的值。</span><span class="sxs-lookup"><span data-stu-id="97268-108">The **key** property specifies the actual value (by `FileType` or `contentclass`) for those matching **listItem** objects that are aggregated in the same bucket by that value.</span></span>
- <span data-ttu-id="97268-109">count 属性指定聚合在同一存储桶中的此类对象的数量。</span><span class="sxs-lookup"><span data-stu-id="97268-109">The **count** property specifies the number of such objects aggregated in the same bucket.</span></span> <span data-ttu-id="97268-110">请注意，此数字是匹配数的近似值，不会提供确切的匹配数。</span><span class="sxs-lookup"><span data-stu-id="97268-110">Note that this number is an approximation of the number of matches and will not provide an exact number of matches.</span></span>
- <span data-ttu-id="97268-111">按文件类型聚合的结果存储桶按计数降序排序。</span><span class="sxs-lookup"><span data-stu-id="97268-111">Buckets of results aggregated by file type are sorted by count in descending order.</span></span> <span data-ttu-id="97268-112">本示例中，有 3 个存储桶用于 3 种文件类型：、 `docx` `xlsx` 和 `pptx` 。</span><span class="sxs-lookup"><span data-stu-id="97268-112">In this example, there are 3 buckets for 3 file types: `docx`, `xlsx`, and `pptx`.</span></span>
- <span data-ttu-id="97268-113">由内容类聚合的结果存储桶按内容类的字符串值按降序排序。</span><span class="sxs-lookup"><span data-stu-id="97268-113">Buckets of results aggregated by content class are sorted by the string value of the content class in descending order.</span></span> <span data-ttu-id="97268-114">本示例中，只有一个存储桶，其中所有匹配的对象共享同一个内容类 `STS_ListItem_DocumentLibrary` 。</span><span class="sxs-lookup"><span data-stu-id="97268-114">In this example, there is only one bucket with all the matching objects sharing the same content class, `STS_ListItem_DocumentLibrary`.</span></span>

### <a name="request"></a><span data-ttu-id="97268-115">请求</span><span class="sxs-lookup"><span data-stu-id="97268-115">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="97268-116">响应</span><span class="sxs-lookup"><span data-stu-id="97268-116">Response</span></span>

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

## <a name="example-2-apply-an-aggregation-filter-based-on-a-previous-request"></a><span data-ttu-id="97268-117">示例 2：基于上一个请求应用聚合筛选器</span><span class="sxs-lookup"><span data-stu-id="97268-117">Example 2: Apply an aggregation filter based on a previous request</span></span>

<span data-ttu-id="97268-118">本示例中，我们应用聚合筛选器，该筛选器基于作为示例 1 中的字段返回的 **aggregationFilterToken。** `docx` `FileType`</span><span class="sxs-lookup"><span data-stu-id="97268-118">In this example, we apply an aggregation filter that is based on the **aggregationFilterToken** returned for `docx` as the `FileType` field in example 1.</span></span>

<span data-ttu-id="97268-119">分配给 **aggregationFilters** 属性的字符串值采用格式 **"{field}：" \\ "{aggregationFilterToken} \\ ""**。</span><span class="sxs-lookup"><span data-stu-id="97268-119">The string value assigned to the **aggregationFilters** property follows the format **"{field}:\\"{aggregationFilterToken}\\""**.</span></span> <span data-ttu-id="97268-120">如果同一筛选器需要多个值，则分配给 **aggregationFilters** 属性的字符串值应遵循以下格式 **："{field}：或 (\\ "{aggregationFilterToken1} \\ "， \\ "{aggregationFilterToken2} \\ ") "。**</span><span class="sxs-lookup"><span data-stu-id="97268-120">If multiple values for the same filter are required, the string value assigned to the **aggregationFilters** property should follow this format : **"{field}:or(\\"{aggregationFilterToken1}\\",\\"{aggregationFilterToken2}\\")"**.</span></span>

### <a name="request"></a><span data-ttu-id="97268-121">请求</span><span class="sxs-lookup"><span data-stu-id="97268-121">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="97268-122">响应</span><span class="sxs-lookup"><span data-stu-id="97268-122">Response</span></span>

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

## <a name="example-3-request-aggregation-by-a-numeric-field"></a><span data-ttu-id="97268-123">示例 3：通过数值字段请求聚合</span><span class="sxs-lookup"><span data-stu-id="97268-123">Example 3: Request aggregation by a numeric field</span></span>

<span data-ttu-id="97268-124">以下示例搜索 **driveItem** 资源，并按其大小（即数值）聚合结果。</span><span class="sxs-lookup"><span data-stu-id="97268-124">The following example searches **driveItem** resources and aggregates results by their size which is a numeric value.</span></span> <span data-ttu-id="97268-125">该请求指定 3 个大小范围的聚合：</span><span class="sxs-lookup"><span data-stu-id="97268-125">The request specifies aggregation by 3 size ranges:</span></span>
- <span data-ttu-id="97268-126">小于 100 的大小</span><span class="sxs-lookup"><span data-stu-id="97268-126">Size less than 100</span></span>
- <span data-ttu-id="97268-127">大小介于 100 和 1000 之间</span><span class="sxs-lookup"><span data-stu-id="97268-127">Size between 100 and 1000</span></span>
- <span data-ttu-id="97268-128">大小 1000 及更高版本</span><span class="sxs-lookup"><span data-stu-id="97268-128">Size 1000 and higher</span></span>

<span data-ttu-id="97268-129">该响应包括 3 **个 searchBucket** 对象，每个大小范围聚合一个：</span><span class="sxs-lookup"><span data-stu-id="97268-129">The response includes 3 **searchBucket** objects, one for each size range aggregation:</span></span>
- <span data-ttu-id="97268-130">小尺寸范围的 2 个存储桶不包含任何搜索匹配项。</span><span class="sxs-lookup"><span data-stu-id="97268-130">The 2 buckets of the lower size ranges don't include any search matches.</span></span>
- <span data-ttu-id="97268-131">所有 9 个搜索匹配项的大小都为 1000 或更大。</span><span class="sxs-lookup"><span data-stu-id="97268-131">All 9 search matches have sizes 1000 or higher.</span></span>

### <a name="request"></a><span data-ttu-id="97268-132">请求</span><span class="sxs-lookup"><span data-stu-id="97268-132">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="97268-133">响应</span><span class="sxs-lookup"><span data-stu-id="97268-133">Response</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="97268-134">已知限制</span><span class="sxs-lookup"><span data-stu-id="97268-134">Known limitations</span></span>

<span data-ttu-id="97268-135">聚合仅受 SharePoint 或 OneDrive 项支持。</span><span class="sxs-lookup"><span data-stu-id="97268-135">Aggregations are supported only for SharePoint or OneDrive items.</span></span> <span data-ttu-id="97268-136">消息或事件 **不支持\*\*\*\*它们**。</span><span class="sxs-lookup"><span data-stu-id="97268-136">They are not supported for **message** or **event**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="97268-137">后续步骤</span><span class="sxs-lookup"><span data-stu-id="97268-137">Next steps</span></span>

- [<span data-ttu-id="97268-138">使用 Microsoft 搜索 API 查询数据</span><span class="sxs-lookup"><span data-stu-id="97268-138">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
