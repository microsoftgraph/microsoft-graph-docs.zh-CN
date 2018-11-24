# <a name="get-event"></a><span data-ttu-id="97621-101">获取事件</span><span class="sxs-lookup"><span data-stu-id="97621-101">Get event</span></span>

<span data-ttu-id="97621-102">获取指定的 [event](../resources/event.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="97621-102">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="97621-103">目前，此操作返回纯 HTML 格式的事件正文。</span><span class="sxs-lookup"><span data-stu-id="97621-103">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="97621-104">有两种方案，其中应用程序可在另一个用户的日历中获取事件：</span><span class="sxs-lookup"><span data-stu-id="97621-104">There are two scenarios where an app can get an event in another user's calendar:</span></span>

* <span data-ttu-id="97621-105">如果应用程序具有应用程序权限，或，</span><span class="sxs-lookup"><span data-stu-id="97621-105">If the app has application permissions, or,</span></span>
* <span data-ttu-id="97621-106">如果应用程序具有相应从一个用户委派[权限](#permissions)，并另一个用户具有与该用户，共享日历，或具有委派的访问赋予该用户。</span><span class="sxs-lookup"><span data-stu-id="97621-106">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="97621-107">请参阅[详细信息和示例](../../../concepts/outlook-get-shared-events-calendars.md)。</span><span class="sxs-lookup"><span data-stu-id="97621-107">See [details and an example](../../../concepts/outlook-get-shared-events-calendars.md).</span></span>

<span data-ttu-id="97621-108">由于**事件**资源支持[扩展](../../../concepts/extensibility_overview.md)，因此也可使用 `GET` 操作获取**事件**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="97621-108">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="97621-109">支持不同时区</span><span class="sxs-lookup"><span data-stu-id="97621-109">Support various time zones</span></span>

<span data-ttu-id="97621-110">对于返回事件的所有 GET 操作，你可以使用 `Prefer: outlook.timezone` 标头在响应中指定事件开始和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="97621-110">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="97621-111">例如，下面的 `Prefer: outlook.timezone` 标头将响应中的开始和结束时间设置为东部标准时间。</span><span class="sxs-lookup"><span data-stu-id="97621-111">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="97621-p102">如果该事件是在不同的时区中创建的，则根据 `Prefer` 标头中指定的时区调整开始和结束时间。请查看此 [列表](../resources/datetimetimezone.md) 了解支持的时区名称。如果未指定 `Prefer: outlook.timezone` 标头，则返回用 UTC 表示的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="97621-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="97621-115">可以使用**事件**资源中的 **OriginalStartTimeZone** 和 **OriginalEndTimeZone** 属性来查找创建事件时使用的时区。</span><span class="sxs-lookup"><span data-stu-id="97621-115">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>


## <a name="permissions"></a><span data-ttu-id="97621-116">权限</span><span class="sxs-lookup"><span data-stu-id="97621-116">Permissions</span></span>
<span data-ttu-id="97621-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="97621-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="97621-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="97621-119">Permission type</span></span>      | <span data-ttu-id="97621-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97621-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97621-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97621-121">Delegated (work or school account)</span></span> | <span data-ttu-id="97621-122">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="97621-122">Calendars.Read</span></span>    |
|<span data-ttu-id="97621-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97621-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97621-124">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="97621-124">Calendars.Read</span></span>    |
|<span data-ttu-id="97621-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="97621-125">Application</span></span> | <span data-ttu-id="97621-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="97621-126">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="97621-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97621-127">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="97621-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="97621-128">Optional query parameters</span></span>
<span data-ttu-id="97621-129">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="97621-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="97621-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="97621-130">Request headers</span></span>
| <span data-ttu-id="97621-131">名称</span><span class="sxs-lookup"><span data-stu-id="97621-131">Name</span></span>       | <span data-ttu-id="97621-132">类型</span><span class="sxs-lookup"><span data-stu-id="97621-132">Type</span></span> | <span data-ttu-id="97621-133">说明</span><span class="sxs-lookup"><span data-stu-id="97621-133">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="97621-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="97621-134">Authorization</span></span>  | <span data-ttu-id="97621-135">string</span><span class="sxs-lookup"><span data-stu-id="97621-135">string</span></span> | <span data-ttu-id="97621-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="97621-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="97621-138">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="97621-138">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="97621-139">string</span><span class="sxs-lookup"><span data-stu-id="97621-139">string</span></span> | <span data-ttu-id="97621-140">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="97621-140">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="97621-141">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="97621-141">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="97621-142">可选。</span><span class="sxs-lookup"><span data-stu-id="97621-142">Optional.</span></span> |
| <span data-ttu-id="97621-143">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="97621-143">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="97621-144">string</span><span class="sxs-lookup"><span data-stu-id="97621-144">string</span></span> | <span data-ttu-id="97621-145">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="97621-145">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="97621-146">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="97621-146">Values can be "text" or "html".</span></span> <span data-ttu-id="97621-147">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="97621-147">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="97621-148">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="97621-148">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="97621-149">可选。</span><span class="sxs-lookup"><span data-stu-id="97621-149">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97621-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="97621-150">Request body</span></span>
<span data-ttu-id="97621-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="97621-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97621-152">响应</span><span class="sxs-lookup"><span data-stu-id="97621-152">Response</span></span>

<span data-ttu-id="97621-153">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="97621-153">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="97621-154">示例</span><span class="sxs-lookup"><span data-stu-id="97621-154">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="97621-155">请求 1</span><span class="sxs-lookup"><span data-stu-id="97621-155">Request 1</span></span>
<span data-ttu-id="97621-p107">第一个示例获取指定的事件。它指定以下内容：</span><span class="sxs-lookup"><span data-stu-id="97621-p107">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="97621-158">获取以太平洋标准时间格式返回的日期时间值的 `Prefer: outlook.timezone` 标头。</span><span class="sxs-lookup"><span data-stu-id="97621-158">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="97621-p108">返回特定属性的 `$select` 查询参数。如果没有 `$select` 参数，将返回所有事件属性。</span><span class="sxs-lookup"><span data-stu-id="97621-p108">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGIAAAoZDOFAAA="],
  "name": "get_event"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/events/AAMkAGIAAAoZDOFAAA=?$select=subject,body,bodyPreview,organizer,attendees,start,end,location 
Prefer: outlook.timezone="Pacific Standard Time"
```

##### <a name="response-1"></a><span data-ttu-id="97621-161">响应 1</span><span class="sxs-lookup"><span data-stu-id="97621-161">Response 1</span></span>

<span data-ttu-id="97621-p109">下面是一个响应示例。以 HTML 默认格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="97621-p109">Here is an example of the response. The **body** property is returned in the default format of HTML.</span></span>

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


##### <a name="request-2"></a><span data-ttu-id="97621-164">请求 2</span><span class="sxs-lookup"><span data-stu-id="97621-164">Request 2</span></span>

<span data-ttu-id="97621-165">第二个示例显示获取指定多个地点的事件。</span><span class="sxs-lookup"><span data-stu-id="97621-165">The second example shows getting an event that specifies more than one location.</span></span> <span data-ttu-id="97621-166">该请求指定返回特定属性的 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="97621-166">The request specifies a `$select` query parameter to return specific properties.</span></span> 

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADAGAADDdm4NAAA="],
  "name": "get_event_multiple_locations"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/AAMkADAGAADDdm4NAAA=?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
##### <a name="response-2"></a><span data-ttu-id="97621-167">响应 2</span><span class="sxs-lookup"><span data-stu-id="97621-167">Response 2</span></span>
<span data-ttu-id="97621-168">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="97621-168">Here is an example of the response.</span></span> <span data-ttu-id="97621-169">**locations** 属性包括组织事件的 3 个地点的详细信息。</span><span class="sxs-lookup"><span data-stu-id="97621-169">The **locations** property includes details for the 3 locations that the event is organized for.</span></span> 

<span data-ttu-id="97621-170">由于该请求未指定任何 `Prefer: outlook.timezone` 标头，**start** 和 **end** 属性将以默认的 UTC 时区显示。</span><span class="sxs-lookup"><span data-stu-id="97621-170">Because the request does not specify any `Prefer: outlook.timezone` header, the **start** and **end** properties are displayed in the default UTC time zone.</span></span> 

<span data-ttu-id="97621-171">事件正文采用的是默认的 HTML 格式。</span><span class="sxs-lookup"><span data-stu-id="97621-171">The event body is in the default HTML format.</span></span>  

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



## <a name="see-also"></a><span data-ttu-id="97621-172">另请参阅</span><span class="sxs-lookup"><span data-stu-id="97621-172">See also</span></span>

- [<span data-ttu-id="97621-173">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="97621-173">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="97621-174">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="97621-174">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="97621-175">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="97621-175">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
