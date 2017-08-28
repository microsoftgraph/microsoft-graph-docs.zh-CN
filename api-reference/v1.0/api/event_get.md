# <a name="get-event"></a><span data-ttu-id="a208c-101">获取事件</span><span class="sxs-lookup"><span data-stu-id="a208c-101">Get event</span></span>

<span data-ttu-id="a208c-102">获取指定的 [event](../resources/event.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a208c-102">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="a208c-103">目前，此操作返回纯 HTML 格式的事件正文。</span><span class="sxs-lookup"><span data-stu-id="a208c-103">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="a208c-104">由于**事件**资源支持[扩展](../../../concepts/extensibility_overview.md)，因此也可使用 `GET` 操作获取**事件**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="a208c-104">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>

### <a name="support-various-time-zones"></a><span data-ttu-id="a208c-105">支持不同时区</span><span class="sxs-lookup"><span data-stu-id="a208c-105">Support various time zones</span></span>

<span data-ttu-id="a208c-106">对于返回事件的所有 GET 操作，你可以使用 `Prefer: outlook.timezone` 标头在响应中指定事件开始和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="a208c-106">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="a208c-107">例如，下面的 `Prefer: outlook.timezone` 标头将响应中的开始和结束时间设置为东部标准时间。</span><span class="sxs-lookup"><span data-stu-id="a208c-107">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="a208c-p101">如果该事件是在不同的时区中创建的，则根据 `Prefer` 标头中指定的时区调整开始和结束时间。请查看此 [列表](../resources/datetimetimezone.md) 了解支持的时区名称。如果未指定 `Prefer: outlook.timezone` 标头，则返回用 UTC 表示的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="a208c-p101">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="a208c-111">可以使用**事件**资源中的 **OriginalStartTimeZone** 和 **OriginalEndTimeZone** 属性来查找创建事件时使用的时区。</span><span class="sxs-lookup"><span data-stu-id="a208c-111">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>


## <a name="permissions"></a><span data-ttu-id="a208c-112">权限</span><span class="sxs-lookup"><span data-stu-id="a208c-112">Permissions</span></span>
<span data-ttu-id="a208c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a208c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a208c-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="a208c-115">Permission type</span></span>      | <span data-ttu-id="a208c-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a208c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a208c-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a208c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="a208c-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a208c-118">Calendars.Read</span></span>    |
|<span data-ttu-id="a208c-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a208c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a208c-120">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a208c-120">Calendars.Read</span></span>    |
|<span data-ttu-id="a208c-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="a208c-121">Application</span></span> | <span data-ttu-id="a208c-122">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a208c-122">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="a208c-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a208c-123">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="a208c-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a208c-124">Optional query parameters</span></span>
<span data-ttu-id="a208c-125">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a208c-125">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a208c-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="a208c-126">Request headers</span></span>
| <span data-ttu-id="a208c-127">名称</span><span class="sxs-lookup"><span data-stu-id="a208c-127">Name</span></span>       | <span data-ttu-id="a208c-128">类型</span><span class="sxs-lookup"><span data-stu-id="a208c-128">Type</span></span> | <span data-ttu-id="a208c-129">说明</span><span class="sxs-lookup"><span data-stu-id="a208c-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a208c-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="a208c-130">Authorization</span></span>  | <span data-ttu-id="a208c-131">string</span><span class="sxs-lookup"><span data-stu-id="a208c-131">string</span></span>  | <span data-ttu-id="a208c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a208c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a208c-134">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="a208c-134">Prefer: outlook.timezone</span></span> | <span data-ttu-id="a208c-135">string</span><span class="sxs-lookup"><span data-stu-id="a208c-135">string</span></span> | <span data-ttu-id="a208c-136">事件在响应中的默认时区。</span><span class="sxs-lookup"><span data-stu-id="a208c-136">The default time zone for events in the response.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a208c-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="a208c-137">Request body</span></span>
<span data-ttu-id="a208c-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a208c-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a208c-139">响应</span><span class="sxs-lookup"><span data-stu-id="a208c-139">Response</span></span>

<span data-ttu-id="a208c-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a208c-140">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a208c-141">示例</span><span class="sxs-lookup"><span data-stu-id="a208c-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a208c-142">请求</span><span class="sxs-lookup"><span data-stu-id="a208c-142">Request</span></span>
<span data-ttu-id="a208c-p104">第一个示例获取指定的事件。它指定以下内容：</span><span class="sxs-lookup"><span data-stu-id="a208c-p104">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="a208c-145">获取以太平洋标准时间格式返回的日期时间值的 `Prefer: outlook.timezone` 标头。</span><span class="sxs-lookup"><span data-stu-id="a208c-145">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="a208c-p105">返回特定属性的 `$select` 查询参数。如果没有 `$select` 参数，将返回所有事件属性。</span><span class="sxs-lookup"><span data-stu-id="a208c-p105">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_event"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGIAAAoZDOFAAA=')?$select=subject,body,bodyPreview,organizer,attendees,start,end,location 
Prefer: outlook.timezone="Pacific Standard Time"
```

##### <a name="response"></a><span data-ttu-id="a208c-148">响应</span><span class="sxs-lookup"><span data-stu-id="a208c-148">Response</span></span>

<span data-ttu-id="a208c-p106">下面是一个响应示例。以 HTML 默认格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="a208c-p106">Here is an example of the response. The **body** property is returned in the default format of HTML.</span></span>

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
    "location":{
        "displayName":"Assembly Hall"
    },
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Fanny Downs",
                "address":"fannyd@a830edad905084922E17020313.onmicrosoft.com"
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
            "name":"Fanny Downs",
            "address":"fannyd@a830edad905084922E17020313.onmicrosoft.com"
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="a208c-151">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a208c-151">See also</span></span>

- [<span data-ttu-id="a208c-152">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="a208c-152">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="a208c-153">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="a208c-153">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
