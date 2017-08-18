# <a name="list-calendarview"></a><span data-ttu-id="66a23-101">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="66a23-101">List calendarView</span></span>

<span data-ttu-id="66a23-102">从用户的默认日历或其他一些日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="66a23-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="66a23-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="66a23-103">Prerequisites</span></span>
<span data-ttu-id="66a23-104">要执行此 API，需要以下**范围**之一：*Calendars.Read；Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="66a23-104">One of the following scopes is required to execute this API: Calendars.Read; Calendars.ReadWrite</span></span>
## <a name="http-request"></a><span data-ttu-id="66a23-105">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66a23-105">HTTP request</span></span>

<span data-ttu-id="66a23-106">用户的默认 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="66a23-106">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="66a23-107">默认 [calendarGroup](../resources/calendargroup.md) 中的用户 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="66a23-107">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="66a23-108">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="66a23-108">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="66a23-109">查询参数</span><span class="sxs-lookup"><span data-stu-id="66a23-109">Query parameters</span></span>

<span data-ttu-id="66a23-110">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="66a23-110">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="66a23-111">参数</span><span class="sxs-lookup"><span data-stu-id="66a23-111">Parameter</span></span>    | <span data-ttu-id="66a23-112">类型</span><span class="sxs-lookup"><span data-stu-id="66a23-112">Type</span></span>   |<span data-ttu-id="66a23-113">说明</span><span class="sxs-lookup"><span data-stu-id="66a23-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66a23-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="66a23-114">startDateTime</span></span>|<span data-ttu-id="66a23-115">String</span><span class="sxs-lookup"><span data-stu-id="66a23-115">String</span></span>|<span data-ttu-id="66a23-p101">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="66a23-p101">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="66a23-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="66a23-118">endDateTime</span></span>|<span data-ttu-id="66a23-119">String</span><span class="sxs-lookup"><span data-stu-id="66a23-119">String</span></span>|<span data-ttu-id="66a23-p102">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="66a23-p102">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="66a23-122">此方法还支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="66a23-122">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="66a23-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="66a23-123">Request headers</span></span>
| <span data-ttu-id="66a23-124">名称</span><span class="sxs-lookup"><span data-stu-id="66a23-124">Name</span></span>       | <span data-ttu-id="66a23-125">类型</span><span class="sxs-lookup"><span data-stu-id="66a23-125">Type</span></span> | <span data-ttu-id="66a23-126">说明</span><span class="sxs-lookup"><span data-stu-id="66a23-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="66a23-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="66a23-127">Authorization</span></span>  | <span data-ttu-id="66a23-128">string</span><span class="sxs-lookup"><span data-stu-id="66a23-128">string</span></span>  | <span data-ttu-id="66a23-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="66a23-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66a23-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="66a23-131">Content-Type</span></span>   | <span data-ttu-id="66a23-132">string</span><span class="sxs-lookup"><span data-stu-id="66a23-132">string</span></span>  | <span data-ttu-id="66a23-133">application/json</span><span class="sxs-lookup"><span data-stu-id="66a23-133">application/json</span></span> | 
| <span data-ttu-id="66a23-134">Prefer</span><span class="sxs-lookup"><span data-stu-id="66a23-134">Prefer</span></span> | <span data-ttu-id="66a23-135">string</span><span class="sxs-lookup"><span data-stu-id="66a23-135">string</span></span> | <span data-ttu-id="66a23-p104">outlook.timezone=“东部标准时间”。可选。使用此选项指定响应中开始时间和结束时间的时区。如果未指定，则按 UTC 时间返回响应。</span><span class="sxs-lookup"><span data-stu-id="66a23-p104">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66a23-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="66a23-140">Request body</span></span>
<span data-ttu-id="66a23-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="66a23-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66a23-142">响应</span><span class="sxs-lookup"><span data-stu-id="66a23-142">Response</span></span>

<span data-ttu-id="66a23-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="66a23-143">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="66a23-144">示例</span><span class="sxs-lookup"><span data-stu-id="66a23-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66a23-145">请求</span><span class="sxs-lookup"><span data-stu-id="66a23-145">Request</span></span>
<span data-ttu-id="66a23-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="66a23-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000 
```
##### <a name="response"></a><span data-ttu-id="66a23-147">响应</span><span class="sxs-lookup"><span data-stu-id="66a23-147">Response</span></span>
<span data-ttu-id="66a23-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="66a23-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "response": "",
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
