# <a name="list-events"></a><span data-ttu-id="468ee-101">列出事件</span><span class="sxs-lookup"><span data-stu-id="468ee-101">List events</span></span>
<span data-ttu-id="468ee-102">检索 [event](../resources/event.md) 对象列表.</span><span class="sxs-lookup"><span data-stu-id="468ee-102">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="468ee-103">权限</span><span class="sxs-lookup"><span data-stu-id="468ee-103">Permissions</span></span>
<span data-ttu-id="468ee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="468ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="468ee-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="468ee-106">Permission type</span></span>      | <span data-ttu-id="468ee-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="468ee-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="468ee-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="468ee-108">Delegated (work or school account)</span></span> | <span data-ttu-id="468ee-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="468ee-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="468ee-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="468ee-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="468ee-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="468ee-111">Not supported.</span></span>    |
|<span data-ttu-id="468ee-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="468ee-112">Application</span></span> | <span data-ttu-id="468ee-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="468ee-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="468ee-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="468ee-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="468ee-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="468ee-115">Optional query parameters</span></span>
<span data-ttu-id="468ee-116">此方法支持 [OData 查询参数](../../../concepts/query_parameters.md) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="468ee-116">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="468ee-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="468ee-117">Request headers</span></span>
| <span data-ttu-id="468ee-118">名称</span><span class="sxs-lookup"><span data-stu-id="468ee-118">Name</span></span>       | <span data-ttu-id="468ee-119">类型</span><span class="sxs-lookup"><span data-stu-id="468ee-119">Type</span></span> | <span data-ttu-id="468ee-120">说明</span><span class="sxs-lookup"><span data-stu-id="468ee-120">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="468ee-121">授权</span><span class="sxs-lookup"><span data-stu-id="468ee-121">Authorization</span></span>  | <span data-ttu-id="468ee-122">字符串</span><span class="sxs-lookup"><span data-stu-id="468ee-122">string</span></span> | <span data-ttu-id="468ee-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="468ee-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="468ee-125">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="468ee-125">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="468ee-126">string</span><span class="sxs-lookup"><span data-stu-id="468ee-126">string</span></span> | <span data-ttu-id="468ee-127">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="468ee-127">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="468ee-128">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="468ee-128">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="468ee-129">可选。</span><span class="sxs-lookup"><span data-stu-id="468ee-129">Optional.</span></span> |
| <span data-ttu-id="468ee-130">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="468ee-130">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="468ee-131">string</span><span class="sxs-lookup"><span data-stu-id="468ee-131">string</span></span> | <span data-ttu-id="468ee-132">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="468ee-132">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="468ee-133">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="468ee-133">Values can be "text" or "html".</span></span> <span data-ttu-id="468ee-134">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="468ee-134">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="468ee-135">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="468ee-135">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="468ee-136">可选。</span><span class="sxs-lookup"><span data-stu-id="468ee-136">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="468ee-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="468ee-137">Request body</span></span>
<span data-ttu-id="468ee-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="468ee-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="468ee-139">响应</span><span class="sxs-lookup"><span data-stu-id="468ee-139">Response</span></span>
<span data-ttu-id="468ee-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="468ee-140">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="468ee-141">示例</span><span class="sxs-lookup"><span data-stu-id="468ee-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="468ee-142">请求</span><span class="sxs-lookup"><span data-stu-id="468ee-142">Request</span></span>
<span data-ttu-id="468ee-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="468ee-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315"],
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events
```

#### <a name="response"></a><span data-ttu-id="468ee-144">响应</span><span class="sxs-lookup"><span data-stu-id="468ee-144">Response</span></span>
<span data-ttu-id="468ee-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="468ee-145">The following is an example of the response.</span></span>
><span data-ttu-id="468ee-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="468ee-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "id": "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA==",
      "createdDateTime": "2017-07-31T18:59:01.982289Z",
      "lastModifiedDateTime": "2017-09-06T04:29:38.6647687Z",
      "changeKey": "xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
      "categories": [],
      "originalStartTimeZone": "Eastern Standard Time",
      "originalEndTimeZone": "Eastern Standard Time",
      "iCalUId": "040000008200E00074C5B7101A82E00800000000824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
      "reminderMinutesBeforeStart": 15,
      "isReminderOn": true,
      "hasAttachments": false,
      "subject": "New Training Plans",
      "bodyPreview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
      "importance": "normal",
      "sensitivity": "normal",
      "isAllDay": false,
      "isCancelled": false,
      "isOrganizer": true,
      "responseRequested": true,
      "seriesMasterId": null,
      "showAs": "busy",
      "type": "seriesMaster",
      "webLink": "https://outlook.office365.com/owa/?itemid=AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA%2Bb2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA%3D%3D&exvsurl=1&path=/calendar/item",
      "onlineMeetingUrl": null,
      "responseStatus": {
          "response": "organizer",
          "time": "0001-01-01T00:00:00Z"
      },
      "body": {
          "contentType": "html",
          "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n</head>\r\n<body>\r\n<div>Meeting to plan new trainings.</div>\r\n<div><br>\r\n<br>\r\n<br>\r\n<a href=\"https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35\">Join Microsoft Teams Online Meeting</a></div>\r\n</body>\r\n</html>\r\n"
      },
      "start": {
          "dateTime": "2017-08-14T21:00:00.0000000",
          "timeZone": "UTC"
      },
      "end": {
          "dateTime": "2017-08-14T22:00:00.0000000",
          "timeZone": "UTC"
      },
      "location": {
          "displayName": "HR Taskforce / Facilities"
      },
      "recurrence": {
          "pattern": {
              "type": "weekly",
              "interval": 1,
              "month": 0,
              "dayOfMonth": 0,
              "daysOfWeek": [
                  "monday",
                  "wednesday",
                  "friday"
              ],
              "firstDayOfWeek": "sunday",
              "index": "first"
          },
          "range": {
              "type": "noEnd",
              "startDate": "2017-08-14",
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
                  "time": "2017-07-31T18:59:06.4180028Z"
              },
              "emailAddress": {
                  "name": "Joni Sherman",
                  "address": "JoniS@contoso.onmicrosoft.com"
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
                  "address": "HRTaskforce@contoso.onmicrosoft.com"
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
                  "address": "MeganB@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Lidia Holloway",
                  "address": "LidiaH@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Emily Braun",
                  "address": "EmilyB@contoso.onmicrosoft.com"
              }
          }
      ],
      "organizer": {
          "emailAddress": {
              "name": "HR Taskforce",
              "address": "HRTaskforce@contoso.onmicrosoft.com"
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
