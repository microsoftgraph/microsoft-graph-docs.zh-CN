---
title: 列出事件
description: '从用户的默认日历或指定的日历获取事件对象列表。 '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 809325e45540deac3d3e260a7b8e62953e697646
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867308"
---
# <a name="list-events"></a><span data-ttu-id="411f7-103">列出事件</span><span class="sxs-lookup"><span data-stu-id="411f7-103">List events</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="411f7-104">从用户的默认日历或指定的日历获取[事件](../resources/event.md)对象列表。</span><span class="sxs-lookup"><span data-stu-id="411f7-104">Get a list of [event](../resources/event.md) objects from the user's default calendar or from a specified calendar.</span></span> <span data-ttu-id="411f7-105">该列表包含单实例会议和系列主控事件。</span><span class="sxs-lookup"><span data-stu-id="411f7-105">The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="411f7-106">要获取扩展的事件实例，可以[获取日历视图](calendar-list-calendarview.md)，或者[获取事件的实例](event-list-instances.md)。</span><span class="sxs-lookup"><span data-stu-id="411f7-106">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

<span data-ttu-id="411f7-107">在以下两种情况下，应用程序可以获取其他用户的日历中的事件：</span><span class="sxs-lookup"><span data-stu-id="411f7-107">There are two scenarios where an app can get events in another user's calendar:</span></span>

* <span data-ttu-id="411f7-108">如果该应用程序具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="411f7-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="411f7-109">如果应用程序具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了日历，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="411f7-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="411f7-110">请参阅[详细信息和示例](/graph/outlook-get-shared-events-calendars)。</span><span class="sxs-lookup"><span data-stu-id="411f7-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="411f7-111">支持不同时区</span><span class="sxs-lookup"><span data-stu-id="411f7-111">Support various time zones</span></span>

<span data-ttu-id="411f7-112">对于返回事件的所有 GET 操作，你可以使用 `Prefer: outlook.timezone` 标头在响应中指定事件开始和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="411f7-112">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="411f7-113">例如，下面的 `Prefer: outlook.timezone` 标头将响应中的开始和结束时间设置为东部标准时间。</span><span class="sxs-lookup"><span data-stu-id="411f7-113">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="411f7-p103">如果该事件是在不同的时区中创建的，则根据 `Prefer` 标头中指定的时区调整开始和结束时间。请查看此 [列表](../resources/datetimetimezone.md) 了解支持的时区名称。如果未指定 `Prefer: outlook.timezone` 标头，则返回用 UTC 表示的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="411f7-p103">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="411f7-117">可以使用**事件**资源中的 **OriginalStartTimeZone** 和 **OriginalEndTimeZone** 属性来查找创建事件时使用的时区。</span><span class="sxs-lookup"><span data-stu-id="411f7-117">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="411f7-118">权限</span><span class="sxs-lookup"><span data-stu-id="411f7-118">Permissions</span></span>
<span data-ttu-id="411f7-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="411f7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="411f7-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="411f7-121">Permission type</span></span>      | <span data-ttu-id="411f7-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="411f7-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="411f7-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="411f7-123">Delegated (work or school account)</span></span> | <span data-ttu-id="411f7-124">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="411f7-124">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="411f7-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="411f7-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="411f7-126">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="411f7-126">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="411f7-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="411f7-127">Application</span></span> | <span data-ttu-id="411f7-128">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="411f7-128">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="411f7-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="411f7-129">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="411f7-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="411f7-130">Optional query parameters</span></span>
<span data-ttu-id="411f7-131">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="411f7-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="411f7-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="411f7-132">Request headers</span></span>
| <span data-ttu-id="411f7-133">名称</span><span class="sxs-lookup"><span data-stu-id="411f7-133">Name</span></span>       | <span data-ttu-id="411f7-134">类型</span><span class="sxs-lookup"><span data-stu-id="411f7-134">Type</span></span> | <span data-ttu-id="411f7-135">说明</span><span class="sxs-lookup"><span data-stu-id="411f7-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="411f7-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="411f7-136">Authorization</span></span>  | <span data-ttu-id="411f7-137">string</span><span class="sxs-lookup"><span data-stu-id="411f7-137">string</span></span>  | <span data-ttu-id="411f7-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="411f7-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="411f7-140">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="411f7-140">Prefer: outlook.timezone</span></span> | <span data-ttu-id="411f7-141">string</span><span class="sxs-lookup"><span data-stu-id="411f7-141">string</span></span> | <span data-ttu-id="411f7-142">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="411f7-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="411f7-143">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="411f7-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="411f7-144">可选。</span><span class="sxs-lookup"><span data-stu-id="411f7-144">Optional.</span></span> |
| <span data-ttu-id="411f7-145">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="411f7-145">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="411f7-146">string</span><span class="sxs-lookup"><span data-stu-id="411f7-146">string</span></span> | <span data-ttu-id="411f7-147">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="411f7-147">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="411f7-148">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="411f7-148">Values can be "text" or "html".</span></span> <span data-ttu-id="411f7-149">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="411f7-149">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="411f7-150">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="411f7-150">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="411f7-151">可选。</span><span class="sxs-lookup"><span data-stu-id="411f7-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="411f7-152">请求正文</span><span class="sxs-lookup"><span data-stu-id="411f7-152">Request body</span></span>
<span data-ttu-id="411f7-153">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="411f7-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="411f7-154">响应</span><span class="sxs-lookup"><span data-stu-id="411f7-154">Response</span></span>

