---
title: 使用 Microsoft 搜索 API 剪裁重复的搜索结果
description: 可以使用 Microsoft Graph 中的 Microsoft 搜索 API trimDuplicates 属性来剪裁重复的搜索结果。 仅在 SharePoint 文件上受支持。
author: yiwenwang
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: 8101b6c2a74ec7c30d8b9ca6478bbb13e59d7293
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438253"
---
# <a name="use-the-microsoft-search-api-to-trim-duplicate-search-results"></a>使用 Microsoft 搜索 API 剪裁重复的搜索结果

可以使用 Microsoft Graph 中的 Microsoft 搜索 API 来剪裁重复的搜索结果。 指定 [searchRequest](/graph/api/resources/searchrequest) 对象中的 **trimDuplicates** 属性以剪裁重复的搜索结果。 **trimDuplicates** 属性仅在 SharePoint 中托管的文件上受支持。 默认值为 `false`。

## <a name="example"></a>示例
以下示例演示一个请求，该请求搜索 SharePoint 中托管的文件，并使用 **trimDuplicates** 属性来剪裁重复的搜索结果。

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
        "queryString": "Adatum Corporation"
      },
      "trimDuplicates": true
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
    "searchTerms": [
        "Adatum",
        "Corporation"
    ],
    "hitsContainers": [
        {
            "total": 2,
            "moreResultsAvailable": false,
            "@odata.type": "#microsoft.graph.searchHitsContainer",
            "hits": [
                {
                    "@odata.type": "#microsoft.graph.searchHit",
                    "hitId": "01VRZMWHPGDM5KTXS53RF3SSGHW7SGGPKL",
                    "rank": 1,
                    "summary": "Unique Item 1 which created by Adatum Corporation ",
                    "resource": {
                        "@odata.type": "#microsoft.graph.driveItem",
                        "size": 971838,
                        "fileSystemInfo": {
                            "createdDateTime": "2020-07-22T21:14:59Z",
                            "lastModifiedDateTime": "2018-09-12T16:20:16Z"
                        },
                        "id": "01VRZMWHPGDM5KTXS53RF3SSGHW7SGGPKL",
                        "createdBy": {
                            "user": {
                                "displayName": "Adatum Corporation"
                            }
                        },
                        "createdDateTime": "2020-07-22T21:14:59+00:00",
                        "lastModifiedBy": {
                            "user": {
                                "displayName": "Adatum Corporation"
                            }
                        },
                        "lastModifiedDateTime": "2018-09-12T16:20:16+00:00",
                        "name": "Adatum Corporation Name",
                        "parentReference": {
                            "siteId": "Contoso066a,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0",
                            "driveId": "b!NAe_rKr80k-n7e5zlCVIqSnIwTNsGBVBlusjEvRHgjMmmcA3Ubc7R4Kyao9hbgL4",
                            "sharepointIds": {
                                "listId": "c61d1892-ca82-4f53-b16f-6bb8a379e2b2",
                                "listItemId": "1027",
                                "listItemUniqueId": "E320AFEB-AD73-46A2-83D7-985FAA4B206D"
                            }
                        },
                        "webUrl": "http://www.adatum.com/"
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.searchHit",
                    "hitId": "01BTQFB3LHZTAYBV2VXVEK22ETF5WOQGT2",
                    "rank": 2,
                    "summary": "Unique item 2 which modified by Adatum Corporation",
                    "resource": {
                        "@odata.type": "#microsoft.graph.driveItem",
                        "size": 34428,
                        "fileSystemInfo": {
                            "createdDateTime": "2020-07-22T21:23:50Z",
                            "lastModifiedDateTime": "2012-10-29T17:52:10Z"
                        },
                        "id": "01BTQFB3LHZTAYBV2VXVEK22ETF5WOQGT2",
                        "createdBy": {
                            "user": {
                                "displayName": "Adventure Works Cycles"
                            }
                        },
                        "createdDateTime": "2020-07-22T21:23:50+00:00",
                        "lastModifiedBy": {
                            "user": {
                                "displayName": "Adatum Corporation"
                            }
                        },
                        "lastModifiedDateTime": "2012-10-29T17:52:10+00:00",
                        "name": "Adventure Works Cycles Name",
                        "parentReference": {
                            "siteId": "Contoso066a,893378cb-d2cd-4076-a2c9-e50587a26832,04120cf2-7863-4701-8541-eb26266a25e6",
                            "driveId": "b!H9kkVwxlEEiDzGGogYkX1twlusOfLMtIg750zfaOpaBq9eOBX6MXQapv1hTT-bIt",
                            "sharepointIds": {
                                "listId": "c61d1892-ca82-4f53-b16f-6bb8a379e2b2",
                                "listItemId": "1027",
                                "listItemUniqueId": "E320AFEB-AD73-46A2-83D7-985FAA4B206D"
                            }
                        },
                        "webUrl": "http://www.adventure-works.com/"
                    }
                }
            ]
        }
    ]
}
```

## <a name="known-limitations"></a>已知限制

以下资源不支持 **trimDuplicates** 属性： **消息**、 **事件** 和 **externalItem**。

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview)
