---
title: '获取日历视图中事件的增量更改 '
description: '日历视图是默认日历中特定日期/时间范围内的事件集合 (../me/calendarview)。 '
author: piotrci
ms.openlocfilehash: adfc8e8fb595e721781901f80c7d730b06112b72
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334837"
---
# <a name="get-incremental-changes-to-events-in-a-calendar-view"></a><span data-ttu-id="c8fbd-103">获取日历视图中事件的增量更改</span><span class="sxs-lookup"><span data-stu-id="c8fbd-103">Get incremental changes to events in a calendar view</span></span> 

<span data-ttu-id="c8fbd-p101">日历视图是一系列来自默认日历 (../me/calendarview) 或用户的其他某个日历且位于日期/时间范围内的事件。使用增量查询，可以获取日历视图中的新建、已更新或已删除事件。返回的事件可能包括定期系列事件的发生次数和例外情况，以及单个实例。借助增量数据，可以维护和同步用户事件的本地存储，而无需每次都从服务器提取整组用户事件。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-p101">A calendar view is a collection of events in a date/time range from the default calendar (../me/calendarview) or some other calendar of the user's. By using delta query, you can get new, updated, or deleted events in a calendar view. The returned events may include occurrences and exceptions of a recurring series, and single instances. The delta data enables you to maintain and synchronize a local store of a user's events, without having to fetch the entire set of the user's events from the server every time.</span></span>

<span data-ttu-id="c8fbd-p102">增量查询既支持可检索指定日历视图中的所有事件的完全同步，也支持可检索自上次同步后日历视图中发生变化的事件的增量同步。通常情况下，开始时会执行一次完全同步，随后会定期获取相应日历视图的增量更改。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-p102">Delta query supports both full synchronization that retrieves all the events in the specified calendar view, and incremental synchronization that retrieves those events that have changed in the calendar view since the last synchronization. Typically, you would do an initial full synchronization, and subsequently, get incremental changes to that calendar view periodically.</span></span> 

## <a name="track-event-changes-in-a-calendar-view"></a><span data-ttu-id="c8fbd-110">跟踪日历视图中的事件更改</span><span class="sxs-lookup"><span data-stu-id="c8fbd-110">Track event changes in a calendar view</span></span>

<span data-ttu-id="c8fbd-p103">对事件执行增量查询专门针对你指定的日历和日期/时间范围（即日历视图）。若要跟踪多个日历中的更改，需要单独跟踪各个日历。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-p103">Delta query for events is specific to a calendar and date/time range that you specify (i.e., a calendar view). To track the changes in multiple calendars, you need to track each calendar individually.</span></span> 

<span data-ttu-id="c8fbd-p104">跟踪日历视图中的事件更改通常需要使用 [delta](/graph/api/event-delta?view=graph-rest-1.0) 函数按轮发出一个或多个 GET 请求。初始 GET 请求非常类似于[列出 calendarView](/graph/api/calendar-list-calendarview?view=graph-rest-1.0)，区别在于要添加 **delta** 函数：</span><span class="sxs-lookup"><span data-stu-id="c8fbd-p104">Tracking event changes in a calendar view typically is a round of one or more GET requests with the [delta](/graph/api/event-delta?view=graph-rest-1.0) function. The initial GET request is very much like the way you [list a calendarView](/graph/api/calendar-list-calendarview?view=graph-rest-1.0), except that you include the **delta** function:</span></span>