<span data-ttu-id="411f7-155">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="411f7-155">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="411f7-156">示例</span><span class="sxs-lookup"><span data-stu-id="411f7-156">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="411f7-157">请求 1</span><span class="sxs-lookup"><span data-stu-id="411f7-157">Request 1</span></span>
<span data-ttu-id="411f7-158">第一个示例获取用户的所有事件。</span><span class="sxs-lookup"><span data-stu-id="411f7-158">The first example gets all the user's events.</span></span> <span data-ttu-id="411f7-159">它指定以下内容：</span><span class="sxs-lookup"><span data-stu-id="411f7-159">It specifies the following:</span></span>

- <span data-ttu-id="411f7-160">获取以太平洋标准时间格式返回的日期时间值的 `Prefer: outlook.timezone` 标头。</span><span class="sxs-lookup"><span data-stu-id="411f7-160">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="411f7-p109">返回特定属性的 `$select` 查询参数。如果没有 `$select` 参数，将返回所有事件属性。</span><span class="sxs-lookup"><span data-stu-id="411f7-p109">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<span data-ttu-id="411f7-163">该请求未指定任何 `Prefer: outlook.body-content-type` 标头来指示返回的事件正文的特定格式。</span><span class="sxs-lookup"><span data-stu-id="411f7-163">The request does not specify any `Prefer: outlook.body-content-type` header to indicate a specific format for the returned event body.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="411f7-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="411f7-164">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/beta/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="411f7-165">C#</span><span class="sxs-lookup"><span data-stu-id="411f7-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="411f7-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="411f7-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="411f7-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="411f7-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="411f7-168">Java</span><span class="sxs-lookup"><span data-stu-id="411f7-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="411f7-169">响应 1</span><span class="sxs-lookup"><span data-stu-id="411f7-169">Response 1</span></span>
<span data-ttu-id="411f7-170">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="411f7-170">Here is an example of the response.</span></span> <span data-ttu-id="411f7-171">由于未指定任何 `Prefer: outlook.body-content-type` 标头，将以默认 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="411f7-171">Because no `Prefer: outlook.body-content-type` header was specified, the **body** property is returned in the default HTML format.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="411f7-172">请求 2</span><span class="sxs-lookup"><span data-stu-id="411f7-172">Request 2</span></span>
<span data-ttu-id="411f7-173">第二个示例介绍如何使用 `Prefer: outlook.body-content-type="text"` 标头获取采用文本格式的指定消息的 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="411f7-173">The second example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified message in text format.</span></span>

<span data-ttu-id="411f7-174">该请求还使用 `$select` 查询参数返回特定属性。</span><span class="sxs-lookup"><span data-stu-id="411f7-174">The request also uses a `$select` query parameter to return specific properties.</span></span> <span data-ttu-id="411f7-175">如果没有 `$select` 参数，将返回所有事件属性。</span><span class="sxs-lookup"><span data-stu-id="411f7-175">Without a `$select` parameter, all of the event properties will be returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="411f7-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="411f7-176">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_events_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/events?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text" 
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="411f7-177">C#</span><span class="sxs-lookup"><span data-stu-id="411f7-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-events-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="411f7-178">Javascript</span><span class="sxs-lookup"><span data-stu-id="411f7-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-events-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="411f7-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="411f7-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-events-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="411f7-180">Java</span><span class="sxs-lookup"><span data-stu-id="411f7-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-events-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="411f7-181">响应 2</span><span class="sxs-lookup"><span data-stu-id="411f7-181">Response 2</span></span>
<span data-ttu-id="411f7-182">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="411f7-182">Here is an example of the response.</span></span> <span data-ttu-id="411f7-183">以文本格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="411f7-183">The **body** property is returned in text format.</span></span> 

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
  ]
}
-->
