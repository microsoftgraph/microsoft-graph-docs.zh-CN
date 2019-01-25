---
title: 获取事件
description: 获取指定的 event 对象的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 49a4e16e6f24ebac22c760cf11e63c220181d0b9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509082"
---
# <a name="get-event"></a><span data-ttu-id="82f7e-103">获取事件</span><span class="sxs-lookup"><span data-stu-id="82f7e-103">Get event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82f7e-104">获取指定的 [event](../resources/event.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="82f7e-104">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="82f7e-105">有两种方案，其中应用程序可在另一个用户的日历中获取事件：</span><span class="sxs-lookup"><span data-stu-id="82f7e-105">There are two scenarios where an app can get an event in another user's calendar:</span></span>

* <span data-ttu-id="82f7e-106">如果应用程序具有应用程序权限，或，</span><span class="sxs-lookup"><span data-stu-id="82f7e-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="82f7e-107">如果应用程序具有相应从一个用户委派[权限](#permissions)，并另一个用户具有与该用户，共享日历，或具有委派的访问赋予该用户。</span><span class="sxs-lookup"><span data-stu-id="82f7e-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="82f7e-108">请参阅[详细信息和示例](/graph/outlook-get-shared-events-calendars)。</span><span class="sxs-lookup"><span data-stu-id="82f7e-108">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

<span data-ttu-id="82f7e-109">由于**事件**资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取**事件**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="82f7e-109">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="82f7e-110">支持不同时区</span><span class="sxs-lookup"><span data-stu-id="82f7e-110">Support various time zones</span></span>

<span data-ttu-id="82f7e-111">对于返回事件的所有 GET 操作，你可以使用 `Prefer: outlook.timezone` 标头在响应中指定事件开始和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="82f7e-111">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="82f7e-112">例如，下面的 `Prefer: outlook.timezone` 标头将响应中的开始和结束时间设置为东部标准时间。</span><span class="sxs-lookup"><span data-stu-id="82f7e-112">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="82f7e-p102">如果该事件是在不同的时区中创建的，则根据 `Prefer` 标头中指定的时区调整开始和结束时间。请查看此 [列表](../resources/datetimetimezone.md) 了解支持的时区名称。如果未指定 `Prefer: outlook.timezone` 标头，则返回用 UTC 表示的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="82f7e-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="82f7e-116">可以使用**事件**资源中的 **OriginalStartTimeZone** 和 **OriginalEndTimeZone** 属性来查找创建事件时使用的时区。</span><span class="sxs-lookup"><span data-stu-id="82f7e-116">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="82f7e-117">权限</span><span class="sxs-lookup"><span data-stu-id="82f7e-117">Permissions</span></span>
<span data-ttu-id="82f7e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82f7e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82f7e-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="82f7e-120">Permission type</span></span>      | <span data-ttu-id="82f7e-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82f7e-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82f7e-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82f7e-122">Delegated (work or school account)</span></span> | <span data-ttu-id="82f7e-123">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="82f7e-123">Calendars.Read</span></span>    |
|<span data-ttu-id="82f7e-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82f7e-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82f7e-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="82f7e-125">Calendars.Read</span></span>    |
|<span data-ttu-id="82f7e-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="82f7e-126">Application</span></span> | <span data-ttu-id="82f7e-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="82f7e-127">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="82f7e-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82f7e-128">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="82f7e-129">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="82f7e-129">Optional query parameters</span></span>
<span data-ttu-id="82f7e-130">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="82f7e-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="82f7e-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="82f7e-131">Request headers</span></span>
| <span data-ttu-id="82f7e-132">名称</span><span class="sxs-lookup"><span data-stu-id="82f7e-132">Name</span></span>       | <span data-ttu-id="82f7e-133">类型</span><span class="sxs-lookup"><span data-stu-id="82f7e-133">Type</span></span> | <span data-ttu-id="82f7e-134">说明</span><span class="sxs-lookup"><span data-stu-id="82f7e-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="82f7e-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="82f7e-135">Authorization</span></span>  | <span data-ttu-id="82f7e-136">string</span><span class="sxs-lookup"><span data-stu-id="82f7e-136">string</span></span>  | <span data-ttu-id="82f7e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="82f7e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="82f7e-139">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="82f7e-139">Prefer: outlook.timezone</span></span> | <span data-ttu-id="82f7e-140">string</span><span class="sxs-lookup"><span data-stu-id="82f7e-140">string</span></span> | <span data-ttu-id="82f7e-141">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="82f7e-141">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="82f7e-142">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="82f7e-142">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="82f7e-143">可选。</span><span class="sxs-lookup"><span data-stu-id="82f7e-143">Optional.</span></span> |
| <span data-ttu-id="82f7e-144">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="82f7e-144">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="82f7e-145">string</span><span class="sxs-lookup"><span data-stu-id="82f7e-145">string</span></span> | <span data-ttu-id="82f7e-146">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="82f7e-146">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="82f7e-147">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="82f7e-147">Values can be "text" or "html".</span></span> <span data-ttu-id="82f7e-148">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="82f7e-148">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="82f7e-149">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="82f7e-149">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="82f7e-150">可选。</span><span class="sxs-lookup"><span data-stu-id="82f7e-150">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82f7e-151">请求正文</span><span class="sxs-lookup"><span data-stu-id="82f7e-151">Request body</span></span>
<span data-ttu-id="82f7e-152">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="82f7e-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82f7e-153">响应</span><span class="sxs-lookup"><span data-stu-id="82f7e-153">Response</span></span>

