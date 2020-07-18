---
title: '获取日历视图中事件的增量更改 '
description: '日历视图是默认日历中特定日期/时间范围内的事件集合 (../me/calendarview)。 '
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 5b5e41a689a62157bb686ca6bb97ef63af9ac02a
ms.sourcegitcommit: b469176f49aacbd02cd06838cc7c8d36cf5bc768
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2020
ms.locfileid: "45165042"
---
# <a name="get-incremental-changes-to-events-in-a-calendar-view"></a><span data-ttu-id="094ad-103">获取日历视图中事件的增量更改</span><span class="sxs-lookup"><span data-stu-id="094ad-103">Get incremental changes to events in a calendar view</span></span> 

<span data-ttu-id="094ad-104">通过使用增量查询，你可以在指定的日历，或者日历中的定义事件集合（作为日历视图）中获取新的、更新的或删除的事件。</span><span class="sxs-lookup"><span data-stu-id="094ad-104">By using delta query, you can get new, updated, or deleted events in a specified calendar(s), or within a defined collection of events (as a calendar view) in the calendar.</span></span> <span data-ttu-id="094ad-105">本文将介绍后一种情况（在日历视图中对事件进行此类增量更改）。</span><span class="sxs-lookup"><span data-stu-id="094ad-105">This article describes the latter - getting such incremental changes to events in a calendar view.</span></span> 

> <span data-ttu-id="094ad-106">**注意** 前者（对日历中的事件进行增量更改，而不受固定的开始日期和结束日期范围的约束）的功能目前仅在 beta 版中可用。</span><span class="sxs-lookup"><span data-stu-id="094ad-106">**Note** The capability for the former - getting incremental changes to events in a calendar not bound to a fixed start and end date range - is currently available only in the beta version.</span></span> <span data-ttu-id="094ad-107">有关更多信息，请参阅 [delta](/graph/api/event-delta?view=graph-rest-beta) 函数。</span><span class="sxs-lookup"><span data-stu-id="094ad-107">For more information, see [delta](/graph/api/event-delta?view=graph-rest-beta) function.</span></span>

<span data-ttu-id="094ad-108">日历视图是某个日期/递减范围 (../me/calendarview) 内来自默认日历、用户的其他某个指定日历或者组日历的事件集合。</span><span class="sxs-lookup"><span data-stu-id="094ad-108">A calendar view is a collection of events in a date/time range (../me/calendarview) from the default calendar or some other specified calendar of a user, or from a group calendar.</span></span> <span data-ttu-id="094ad-109">返回的事件可能包括定期系列事件的单个实例、发生次数和例外情况。</span><span class="sxs-lookup"><span data-stu-id="094ad-109">The returned events may include single instances, or occurrences and exceptions of a recurring series.</span></span> <span data-ttu-id="094ad-110">借助增量数据，可以维护和同步用户事件的本地存储，而无需每次都从服务器提取整组用户事件。</span><span class="sxs-lookup"><span data-stu-id="094ad-110">The delta data enables you to maintain and synchronize a local store of a user's events, without having to fetch the entire set of the user's events from the server every time.</span></span>

<span data-ttu-id="094ad-p104">增量查询既支持可检索指定日历视图中的所有事件的完全同步，也支持可检索自上次同步后日历视图中发生变化的事件的增量同步。通常情况下，开始时会执行一次完全同步，随后会定期获取相应日历视图的增量更改。</span><span class="sxs-lookup"><span data-stu-id="094ad-p104">Delta query supports both full synchronization that retrieves all the events in the specified calendar view, and incremental synchronization that retrieves those events that have changed in the calendar view since the last synchronization. Typically, you would do an initial full synchronization, and subsequently, get incremental changes to that calendar view periodically.</span></span> 

## <a name="track-event-changes-in-a-calendar-view"></a><span data-ttu-id="094ad-113">跟踪日历视图中的事件更改</span><span class="sxs-lookup"><span data-stu-id="094ad-113">Track event changes in a calendar view</span></span>

