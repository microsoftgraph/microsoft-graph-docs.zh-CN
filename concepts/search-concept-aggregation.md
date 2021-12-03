---
title: 使用 Microsoft Microsoft 搜索 API Graph聚合优化查询
description: 可以使用 Microsoft 搜索 API 检索 aggreations
author: nmoreau
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: 49e3739985f2a715449ff28c1183d0427543b2c5
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285082"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-refine-queries-with-aggregations"></a>使用 Microsoft Microsoft 搜索 API Graph聚合优化查询

可以使用 Microsoft Microsoft 搜索 API 来Graph搜索结果，在索引中显示搜索结果的分布。 

若要优化结果，在搜索请求 [中，](/graph/api/resources/searchRequest?view=graph-rest-beta&preserve-view=true)指定 [aggregationOption](/graph/api/resources/aggregationOption?view=graph-rest-beta&preserve-view=true)。 每个 **aggregationOption** 指定应计算聚合的属性，以及响应中返回的 [searchBucket](/graph/api/resources/searchBucket?view=graph-rest-beta&preserve-view=true) 项目数。

## <a name="example-1-request-aggregations-by-string-fields"></a>示例 1：按字符串字段请求聚合

以下示例搜索 **listItem** 资源，并按文件类型、内容类和上次修改时间聚合结果，所有这些都是字符串值。

该响应包含两个聚合的 [searchBucket](/graph/api/resources/searchbucket?view=graph-rest-beta&preserve-view=true) 对象：
- **key** 属性 实际值 (指定由、) 值聚合在同一存储桶中的 `fileType` `contentclass` `lastModifiedTime` **那些匹配的 listItem** 对象的) 、 或 值的值。
- **count** 属性指定聚合在同一存储桶中的此类对象的数量。 请注意，此数字是匹配数的近似值，不会提供匹配项的准确数量。
- 按文件类型聚合的结果存储桶按计数降序排序。 本示例中，有 3 个存储桶用于 3 种文件类型 `docx` ：、 `xlsx` 和 `pptx` 。
- 内容类聚合的结果存储桶按内容类的字符串值按降序排序。 本示例中，只有一个存储桶，所有匹配对象共享同一个内容类 `STS_ListItem_DocumentLibrary` 。
- lastModifiedTime 聚合的结果存储桶按 lastModifiedTime 的字符串值按降序排序。 此示例包括三个存储桶 `Before 2021-09-01T09:08:19.6224752Z` ：、 `From 2021-09-01T09:08:19.6224752Z up to 2021-11-09T09:08:19.6224752Z` 和 `2021-11-09T09:08:19.6224752Z or later` 。

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
              "field": "fileType",
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
          },
          {
              "field": "lastModifiedTime",
              "size": 2,
              "bucketDefinition": {
                  "sortBy": "KeyAsString",
                  "isDescending": "true",
                  "minimumCount": 0,
                  "ranges": [
                      {
                          "to": "2021-09-01T09:08:19.6224752Z"
                      },
                      {
                          "from": "2021-09-01T09:08:19.6224752Z",
                          "to": "2021-11-09T09:08:19.6224752Z"
                      },
                      {
                          "from": "2021-11-09T09:08:19.6224752Z"
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
                    "field": "fileType",
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
                },
                {
                    "@odata.type": "#microsoft.substrateSearch.searchAggregation",
                    "field": "lastModifiedTime",
                    "buckets": [
                        {
                            "key": "Before 2021-09-01T09:08:19.6224752Z",
                            "count": 5,
                            "aggregationFilterToken": "range(min, 2021-09-01T09:08:19.6224752Z)"
                        },
                        {
                            "key": "From 2021-09-01T09:08:19.6224752Z up to 2021-11-09T09:08:19.6224752Z",
                            "count": 3,
                            "aggregationFilterToken": "range(2021-09-01T09:08:19.6224752Z, 2021-11-09T09:08:19.6224752Z)"
                        },
                        {
                            "key": "2021-11-09T09:08:19.6224752Z or later",
                            "count": 1,
                            "aggregationFilterToken": "range(2021-11-09T09:08:19.6224752Z, max, to=\"le\")"
                        }
                    ]
                }
            ]
        }
    ]
}
```

## <a name="example-2-apply-an-aggregation-filter-based-on-a-previous-request"></a>示例 2：基于上一个请求应用聚合筛选器

此示例应用聚合筛选器，该筛选器基于作为字段和示例 1 中的字段返回的 **aggregationFilterToken。** `docx` `fileType` `From 2021-09-01T09:08:19.6224752Z up to 2021-11-09T09:08:19.6224752Z` `lastModifiedTime`

分配给 **aggregationFilters** 属性的字符串值采用格式 **"{field}：" \\ "{aggregationFilterToken} \\ ""**。 如果同一筛选器需要多个值，则分配给 **aggregationFilters** 属性的字符串值应遵循以下格式 **："{field}：或 (\\ "{aggregationFilterToken1} \\ "， \\ "{aggregationFilterToken2} \\ ") "。**

分配给 **aggregationFilters** 属性的日期时间格式字符串值遵循格式 **"{field}：{aggregationFilterToken}"。**


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
              "field": "fileType",
              "size": 10,
              "bucketDefinition": {
                  "sortBy": "count",
                  "isDescending": "true",
                  "minimumCount": 0
              }
          }
      ],
      "aggregationFilters": [
        "fileType:\"ǂǂ68746d6c\"",
        "lastModifiedTime:range(2021-09-01T09:08:19.6224752Z, 2021-11-09T09:08:19.6224752Z)"
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
                    "field": "fileType",
                    "buckets": [
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "html",
                            "count": 69960,
                            "aggregationFilterToken": "\"ǂǂ68746d6c\""
                        }
                    ]
                },
                {
                    "@odata.type": "#microsoft.substrateSearch.searchAggregation",
                    "field": "lastModifiedTime",
                    "buckets": [
                        {
                            "key": "Before 2021-09-01T09:08:19.6224752Z",
                            "count": 0,
                            "aggregationFilterToken": "range(min, 2021-09-01T09:08:19.6224752Z)"
                        },
                        {
                            "key": "From 2021-09-01T09:08:19.6224752Z up to 2021-11-09T09:08:19.6224752Z",
                            "count": 69960,
                            "aggregationFilterToken": "range(2021-09-01T09:08:19.6224752Z, 2021-11-09T09:08:19.6224752Z)"
                        },
                        {
                            "key": "2021-11-09T09:08:19.6224752Z or later",
                            "count": 0,
                            "aggregationFilterToken": "range(2021-11-09T09:08:19.6224752Z, max, to=\"le\")"
                        }
                    ]
                }
            ]
        }
    ]
}
```

## <a name="example-3-request-aggregation-by-a-numeric-field"></a>示例 3：按数值字段请求聚合

以下示例搜索 **driveItem** 资源，并按结果大小（数字值）聚合结果。 请求按 3 个大小范围指定聚合：
- 小于 100 的大小
- 大小介于 100 和 1000 之间
- 大小 1000 及更高版本

该响应包括 3 **个 searchBucket** 对象，每个大小范围聚合一个：
- 较低大小范围的 2 个存储桶不包含任何搜索匹配项。
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

聚合仅受项目SharePoint OneDrive支持。 邮件或事件 **不支持****它们**。

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
