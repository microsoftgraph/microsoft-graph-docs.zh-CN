# <a name="list-calendarview"></a><span data-ttu-id="06165-101">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="06165-101">List calendarView</span></span>

<span data-ttu-id="06165-102">从用户的默认日历或其他一些日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="06165-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="06165-103">权限</span><span class="sxs-lookup"><span data-stu-id="06165-103">Permissions</span></span>
<span data-ttu-id="06165-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="06165-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="06165-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="06165-106">Permission type</span></span>      | <span data-ttu-id="06165-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="06165-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06165-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06165-108">Delegated (work or school account)</span></span> | <span data-ttu-id="06165-109">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06165-109">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="06165-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06165-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06165-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06165-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="06165-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="06165-112">Application</span></span> | <span data-ttu-id="06165-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06165-113">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="06165-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06165-114">HTTP request</span></span>

<span data-ttu-id="06165-115">用户的默认 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="06165-115">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="06165-116">默认 [calendarGroup](../resources/calendargroup.md) 中的用户 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="06165-116">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="06165-117">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="06165-117">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="06165-118">查询参数</span><span class="sxs-lookup"><span data-stu-id="06165-118">Query parameters</span></span>

<span data-ttu-id="06165-119">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="06165-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="06165-120">参数</span><span class="sxs-lookup"><span data-stu-id="06165-120">Parameter</span></span>    | <span data-ttu-id="06165-121">类型</span><span class="sxs-lookup"><span data-stu-id="06165-121">Type</span></span>   |<span data-ttu-id="06165-122">说明</span><span class="sxs-lookup"><span data-stu-id="06165-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06165-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="06165-123">startDateTime</span></span>|<span data-ttu-id="06165-124">String</span><span class="sxs-lookup"><span data-stu-id="06165-124">String</span></span>|<span data-ttu-id="06165-p102">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="06165-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="06165-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="06165-127">endDateTime</span></span>|<span data-ttu-id="06165-128">String</span><span class="sxs-lookup"><span data-stu-id="06165-128">String</span></span>|<span data-ttu-id="06165-p103">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="06165-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="06165-131">此方法还支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="06165-131">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="06165-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="06165-132">Request headers</span></span>
| <span data-ttu-id="06165-133">名称</span><span class="sxs-lookup"><span data-stu-id="06165-133">Name</span></span>       | <span data-ttu-id="06165-134">类型</span><span class="sxs-lookup"><span data-stu-id="06165-134">Type</span></span> | <span data-ttu-id="06165-135">说明</span><span class="sxs-lookup"><span data-stu-id="06165-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="06165-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="06165-136">Authorization</span></span>  | <span data-ttu-id="06165-137">string</span><span class="sxs-lookup"><span data-stu-id="06165-137">string</span></span>  | <span data-ttu-id="06165-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="06165-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="06165-140">Content-Type</span><span class="sxs-lookup"><span data-stu-id="06165-140">Content-Type</span></span>   | <span data-ttu-id="06165-141">string</span><span class="sxs-lookup"><span data-stu-id="06165-141">string</span></span>  | <span data-ttu-id="06165-142">application/json</span><span class="sxs-lookup"><span data-stu-id="06165-142">application/json</span></span> |
| <span data-ttu-id="06165-143">Prefer</span><span class="sxs-lookup"><span data-stu-id="06165-143">Prefer</span></span> | <span data-ttu-id="06165-144">string</span><span class="sxs-lookup"><span data-stu-id="06165-144">string</span></span> | <span data-ttu-id="06165-p105">outlook.timezone=“东部标准时间”。可选。使用此选项指定响应中开始时间和结束时间的时区。如果未指定，则按 UTC 时间返回响应。</span><span class="sxs-lookup"><span data-stu-id="06165-p105">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06165-149">请求正文</span><span class="sxs-lookup"><span data-stu-id="06165-149">Request body</span></span>
<span data-ttu-id="06165-150">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="06165-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06165-151">响应</span><span class="sxs-lookup"><span data-stu-id="06165-151">Response</span></span>

<span data-ttu-id="06165-152">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="06165-152">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="06165-153">示例</span><span class="sxs-lookup"><span data-stu-id="06165-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06165-154">请求</span><span class="sxs-lookup"><span data-stu-id="06165-154">Request</span></span>
<span data-ttu-id="06165-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="06165-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000 
```
##### <a name="response"></a><span data-ttu-id="06165-156">响应</span><span class="sxs-lookup"><span data-stu-id="06165-156">Response</span></span>
<span data-ttu-id="06165-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="06165-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
