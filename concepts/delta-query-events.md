---
title: 获取日历视图中事件的增量更改
description: 使用带有 delta 函数的 GET 请求跟踪日历视图中的事件更改。 示例演示如何在设置的时间范围内同步用户的默认日历。
author: Jumaodhiss
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: 9bc69ddd9a1f49475275ac029090c9625ad97da4
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66667542"
---
# <a name="get-incremental-changes-to-events-in-a-calendar-view"></a>获取日历视图中事件的增量更改

通过使用 delta 查询，你可以在指定的日历或在日历中定义的事件集合（作为日历视图）中获取新的、更新的或删除的事件。 本文将介绍后一种情况，即在日历视图中获取此类对事件的增量更改。

> [!NOTE]
> 前者的功能&mdash;获取日历中事件的增量更改，而不限于固定的开始和结束日期范围&mdash;目前仅在 beta 版中可用。 有关更多信息，请参阅 [delta](/graph/api/event-delta) 函数。

日历视图是某个日期/时间范围 (../me/calendarview) 内来自默认日历、用户的某个其他指定日历或者组日历的事件集合。 返回的事件可能包括单个实例或定期系列事件的发生和例外情况。 借助 delta 数据，你能够维护和同步本地存储的用户事件，而无需每次从服务器提取整组用户事件。

增量查询既支持可检索指定日历视图中的所有事件的完全同步，也支持可检索自上次同步后日历视图中发生变化的事件的增量同步。 通常情况下，开始时会执行一次完全同步，随后会定期获取该日历视图的增量更改。

## <a name="track-event-changes-in-a-calendar-view"></a>跟踪日历视图中的事件更改

日历视图中事件的 Delta 查询是针对指定的日历和日期/时间范围的。若要跟踪多个日历的变化，则需要单独跟踪每个日历。

跟踪日历视图中的事件更改通常需要使用 [delta](/graph/api/event-delta) 函数按轮发出一个或多个 GET 请求。 初始 GET 请求与 [列出 calendarView](/graph/api/calendar-list-calendarview) 非常相似，区别在于要包括 **delta** 函数。 下面是登录用户的默认日历中，“日历”视图的初始 GET 增量请求：

```
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
```

使用 **delta** 函数的 GET 请求返回以下任一内容：

- `@odata.nextLink`（包含具有 **delta** 函数调用和 `$skipToken` 的 URL），或 
- `@odata.deltaLink`（包含具有 **delta** 函数调用和 `$deltaToken` 的 URL）。

