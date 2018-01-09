# <a name="list-calendarview"></a><span data-ttu-id="2af2c-101">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="2af2c-101">List calendarView</span></span>

<span data-ttu-id="2af2c-102">从用户或群组的默认日历 `(../me/calendarview)` 或用户的其他一些日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="2af2c-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="2af2c-103">权限</span><span class="sxs-lookup"><span data-stu-id="2af2c-103">Permissions</span></span>
<span data-ttu-id="2af2c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2af2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

* <span data-ttu-id="2af2c-106">用户日历中的事件：Calendars.Read 或 Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2af2c-106">Events in a user's calendar: Calendars.Read or Calendars.ReadWrite</span></span>
* <span data-ttu-id="2af2c-107">群组日历中的事件：Group.Read.All 或 Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2af2c-107">Events in a group calendar: Group.Read.All or Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="2af2c-108">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2af2c-108">HTTP request</span></span>

<span data-ttu-id="2af2c-109">用户或组的默认 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="2af2c-109">A user's or group's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="2af2c-110">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="2af2c-110">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="2af2c-111">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="2af2c-111">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="2af2c-112">查询参数</span><span class="sxs-lookup"><span data-stu-id="2af2c-112">Query parameters</span></span>

<span data-ttu-id="2af2c-113">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="2af2c-113">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="2af2c-114">参数</span><span class="sxs-lookup"><span data-stu-id="2af2c-114">Parameter</span></span>    | <span data-ttu-id="2af2c-115">类型</span><span class="sxs-lookup"><span data-stu-id="2af2c-115">Type</span></span>   |<span data-ttu-id="2af2c-116">说明</span><span class="sxs-lookup"><span data-stu-id="2af2c-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2af2c-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2af2c-117">startDateTime</span></span>|<span data-ttu-id="2af2c-118">String</span><span class="sxs-lookup"><span data-stu-id="2af2c-118">String</span></span>|<span data-ttu-id="2af2c-p102">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="2af2c-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="2af2c-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="2af2c-121">endDateTime</span></span>|<span data-ttu-id="2af2c-122">String</span><span class="sxs-lookup"><span data-stu-id="2af2c-122">String</span></span>|<span data-ttu-id="2af2c-p103">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="2af2c-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="2af2c-125">此方法还支持 [OData 查询参数]((http://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters)) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2af2c-125">This method also supports the [OData Query Parameters]((http://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters)) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2af2c-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="2af2c-126">Request headers</span></span>
| <span data-ttu-id="2af2c-127">名称</span><span class="sxs-lookup"><span data-stu-id="2af2c-127">Name</span></span>       | <span data-ttu-id="2af2c-128">类型</span><span class="sxs-lookup"><span data-stu-id="2af2c-128">Type</span></span> | <span data-ttu-id="2af2c-129">说明</span><span class="sxs-lookup"><span data-stu-id="2af2c-129">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="2af2c-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="2af2c-130">Authorization</span></span>  | <span data-ttu-id="2af2c-131">string</span><span class="sxs-lookup"><span data-stu-id="2af2c-131">string</span></span> | <span data-ttu-id="2af2c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2af2c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2af2c-134">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="2af2c-134">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="2af2c-135">string</span><span class="sxs-lookup"><span data-stu-id="2af2c-135">string</span></span> | <span data-ttu-id="2af2c-136">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="2af2c-136">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> <span data-ttu-id="2af2c-137">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="2af2c-137">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="2af2c-138">可选。</span><span class="sxs-lookup"><span data-stu-id="2af2c-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2af2c-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="2af2c-139">Request body</span></span>
<span data-ttu-id="2af2c-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2af2c-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2af2c-141">响应</span><span class="sxs-lookup"><span data-stu-id="2af2c-141">Response</span></span>

<span data-ttu-id="2af2c-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2af2c-142">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2af2c-143">示例</span><span class="sxs-lookup"><span data-stu-id="2af2c-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2af2c-144">请求</span><span class="sxs-lookup"><span data-stu-id="2af2c-144">Request</span></span>
<span data-ttu-id="2af2c-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2af2c-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="2af2c-146">响应</span><span class="sxs-lookup"><span data-stu-id="2af2c-146">Response</span></span>
<span data-ttu-id="2af2c-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2af2c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "response-value",
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
