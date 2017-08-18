# <a name="list-instances"></a><span data-ttu-id="13609-101">列出实例</span><span class="sxs-lookup"><span data-stu-id="13609-101">List instances</span></span>

<span data-ttu-id="13609-p101">获取指定的时间范围的事件的实例（发生次数）。如果事件的类型是 `SeriesMaster`，这将返回在指定的时间范围内事件的发生次数和异常。</span><span class="sxs-lookup"><span data-stu-id="13609-p101">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13609-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="13609-104">Prerequisites</span></span>
<span data-ttu-id="13609-105">要执行此 API，需要以下**范围**之一：*Calendars.Read*</span><span class="sxs-lookup"><span data-stu-id="13609-105">One of the following **scopes** is required to execute this API: *Calendars.Read*</span></span>
## <a name="http-request"></a><span data-ttu-id="13609-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13609-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="13609-107">查询参数</span><span class="sxs-lookup"><span data-stu-id="13609-107">Query parameters</span></span>

<span data-ttu-id="13609-108">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="13609-108">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="13609-109">参数</span><span class="sxs-lookup"><span data-stu-id="13609-109">Parameter</span></span>    | <span data-ttu-id="13609-110">类型</span><span class="sxs-lookup"><span data-stu-id="13609-110">Type</span></span>   |<span data-ttu-id="13609-111">说明</span><span class="sxs-lookup"><span data-stu-id="13609-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13609-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="13609-112">startDateTime</span></span>|<span data-ttu-id="13609-113">String</span><span class="sxs-lookup"><span data-stu-id="13609-113">String</span></span>|<span data-ttu-id="13609-p102">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="13609-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="13609-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="13609-116">endDateTime</span></span>|<span data-ttu-id="13609-117">String</span><span class="sxs-lookup"><span data-stu-id="13609-117">String</span></span>|<span data-ttu-id="13609-p103">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="13609-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="13609-120">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="13609-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="13609-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="13609-121">Request headers</span></span>
| <span data-ttu-id="13609-122">名称</span><span class="sxs-lookup"><span data-stu-id="13609-122">Name</span></span>       | <span data-ttu-id="13609-123">类型</span><span class="sxs-lookup"><span data-stu-id="13609-123">Type</span></span> | <span data-ttu-id="13609-124">说明</span><span class="sxs-lookup"><span data-stu-id="13609-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="13609-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="13609-125">Authorization</span></span>  | <span data-ttu-id="13609-126">string</span><span class="sxs-lookup"><span data-stu-id="13609-126">string</span></span>  | <span data-ttu-id="13609-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="13609-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="13609-129">Prefer</span><span class="sxs-lookup"><span data-stu-id="13609-129">Prefer</span></span> | <span data-ttu-id="13609-130">string</span><span class="sxs-lookup"><span data-stu-id="13609-130">string</span></span> | <span data-ttu-id="13609-p105">outlook.timezone=“东部标准时间”。可选。使用此选项指定响应中开始时间和结束时间的时区。如果未指定，则按 UTC 时间返回响应。</span><span class="sxs-lookup"><span data-stu-id="13609-p105">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13609-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="13609-135">Request body</span></span>
<span data-ttu-id="13609-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="13609-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13609-137">响应</span><span class="sxs-lookup"><span data-stu-id="13609-137">Response</span></span>

<span data-ttu-id="13609-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="13609-138">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="13609-139">示例</span><span class="sxs-lookup"><span data-stu-id="13609-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13609-140">请求</span><span class="sxs-lookup"><span data-stu-id="13609-140">Request</span></span>
<span data-ttu-id="13609-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="13609-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="13609-142">响应</span><span class="sxs-lookup"><span data-stu-id="13609-142">Response</span></span>
<span data-ttu-id="13609-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="13609-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List instances",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