这些令牌是 [状态令牌](delta-query-overview.md#state-tokens)，负责对 _startDateTime_、_endDateTime_ 参数以及初始增量查询 GET 请求中的其他任何查询参数进行编码。 在后续请求中，无需包括这些参数，因为它们已在令牌中编码。

状态令牌对客户端完全不透明。若要继续一轮事件更改跟踪，只需将最后一个 GET 请求返回的 `@odata.nextLink` 或 `@odata.deltaLink` URL 复制并应用到同一日历视图的下一个 **delta** 函数调用即可。响应中返回的 `@odata.deltaLink` 表示当前一轮更改跟踪已完成。可以保存 `@odata.deltaLink` URL，并在开始下一轮时使用。

要了解如何使用 `@odata.nextLink` 和 `@odata.deltaLink` URL，请参阅 [示例](#example-synchronize-events-in-a-calendar-view)。

### <a name="use-query-parameters-in-a-delta-query-for-calendar-view"></a>在日历视图的增量查询中使用查询参数

- 添加 _startDateTime_ 和 _endDateTime_ 参数可以定义日历视图的日期/时间范围。
- 不支持 `$select`。


### <a name="optional-request-header"></a>可选的请求头

每个增量查询 GET 请求在响应中返回一个或多个事件的集合。可以视需要指定请求头 `Prefer: odata.maxpagesize={x}`，设置在响应中返回的事件数上限。


## <a name="example-synchronize-events-in-a-calendar-view"></a>示例：同步日历视图中的事件

以下示例展示了如何通过 3 个请求同步特定时间范围内的用户默认日历。此日历视图中有 5 个事件。

- [第 1 步：示例第一个请求](#step-1-sample-initial-request)和[响应](#sample-initial-response)
- [第 2 步：示例第二个请求](#step-2-sample-second-request)和[响应](#sample-second-response)
- [第 3 步：示例第三个请求](#step-3-sample-third-request)和[最终响应](#sample-third-and-final-response)

为简洁起见，示例响应仅显示一部分事件属性。在实际调用中，大多数事件属性都会返回。 

请了解 [下一轮](#the-next-round-sample-first-response) 将执行的操作。


### <a name="step-1-sample-initial-request"></a>第 1 步：示例第一个请求

在该示例中，是第一次同步登录用户默认日历中的指定日历视图，所以初始同步请求不包括任何状态标记。这一轮将返回该日历视图中的所有事件。

第一个请求指定以下内容：

- _startDateTime_ 和 _endDateTime_ 参数的日期/时间值。
- [可选的请求头](#optional-request-header) _odata.maxpagesize_，表示一次返回 2 个事件。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?startdatetime=2016-12-01T00:00:00Z&enddatetime=2016-12-30T00:00:00Z HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="sample-initial-response"></a>示例第一个响应

响应中返回两个事件和一个包含 `skipToken` 的 `@odata.nextLink` 响应头。`@odata.nextLink` URL 表示此日历视图中还有更多事件可获取。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmcCM996atia_s",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIQ==\"",
            "subject":"Plan shopping list",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-09T20:30:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-09T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },      
            "id":"AAMkADNVxRAAA="
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIg==\"",
            "subject":"Pick up car",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T01:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-10T02:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxSAAA="
        }
    ]
}
```

### <a name="step-2-sample-second-request"></a>第 2 步：示例第二个请求

第二个请求指定上一个响应中返回的 `@odata.nextLink` URL。请注意，不再需要像第一个请求一样指定相同的 _startDateTime_ 和 _endDateTime_ 参数，因为 `@odata.nextLink` URL 中的 `skipToken` 已将其编码并包含在内。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmcCM996atia_s HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="sample-second-response"></a>示例第二个响应 

第二个响应中返回此日历视图中接下来的 2 个事件和另一个 `@odata.nextLink`（表示此日历视图中还有更多事件可获取）。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmci39OQxqJrxK4",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIw==\"",
            "subject":"Get food",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T19:30:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-10T21:30:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxTAAA="
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvJA==\"",
            "subject":"Prepare food",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-11T00:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxUAAA="
        }
    ]
}
```


### <a name="step-3-sample-third-request"></a>第 3 步：示例第三个请求

第三个请求继续使用上一个同步请求返回的最新 `@odata.nextLink`。 
 


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmci39OQxqJrxK4 HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="sample-third-and-final-response"></a>示例第三个响应（即最终响应）

第三个响应中返回此日历视图中仅剩的事件，以及表示已完成同步此日历视图的 `@odata.deltaLink` URL。保存并使用 `@odata.deltaLink` URL [在下一轮中同步此日历视图](#the-next-round-sample-first-request)。


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcMDNGg0J1E",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAALZu97g==\"",
            "subject":"Rest!",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-12T02:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-12T07:30:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"Home"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADj1HuAAA="
        }
    ]
}
```


### <a name="the-next-round-sample-first-request"></a>下一轮：示例第一个请求

使用上一轮中[最后一个请求](#step-3-sample-third-request)返回的 `@odata.deltaLink`，可以只获取从那以后此日历视图中发生变化（已添加、删除或更新）的事件。假设你愿意在响应中保持页面大小上限不变，下一轮的第一个请求如下所示：


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_next"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcMDNGg0J1E HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-next-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-next-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-next-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-next-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="the-next-round-sample-first-response"></a>下一轮：示例第一个响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcFuQtZdtpk4",
    "value":[
        {
            "@odata.type": "#microsoft.graph.event",
            "id": "AAMkADk0MGFkODE3LWE4MmYtNDRhOS04OGQLkRkXbBznTvAADb6ytyAAA=",
            "@removed": {
                "reason": "deleted"
            }
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAALZu97w==\"",
            "subject":"Attend service",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-25T06:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-25T07:30:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"Chapel of Saint Ignatius",
                "address":{
                    "street":"900 Broadway",
                    "city":"Seattle",
                    "state":"WA",
                    "countryOrRegion":"United States",
                    "postalCode":""
                },
                "coordinates":{
                    "latitude":47.6105,
                    "longitude":-122.321
                }
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADj1HvAAA="
        }
    ]
}
```

## <a name="see-also"></a>另请参阅

- [Microsoft Graph 增量查询](delta-query-overview.md)
- [获取邮件的增量更改](delta-query-messages.md)
- [获取组的增量更改](delta-query-groups.md)
- [获取用户的增量更改](delta-query-users.md)
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example to synchronize events in a calendar view",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
