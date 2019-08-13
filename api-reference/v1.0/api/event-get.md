---
title: 获取事件
description: 获取指定的 event 对象的属性和关系。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8c693498a2e6742b46276fdae9bfdd8ec4abaa9f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372039"
---
# <a name="get-event"></a><span data-ttu-id="f7af3-103">获取事件</span><span class="sxs-lookup"><span data-stu-id="f7af3-103">Get event</span></span>

<span data-ttu-id="f7af3-104">获取指定的 [event](../resources/event.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f7af3-104">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="f7af3-105">目前，此操作返回纯 HTML 格式的事件正文。</span><span class="sxs-lookup"><span data-stu-id="f7af3-105">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="f7af3-106">在下列两种情况下，应用程序可获取其他用户的日历中的事件：</span><span class="sxs-lookup"><span data-stu-id="f7af3-106">There are two scenarios where an app can get an event in another user's calendar:</span></span>

* <span data-ttu-id="f7af3-107">如果该应用具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="f7af3-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="f7af3-108">如果应用程序具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了日历，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="f7af3-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="f7af3-109">请参阅[详细信息和示例](/graph/outlook-get-shared-events-calendars)。</span><span class="sxs-lookup"><span data-stu-id="f7af3-109">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

<span data-ttu-id="f7af3-110">由于 **event** 资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取**事件**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="f7af3-110">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="f7af3-111">支持不同时区</span><span class="sxs-lookup"><span data-stu-id="f7af3-111">Support various time zones</span></span>

<span data-ttu-id="f7af3-112">对于返回事件的所有 GET 操作，你可以使用 `Prefer: outlook.timezone` 标头在响应中指定事件开始和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="f7af3-112">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="f7af3-113">例如，下面的 `Prefer: outlook.timezone` 标头将响应中的开始和结束时间设置为东部标准时间。</span><span class="sxs-lookup"><span data-stu-id="f7af3-113">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="f7af3-p102">如果该事件是在不同的时区中创建的，则根据 `Prefer` 标头中指定的时区调整开始和结束时间。请查看此 [列表](../resources/datetimetimezone.md) 了解支持的时区名称。如果未指定 `Prefer: outlook.timezone` 标头，则返回用 UTC 表示的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="f7af3-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="f7af3-117">可以使用**事件**资源中的 **OriginalStartTimeZone** 和 **OriginalEndTimeZone** 属性来查找创建事件时使用的时区。</span><span class="sxs-lookup"><span data-stu-id="f7af3-117">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>


## <a name="permissions"></a><span data-ttu-id="f7af3-118">权限</span><span class="sxs-lookup"><span data-stu-id="f7af3-118">Permissions</span></span>
<span data-ttu-id="f7af3-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7af3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7af3-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7af3-121">Permission type</span></span>      | <span data-ttu-id="f7af3-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7af3-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7af3-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7af3-123">Delegated (work or school account)</span></span> | <span data-ttu-id="f7af3-124">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f7af3-124">Calendars.Read</span></span>    |
|<span data-ttu-id="f7af3-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7af3-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7af3-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f7af3-126">Calendars.Read</span></span>    |
|<span data-ttu-id="f7af3-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7af3-127">Application</span></span> | <span data-ttu-id="f7af3-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f7af3-128">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7af3-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7af3-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}
GET /users/{id | userPrincipalName}/events/{id}
GET /groups/{id}/events/{id}

GET /me/calendar/events/{id}
GET /users/{id | userPrincipalName}/calendar/events/{id}
GET /groups/{id}/calendar/events/{id}

GET /me/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}

