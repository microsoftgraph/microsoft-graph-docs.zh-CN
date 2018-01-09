# <a name="list-calendarview"></a><span data-ttu-id="bd058-101">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="bd058-101">List calendarView</span></span>

<span data-ttu-id="bd058-102">从用户的默认日历或其他一些日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="bd058-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="bd058-103">权限</span><span class="sxs-lookup"><span data-stu-id="bd058-103">Permissions</span></span>
<span data-ttu-id="bd058-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="bd058-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bd058-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd058-106">Permission type</span></span>      | <span data-ttu-id="bd058-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd058-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd058-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd058-108">Delegated (work or school account)</span></span> | <span data-ttu-id="bd058-109">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd058-109">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bd058-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd058-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd058-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd058-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bd058-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd058-112">Application</span></span> | <span data-ttu-id="bd058-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd058-113">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd058-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd058-114">HTTP request</span></span>

<span data-ttu-id="bd058-115">用户的默认 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="bd058-115">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="bd058-116">默认 [calendarGroup](../resources/calendargroup.md) 中的用户 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="bd058-116">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="bd058-117">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="bd058-117">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="bd058-118">查询参数</span><span class="sxs-lookup"><span data-stu-id="bd058-118">Query parameters</span></span>

<span data-ttu-id="bd058-119">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="bd058-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="bd058-120">参数</span><span class="sxs-lookup"><span data-stu-id="bd058-120">Parameter</span></span>    | <span data-ttu-id="bd058-121">类型</span><span class="sxs-lookup"><span data-stu-id="bd058-121">Type</span></span>   |<span data-ttu-id="bd058-122">说明</span><span class="sxs-lookup"><span data-stu-id="bd058-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd058-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bd058-123">startDateTime</span></span>|<span data-ttu-id="bd058-124">String</span><span class="sxs-lookup"><span data-stu-id="bd058-124">String</span></span>|<span data-ttu-id="bd058-p102">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="bd058-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="bd058-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="bd058-127">endDateTime</span></span>|<span data-ttu-id="bd058-128">String</span><span class="sxs-lookup"><span data-stu-id="bd058-128">String</span></span>|<span data-ttu-id="bd058-p103">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="bd058-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="bd058-131">此方法还支持 [OData 查询参数]((http://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters)) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bd058-131">This method also supports the [OData Query Parameters]((http://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters)) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bd058-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd058-132">Request headers</span></span>
| <span data-ttu-id="bd058-133">名称</span><span class="sxs-lookup"><span data-stu-id="bd058-133">Name</span></span>       | <span data-ttu-id="bd058-134">类型</span><span class="sxs-lookup"><span data-stu-id="bd058-134">Type</span></span> | <span data-ttu-id="bd058-135">说明</span><span class="sxs-lookup"><span data-stu-id="bd058-135">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="bd058-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd058-136">Authorization</span></span>  | <span data-ttu-id="bd058-137">string</span><span class="sxs-lookup"><span data-stu-id="bd058-137">string</span></span> | <span data-ttu-id="bd058-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bd058-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bd058-140">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="bd058-140">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="bd058-141">string</span><span class="sxs-lookup"><span data-stu-id="bd058-141">string</span></span> | <span data-ttu-id="bd058-142">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="bd058-142">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> <span data-ttu-id="bd058-143">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="bd058-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="bd058-144">可选。</span><span class="sxs-lookup"><span data-stu-id="bd058-144">Optional.</span></span> |
| <span data-ttu-id="bd058-145">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="bd058-145">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="bd058-146">string</span><span class="sxs-lookup"><span data-stu-id="bd058-146">string</span></span> | <span data-ttu-id="bd058-147">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="bd058-147">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="bd058-148">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="bd058-148">Values can be "text" or "html".</span></span> <span data-ttu-id="bd058-149">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="bd058-149">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="bd058-150">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="bd058-150">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="bd058-151">可选。</span><span class="sxs-lookup"><span data-stu-id="bd058-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd058-152">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd058-152">Request body</span></span>
<span data-ttu-id="bd058-153">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bd058-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd058-154">响应</span><span class="sxs-lookup"><span data-stu-id="bd058-154">Response</span></span>

<span data-ttu-id="bd058-155">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bd058-155">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bd058-156">示例</span><span class="sxs-lookup"><span data-stu-id="bd058-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bd058-157">请求</span><span class="sxs-lookup"><span data-stu-id="bd058-157">Request</span></span>
<span data-ttu-id="bd058-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bd058-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000 
```
##### <a name="response"></a><span data-ttu-id="bd058-159">响应</span><span class="sxs-lookup"><span data-stu-id="bd058-159">Response</span></span>
<span data-ttu-id="bd058-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bd058-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
