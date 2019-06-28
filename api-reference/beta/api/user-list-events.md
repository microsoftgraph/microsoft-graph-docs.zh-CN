---
title: 列出事件
description: '从用户的默认日历或指定的日历获取事件对象列表。 '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1d0cb44f302b484b610f2996aa7f7e1c5a24cc68
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270145"
---
# <a name="list-events"></a><span data-ttu-id="e0ccb-103">列出事件</span><span class="sxs-lookup"><span data-stu-id="e0ccb-103">List events</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0ccb-104">从用户的默认日历或指定的日历获取[事件](../resources/event.md)对象列表。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-104">Get a list of [event](../resources/event.md) objects from the user's default calendar or from a specified calendar.</span></span> <span data-ttu-id="e0ccb-105">该列表包含单实例会议和系列主控事件。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-105">The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="e0ccb-106">要获取扩展的事件实例，可以[获取日历视图](calendar-list-calendarview.md)，或者[获取事件的实例](event-list-instances.md)。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-106">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

<span data-ttu-id="e0ccb-107">在以下两种情况下，应用程序可以获取其他用户的日历中的事件：</span><span class="sxs-lookup"><span data-stu-id="e0ccb-107">There are two scenarios where an app can get events in another user's calendar:</span></span>

* <span data-ttu-id="e0ccb-108">如果该应用程序具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="e0ccb-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="e0ccb-109">如果应用程序具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了日历，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="e0ccb-110">请参阅[详细信息和示例](/graph/outlook-get-shared-events-calendars)。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="e0ccb-111">支持不同时区</span><span class="sxs-lookup"><span data-stu-id="e0ccb-111">Support various time zones</span></span>

<span data-ttu-id="e0ccb-112">对于返回事件的所有 GET 操作，你可以使用 `Prefer: outlook.timezone` 标头在响应中指定事件开始和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-112">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="e0ccb-113">例如，下面的 `Prefer: outlook.timezone` 标头将响应中的开始和结束时间设置为东部标准时间。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-113">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="e0ccb-p103">如果该事件是在不同的时区中创建的，则根据 `Prefer` 标头中指定的时区调整开始和结束时间。请查看此 [列表](../resources/datetimetimezone.md) 了解支持的时区名称。如果未指定 `Prefer: outlook.timezone` 标头，则返回用 UTC 表示的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-p103">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="e0ccb-117">可以使用**事件**资源中的 **OriginalStartTimeZone** 和 **OriginalEndTimeZone** 属性来查找创建事件时使用的时区。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-117">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0ccb-118">权限</span><span class="sxs-lookup"><span data-stu-id="e0ccb-118">Permissions</span></span>
<span data-ttu-id="e0ccb-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0ccb-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0ccb-121">Permission type</span></span>      | <span data-ttu-id="e0ccb-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0ccb-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0ccb-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0ccb-123">Delegated (work or school account)</span></span> | <span data-ttu-id="e0ccb-124">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0ccb-124">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e0ccb-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0ccb-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0ccb-126">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0ccb-126">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e0ccb-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0ccb-127">Application</span></span> | <span data-ttu-id="e0ccb-128">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0ccb-128">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0ccb-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0ccb-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events
GET /users/{id | userPrincipalName}/events

GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events

GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendargroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events

GET /me/calendargroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e0ccb-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e0ccb-130">Optional query parameters</span></span>
<span data-ttu-id="e0ccb-131">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e0ccb-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0ccb-132">Request headers</span></span>
| <span data-ttu-id="e0ccb-133">名称</span><span class="sxs-lookup"><span data-stu-id="e0ccb-133">Name</span></span>       | <span data-ttu-id="e0ccb-134">类型</span><span class="sxs-lookup"><span data-stu-id="e0ccb-134">Type</span></span> | <span data-ttu-id="e0ccb-135">说明</span><span class="sxs-lookup"><span data-stu-id="e0ccb-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e0ccb-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0ccb-136">Authorization</span></span>  | <span data-ttu-id="e0ccb-137">string</span><span class="sxs-lookup"><span data-stu-id="e0ccb-137">string</span></span>  | <span data-ttu-id="e0ccb-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e0ccb-140">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="e0ccb-140">Prefer: outlook.timezone</span></span> | <span data-ttu-id="e0ccb-141">string</span><span class="sxs-lookup"><span data-stu-id="e0ccb-141">string</span></span> | <span data-ttu-id="e0ccb-142">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="e0ccb-143">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="e0ccb-144">可选。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-144">Optional.</span></span> |
| <span data-ttu-id="e0ccb-145">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="e0ccb-145">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="e0ccb-146">string</span><span class="sxs-lookup"><span data-stu-id="e0ccb-146">string</span></span> | <span data-ttu-id="e0ccb-147">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-147">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="e0ccb-148">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-148">Values can be "text" or "html".</span></span> <span data-ttu-id="e0ccb-149">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-149">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="e0ccb-150">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-150">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="e0ccb-151">可选。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0ccb-152">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0ccb-152">Request body</span></span>
<span data-ttu-id="e0ccb-153">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0ccb-154">响应</span><span class="sxs-lookup"><span data-stu-id="e0ccb-154">Response</span></span>