```
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="c8fbd-115">使用 **delta** 函数的 GET 请求返回以下任一内容：</span><span class="sxs-lookup"><span data-stu-id="c8fbd-115">A GET request with the **delta** function returns either:</span></span>

- <span data-ttu-id="c8fbd-116">`nextLink`（包含具有 **delta** 函数调用和 _skipToken_ 的 URL），或</span><span class="sxs-lookup"><span data-stu-id="c8fbd-116">A `nextLink` (that contains a URL with a **delta** function call and a _skipToken_), or</span></span> 
- <span data-ttu-id="c8fbd-117">`deltaLink`（包含具有 **delta** 函数调用和 deltaToken 的 URL）。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-117">A `deltaLink` (that contains a URL with a **delta** function call and _deltaToken_).</span></span>

<span data-ttu-id="c8fbd-118">这些令牌是[状态令牌](delta-query-overview.md#state-tokens)，负责对 refs/remotes/microsoftgraph/master startDateTime、endDateTime 参数以及初始增量查询 GET 请求中的任何其他查询参数进行编码。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-118">These tokens are [state tokens](delta-query-overview.md#state-tokens) which encode the refs/remotes/microsoftgraph/master _startDateTime_ and _endDateTime_ parameters, and any other query parameter in your initial delta query GET request.</span></span> 

<span data-ttu-id="c8fbd-p105">状态令牌对客户端完全不透明。若要继续一轮事件更改跟踪，只需将最后一个 GET 请求返回的 `nextLink` 或 `deltaLink` URL 复制并应用到同一日历视图的下一个 **delta** 函数调用即可。响应中返回的 `deltaLink` 表示当前一轮更改跟踪已完成。可以保存 `deltaLink` URL，并在开始下一轮时使用。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-p105">State tokens are completely opaque to the client. To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next **delta** function call for that same calendar view. A `deltaLink` returned in a response signifies that the current round of change tracking is complete. You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="c8fbd-123">若要了解如何使用这些 `nextLink` 和 `deltaLink` URL，请参阅下面的[示例](#example-to-synchronize-events-in-a-calendar-view)。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-123">See the [example](#example-to-synchronize-events-in-a-calendar-view) below to learn how to use these `nextLink` and `deltaLink` URLs.</span></span>

### <a name="use-query-parameters-in-a-delta-query-for-calendar-view"></a><span data-ttu-id="c8fbd-124">在日历视图的增量查询中使用查询参数</span><span class="sxs-lookup"><span data-stu-id="c8fbd-124">Use query parameters in a delta query for calendar view</span></span>

- <span data-ttu-id="c8fbd-125">添加 _startDateTime_ 和 _endDateTime_ 参数可以定义日历视图的日期/时间范围。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-125">Include the _startDateTime_ and _endDateTime_ parameters to define a date/time range for your calendar view.</span></span>
- <span data-ttu-id="c8fbd-126">不支持 `$select`。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-126">`$select` is not supported.</span></span>


### <a name="optional-request-header"></a><span data-ttu-id="c8fbd-127">可选的请求头</span><span class="sxs-lookup"><span data-stu-id="c8fbd-127">Optional request header</span></span>

<span data-ttu-id="c8fbd-128">每个 delta 查询 GET 请求在响应中返回包含一个或多个事件的集合。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-128">Each delta query GET request returns a collection of one or more events in the response.</span></span> <span data-ttu-id="c8fbd-129">可以视需要指定请求头 `Prefer: odata.maxpagesize={x}`，设置响应中可包含的事件数上限。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-129">You can optionally specify the request header, `Prefer: odata.maxpagesize={x}`, to set the maximum number of events in a response.</span></span>


## <a name="example-to-synchronize-events-in-a-calendar-view"></a><span data-ttu-id="c8fbd-130">同步日历视图中事件的示例</span><span class="sxs-lookup"><span data-stu-id="c8fbd-130">Example to synchronize events in a calendar view</span></span>

<span data-ttu-id="c8fbd-p107">以下示例展示了如何通过 3 个请求同步特定时间范围内的用户默认日历。此日历视图中有 5 个事件。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-p107">The following example shows a series of 3 requests to synchronize the user's default calendar in a specific time range. There are 5 events in that calendar view.</span></span>

- <span data-ttu-id="c8fbd-133">[第 1 步：示例第一个请求](#step-1-sample-initial-request)和[响应](#sample-initial-response)</span><span class="sxs-lookup"><span data-stu-id="c8fbd-133">[Step 1: sample initial request](#step-1-sample-initial-request) and [response](#sample-initial-response)</span></span>
- <span data-ttu-id="c8fbd-134">[第 2 步：示例第二个请求](#step-2-sample-second-request)和[响应](#sample-second-response)</span><span class="sxs-lookup"><span data-stu-id="c8fbd-134">[Step 2: sample second request](#step-2-sample-second-request) and [response](#sample-second-response)</span></span>
- <span data-ttu-id="c8fbd-135">[第 3 步：示例第三个请求](#step-3-sample-third-request)和[最终响应](#sample-third-and-final-response)</span><span class="sxs-lookup"><span data-stu-id="c8fbd-135">[Step 3: sample third request](#step-3-sample-third-request) and [final response](#sample-third-and-final-response)</span></span>

<span data-ttu-id="c8fbd-p108">为简洁起见，示例响应仅显示一部分事件属性。在实际调用中，大多数事件属性都会返回。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-p108">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span> 

<span data-ttu-id="c8fbd-138">另请了解[下一轮](#the-next-round-sample-first-response)该执行哪些操作。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-138">See also what you'll do in the [next round](#the-next-round-sample-first-response).</span></span>


### <a name="step-1-sample-initial-request"></a><span data-ttu-id="c8fbd-139">第 1 步：示例第一个请求</span><span class="sxs-lookup"><span data-stu-id="c8fbd-139">Step 1: sample initial request</span></span>

<span data-ttu-id="c8fbd-p109">在该示例中，由于指定日历视图为首次同步，因此第一个同步请求不含任何状态令牌。这一轮将返回此日历视图中的所有事件。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-p109">In this example, the specified calendar view is being synchronized for the first time, so the initial sync request does not include any state token. This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="c8fbd-142">第一个请求指定以下内容：</span><span class="sxs-lookup"><span data-stu-id="c8fbd-142">The first request specifies the following:</span></span>

- <span data-ttu-id="c8fbd-143">_startDateTime_ 和 _endDateTime_ 参数的日期/时间值。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-143">Date/time values for the _startDateTime_ and _endDateTime_ parameters.</span></span>
- <span data-ttu-id="c8fbd-144">[可选的请求头](#optional-request-header) _odata.maxpagesize_，表示一次返回 2 个事件。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-144">The [optional request header](#optional-request-header), _odata.maxpagesize_, returning 2 events at a time.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?startdatetime=2016-12-01T00:00:00Z&enddatetime=2016-12-30T00:00:00Z HTTP/1.1
Prefer: odata.maxpagesize=2
```