GET /me/calendargroup/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f7af3-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f7af3-130">Optional query parameters</span></span>
<span data-ttu-id="f7af3-131">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f7af3-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f7af3-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7af3-132">Request headers</span></span>
| <span data-ttu-id="f7af3-133">名称</span><span class="sxs-lookup"><span data-stu-id="f7af3-133">Name</span></span>       | <span data-ttu-id="f7af3-134">类型</span><span class="sxs-lookup"><span data-stu-id="f7af3-134">Type</span></span> | <span data-ttu-id="f7af3-135">说明</span><span class="sxs-lookup"><span data-stu-id="f7af3-135">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="f7af3-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7af3-136">Authorization</span></span>  | <span data-ttu-id="f7af3-137">string</span><span class="sxs-lookup"><span data-stu-id="f7af3-137">string</span></span> | <span data-ttu-id="f7af3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7af3-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f7af3-140">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="f7af3-140">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="f7af3-141">string</span><span class="sxs-lookup"><span data-stu-id="f7af3-141">string</span></span> | <span data-ttu-id="f7af3-142">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="f7af3-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="f7af3-143">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="f7af3-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="f7af3-144">可选。</span><span class="sxs-lookup"><span data-stu-id="f7af3-144">Optional.</span></span> |
| <span data-ttu-id="f7af3-145">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="f7af3-145">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="f7af3-146">string</span><span class="sxs-lookup"><span data-stu-id="f7af3-146">string</span></span> | <span data-ttu-id="f7af3-147">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="f7af3-147">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="f7af3-148">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="f7af3-148">Values can be "text" or "html".</span></span> <span data-ttu-id="f7af3-149">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="f7af3-149">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="f7af3-150">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="f7af3-150">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="f7af3-151">可选。</span><span class="sxs-lookup"><span data-stu-id="f7af3-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7af3-152">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7af3-152">Request body</span></span>
<span data-ttu-id="f7af3-153">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f7af3-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7af3-154">响应</span><span class="sxs-lookup"><span data-stu-id="f7af3-154">Response</span></span>

<span data-ttu-id="f7af3-155">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f7af3-155">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f7af3-156">示例</span><span class="sxs-lookup"><span data-stu-id="f7af3-156">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="f7af3-157">请求 1</span><span class="sxs-lookup"><span data-stu-id="f7af3-157">Request 1</span></span>
<span data-ttu-id="f7af3-p107">第一个示例获取指定的事件。它指定以下内容：</span><span class="sxs-lookup"><span data-stu-id="f7af3-p107">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="f7af3-160">获取以太平洋标准时间格式返回的日期时间值的 `Prefer: outlook.timezone` 标头。</span><span class="sxs-lookup"><span data-stu-id="f7af3-160">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="f7af3-p108">返回特定属性的 `$select` 查询参数。如果没有 `$select` 参数，将返回所有事件属性。</span><span class="sxs-lookup"><span data-stu-id="f7af3-p108">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f7af3-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7af3-163">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGIAAAoZDOFAAA="],
  "name": "get_event"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/events/AAMkAGIAAAoZDOFAAA=?$select=subject,body,bodyPreview,organizer,attendees,start,end,location 
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f7af3-164">C#</span><span class="sxs-lookup"><span data-stu-id="f7af3-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7af3-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7af3-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f7af3-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7af3-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f7af3-167">Java</span><span class="sxs-lookup"><span data-stu-id="f7af3-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="f7af3-168">响应 1</span><span class="sxs-lookup"><span data-stu-id="f7af3-168">Response 1</span></span>

