# <a name="get-event"></a><span data-ttu-id="4fe64-101">获取事件</span><span class="sxs-lookup"><span data-stu-id="4fe64-101">Get event</span></span>
<span data-ttu-id="4fe64-102">获取 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4fe64-102">Get an [event](../resources/event.md) instance:</span></span>

## <a name="permissions"></a><span data-ttu-id="4fe64-103">权限</span><span class="sxs-lookup"><span data-stu-id="4fe64-103">Permissions</span></span>
<span data-ttu-id="4fe64-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4fe64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4fe64-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="4fe64-106">Permission type</span></span>      | <span data-ttu-id="4fe64-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4fe64-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4fe64-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4fe64-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4fe64-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fe64-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4fe64-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4fe64-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fe64-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fe64-111">Not supported.</span></span>    |
|<span data-ttu-id="4fe64-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="4fe64-112">Application</span></span> | <span data-ttu-id="4fe64-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fe64-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fe64-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4fe64-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}
GET /groups/{id}/calendar/events/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4fe64-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4fe64-115">Optional query parameters</span></span>
<span data-ttu-id="4fe64-116">此方法支持 [OData 查询参数](../../../concepts/query_parameters.md) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4fe64-116">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4fe64-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="4fe64-117">Request headers</span></span>
| <span data-ttu-id="4fe64-118">标头</span><span class="sxs-lookup"><span data-stu-id="4fe64-118">Header</span></span>       | <span data-ttu-id="4fe64-119">值</span><span class="sxs-lookup"><span data-stu-id="4fe64-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4fe64-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fe64-120">Authorization</span></span>  | <span data-ttu-id="4fe64-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4fe64-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4fe64-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="4fe64-123">Request body</span></span>
<span data-ttu-id="4fe64-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4fe64-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4fe64-125">响应</span><span class="sxs-lookup"><span data-stu-id="4fe64-125">Response</span></span>
<span data-ttu-id="4fe64-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4fe64-126">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fe64-127">示例</span><span class="sxs-lookup"><span data-stu-id="4fe64-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4fe64-128">请求</span><span class="sxs-lookup"><span data-stu-id="4fe64-128">Request</span></span>
<span data-ttu-id="4fe64-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4fe64-129">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_event"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```

#### <a name="response"></a><span data-ttu-id="4fe64-130">响应</span><span class="sxs-lookup"><span data-stu-id="4fe64-130">Response</span></span>
<span data-ttu-id="4fe64-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4fe64-131">Here is an example of the response.</span></span>
><span data-ttu-id="4fe64-132">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4fe64-132">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4fe64-133">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4fe64-133">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1728

{
    "id": "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==",
    "createdDateTime": "2017-07-31T18:58:31.011909Z",
    "lastModifiedDateTime": "2017-07-31T18:58:35.418473Z",
    "changeKey": "xPZF2y46pEiVBni87OnrpgAAAAAJTg==",
    "categories": [],
    "originalStartTimeZone": "Eastern Standard Time",
    "originalEndTimeZone": "Eastern Standard Time",
    "iCalUId": "040000008200E00074C5B7101A82E00800000000B23663002F0AD301000000000000000010000000B7C936D4C2FEC749824EE24B2FD7DA62",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Continuing Education Sync",
    "bodyPreview": "Higher Education Planning.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3acc89e82c01e349d4998655891d93e12e%40thread.skype/1501527510806?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "seriesMaster",
    "webLink": "https://outlook.office365.com/owa/?itemid=AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA%2Bb2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA%3D%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n</head>\r\n<body>\r\n<div>Higher Education Planning.</div>\r\n<div><br>\r\n<br>\r\n<br>\r\n<a href=\"https://teams.microsoft.com/l/meetup-join/19%3acc89e82c01e349d4998655891d93e12e%40thread.skype/1501527510806?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35\">Join Microsoft Teams Online Meeting</a></div>\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2017-08-15T14:30:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2017-08-15T15:30:00.0000000",
        "timeZone": "UTC"
    },
    "location": {
        "displayName": "HR Taskforce / Benefits"
    },
    "recurrence": {
        "pattern": {
            "type": "weekly",
            "interval": 1,
            "month": 0,
            "dayOfMonth": 0,
            "daysOfWeek": [
                "tuesday",
                "thursday"
            ],
            "firstDayOfWeek": "sunday",
            "index": "first"
        },
        "range": {
            "type": "noEnd",
            "startDate": "2017-08-15",
            "endDate": "0001-01-01",
            "recurrenceTimeZone": "Eastern Standard Time",
            "numberOfOccurrences": 0
        }
    },
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "accepted",
                "time": "2017-07-31T18:58:34.3298022Z"
            },
            "emailAddress": {
                "name": "Lidia Holloway",
                "address": "LidiaH@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "HR Taskforce",
                "address": "HRTaskforce@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Diego Siciliani",
                "address": "DiegoS@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Johanna Lorenz",
                "address": "JohannaL@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "HR Taskforce",
            "address": "HRTaskforce@contoso.com"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
