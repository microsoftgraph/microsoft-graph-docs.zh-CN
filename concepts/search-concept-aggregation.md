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
# <a name="refine-search-results-using-aggregations-preview"></a>使用聚合和预览 (优化) 

优化搜索结果，在索引中显示其分布。

## <a name="example-1-request-aggregations-by-string-fields"></a>示例 1：按字符串字段请求聚合

以下示例搜索 **listItem** 资源，并按其文件类型和内容类聚合结果，两者都是字符串值。

该响应包括两个聚合的 [searchBucket](/graph/api/resources/searchbucket?view=graph-rest-beta&preserve-view=true) 对象：
- 键 **属性** 指定实际值 (聚合) 同一存储桶中的 `FileType` `contentclass` **那些匹配的 listItem** 对象的值。
- count 属性指定聚合在同一存储桶中的此类对象的数量。 请注意，此数字是匹配数的近似值，不会提供确切的匹配数。
- 按文件类型聚合的结果存储桶按计数降序排序。 本示例中，有 3 个存储桶用于 3 种文件类型：、 `docx` `xlsx` 和 `pptx` 。
- 由内容类聚合的结果存储桶按内容类的字符串值按降序排序。 本示例中，只有一个存储桶，其中所有匹配的对象共享同一个内容类 `STS_ListItem_DocumentLibrary` 。

### <a name="request"></a>请求

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

### <a name="response"></a>响应

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

## <a name="example-2-apply-an-aggregation-filter-based-on-a-previous-request"></a>示例 2：基于上一个请求应用聚合筛选器

本示例中，我们应用聚合筛选器，该筛选器基于作为示例 1 中的字段返回的 **aggregationFilterToken。** `docx` `FileType`

分配给 **aggregationFilters** 属性的字符串值采用格式 **"{field}：" \\ "{aggregationFilterToken} \\ ""**。 如果同一筛选器需要多个值，则分配给 **aggregationFilters** 属性的字符串值应遵循以下格式 **："{field}：或 (\\ "{aggregationFilterToken1} \\ "， \\ "{aggregationFilterToken2} \\ ") "。**

### <a name="request"></a>请求

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

### <a name="response"></a>响应

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

## <a name="example-3-request-aggregation-by-a-numeric-field"></a>示例 3：通过数值字段请求聚合

以下示例搜索 **driveItem** 资源，并按其大小（即数值）聚合结果。 该请求指定 3 个大小范围的聚合：
- 小于 100 的大小
- 大小介于 100 和 1000 之间
- 大小 1000 及更高版本

该响应包括 3 **个 searchBucket** 对象，每个大小范围聚合一个：
- 小尺寸范围的 2 个存储桶不包含任何搜索匹配项。
- 所有 9 个搜索匹配项的大小都为 1000 或更大。

### <a name="request"></a>请求

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

### <a name="response"></a>响应

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

## <a name="known-limitations"></a>已知限制

聚合仅受 SharePoint 或 OneDrive 项支持。 消息或事件 **不支持****它们**。

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
