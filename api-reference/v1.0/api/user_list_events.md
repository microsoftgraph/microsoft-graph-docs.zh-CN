# <a name="list-events"></a><span data-ttu-id="82ffc-101">列出事件</span><span class="sxs-lookup"><span data-stu-id="82ffc-101">List events</span></span>

<span data-ttu-id="82ffc-p101">获取用户邮箱中的 [event](../resources/event.md) 对象列表。该列表包含单个实例会议和系列主控形状。</span><span class="sxs-lookup"><span data-stu-id="82ffc-p101">Get a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="82ffc-104">目前，此操作返回纯 HTML 格式的事件正文。</span><span class="sxs-lookup"><span data-stu-id="82ffc-104">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="82ffc-105">要获取扩展的事件实例，可以[获取日历视图](calendar_list_calendarview.md)，或者[获取事件的实例](event_list_instances.md)。</span><span class="sxs-lookup"><span data-stu-id="82ffc-105">To get expanded event instances, you can [get the calendar view](calendar_list_calendarview.md), or [get the instances of an event](event_list_instances.md).</span></span>

### <a name="support-various-time-zones"></a><span data-ttu-id="82ffc-106">支持不同时区</span><span class="sxs-lookup"><span data-stu-id="82ffc-106">Support various time zones</span></span>

<span data-ttu-id="82ffc-107">对于返回事件的所有 GET 操作，你可以使用 `Prefer: outlook.timezone` 标头在响应中指定事件开始和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="82ffc-107">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="82ffc-108">例如，下面的 `Prefer: outlook.timezone` 标头将响应中的开始和结束时间设置为东部标准时间。</span><span class="sxs-lookup"><span data-stu-id="82ffc-108">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="82ffc-p102">如果该事件是在不同的时区中创建的，则根据 `Prefer` 标头中指定的时区调整开始和结束时间。请查看此 [列表](../resources/datetimetimezone.md) 了解支持的时区名称。如果未指定 `Prefer: outlook.timezone` 标头，则返回用 UTC 表示的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="82ffc-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="82ffc-112">可以使用**事件**资源中的 **OriginalStartTimeZone** 和 **OriginalEndTimeZone** 属性来查找创建事件时使用的时区。</span><span class="sxs-lookup"><span data-stu-id="82ffc-112">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="82ffc-113">权限</span><span class="sxs-lookup"><span data-stu-id="82ffc-113">Permissions</span></span>
<span data-ttu-id="82ffc-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="82ffc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="82ffc-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="82ffc-116">Permission type</span></span>      | <span data-ttu-id="82ffc-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82ffc-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82ffc-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82ffc-118">Delegated (work or school account)</span></span> | <span data-ttu-id="82ffc-119">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82ffc-119">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="82ffc-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82ffc-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82ffc-121">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82ffc-121">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="82ffc-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="82ffc-122">Application</span></span> | <span data-ttu-id="82ffc-123">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82ffc-123">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="82ffc-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82ffc-124">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="82ffc-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="82ffc-125">Optional query parameters</span></span>
<span data-ttu-id="82ffc-126">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="82ffc-126">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="82ffc-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="82ffc-127">Request headers</span></span>
| <span data-ttu-id="82ffc-128">名称</span><span class="sxs-lookup"><span data-stu-id="82ffc-128">Name</span></span>       | <span data-ttu-id="82ffc-129">类型</span><span class="sxs-lookup"><span data-stu-id="82ffc-129">Type</span></span> | <span data-ttu-id="82ffc-130">说明</span><span class="sxs-lookup"><span data-stu-id="82ffc-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="82ffc-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="82ffc-131">Authorization</span></span>  | <span data-ttu-id="82ffc-132">string</span><span class="sxs-lookup"><span data-stu-id="82ffc-132">string</span></span>  | <span data-ttu-id="82ffc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="82ffc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="82ffc-135">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="82ffc-135">Prefer: outlook.timezone</span></span> | <span data-ttu-id="82ffc-136">字符串</span><span class="sxs-lookup"><span data-stu-id="82ffc-136">string</span></span> | <span data-ttu-id="82ffc-p105">事件在响应中的默认时区。可选。</span><span class="sxs-lookup"><span data-stu-id="82ffc-p105">The default time zone for events in the response. Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82ffc-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="82ffc-139">Request body</span></span>
<span data-ttu-id="82ffc-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="82ffc-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82ffc-141">响应</span><span class="sxs-lookup"><span data-stu-id="82ffc-141">Response</span></span>

<span data-ttu-id="82ffc-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="82ffc-142">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="82ffc-143">示例</span><span class="sxs-lookup"><span data-stu-id="82ffc-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82ffc-144">请求</span><span class="sxs-lookup"><span data-stu-id="82ffc-144">Request</span></span>
<span data-ttu-id="82ffc-p106">下面是一个请求示例。它指定以下内容：</span><span class="sxs-lookup"><span data-stu-id="82ffc-p106">Here is an example of the request. It specifies the following:</span></span>

- <span data-ttu-id="82ffc-147">获取以太平洋标准时间格式返回的日期时间值的 `Prefer: outlook.timezone` 标头。</span><span class="sxs-lookup"><span data-stu-id="82ffc-147">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="82ffc-p107">返回特定属性的 `$select` 查询参数。如果没有 `$select` 参数，将返回所有事件属性。</span><span class="sxs-lookup"><span data-stu-id="82ffc-p107">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response"></a><span data-ttu-id="82ffc-150">响应</span><span class="sxs-lookup"><span data-stu-id="82ffc-150">Response</span></span>
<span data-ttu-id="82ffc-p108">下面是一个响应示例。以默认的 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="82ffc-p108">Here is an example of the response. The **body** property is returned in the default HTML format.</span></span>
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
  "tocPath": ""
}-->
