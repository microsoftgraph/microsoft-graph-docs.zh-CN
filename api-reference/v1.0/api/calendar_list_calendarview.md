# <a name="list-calendarview"></a><span data-ttu-id="b067f-101">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="b067f-101">List calendarView</span></span>

<span data-ttu-id="b067f-102">从用户或群组的默认日历 `(../me/calendarview)` 或用户的其他一些日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="b067f-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b067f-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="b067f-103">Prerequisites</span></span>
<span data-ttu-id="b067f-104">若要执行此 API，必须有以下**范围**之一：</span><span class="sxs-lookup"><span data-stu-id="b067f-104">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="b067f-105">用户日历中的事件：_Calendars.Read_ 或 _Calendars.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="b067f-105">Events in a user's calendar: _Calendars.Read_ or _Calendars.ReadWrite_</span></span>
* <span data-ttu-id="b067f-106">群组日历中的事件：_Group.Read.All_ 或 _Group.ReadWrite.All_</span><span class="sxs-lookup"><span data-stu-id="b067f-106">Events in a group calendar: _Group.Read.All_ or _Group.ReadWrite.All_</span></span>

## <a name="http-request"></a><span data-ttu-id="b067f-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b067f-107">HTTP request</span></span>

<span data-ttu-id="b067f-108">用户或组的默认 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="b067f-108">A user's or group's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="b067f-109">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="b067f-109">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="b067f-110">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="b067f-110">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="b067f-111">查询参数</span><span class="sxs-lookup"><span data-stu-id="b067f-111">Query parameters</span></span>

<span data-ttu-id="b067f-112">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="b067f-112">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="b067f-113">参数</span><span class="sxs-lookup"><span data-stu-id="b067f-113">Parameter</span></span>    | <span data-ttu-id="b067f-114">类型</span><span class="sxs-lookup"><span data-stu-id="b067f-114">Type</span></span>   |<span data-ttu-id="b067f-115">说明</span><span class="sxs-lookup"><span data-stu-id="b067f-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b067f-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b067f-116">startDateTime</span></span>|<span data-ttu-id="b067f-117">String</span><span class="sxs-lookup"><span data-stu-id="b067f-117">String</span></span>|<span data-ttu-id="b067f-p101">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="b067f-p101">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="b067f-120">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b067f-120">endDateTime</span></span>|<span data-ttu-id="b067f-121">String</span><span class="sxs-lookup"><span data-stu-id="b067f-121">String</span></span>|<span data-ttu-id="b067f-p102">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="b067f-p102">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="b067f-124">此方法还支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b067f-124">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b067f-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="b067f-125">Request headers</span></span>
| <span data-ttu-id="b067f-126">标头</span><span class="sxs-lookup"><span data-stu-id="b067f-126">Header</span></span>       | <span data-ttu-id="b067f-127">值</span><span class="sxs-lookup"><span data-stu-id="b067f-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b067f-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="b067f-128">Authorization</span></span>  | <span data-ttu-id="b067f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b067f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b067f-131">Prefer</span><span class="sxs-lookup"><span data-stu-id="b067f-131">Prefer</span></span>  | <span data-ttu-id="b067f-p104">outlook.timezone=“东部标准时间”。可选。使用此选项指定响应中开始时间和结束时间的时区。如果未指定，则按 UTC 时间返回响应。</span><span class="sxs-lookup"><span data-stu-id="b067f-p104">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b067f-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="b067f-136">Request body</span></span>
<span data-ttu-id="b067f-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b067f-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b067f-138">响应</span><span class="sxs-lookup"><span data-stu-id="b067f-138">Response</span></span>

<span data-ttu-id="b067f-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b067f-139">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b067f-140">示例</span><span class="sxs-lookup"><span data-stu-id="b067f-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b067f-141">请求</span><span class="sxs-lookup"><span data-stu-id="b067f-141">Request</span></span>
<span data-ttu-id="b067f-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b067f-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="b067f-143">响应</span><span class="sxs-lookup"><span data-stu-id="b067f-143">Response</span></span>
<span data-ttu-id="b067f-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b067f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
