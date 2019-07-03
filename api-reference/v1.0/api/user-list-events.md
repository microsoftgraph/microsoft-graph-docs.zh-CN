---
title: 列出事件
description: '获取用户邮箱中的 event 对象列表。 该列表中包含单个 '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1364e62084aaa45a9c75f4c1c46c80342de2389d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460355"
---
# <a name="list-events"></a><span data-ttu-id="ac086-104">列出事件</span><span class="sxs-lookup"><span data-stu-id="ac086-104">List events</span></span>

<span data-ttu-id="ac086-p102">获取用户邮箱中的 [event](../resources/event.md) 对象列表。该列表包含单个实例会议和系列主控形状。</span><span class="sxs-lookup"><span data-stu-id="ac086-p102">Get a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="ac086-107">要获取扩展的事件实例，可以[获取日历视图](calendar-list-calendarview.md)，或者[获取事件的实例](event-list-instances.md)。</span><span class="sxs-lookup"><span data-stu-id="ac086-107">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

<span data-ttu-id="ac086-108">目前，此操作仅返回 HTML 格式的事件正文。</span><span class="sxs-lookup"><span data-stu-id="ac086-108">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="ac086-109">在以下两种情况下，应用程序可以获取其他用户的日历中的事件：</span><span class="sxs-lookup"><span data-stu-id="ac086-109">There are two scenarios where an app can get events in another user's calendar:</span></span>

* <span data-ttu-id="ac086-110">如果该应用程序具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="ac086-110">If the app has application permissions, or,</span></span>
* <span data-ttu-id="ac086-111">如果应用程序具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了日历，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="ac086-111">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="ac086-112">请参阅[详细信息和示例](/graph/outlook-get-shared-events-calendars)。</span><span class="sxs-lookup"><span data-stu-id="ac086-112">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

### <a name="support-various-time-zones"></a><span data-ttu-id="ac086-113">支持不同时区</span><span class="sxs-lookup"><span data-stu-id="ac086-113">Support various time zones</span></span>

<span data-ttu-id="ac086-114">对于返回事件的所有 GET 操作，你可以使用 `Prefer: outlook.timezone` 标头在响应中指定事件开始和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="ac086-114">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="ac086-115">例如，下面的 `Prefer: outlook.timezone` 标头将响应中的开始和结束时间设置为东部标准时间。</span><span class="sxs-lookup"><span data-stu-id="ac086-115">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="ac086-p104">如果该事件是在不同的时区中创建的，则根据 `Prefer` 标头中指定的时区调整开始和结束时间。请查看此 [列表](../resources/datetimetimezone.md) 了解支持的时区名称。如果未指定 `Prefer: outlook.timezone` 标头，则返回用 UTC 表示的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="ac086-p104">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="ac086-119">可以使用**事件**资源中的 **OriginalStartTimeZone** 和 **OriginalEndTimeZone** 属性来查找创建事件时使用的时区。</span><span class="sxs-lookup"><span data-stu-id="ac086-119">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac086-120">权限</span><span class="sxs-lookup"><span data-stu-id="ac086-120">Permissions</span></span>
<span data-ttu-id="ac086-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac086-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac086-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac086-123">Permission type</span></span>      | <span data-ttu-id="ac086-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac086-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac086-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac086-125">Delegated (work or school account)</span></span> | <span data-ttu-id="ac086-126">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac086-126">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ac086-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac086-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac086-128">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac086-128">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ac086-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac086-129">Application</span></span> | <span data-ttu-id="ac086-130">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac086-130">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac086-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac086-131">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="ac086-132">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ac086-132">Optional query parameters</span></span>
<span data-ttu-id="ac086-133">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ac086-133">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ac086-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac086-134">Request headers</span></span>
| <span data-ttu-id="ac086-135">名称</span><span class="sxs-lookup"><span data-stu-id="ac086-135">Name</span></span>       | <span data-ttu-id="ac086-136">类型</span><span class="sxs-lookup"><span data-stu-id="ac086-136">Type</span></span> | <span data-ttu-id="ac086-137">说明</span><span class="sxs-lookup"><span data-stu-id="ac086-137">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="ac086-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac086-138">Authorization</span></span>  | <span data-ttu-id="ac086-139">string</span><span class="sxs-lookup"><span data-stu-id="ac086-139">string</span></span> | <span data-ttu-id="ac086-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ac086-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ac086-142">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="ac086-142">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="ac086-143">string</span><span class="sxs-lookup"><span data-stu-id="ac086-143">string</span></span> | <span data-ttu-id="ac086-144">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="ac086-144">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="ac086-145">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ac086-145">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="ac086-146">可选。</span><span class="sxs-lookup"><span data-stu-id="ac086-146">Optional.</span></span> |
| <span data-ttu-id="ac086-147">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="ac086-147">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="ac086-148">string</span><span class="sxs-lookup"><span data-stu-id="ac086-148">string</span></span> | <span data-ttu-id="ac086-149">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="ac086-149">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="ac086-150">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="ac086-150">Values can be "text" or "html".</span></span> <span data-ttu-id="ac086-151">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="ac086-151">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="ac086-152">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="ac086-152">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="ac086-153">可选。</span><span class="sxs-lookup"><span data-stu-id="ac086-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac086-154">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac086-154">Request body</span></span>
<span data-ttu-id="ac086-155">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ac086-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac086-156">响应</span><span class="sxs-lookup"><span data-stu-id="ac086-156">Response</span></span>

<span data-ttu-id="ac086-157">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ac086-157">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ac086-158">示例</span><span class="sxs-lookup"><span data-stu-id="ac086-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ac086-159">请求</span><span class="sxs-lookup"><span data-stu-id="ac086-159">Request</span></span>
<span data-ttu-id="ac086-p109">下面是一个请求示例。它指定以下内容：</span><span class="sxs-lookup"><span data-stu-id="ac086-p109">Here is an example of the request. It specifies the following:</span></span>

- <span data-ttu-id="ac086-162">获取以太平洋标准时间格式返回的日期时间值的 `Prefer: outlook.timezone` 标头。</span><span class="sxs-lookup"><span data-stu-id="ac086-162">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="ac086-p110">返回特定属性的 `$select` 查询参数。如果没有 `$select` 参数，将返回所有事件属性。</span><span class="sxs-lookup"><span data-stu-id="ac086-p110">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ac086-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac086-165">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ac086-166">C#</span><span class="sxs-lookup"><span data-stu-id="ac086-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ac086-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="ac086-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ac086-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac086-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ac086-169">响应</span><span class="sxs-lookup"><span data-stu-id="ac086-169">Response</span></span>
<span data-ttu-id="ac086-p111">下面是一个响应示例。以默认的 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="ac086-p111">Here is an example of the response. The **body** property is returned in the default HTML format.</span></span>
<!-- {
  "blockType": "response",
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