<span data-ttu-id="094ad-114">在日历视图中对事件执行增量查询专门针对你指定的日历和日期/时间范围。</span><span class="sxs-lookup"><span data-stu-id="094ad-114">Delta query for events in a calendar view is specific to a calendar and date/time range that you specify.</span></span> <span data-ttu-id="094ad-115">若要跟踪多个日历中的更改，需要单独跟踪各个日历。</span><span class="sxs-lookup"><span data-stu-id="094ad-115">To track the changes in multiple calendars, you need to track each calendar individually.</span></span> 

<span data-ttu-id="094ad-116">跟踪日历视图中的事件更改通常需要使用 [delta](/graph/api/event-delta?view=graph-rest-1.0) 函数按轮发出一个或多个 GET 请求。</span><span class="sxs-lookup"><span data-stu-id="094ad-116">Tracking event changes in a calendar view typically is a round of one or more GET requests with the [delta](/graph/api/event-delta?view=graph-rest-1.0) function.</span></span> <span data-ttu-id="094ad-117">初始 GET 请求非常类似于[列出 calendarView](/graph/api/calendar-list-calendarview?view=graph-rest-1.0)，区别在于要添加 **delta** 函数。</span><span class="sxs-lookup"><span data-stu-id="094ad-117">The initial GET request is very much like the way you [list a calendarView](/graph/api/calendar-list-calendarview?view=graph-rest-1.0), except that you include the **delta** function.</span></span> <span data-ttu-id="094ad-118">下面是登录用户的默认日历中，“日历”视图的初始 GET 增量请求：</span><span class="sxs-lookup"><span data-stu-id="094ad-118">The following is the initial GET delta request of a calendar view in the signed-in user's default calendar:</span></span>

