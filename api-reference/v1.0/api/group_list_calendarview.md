# <a name="list-calendarview"></a><span data-ttu-id="4e962-101">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="4e962-101">List calendarView</span></span>

<span data-ttu-id="4e962-102">从群组的默认日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="4e962-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4e962-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="4e962-103">Prerequisites</span></span>
<span data-ttu-id="4e962-104">若要执行此 API，必须有以下任意一个**范围**：*Group.Read.All* 或 *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="4e962-104">One of the following **scopes** is required to execute this API: *Group.Read.All* or *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="4e962-105">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e962-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="4e962-106">查询参数</span><span class="sxs-lookup"><span data-stu-id="4e962-106">Query parameters</span></span>

<span data-ttu-id="4e962-107">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="4e962-107">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="4e962-108">参数</span><span class="sxs-lookup"><span data-stu-id="4e962-108">Parameter</span></span>    | <span data-ttu-id="4e962-109">类型</span><span class="sxs-lookup"><span data-stu-id="4e962-109">Type</span></span>   |<span data-ttu-id="4e962-110">说明</span><span class="sxs-lookup"><span data-stu-id="4e962-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e962-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4e962-111">startDateTime</span></span>|<span data-ttu-id="4e962-112">String</span><span class="sxs-lookup"><span data-stu-id="4e962-112">String</span></span>|<span data-ttu-id="4e962-p101">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="4e962-p101">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="4e962-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4e962-115">endDateTime</span></span>|<span data-ttu-id="4e962-116">String</span><span class="sxs-lookup"><span data-stu-id="4e962-116">String</span></span>|<span data-ttu-id="4e962-p102">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="4e962-p102">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="4e962-119">此方法还支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4e962-119">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4e962-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e962-120">Request headers</span></span>
| <span data-ttu-id="4e962-121">标头</span><span class="sxs-lookup"><span data-stu-id="4e962-121">Header</span></span>       | <span data-ttu-id="4e962-122">值</span><span class="sxs-lookup"><span data-stu-id="4e962-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4e962-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e962-123">Authorization</span></span>  | <span data-ttu-id="4e962-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e962-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4e962-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="4e962-126">Prefer</span></span> | <span data-ttu-id="4e962-127">string</span><span class="sxs-lookup"><span data-stu-id="4e962-127">string</span></span> | <span data-ttu-id="4e962-p104">outlook.timezone=“东部标准时间”。可选。使用此选项指定响应中开始时间和结束时间的时区。如果未指定，则按 UTC 时间返回响应。</span><span class="sxs-lookup"><span data-stu-id="4e962-p104">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e962-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e962-132">Request body</span></span>
<span data-ttu-id="4e962-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4e962-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e962-134">响应</span><span class="sxs-lookup"><span data-stu-id="4e962-134">Response</span></span>

<span data-ttu-id="4e962-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4e962-135">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4e962-136">示例</span><span class="sxs-lookup"><span data-stu-id="4e962-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e962-137">请求</span><span class="sxs-lookup"><span data-stu-id="4e962-137">Request</span></span>
<span data-ttu-id="4e962-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4e962-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/calendarView
```
##### <a name="response"></a><span data-ttu-id="4e962-139">响应</span><span class="sxs-lookup"><span data-stu-id="4e962-139">Response</span></span>
<span data-ttu-id="4e962-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4e962-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