### <a name="sample-initial-response"></a><span data-ttu-id="c8fbd-145">示例第一个响应</span><span class="sxs-lookup"><span data-stu-id="c8fbd-145">Sample initial response</span></span>

<span data-ttu-id="c8fbd-p110">响应中返回两个事件和一个包含 `skipToken` 的 `@odata.nextLink` 响应头。`nextLink` URL 表示此日历视图中还有更多事件可获取。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-p110">The response includes two events and a `@odata.nextLink` response header with a `skipToken`. The `nextLink` URL indicates there are more events in the calendar view to get.</span></span>

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

### <a name="step-2-sample-second-request"></a><span data-ttu-id="c8fbd-148">第 2 步：示例第二个请求</span><span class="sxs-lookup"><span data-stu-id="c8fbd-148">Step 2: sample second request</span></span>

<span data-ttu-id="c8fbd-p111">第二个请求指定上一个响应中返回的 `nextLink` URL。请注意，不再需要像第一个请求一样指定相同的 _startDateTime_ 和 _endDateTime_ 参数，因为 `nextLink` URL 中的 `skipToken` 已将其编码并包含在内。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-p111">The second request specifies the `nextLink` URL returned from the previous response. Notice that it no longer has to specify the same _startDateTime_ and _endDateTime_ parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmcCM996atia_s HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-second-response"></a><span data-ttu-id="c8fbd-151">示例第二个响应</span><span class="sxs-lookup"><span data-stu-id="c8fbd-151">Sample second response</span></span> 