<span data-ttu-id="f7af3-p109">下面是一个响应示例。以 HTML 默认格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="f7af3-p109">Here is an example of the response. The **body** property is returned in the default format of HTML.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-length: 1928

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)/$entity",
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
```


##### <a name="request-2"></a><span data-ttu-id="f7af3-171">请求 2</span><span class="sxs-lookup"><span data-stu-id="f7af3-171">Request 2</span></span>

<span data-ttu-id="f7af3-172">第二个示例显示获取指定多个地点的事件。</span><span class="sxs-lookup"><span data-stu-id="f7af3-172">The second example shows getting an event that specifies more than one location.</span></span> <span data-ttu-id="f7af3-173">该请求指定返回特定属性的 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="f7af3-173">The request specifies a `$select` query parameter to return specific properties.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="f7af3-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7af3-174">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADAGAADDdm4NAAA="],
  "name": "get_event_multiple_locations"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/AAMkADAGAADDdm4NAAA=?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f7af3-175">C#</span><span class="sxs-lookup"><span data-stu-id="f7af3-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-multiple-locations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7af3-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7af3-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-multiple-locations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f7af3-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7af3-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-multiple-locations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f7af3-178">Java</span><span class="sxs-lookup"><span data-stu-id="f7af3-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-multiple-locations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="f7af3-179">响应 2</span><span class="sxs-lookup"><span data-stu-id="f7af3-179">Response 2</span></span>
<span data-ttu-id="f7af3-180">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f7af3-180">Here is an example of the response.</span></span> <span data-ttu-id="f7af3-181">**locations** 属性包括组织事件的 3 个地点的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f7af3-181">The **locations** property includes details for the 3 locations that the event is organized for.</span></span> 

<span data-ttu-id="f7af3-182">由于该请求未指定任何 `Prefer: outlook.timezone` 标头，**start** 和 **end** 属性将以默认的 UTC 时区显示。</span><span class="sxs-lookup"><span data-stu-id="f7af3-182">Because the request does not specify any `Prefer: outlook.timezone` header, the **start** and **end** properties are displayed in the default UTC time zone.</span></span> 

<span data-ttu-id="f7af3-183">事件正文采用的是默认的 HTML 格式。</span><span class="sxs-lookup"><span data-stu-id="f7af3-183">The event body is in the default HTML format.</span></span>  

<!-- {
  "blockType": "response",
  "name": "get_event_multiple_locations",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1992

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,locations)/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "subject":"Plan summer company picnic",
  "bodyPreview":"Let's kick-start this event planning!",
  "body":{
    "contentType":"html",
    "content":"<html>\r\n<head>\r\n</head>\r\n<body>\r\nLet's kick-start this event planning!\r\n</body>\r\n</html>\r\n"
  },
  "start":{
    "dateTime":"2017-08-30T11:00:00.0000000",
    "timeZone":"UTC"
  },
  "end":{
    "dateTime":"2017-08-30T12:00:00.0000000",
    "timeZone":"UTC"
  },
  "location":{
    "displayName":"Conf Room 3; Fourth Coffee; Home Office",
    "locationType":"default",
    "uniqueId":"Conf Room 3; Fourth Coffee; Home Office",
    "uniqueIdType":"private"
  },
  "locations":[
    {
      "displayName":"Conf Room 3",
      "locationType":"default",
      "uniqueIdType":"unknown"
    },
    {
      "displayName":"Fourth Coffee",
      "locationType":"default",
      "uniqueId":"Fourth Coffee",
      "uniqueIdType":"private",
      "address":{
        "street":"4567 Main St",
        "city":"Redmond",
        "state":"WA",
        "countryOrRegion":"US",
        "postalCode":"32008"
      },
      "coordinates":{
        "latitude":47.672,
        "longitude":-102.103
      }
    },
    {
      "displayName":"Home Office",
      "locationType":"default",
      "uniqueIdType":"unknown"
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
        "name":"Dana Swope",
        "address":"DanaS@contoso.onmicrosoft.com"
      }
    },
    {
      "type":"required",
      "status":{
        "response":"none",
        "time":"0001-01-01T00:00:00Z"
      },
      "emailAddress":{
        "name":"Alex Wilber",
        "address":"AlexW@contoso.onmicrosoft.com"
      }
    }
  ],
  "organizer":{
    "emailAddress":{
      "name":"Adele Vance",
      "address":"AdeleV@contoso.onmicrosoft.com"
    }
  }
}
```



## <a name="see-also"></a><span data-ttu-id="f7af3-184">另请参阅</span><span class="sxs-lookup"><span data-stu-id="f7af3-184">See also</span></span>

- [<span data-ttu-id="f7af3-185">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="f7af3-185">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f7af3-186">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="f7af3-186">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="f7af3-187">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="f7af3-187">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