<span data-ttu-id="82f7e-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="82f7e-154">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="82f7e-155">示例</span><span class="sxs-lookup"><span data-stu-id="82f7e-155">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="82f7e-156">请求 1</span><span class="sxs-lookup"><span data-stu-id="82f7e-156">Request 1</span></span>
<span data-ttu-id="82f7e-p107">第一个示例获取指定的事件。它指定以下内容：</span><span class="sxs-lookup"><span data-stu-id="82f7e-p107">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="82f7e-159">获取以太平洋标准时间格式返回的日期时间值的 `Prefer: outlook.timezone` 标头。</span><span class="sxs-lookup"><span data-stu-id="82f7e-159">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="82f7e-p108">返回特定属性的 `$select` 查询参数。如果没有 `$select` 参数，将返回所有事件属性。</span><span class="sxs-lookup"><span data-stu-id="82f7e-p108">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<span data-ttu-id="82f7e-162">请求不指定任何`Prefer: outlook.body-content-type`标头以指示返回的事件正文的特定格式。</span><span class="sxs-lookup"><span data-stu-id="82f7e-162">The request does not specify any `Prefer: outlook.body-content-type` header to indicate a specific format for the returned event body.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_event"
}-->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGIAAAoZDOFAAA=')?$select=subject,body,bodyPreview,organizer,attendees,start,end,location 
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response-1"></a><span data-ttu-id="82f7e-163">响应 1</span><span class="sxs-lookup"><span data-stu-id="82f7e-163">Response 1</span></span>
<span data-ttu-id="82f7e-164">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="82f7e-164">Here is an example of the response.</span></span> <span data-ttu-id="82f7e-165">因为没有`Prefer: outlook.body-content-type`指定标头，以默认的 HTML 格式返回**body**属性。</span><span class="sxs-lookup"><span data-stu-id="82f7e-165">Because no `Prefer: outlook.body-content-type` header was specified, the **body** property is returned in the default HTML format.</span></span> 

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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)/$entity",
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

##### <a name="request-2"></a><span data-ttu-id="82f7e-166">请求 2</span><span class="sxs-lookup"><span data-stu-id="82f7e-166">Request 2</span></span>
<span data-ttu-id="82f7e-167">第二个示例演示如何使用`Prefer: outlook.body-content-type="text"`标头以文本格式获取指定的事件的**body**属性。</span><span class="sxs-lookup"><span data-stu-id="82f7e-167">The second example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified event in text format.</span></span>

<span data-ttu-id="82f7e-168">请求还使用`$select`查询参数返回特定属性。</span><span class="sxs-lookup"><span data-stu-id="82f7e-168">The request also uses a `$select` query parameter to return specific properties.</span></span> <span data-ttu-id="82f7e-169">不带`$select`参数的所有事件属性将返回。</span><span class="sxs-lookup"><span data-stu-id="82f7e-169">Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_event_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGI1AAAoZDOFAAA=')?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text"
```
##### <a name="response-2"></a><span data-ttu-id="82f7e-170">响应 2</span><span class="sxs-lookup"><span data-stu-id="82f7e-170">Response 2</span></span>
<span data-ttu-id="82f7e-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="82f7e-171">Here is an example of the response.</span></span> <span data-ttu-id="82f7e-172">**Body**属性返回文本格式。</span><span class="sxs-lookup"><span data-stu-id="82f7e-172">The **body** property is returned in text format.</span></span> 

<!-- {
  "blockType": "response",
  "name": "get_event_in_text",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"
Content-length: 636

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview)/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
    "id":"AAMkAGI1AAAoZDOFAAA=",
    "subject":"Orientation ",
    "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
    "body":{
        "contentType":"text",
        "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
    }
}
```


##### <a name="request-3"></a><span data-ttu-id="82f7e-173">请求 3</span><span class="sxs-lookup"><span data-stu-id="82f7e-173">Request 3</span></span>

<span data-ttu-id="82f7e-174">第三个示例演示如何获取指定多个位置的事件</span><span class="sxs-lookup"><span data-stu-id="82f7e-174">The third example shows getting an event that specifies more than one location.</span></span> <span data-ttu-id="82f7e-175">该请求指定返回特定属性的 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="82f7e-175">The request specifies a `$select` query parameter to return specific properties.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_event_multiple_locations"
}-->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkADAGAADDdm4NAAA=')?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
##### <a name="response-3"></a><span data-ttu-id="82f7e-176">响应 3</span><span class="sxs-lookup"><span data-stu-id="82f7e-176">Response 3</span></span>
<span data-ttu-id="82f7e-177">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="82f7e-177">Here is an example of the response.</span></span> <span data-ttu-id="82f7e-178">**locations** 属性包括组织事件的 3 个地点的详细信息。</span><span class="sxs-lookup"><span data-stu-id="82f7e-178">The **locations** property includes details for the 3 locations that the event is organized for.</span></span> 

<span data-ttu-id="82f7e-179">由于该请求未指定任何`Prefer: outlook.timezone`或`Prefer: outlook.body-content-type`中默认 UTC 时区，显示标头、**开始**和**结束**属性和正文采用默认的 HTML 格式。</span><span class="sxs-lookup"><span data-stu-id="82f7e-179">Because the request does not specify any `Prefer: outlook.timezone` or `Prefer: outlook.body-content-type` header, the **start** and **end** properties are displayed in the default UTC time zone, and the body is in the default HTML format.</span></span>  

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,locations)/$entity",
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
        "type":"unknown",
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

## <a name="see-also"></a><span data-ttu-id="82f7e-180">另请参阅</span><span class="sxs-lookup"><span data-stu-id="82f7e-180">See also</span></span>

- [<span data-ttu-id="82f7e-181">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="82f7e-181">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="82f7e-182">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="82f7e-182">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="82f7e-183">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="82f7e-183">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