<span data-ttu-id="e0ccb-155">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-155">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e0ccb-156">示例</span><span class="sxs-lookup"><span data-stu-id="e0ccb-156">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="e0ccb-157">请求 1</span><span class="sxs-lookup"><span data-stu-id="e0ccb-157">Request 1</span></span>
<span data-ttu-id="e0ccb-158">第一个示例获取用户的所有事件。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-158">The first example gets all the user's events.</span></span> <span data-ttu-id="e0ccb-159">它指定以下内容：</span><span class="sxs-lookup"><span data-stu-id="e0ccb-159">It specifies the following:</span></span>

- <span data-ttu-id="e0ccb-160">获取以太平洋标准时间格式返回的日期时间值的 `Prefer: outlook.timezone` 标头。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-160">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="e0ccb-p109">返回特定属性的 `$select` 查询参数。如果没有 `$select` 参数，将返回所有事件属性。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-p109">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<span data-ttu-id="e0ccb-163">该请求未指定任何 `Prefer: outlook.body-content-type` 标头来指示返回的事件正文的特定格式。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-163">The request does not specify any `Prefer: outlook.body-content-type` header to indicate a specific format for the returned event body.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/beta/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response-1"></a><span data-ttu-id="e0ccb-164">响应 1</span><span class="sxs-lookup"><span data-stu-id="e0ccb-164">Response 1</span></span>
<span data-ttu-id="e0ccb-165">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-165">Here is an example of the response.</span></span> <span data-ttu-id="e0ccb-166">由于未指定任何 `Prefer: outlook.body-content-type` 标头，将以默认 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-166">Because no `Prefer: outlook.body-content-type` header was specified, the **body** property is returned in the default HTML format.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_events",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-length: 1932

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)",
    "value":[
        {
            "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
            "id":"AAMkAGIAAAoZDOFAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"html",
                "content":"<html><head></head><body><p>Dana, this is the time you selected for our orientation. Please bring the notes I sent you.</p></body></html>"
            },
            "start":{
                "dateTime":"2017-04-21T10:00:00.0000000",
                "timeZone":"Pacific Standard Time"
            },
            "end":{
                "dateTime":"2017-04-21T12:00:00.0000000",
                "timeZone":"Pacific Standard Time"
            },
            "location": {
                "displayName": "Assembly Hall",
                "locationType": "default",
                "uniqueId": "Assembly Hall",
                "uniqueIdType": "private"
            },
            "locations": [
                {
                    "displayName": "Assembly Hall",
                    "locationType": "default",
                    "uniqueIdType": "unknown"
                }
            ],
            "attendees":[
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Samantha Booth",
                        "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
                    }
                },
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Dana Swope",
                        "address":"danas@a830edad905084922E17020313.onmicrosoft.com"
                    }
                }
            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
                }
            }
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e0ccb-167">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e0ccb-167">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e0ccb-168">C#</span><span class="sxs-lookup"><span data-stu-id="e0ccb-168">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_events-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0ccb-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="e0ccb-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_events-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e0ccb-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0ccb-170">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_events-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="e0ccb-171">请求 2</span><span class="sxs-lookup"><span data-stu-id="e0ccb-171">Request 2</span></span>
<span data-ttu-id="e0ccb-172">第二个示例介绍如何使用 `Prefer: outlook.body-content-type="text"` 标头获取采用文本格式的指定消息的 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-172">The second example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified message in text format.</span></span>

<span data-ttu-id="e0ccb-173">该请求还使用 `$select` 查询参数返回特定属性。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-173">The request also uses a `$select` query parameter to return specific properties.</span></span> <span data-ttu-id="e0ccb-174">如果没有 `$select` 参数，将返回所有事件属性。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-174">Without a `$select` parameter, all of the event properties will be returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/events?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text" 
```
##### <a name="response-2"></a><span data-ttu-id="e0ccb-175">响应 2</span><span class="sxs-lookup"><span data-stu-id="e0ccb-175">Response 2</span></span>
<span data-ttu-id="e0ccb-176">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-176">Here is an example of the response.</span></span> <span data-ttu-id="e0ccb-177">以文本格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="e0ccb-177">The **body** property is returned in text format.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"
Content-length: 640

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview)",
    "value":[
        {
            "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
            "id":"AAMkAGIAAAoZDOFAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            }
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e0ccb-178">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e0ccb-178">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e0ccb-179">C#</span><span class="sxs-lookup"><span data-stu-id="e0ccb-179">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_events_in_text-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0ccb-180">Javascript</span><span class="sxs-lookup"><span data-stu-id="e0ccb-180">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_events_in_text-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e0ccb-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0ccb-181">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_events_in_text-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-events.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-list-events.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-events.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-list-events.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-events.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