<span data-ttu-id="c8fbd-152">第二个响应中返回此日历视图中接下来的 2 个事件和另一个 `nextLink`（表示此日历视图中还有更多事件可获取）。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-152">The second response returns the next 2 events in the calendar view and another `nextLink`, indicating there are more events to get from the calendar view.</span></span>

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


### <a name="step-3-sample-third-request"></a><span data-ttu-id="c8fbd-153">第 3 步：示例第三个请求</span><span class="sxs-lookup"><span data-stu-id="c8fbd-153">Step 3: sample third request</span></span>

<span data-ttu-id="c8fbd-154">第三个请求继续使用上一个同步请求返回的最新 `nextLink`。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-154">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span> 
 

<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_3"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmci39OQxqJrxK4 HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-third-and-final-response"></a><span data-ttu-id="c8fbd-155">示例第三个响应（即最终响应）</span><span class="sxs-lookup"><span data-stu-id="c8fbd-155">Sample third and final response</span></span>

<span data-ttu-id="c8fbd-p112">第三个响应中返回此日历视图中仅剩的事件，以及表示已完成同步此日历视图的 `deltaLink` URL。保存并使用 `deltaLink` URL [在下一轮中同步此日历视图](#the-next-round-sample-first-request)。</span><span class="sxs-lookup"><span data-stu-id="c8fbd-p112">The third response returns the only remaining event in the calendar view, and a `deltaLink` URL which indicates synchronization is complete for this calendar view. Save and use the `deltaLink` URL to [synchronize that calendar view in the next round](#the-next-round-sample-first-request).</span></span>


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


### <a name="the-next-round-sample-first-request"></a><span data-ttu-id="c8fbd-158">下一轮：示例第一个请求</span><span class="sxs-lookup"><span data-stu-id="c8fbd-158">The next round: sample first request</span></span>

<span data-ttu-id="c8fbd-p113">使用上一轮中[最后一个请求](#step-3-sample-third-request)返回的 `deltaLink`，可以只获取从那以后此日历视图中发生变化（已添加、删除或更新）的事件。假设你愿意在响应中保持页面大小上限不变，下一轮的第一个请求如下所示：</span><span class="sxs-lookup"><span data-stu-id="c8fbd-p113">Using the `deltaLink` from the [last request](#step-3-sample-third-request) in the last round, you will be able to get only those events that have changed (by being added, deleted, or updated) in that calendar view since then. Your first request in the next round will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_next"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcMDNGg0J1E HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="the-next-round-sample-first-response"></a><span data-ttu-id="c8fbd-161">下一轮：示例第一个响应</span><span class="sxs-lookup"><span data-stu-id="c8fbd-161">The next round: sample first response</span></span>

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

## <a name="see-also"></a><span data-ttu-id="c8fbd-162">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c8fbd-162">See also</span></span>

- [<span data-ttu-id="c8fbd-163">Microsoft Graph 增量查询</span><span class="sxs-lookup"><span data-stu-id="c8fbd-163">Microsoft Graph delta query</span></span>](delta-query-overview.md)
- [<span data-ttu-id="c8fbd-164">获取邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="c8fbd-164">Get incremental changes to messages</span></span>](delta-query-messages.md)
- [<span data-ttu-id="c8fbd-165">获取组的增量更改</span><span class="sxs-lookup"><span data-stu-id="c8fbd-165">Get incremental changes to groups</span></span>](delta-query-groups.md)
- [<span data-ttu-id="c8fbd-166">获取用户的增量更改</span><span class="sxs-lookup"><span data-stu-id="c8fbd-166">Get incremental changes to users</span></span>](delta-query-users.md)
