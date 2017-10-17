# <a name="list-events"></a><span data-ttu-id="d03d9-101">列出事件</span><span class="sxs-lookup"><span data-stu-id="d03d9-101">List events</span></span>

<span data-ttu-id="d03d9-p101">获取用户邮箱中的 [event](../resources/event.md) 对象列表。该列表包含单个实例会议和系列主控形状。</span><span class="sxs-lookup"><span data-stu-id="d03d9-p101">Get a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="d03d9-104">目前，此操作返回纯 HTML 格式的事件正文。</span><span class="sxs-lookup"><span data-stu-id="d03d9-104">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="d03d9-105">要获取扩展的事件实例，可以[获取日历视图](calendar_list_calendarview.md)，或者[获取事件的实例](event_list_instances.md)。</span><span class="sxs-lookup"><span data-stu-id="d03d9-105">To get expanded event instances, you can [get the calendar view](calendar_list_calendarview.md), or [get the instances of an event](event_list_instances.md).</span></span>


### <a name="get-events-in-another-users-calendar"></a><span data-ttu-id="d03d9-106">获取其他用户的日历中的事件</span><span class="sxs-lookup"><span data-stu-id="d03d9-106">Get events in another user's calendar</span></span>

<span data-ttu-id="d03d9-107">如果你具有应用程序权限，或者具有某个用户的相应的委派[权限](#permissions)，则可以获取其他用户的日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="d03d9-107">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get events from another user's calendar.</span></span> <span data-ttu-id="d03d9-108">本部分重点介绍涉及委派权限的应用场景。</span><span class="sxs-lookup"><span data-stu-id="d03d9-108">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="d03d9-109">例如，你的应用已从用户 John 获得委派权限。</span><span class="sxs-lookup"><span data-stu-id="d03d9-109">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="d03d9-110">假设另一位用户 Garth 与 John 共享了一个日历。</span><span class="sxs-lookup"><span data-stu-id="d03d9-110">Suppose another user, Garth, has shared a calendar with John.</span></span> <span data-ttu-id="d03d9-111">可以通过在下面所示的查询示例中指定 Garth 的用户 ID（或者用户主体名称）来获取该共享日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="d03d9-111">You can get the events in that shared calendar by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/events
```

<span data-ttu-id="d03d9-112">此功能适用于对单个用户执行的所有支持的 GET 事件操作，如下面的 [HTTP 请求](#http-request)部分所示。</span><span class="sxs-lookup"><span data-stu-id="d03d9-112">This capability applies to all the supported GET events operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="d03d9-113">如果 Garth 将他的整个邮箱委派给 John，此功能同样适用。</span><span class="sxs-lookup"><span data-stu-id="d03d9-113">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="d03d9-114">如果 Garth 未与 John 共享他的日历，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。</span><span class="sxs-lookup"><span data-stu-id="d03d9-114">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="d03d9-115">在这种情况下，指定用户 ID 或用户主体名称只适用于获取已登录用户自己的日历中的事件，而此查询等效于使用 /me 快捷方式：</span><span class="sxs-lookup"><span data-stu-id="d03d9-115">In such cases, specifying a user ID or user principal name only works for getting events in the signed-in user’s own calendars, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/events
```

<span data-ttu-id="d03d9-116">此功能仅适用于以下资源的 GET 操作：</span><span class="sxs-lookup"><span data-stu-id="d03d9-116">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="d03d9-117">共享联系人文件夹</span><span class="sxs-lookup"><span data-stu-id="d03d9-117">Shared contact folders</span></span>
- <span data-ttu-id="d03d9-118">共享日历</span><span class="sxs-lookup"><span data-stu-id="d03d9-118">Shared calendars</span></span>
- <span data-ttu-id="d03d9-119">共享文件夹中的联系人和事件</span><span class="sxs-lookup"><span data-stu-id="d03d9-119">Contacts and events in shared folders</span></span>
- <span data-ttu-id="d03d9-120">委派邮箱中的上述资源</span><span class="sxs-lookup"><span data-stu-id="d03d9-120">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="d03d9-121">此功能不适用于针对联系人、事件及其文件夹的其他操作。</span><span class="sxs-lookup"><span data-stu-id="d03d9-121">This capability is not available in other operations for contacts, events, and their folders.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="d03d9-122">支持不同时区</span><span class="sxs-lookup"><span data-stu-id="d03d9-122">Support various time zones</span></span>

<span data-ttu-id="d03d9-123">对于返回事件的所有 GET 操作，你可以使用 `Prefer: outlook.timezone` 标头在响应中指定事件开始和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="d03d9-123">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="d03d9-124">例如，下面的 `Prefer: outlook.timezone` 标头将响应中的开始和结束时间设置为东部标准时间。</span><span class="sxs-lookup"><span data-stu-id="d03d9-124">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="d03d9-p106">如果该事件是在不同的时区中创建的，则根据 `Prefer` 标头中指定的时区调整开始和结束时间。请查看此 [列表](../resources/datetimetimezone.md) 了解支持的时区名称。如果未指定 `Prefer: outlook.timezone` 标头，则返回用 UTC 表示的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="d03d9-p106">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="d03d9-128">可以使用**事件**资源中的 **OriginalStartTimeZone** 和 **OriginalEndTimeZone** 属性来查找创建事件时使用的时区。</span><span class="sxs-lookup"><span data-stu-id="d03d9-128">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="d03d9-129">权限</span><span class="sxs-lookup"><span data-stu-id="d03d9-129">Permissions</span></span>
<span data-ttu-id="d03d9-p107">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d03d9-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d03d9-132">权限类型</span><span class="sxs-lookup"><span data-stu-id="d03d9-132">Permission type</span></span>      | <span data-ttu-id="d03d9-133">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d03d9-133">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d03d9-134">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d03d9-134">Delegated (work or school account)</span></span> | <span data-ttu-id="d03d9-135">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d03d9-135">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d03d9-136">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d03d9-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d03d9-137">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d03d9-137">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d03d9-138">应用程序</span><span class="sxs-lookup"><span data-stu-id="d03d9-138">Application</span></span> | <span data-ttu-id="d03d9-139">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d03d9-139">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d03d9-140">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d03d9-140">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="d03d9-141">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d03d9-141">Optional query parameters</span></span>
<span data-ttu-id="d03d9-142">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d03d9-142">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d03d9-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="d03d9-143">Request headers</span></span>
| <span data-ttu-id="d03d9-144">名称</span><span class="sxs-lookup"><span data-stu-id="d03d9-144">Name</span></span>       | <span data-ttu-id="d03d9-145">类型</span><span class="sxs-lookup"><span data-stu-id="d03d9-145">Type</span></span> | <span data-ttu-id="d03d9-146">说明</span><span class="sxs-lookup"><span data-stu-id="d03d9-146">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d03d9-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="d03d9-147">Authorization</span></span>  | <span data-ttu-id="d03d9-148">string</span><span class="sxs-lookup"><span data-stu-id="d03d9-148">string</span></span>  | <span data-ttu-id="d03d9-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d03d9-p108">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d03d9-151">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="d03d9-151">Prefer: outlook.timezone</span></span> | <span data-ttu-id="d03d9-152">字符串</span><span class="sxs-lookup"><span data-stu-id="d03d9-152">string</span></span> | <span data-ttu-id="d03d9-p109">事件在响应中的默认时区。可选。</span><span class="sxs-lookup"><span data-stu-id="d03d9-p109">The default time zone for events in the response. Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d03d9-155">请求正文</span><span class="sxs-lookup"><span data-stu-id="d03d9-155">Request body</span></span>
<span data-ttu-id="d03d9-156">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d03d9-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d03d9-157">响应</span><span class="sxs-lookup"><span data-stu-id="d03d9-157">Response</span></span>

<span data-ttu-id="d03d9-158">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d03d9-158">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d03d9-159">示例</span><span class="sxs-lookup"><span data-stu-id="d03d9-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d03d9-160">请求</span><span class="sxs-lookup"><span data-stu-id="d03d9-160">Request</span></span>
<span data-ttu-id="d03d9-p110">下面是一个请求示例。它指定以下内容：</span><span class="sxs-lookup"><span data-stu-id="d03d9-p110">Here is an example of the request. It specifies the following:</span></span>

- <span data-ttu-id="d03d9-163">获取以太平洋标准时间格式返回的日期时间值的 `Prefer: outlook.timezone` 标头。</span><span class="sxs-lookup"><span data-stu-id="d03d9-163">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="d03d9-p111">返回特定属性的 `$select` 查询参数。如果没有 `$select` 参数，将返回所有事件属性。</span><span class="sxs-lookup"><span data-stu-id="d03d9-p111">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response"></a><span data-ttu-id="d03d9-166">响应</span><span class="sxs-lookup"><span data-stu-id="d03d9-166">Response</span></span>
<span data-ttu-id="d03d9-p112">下面是一个响应示例。以默认的 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="d03d9-p112">Here is an example of the response. The **body** property is returned in the default HTML format.</span></span>
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
