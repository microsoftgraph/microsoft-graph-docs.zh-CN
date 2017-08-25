# <a name="create-event"></a><span data-ttu-id="b3c08-101">创建事件</span><span class="sxs-lookup"><span data-stu-id="b3c08-101">Create Event</span></span>

<span data-ttu-id="b3c08-102">在用户的默认日历或指定日历中创建[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="b3c08-102">Create an [event](../resources/event.md) in the user's default calendar or specified calendar.</span></span>

<span data-ttu-id="b3c08-103">可以将事件的各开始和结束时间的时区指定为这些值的一部分，因为**开始**和**结束**属性为 [dateTimeTimeZone](../resources/datetimetimezone.md) 类型。</span><span class="sxs-lookup"><span data-stu-id="b3c08-103">You can specify the time zone for each of the start and end times of the event as part of these values, as the **start** and **end** properties are of [dateTimeTimeZone](../resources/datetimetimezone.md) type.</span></span> 

<span data-ttu-id="b3c08-104">创建事件时，服务器将向所有与会者发送邀请。</span><span class="sxs-lookup"><span data-stu-id="b3c08-104">When the event is created, the server send invitations to all attendees.</span></span>


## <a name="permissions"></a><span data-ttu-id="b3c08-105">权限</span><span class="sxs-lookup"><span data-stu-id="b3c08-105">Permissions</span></span>
<span data-ttu-id="b3c08-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b3c08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b3c08-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3c08-108">Permission type</span></span>      | <span data-ttu-id="b3c08-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b3c08-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="b3c08-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3c08-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b3c08-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3c08-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="b3c08-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3c08-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3c08-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3c08-113">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="b3c08-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3c08-114">Application</span></span> | <span data-ttu-id="b3c08-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3c08-115">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b3c08-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3c08-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events
POST /users/{id | userPrincipalName}/events

POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events

POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="b3c08-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3c08-117">Request headers</span></span>
| <span data-ttu-id="b3c08-118">标头</span><span class="sxs-lookup"><span data-stu-id="b3c08-118">Header</span></span>       | <span data-ttu-id="b3c08-119">值</span><span class="sxs-lookup"><span data-stu-id="b3c08-119">Value</span></span> |
|:-----------|:------|
| <span data-ttu-id="b3c08-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3c08-120">Authorization</span></span>  | <span data-ttu-id="b3c08-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b3c08-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b3c08-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b3c08-123">Content-Type</span></span>  | <span data-ttu-id="b3c08-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b3c08-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b3c08-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3c08-126">Request body</span></span>
<span data-ttu-id="b3c08-127">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3c08-127">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

<span data-ttu-id="b3c08-128">由于**事件**资源支持[扩展](../../../concepts/extensibility_overview.md)因此可以使用 `POST` 操作，并在创建事件时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="b3c08-128">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="b3c08-129">响应</span><span class="sxs-lookup"><span data-stu-id="b3c08-129">Response</span></span>

<span data-ttu-id="b3c08-130">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b3c08-130">If successful, this method returns `201, Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3c08-131">示例</span><span class="sxs-lookup"><span data-stu-id="b3c08-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3c08-132">请求</span><span class="sxs-lookup"><span data-stu-id="b3c08-132">Request</span></span>
<span data-ttu-id="b3c08-p104">下面是一个请求示例。它使用 `Prefer: outlook.timezone` 请求标头来指定应使用该时区的响应中的**开始**和**结束**时间。</span><span class="sxs-lookup"><span data-stu-id="b3c08-p104">Here is an example of the request. It uses the `Prefer: outlook.timezone` request header to specify the **start** and **end** times in the response should use that time zone.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 600

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does late morning work for you?"
  },
  "start": {
      "dateTime": "2017-04-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-04-15T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"fannyd@contoso.onmicrosoft.com",
        "name": "Fanny Downs"
      },
      "type": "required"
    }
  ]
}
```
<span data-ttu-id="b3c08-135">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3c08-135">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b3c08-136">响应</span><span class="sxs-lookup"><span data-stu-id="b3c08-136">Response</span></span>
<span data-ttu-id="b3c08-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b3c08-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 2197

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==\"",
    "id":"AAMkAGI1AAAt9AHjAAA=",
    "createdDateTime":"2017-04-15T03:00:50.7579581Z",
    "lastModifiedDateTime":"2017-04-15T03:00:51.245372Z",
    "changeKey":"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "iCalUId":"040000008200E00074C5B7101A82E00800000000DA2B357D94B5D201000000000000000010000000EC4597557F0CB34EA4CC2887EA7B17C3",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "subject":"Let's go brunch",
    "bodyPreview":"Does late morning work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"singleInstance",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI1AAAt9AHjAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html><head></head><body>Does late morning work for you?</body></html>"
    },
    "start":{
        "dateTime":"2017-04-15T11:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-04-15T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location":{
        "displayName":"Harry's Bar"
    },
    "recurrence":null,
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Fanny Downs",
                "address":"fannyd@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Dana Swope",
            "address":"danas@contoso.onmicrosoft.com"
        }
    }
}
```
## <a name="see-also"></a><span data-ttu-id="b3c08-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b3c08-140">See also</span></span>

- [<span data-ttu-id="b3c08-141">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b3c08-141">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="b3c08-142">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="b3c08-142">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
