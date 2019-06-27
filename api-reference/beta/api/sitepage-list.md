---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: 列出网站中的页面
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 938624d1330a36b3f1318f09290b30bf9388e4ce
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271531"
---
# <a name="list-the-pages-in-the-site-pages-list-of-a-site"></a>在网站的 "网站页面" 列表中列出页面

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从网站[网站][]的 "网站页面"[列表][]中获取[sitePage][]对象的集合。 将返回网站中的所有页面 (使用分页)。

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[网站]: ../resources/site.md

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.Read.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

```http
GET /sites/{site-id}/pages

```

## <a name="example"></a>示例

#### <a name="request"></a>请求

<!-- 
{ 
    "blockType": "request",
    "name": "get-pages",
    "scopes": "sites.read.all", 
    "tags": "service.sharepoint"
}
-->

```http
GET /sites/{site-id}/pages
```

#### <a name="response"></a>响应

<!-- 
{ 
    "blockType": "response",
    "@odata.type": "microsoft.graph.sitePage",
    "truncated": true,
    "isCollection":true
} 
-->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "5",
            "eTag": "\"{8BEE5ABE-49B9-431B-AEBA-C96D6DEF44E3},4\"",
            "lastModifiedDateTime": "2018-08-15T19:20:20Z",
            "name": "EventInstructions.aspx",
            "webUrl": "SitePages/EventInstructions.aspx",
            "uniqueId": "8bee5abe-49b9-431b-aeba-c96d6def44e3",
            "description": "",
            "title": "Event Instructions",
            "pageLayoutType": "Article",
            "createdBy": {
                "user": {
                    "displayName": "Jimmy Felts",
                    "email": "jimmy@contoso.com"
                }
            },
            "lastModifiedBy": {
                "user": {
                    "displayName": "Jimmy Felts",
                    "email": "jimmy@contoso.com"
                }
            },
            "parentReference": {
                "listId": "334e40f2-1614-4fdc-87ad-d7b91407c5a9",
                "siteId": "66bed137-bf1f-41c8-a0e9-2bc01097a797"
            },
            "contentType": {
                "id": "0x0101009D1CB255DA76424F860D91F20E6C4118",
                "name": "Site Page"
            },
            "publishingState": {
                "level": "published",
                "versionId": "1.0"
            },
            "webParts": [
                {
                    "type": "daf0b71c-6de8-4ef7-b511-faae7c388708",
                    "data": {
                        "id": "daf0b71c-6de8-4ef7-b511-faae7c388708",
                        "instanceId": "b646d2e4-2b9c-41c7-a567-0c05c2909d5a",
                        "title": "Registration",
                        "description": "...",
                        "serverProcessedContent": {
                            "htmlStrings": {},
                            "searchablePlainTexts": {
                                "title": ""
                            },
                            "imageSources": {},
                            "links": {
                                "baseUrl": "/teams/SPClientTest"
                            },
                            "componentDependencies": {
                                "layoutComponentId": "62680648-d047-46ec-81e0-475ee78e482d"
                            }
                        },
                        "dataVersion": "2.1",
                        "properties": {
                            "webId": "4a15f359-257c-4f31-8350-5025104e30d5",
                            "siteId": "00c6b6c6-c466-4e64-a370-2b6ddb7cdfe3",
                            "query": {  },
                            "templateId": 1,
                            "maxItemsPerPage": 10,
                            "hideWebPartWhenEmpty": false,
                            "kqlQueryTemplate": "...",
                            "displayMaps": {  },
                            "sites": [],
                            "layoutId": "Card",
                            "dataProviderId": "Search"
                        }
                    }
                }
            ]
        },
        {
            "id": "2",
            "eTag": "\"{75bc70e2-6587-45be-8493-c99a956b2e05},7\"",
            "createdDateTime": "2016-12-06T20:04:40Z",
            "lastModifiedDateTime": "2016-12-06T20:05:09Z",
            "webUrl": "https://www.contoso.com/sites/Engineering/SitePages/Events.aspx",
            "createdBy": {
                "user": {
                    "email": "jimmy@contoso.com",
                    "id": "1b37d2e1-5000-4648-b431-7dfa509b5660",
                    "displayName": "Jimmy Felts"
                }
            },
            "lastModifiedBy": {
                "user": {
                    "email": "jimmy@contoso.com",
                    "id": "1b37d2e1-5000-4648-b431-7dfa509b5660",
                    "displayName": "Jimmy Felts"
                }
            },
            "parentReference": {
                "id": "eb3bfd48-56f8-4c1e-8312-e58588b22e7c"
            },
            "contentType": {
                "id": "0x0101009D1CB255DA76424F860D91F20E6C411800C9E7033636784C4B88A284B1823C45FD",
                "name": "Site Page"
            },
            "description": "",
            "title": "Upcoming Events",
            "publishingState": {
                "level": "checkout",
                "versionId": "1.1",
                "checkedOutBy": {
                    "user": {
                        "displayName": "Jimmy Felts",
                        "email": "jimmy@contoso.com"
                    }
                }
            },
            "webParts": [
                {
                    "type": "rte",
                    "data": {
                        "innerHTML": "<p>Here are the team's upcoming events:</p>"
                    }
                },
                {
                    "type": "d1d91016-032f-456d-98a4-721247c305e8",
                    "data": {
                        "title": "Events",
                        "description": "Display upcoming events",
                        "serverProcessedContent": {
                            "htmlStrings": {},
                            "searchablePlainTexts": {
                                "title": ""
                            },
                            "imageSources": {},
                            "links": {
                                "baseUrl": "https://www.contoso.com/sites/Engineering"
                            },
                            "componentDependencies": {
                                "layoutComponentId": "8ac0c53c-e8d0-4e3e-87d0-7449eb0d4027"
                            }
                        },
                        "dataVersion": "1.0",
                        "properties": {
                            "selectedListId": "032e08ab-89b0-4d8f-bc10-73094233615c",
                            "selectedCategory": "",
                            "dateRangeOption": 0,
                            "startDate": "",
                            "endDate": "",
                            "isOnSeeAllPage": false,
                            "layoutId": "FilmStrip",
                            "dataProviderId": "Event",
                            "webId": "0764c419-1ecc-4126-ba32-0c25ae0fffe8",
                            "siteId": "6b4ffc7a-cfc2-4a76-903a-1cc3686dee23"
                        }
                    }
                }
            ]
        }
    ]
}
```
#### <a name="sdk-sample-code"></a>SDK 示例代码
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get-pages-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-pages-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-pages-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "Enumerate the list of pages in a site",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Enumerate",
  "suppressions": [
    "Error: /api-reference/beta/api/sitepage-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/sitepage-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/sitepage-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
