---
title: 获取事件
description: 获取指定的 event 对象的属性和关系。
author: harini84
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e3cfbeba9940c6c7fe69aeb271ff7847dce7749b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448310"
---
# <a name="get-event"></a><span data-ttu-id="de0d5-103">获取事件</span><span class="sxs-lookup"><span data-stu-id="de0d5-103">Get event</span></span>

<span data-ttu-id="de0d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de0d5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de0d5-105">获取指定的 [event](../resources/event.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="de0d5-105">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="de0d5-106">目前，此操作返回纯 HTML 格式的事件正文。</span><span class="sxs-lookup"><span data-stu-id="de0d5-106">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="de0d5-107">在下列两种情况下，应用程序可获取其他用户的日历中的事件：</span><span class="sxs-lookup"><span data-stu-id="de0d5-107">There are two scenarios where an app can get an event in another user's calendar:</span></span>

* <span data-ttu-id="de0d5-108">如果该应用具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="de0d5-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="de0d5-109">如果应用程序具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了日历，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="de0d5-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="de0d5-110">请参阅[详细信息和示例](/graph/outlook-get-shared-events-calendars)。</span><span class="sxs-lookup"><span data-stu-id="de0d5-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

<span data-ttu-id="de0d5-111">由于 **event** 资源支持 [扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取 **事件** 实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="de0d5-111">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="de0d5-112">支持不同时区</span><span class="sxs-lookup"><span data-stu-id="de0d5-112">Support various time zones</span></span>

<span data-ttu-id="de0d5-113">对于返回事件的所有 GET 操作，你可以使用 `Prefer: outlook.timezone` 标头在响应中指定事件开始和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="de0d5-113">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="de0d5-114">例如，下面的 `Prefer: outlook.timezone` 标头将响应中的开始和结束时间设置为东部标准时间。</span><span class="sxs-lookup"><span data-stu-id="de0d5-114">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="de0d5-p102">如果该事件是在不同的时区中创建的，则根据 `Prefer` 标头中指定的时区调整开始和结束时间。请查看此 [列表](../resources/datetimetimezone.md) 了解支持的时区名称。如果未指定 `Prefer: outlook.timezone` 标头，则返回用 UTC 表示的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="de0d5-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="de0d5-118">可以使用 **事件** 资源中的 **OriginalStartTimeZone** 和 **OriginalEndTimeZone** 属性来查找创建事件时使用的时区。</span><span class="sxs-lookup"><span data-stu-id="de0d5-118">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>


## <a name="permissions"></a><span data-ttu-id="de0d5-119">权限</span><span class="sxs-lookup"><span data-stu-id="de0d5-119">Permissions</span></span>
<span data-ttu-id="de0d5-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de0d5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de0d5-122">权限类型</span><span class="sxs-lookup"><span data-stu-id="de0d5-122">Permission type</span></span>      | <span data-ttu-id="de0d5-123">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="de0d5-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de0d5-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de0d5-124">Delegated (work or school account)</span></span> | <span data-ttu-id="de0d5-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="de0d5-125">Calendars.Read</span></span>    |
|<span data-ttu-id="de0d5-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de0d5-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de0d5-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="de0d5-127">Calendars.Read</span></span>    |
|<span data-ttu-id="de0d5-128">应用程序</span><span class="sxs-lookup"><span data-stu-id="de0d5-128">Application</span></span> | <span data-ttu-id="de0d5-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="de0d5-129">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="de0d5-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de0d5-130">HTTP request</span></span>
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

GET /me/calendargroups/{id}/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="de0d5-131">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="de0d5-131">Optional query parameters</span></span>
<span data-ttu-id="de0d5-132">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="de0d5-132">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="de0d5-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="de0d5-133">Request headers</span></span>
| <span data-ttu-id="de0d5-134">名称</span><span class="sxs-lookup"><span data-stu-id="de0d5-134">Name</span></span>       | <span data-ttu-id="de0d5-135">类型</span><span class="sxs-lookup"><span data-stu-id="de0d5-135">Type</span></span> | <span data-ttu-id="de0d5-136">说明</span><span class="sxs-lookup"><span data-stu-id="de0d5-136">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="de0d5-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="de0d5-137">Authorization</span></span>  | <span data-ttu-id="de0d5-138">string</span><span class="sxs-lookup"><span data-stu-id="de0d5-138">string</span></span> | <span data-ttu-id="de0d5-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="de0d5-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="de0d5-141">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="de0d5-141">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="de0d5-142">string</span><span class="sxs-lookup"><span data-stu-id="de0d5-142">string</span></span> | <span data-ttu-id="de0d5-143">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="de0d5-143">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="de0d5-144">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="de0d5-144">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="de0d5-145">可选。</span><span class="sxs-lookup"><span data-stu-id="de0d5-145">Optional.</span></span> |
| <span data-ttu-id="de0d5-146">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="de0d5-146">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="de0d5-147">string</span><span class="sxs-lookup"><span data-stu-id="de0d5-147">string</span></span> | <span data-ttu-id="de0d5-148">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="de0d5-148">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="de0d5-149">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="de0d5-149">Values can be "text" or "html".</span></span> <span data-ttu-id="de0d5-150">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="de0d5-150">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="de0d5-151">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="de0d5-151">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="de0d5-152">可选。</span><span class="sxs-lookup"><span data-stu-id="de0d5-152">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de0d5-153">请求正文</span><span class="sxs-lookup"><span data-stu-id="de0d5-153">Request body</span></span>
<span data-ttu-id="de0d5-154">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="de0d5-154">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de0d5-155">响应</span><span class="sxs-lookup"><span data-stu-id="de0d5-155">Response</span></span>

<span data-ttu-id="de0d5-156">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="de0d5-156">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="de0d5-157">示例</span><span class="sxs-lookup"><span data-stu-id="de0d5-157">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="de0d5-158">请求 1</span><span class="sxs-lookup"><span data-stu-id="de0d5-158">Request 1</span></span>
<span data-ttu-id="de0d5-p107">第一个示例获取指定的事件。它指定以下内容：</span><span class="sxs-lookup"><span data-stu-id="de0d5-p107">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="de0d5-161">获取以太平洋标准时间格式返回的日期时间值的 `Prefer: outlook.timezone` 标头。</span><span class="sxs-lookup"><span data-stu-id="de0d5-161">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="de0d5-p108">返回特定属性的 `$select` 查询参数。如果没有 `$select` 参数，将返回所有事件属性。</span><span class="sxs-lookup"><span data-stu-id="de0d5-p108">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>


# <a name="http"></a>[<span data-ttu-id="de0d5-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="de0d5-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGIAAAoZDOFAAA="],
  "name": "get_event"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/events/AAMkAGIAAAoZDOFAAA=?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees 
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="c"></a>[<span data-ttu-id="de0d5-165">C#</span><span class="sxs-lookup"><span data-stu-id="de0d5-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de0d5-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de0d5-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de0d5-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de0d5-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="de0d5-168">Java</span><span class="sxs-lookup"><span data-stu-id="de0d5-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="de0d5-169">响应 1</span><span class="sxs-lookup"><span data-stu-id="de0d5-169">Response 1</span></span>

<span data-ttu-id="de0d5-p109">下面是一个响应示例。以 HTML 默认格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="de0d5-p109">Here is an example of the response. The **body** property is returned in the default format of HTML.</span></span>

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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees)/$entity",
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
                "response":"tentativelyAccepted",
                "time":"0001-01-01T00:00:00Z"
            },
            "proposedNewTime": {
                "start": {
                    "dateTime": "2019-08-16T12:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-08-16T14:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            },
            "emailAddress":{
                "name":"Dana Swope",
                "address":"danas@a830edad905084922E17020313.onmicrosoft.com"
            }
        }
    ],
    "hideAttendees": false,
    "organizer":{
        "emailAddress":{
            "name":"Samantha Booth",
            "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
        }
    }
}
```


##### <a name="request-2"></a><span data-ttu-id="de0d5-172">请求 2</span><span class="sxs-lookup"><span data-stu-id="de0d5-172">Request 2</span></span>

<span data-ttu-id="de0d5-173">第二个示例显示获取指定多个地点的事件。</span><span class="sxs-lookup"><span data-stu-id="de0d5-173">The second example shows getting an event that specifies more than one location.</span></span> <span data-ttu-id="de0d5-174">该请求指定返回特定属性的 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="de0d5-174">The request specifies a `$select` query parameter to return specific properties.</span></span> 


# <a name="http"></a>[<span data-ttu-id="de0d5-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="de0d5-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADAGAADDdm4NAAA="],
  "name": "get_event_multiple_locations"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/events/AAMkADAGAADDdm4NAAA=?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
# <a name="c"></a>[<span data-ttu-id="de0d5-176">C#</span><span class="sxs-lookup"><span data-stu-id="de0d5-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-multiple-locations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de0d5-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de0d5-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-multiple-locations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de0d5-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de0d5-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-multiple-locations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="de0d5-179">Java</span><span class="sxs-lookup"><span data-stu-id="de0d5-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-multiple-locations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="de0d5-180">响应 2</span><span class="sxs-lookup"><span data-stu-id="de0d5-180">Response 2</span></span>
<span data-ttu-id="de0d5-181">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="de0d5-181">Here is an example of the response.</span></span> <span data-ttu-id="de0d5-182">**locations** 属性包括组织事件的 3 个地点的详细信息。</span><span class="sxs-lookup"><span data-stu-id="de0d5-182">The **locations** property includes details for the 3 locations that the event is organized for.</span></span> 

<span data-ttu-id="de0d5-183">由于该请求未指定任何 `Prefer: outlook.timezone` 标头，**start** 和 **end** 属性将以默认的 UTC 时区显示。</span><span class="sxs-lookup"><span data-stu-id="de0d5-183">Because the request does not specify any `Prefer: outlook.timezone` header, the **start** and **end** properties are displayed in the default UTC time zone.</span></span> 

<span data-ttu-id="de0d5-184">事件正文采用的是默认的 HTML 格式。</span><span class="sxs-lookup"><span data-stu-id="de0d5-184">The event body is in the default HTML format.</span></span>  

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



## <a name="see-also"></a><span data-ttu-id="de0d5-185">另请参阅</span><span class="sxs-lookup"><span data-stu-id="de0d5-185">See also</span></span>

- [<span data-ttu-id="de0d5-186">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="de0d5-186">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="de0d5-187">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="de0d5-187">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="de0d5-188">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="de0d5-188">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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