```
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="094ad-119">使用 **delta** 函数的 GET 请求返回以下任一内容：</span><span class="sxs-lookup"><span data-stu-id="094ad-119">A GET request with the **delta** function returns either:</span></span>

- <span data-ttu-id="094ad-120">`nextLink`（包含具有 **delta** 函数调用和 _skipToken_ 的 URL），或</span><span class="sxs-lookup"><span data-stu-id="094ad-120">A `nextLink` (that contains a URL with a **delta** function call and a _skipToken_), or</span></span> 
- <span data-ttu-id="094ad-121">`deltaLink`（包含具有 **delta** 函数调用和 _deltaToken_ 的 URL）。</span><span class="sxs-lookup"><span data-stu-id="094ad-121">A `deltaLink` (that contains a URL with a **delta** function call and _deltaToken_).</span></span>

<span data-ttu-id="094ad-122">这些令牌是[状态令牌](delta-query-overview.md#state-tokens)，负责对 _startDateTime_、_endDateTime_ 参数以及初始增量查询 GET 请求中的其他任何查询参数进行编码。</span><span class="sxs-lookup"><span data-stu-id="094ad-122">These tokens are [state tokens](delta-query-overview.md#state-tokens) which encode the _startDateTime_ and _endDateTime_ parameters, and any other query parameter in your initial delta query GET request.</span></span> <span data-ttu-id="094ad-123">在后续请求中，无需包括这些参数，因为它们已在令牌中编码。</span><span class="sxs-lookup"><span data-stu-id="094ad-123">You do not need to include these parameters in subsequent requests as they are encoded in the tokens.</span></span>

<span data-ttu-id="094ad-p108">状态令牌对客户端完全不透明。若要继续一轮事件更改跟踪，只需将最后一个 GET 请求返回的 `nextLink` 或 `deltaLink` URL 复制并应用到同一日历视图的下一个 **delta** 函数调用即可。响应中返回的 `deltaLink` 表示当前一轮更改跟踪已完成。可以保存 `deltaLink` URL，并在开始下一轮时使用。</span><span class="sxs-lookup"><span data-stu-id="094ad-p108">State tokens are completely opaque to the client. To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next **delta** function call for that same calendar view. A `deltaLink` returned in a response signifies that the current round of change tracking is complete. You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="094ad-128">若要了解如何使用这些 `nextLink` 和 `deltaLink` URL，请参阅下面的[示例](#example-to-synchronize-events-in-a-calendar-view)。</span><span class="sxs-lookup"><span data-stu-id="094ad-128">See the [example](#example-to-synchronize-events-in-a-calendar-view) below to learn how to use these `nextLink` and `deltaLink` URLs.</span></span>

### <a name="use-query-parameters-in-a-delta-query-for-calendar-view"></a><span data-ttu-id="094ad-129">在日历视图的增量查询中使用查询参数</span><span class="sxs-lookup"><span data-stu-id="094ad-129">Use query parameters in a delta query for calendar view</span></span>

- <span data-ttu-id="094ad-130">添加 _startDateTime_ 和 _endDateTime_ 参数可以定义日历视图的日期/时间范围。</span><span class="sxs-lookup"><span data-stu-id="094ad-130">Include the _startDateTime_ and _endDateTime_ parameters to define a date/time range for your calendar view.</span></span>
- <span data-ttu-id="094ad-131">不支持 `$select`。</span><span class="sxs-lookup"><span data-stu-id="094ad-131">`$select` is not supported.</span></span>


### <a name="optional-request-header"></a><span data-ttu-id="094ad-132">可选的请求头</span><span class="sxs-lookup"><span data-stu-id="094ad-132">Optional request header</span></span>

<span data-ttu-id="094ad-133">每个 delta 查询 GET 请求在响应中返回包含一个或多个事件的集合。</span><span class="sxs-lookup"><span data-stu-id="094ad-133">Each delta query GET request returns a collection of one or more events in the response.</span></span> <span data-ttu-id="094ad-134">可以视需要指定请求头 `Prefer: odata.maxpagesize={x}`，设置响应中可包含的事件数上限。</span><span class="sxs-lookup"><span data-stu-id="094ad-134">You can optionally specify the request header, `Prefer: odata.maxpagesize={x}`, to set the maximum number of events in a response.</span></span>


## <a name="example-to-synchronize-events-in-a-calendar-view"></a><span data-ttu-id="094ad-135">同步日历视图中事件的示例</span><span class="sxs-lookup"><span data-stu-id="094ad-135">Example to synchronize events in a calendar view</span></span>

<span data-ttu-id="094ad-p110">以下示例展示了如何通过 3 个请求同步特定时间范围内的用户默认日历。此日历视图中有 5 个事件。</span><span class="sxs-lookup"><span data-stu-id="094ad-p110">The following example shows a series of 3 requests to synchronize the user's default calendar in a specific time range. There are 5 events in that calendar view.</span></span>

- <span data-ttu-id="094ad-138">[第 1 步：示例第一个请求](#step-1-sample-initial-request)和[响应](#sample-initial-response)</span><span class="sxs-lookup"><span data-stu-id="094ad-138">[Step 1: sample initial request](#step-1-sample-initial-request) and [response](#sample-initial-response)</span></span>
- <span data-ttu-id="094ad-139">[第 2 步：示例第二个请求](#step-2-sample-second-request)和[响应](#sample-second-response)</span><span class="sxs-lookup"><span data-stu-id="094ad-139">[Step 2: sample second request](#step-2-sample-second-request) and [response](#sample-second-response)</span></span>
- <span data-ttu-id="094ad-140">[第 3 步：示例第三个请求](#step-3-sample-third-request)和[最终响应](#sample-third-and-final-response)</span><span class="sxs-lookup"><span data-stu-id="094ad-140">[Step 3: sample third request](#step-3-sample-third-request) and [final response](#sample-third-and-final-response)</span></span>

<span data-ttu-id="094ad-p111">为简洁起见，示例响应仅显示一部分事件属性。在实际调用中，大多数事件属性都会返回。</span><span class="sxs-lookup"><span data-stu-id="094ad-p111">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span> 

<span data-ttu-id="094ad-143">另请了解[下一轮](#the-next-round-sample-first-response)该执行哪些操作。</span><span class="sxs-lookup"><span data-stu-id="094ad-143">See also what you'll do in the [next round](#the-next-round-sample-first-response).</span></span>


### <a name="step-1-sample-initial-request"></a><span data-ttu-id="094ad-144">第 1 步：示例第一个请求</span><span class="sxs-lookup"><span data-stu-id="094ad-144">Step 1: sample initial request</span></span>

<span data-ttu-id="094ad-145">在该示例中，由于登录用户的默认日历中的指定日历视图为首次同步，因此第一个同步请求不含任何状态令牌。</span><span class="sxs-lookup"><span data-stu-id="094ad-145">In this example, the specified calendar view in the signed-in user's default calendar is being synchronized for the first time, so the initial sync request does not include any state token.</span></span> <span data-ttu-id="094ad-146">这一轮将返回此日历视图中的所有事件。</span><span class="sxs-lookup"><span data-stu-id="094ad-146">This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="094ad-147">第一个请求指定以下内容：</span><span class="sxs-lookup"><span data-stu-id="094ad-147">The first request specifies the following:</span></span>

- <span data-ttu-id="094ad-148">_startDateTime_ 和 _endDateTime_ 参数的日期/时间值。</span><span class="sxs-lookup"><span data-stu-id="094ad-148">Date/time values for the _startDateTime_ and _endDateTime_ parameters.</span></span>
- <span data-ttu-id="094ad-149">[可选的请求头](#optional-request-header) _odata.maxpagesize_，表示一次返回 2 个事件。</span><span class="sxs-lookup"><span data-stu-id="094ad-149">The [optional request header](#optional-request-header), _odata.maxpagesize_, returning 2 events at a time.</span></span>


# <a name="http"></a>[<span data-ttu-id="094ad-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="094ad-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?startdatetime=2016-12-01T00:00:00Z&enddatetime=2016-12-30T00:00:00Z HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="094ad-151">C#</span><span class="sxs-lookup"><span data-stu-id="094ad-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="094ad-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="094ad-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="094ad-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="094ad-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="094ad-154">Java</span><span class="sxs-lookup"><span data-stu-id="094ad-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="sample-initial-response"></a><span data-ttu-id="094ad-155">示例第一个响应</span><span class="sxs-lookup"><span data-stu-id="094ad-155">Sample initial response</span></span>

<span data-ttu-id="094ad-p113">响应中返回两个事件和一个包含 `skipToken` 的 `@odata.nextLink` 响应头。`nextLink` URL 表示此日历视图中还有更多事件可获取。</span><span class="sxs-lookup"><span data-stu-id="094ad-p113">The response includes two events and a `@odata.nextLink` response header with a `skipToken`. The `nextLink` URL indicates there are more events in the calendar view to get.</span></span>

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

### <a name="step-2-sample-second-request"></a><span data-ttu-id="094ad-158">第 2 步：示例第二个请求</span><span class="sxs-lookup"><span data-stu-id="094ad-158">Step 2: sample second request</span></span>

<span data-ttu-id="094ad-p114">第二个请求指定上一个响应中返回的 `nextLink` URL。请注意，不再需要像第一个请求一样指定相同的 _startDateTime_ 和 _endDateTime_ 参数，因为 `nextLink` URL 中的 `skipToken` 已将其编码并包含在内。</span><span class="sxs-lookup"><span data-stu-id="094ad-p114">The second request specifies the `nextLink` URL returned from the previous response. Notice that it no longer has to specify the same _startDateTime_ and _endDateTime_ parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>


# <a name="http"></a>[<span data-ttu-id="094ad-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="094ad-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmcCM996atia_s HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="094ad-162">C#</span><span class="sxs-lookup"><span data-stu-id="094ad-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="094ad-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="094ad-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="094ad-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="094ad-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="094ad-165">Java</span><span class="sxs-lookup"><span data-stu-id="094ad-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="sample-second-response"></a><span data-ttu-id="094ad-166">示例第二个响应</span><span class="sxs-lookup"><span data-stu-id="094ad-166">Sample second response</span></span> 

<span data-ttu-id="094ad-167">第二个响应中返回此日历视图中接下来的 2 个事件和另一个 `nextLink`（表示此日历视图中还有更多事件可获取）。</span><span class="sxs-lookup"><span data-stu-id="094ad-167">The second response returns the next 2 events in the calendar view and another `nextLink`, indicating there are more events to get from the calendar view.</span></span>

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


### <a name="step-3-sample-third-request"></a><span data-ttu-id="094ad-168">第 3 步：示例第三个请求</span><span class="sxs-lookup"><span data-stu-id="094ad-168">Step 3: sample third request</span></span>

<span data-ttu-id="094ad-169">第三个请求继续使用上一个同步请求返回的最新 `nextLink`。</span><span class="sxs-lookup"><span data-stu-id="094ad-169">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span> 
 


# <a name="http"></a>[<span data-ttu-id="094ad-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="094ad-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmci39OQxqJrxK4 HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="094ad-171">C#</span><span class="sxs-lookup"><span data-stu-id="094ad-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="094ad-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="094ad-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="094ad-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="094ad-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="094ad-174">Java</span><span class="sxs-lookup"><span data-stu-id="094ad-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="sample-third-and-final-response"></a><span data-ttu-id="094ad-175">示例第三个响应（即最终响应）</span><span class="sxs-lookup"><span data-stu-id="094ad-175">Sample third and final response</span></span>

<span data-ttu-id="094ad-p115">第三个响应中返回此日历视图中仅剩的事件，以及表示已完成同步此日历视图的 `deltaLink` URL。保存并使用 `deltaLink` URL [在下一轮中同步此日历视图](#the-next-round-sample-first-request)。</span><span class="sxs-lookup"><span data-stu-id="094ad-p115">The third response returns the only remaining event in the calendar view, and a `deltaLink` URL which indicates synchronization is complete for this calendar view. Save and use the `deltaLink` URL to [synchronize that calendar view in the next round](#the-next-round-sample-first-request).</span></span>


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


### <a name="the-next-round-sample-first-request"></a><span data-ttu-id="094ad-178">下一轮：示例第一个请求</span><span class="sxs-lookup"><span data-stu-id="094ad-178">The next round: sample first request</span></span>

<span data-ttu-id="094ad-p116">使用上一轮中[最后一个请求](#step-3-sample-third-request)返回的 `deltaLink`，可以只获取从那以后此日历视图中发生变化（已添加、删除或更新）的事件。假设你愿意在响应中保持页面大小上限不变，下一轮的第一个请求如下所示：</span><span class="sxs-lookup"><span data-stu-id="094ad-p116">Using the `deltaLink` from the [last request](#step-3-sample-third-request) in the last round, you will be able to get only those events that have changed (by being added, deleted, or updated) in that calendar view since then. Your first request in the next round will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>


# <a name="http"></a>[<span data-ttu-id="094ad-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="094ad-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_next"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcMDNGg0J1E HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="094ad-182">C#</span><span class="sxs-lookup"><span data-stu-id="094ad-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-next-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="094ad-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="094ad-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-next-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="094ad-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="094ad-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-next-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="094ad-185">Java</span><span class="sxs-lookup"><span data-stu-id="094ad-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-next-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="the-next-round-sample-first-response"></a><span data-ttu-id="094ad-186">下一轮：示例第一个响应</span><span class="sxs-lookup"><span data-stu-id="094ad-186">The next round: sample first response</span></span>

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

## <a name="see-also"></a><span data-ttu-id="094ad-187">另请参阅</span><span class="sxs-lookup"><span data-stu-id="094ad-187">See also</span></span>

- [<span data-ttu-id="094ad-188">Microsoft Graph 增量查询</span><span class="sxs-lookup"><span data-stu-id="094ad-188">Microsoft Graph delta query</span></span>](delta-query-overview.md)
- [<span data-ttu-id="094ad-189">获取邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="094ad-189">Get incremental changes to messages</span></span>](delta-query-messages.md)
- [<span data-ttu-id="094ad-190">获取组的增量更改</span><span class="sxs-lookup"><span data-stu-id="094ad-190">Get incremental changes to groups</span></span>](delta-query-groups.md)
- [<span data-ttu-id="094ad-191">获取用户的增量更改</span><span class="sxs-lookup"><span data-stu-id="094ad-191">Get incremental changes to users</span></span>](delta-query-users.md)
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
