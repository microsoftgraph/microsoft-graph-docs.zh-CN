# <a name="list-instances"></a><span data-ttu-id="3c7b9-101">列出实例</span><span class="sxs-lookup"><span data-stu-id="3c7b9-101">List instances</span></span>

<span data-ttu-id="3c7b9-p101">获取指定的时间范围的事件的实例（发生次数）。如果事件的类型是 `SeriesMaster`，这将返回在指定的时间范围内事件的发生次数和异常。</span><span class="sxs-lookup"><span data-stu-id="3c7b9-p101">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c7b9-104">权限</span><span class="sxs-lookup"><span data-stu-id="3c7b9-104">Permissions</span></span>
<span data-ttu-id="3c7b9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3c7b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3c7b9-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c7b9-107">Permission type</span></span>      | <span data-ttu-id="3c7b9-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c7b9-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="3c7b9-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c7b9-109">Delegated (work or school account)</span></span> | <span data-ttu-id="3c7b9-110">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3c7b9-110">Calendars.Read</span></span>    | 
|<span data-ttu-id="3c7b9-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c7b9-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c7b9-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3c7b9-112">Calendars.Read</span></span>    | 
|<span data-ttu-id="3c7b9-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c7b9-113">Application</span></span> | <span data-ttu-id="3c7b9-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3c7b9-114">Calendars.Read</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3c7b9-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c7b9-115">HTTP request</span></span>
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
## <a name="query-parameters"></a><span data-ttu-id="3c7b9-116">查询参数</span><span class="sxs-lookup"><span data-stu-id="3c7b9-116">Query parameters</span></span>

<span data-ttu-id="3c7b9-117">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="3c7b9-117">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="3c7b9-118">参数</span><span class="sxs-lookup"><span data-stu-id="3c7b9-118">Parameter</span></span>    | <span data-ttu-id="3c7b9-119">类型</span><span class="sxs-lookup"><span data-stu-id="3c7b9-119">Type</span></span>   |<span data-ttu-id="3c7b9-120">说明</span><span class="sxs-lookup"><span data-stu-id="3c7b9-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c7b9-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3c7b9-121">startDateTime</span></span>|<span data-ttu-id="3c7b9-122">String</span><span class="sxs-lookup"><span data-stu-id="3c7b9-122">String</span></span>|<span data-ttu-id="3c7b9-p103">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="3c7b9-p103">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="3c7b9-125">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3c7b9-125">endDateTime</span></span>|<span data-ttu-id="3c7b9-126">String</span><span class="sxs-lookup"><span data-stu-id="3c7b9-126">String</span></span>|<span data-ttu-id="3c7b9-p104">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="3c7b9-p104">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="3c7b9-129">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3c7b9-129">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3c7b9-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c7b9-130">Request headers</span></span>
| <span data-ttu-id="3c7b9-131">名称</span><span class="sxs-lookup"><span data-stu-id="3c7b9-131">Name</span></span>       | <span data-ttu-id="3c7b9-132">类型</span><span class="sxs-lookup"><span data-stu-id="3c7b9-132">Type</span></span> | <span data-ttu-id="3c7b9-133">说明</span><span class="sxs-lookup"><span data-stu-id="3c7b9-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3c7b9-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c7b9-134">Authorization</span></span>  | <span data-ttu-id="3c7b9-135">string</span><span class="sxs-lookup"><span data-stu-id="3c7b9-135">string</span></span>  | <span data-ttu-id="3c7b9-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c7b9-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3c7b9-138">Prefer</span><span class="sxs-lookup"><span data-stu-id="3c7b9-138">Prefer</span></span> | <span data-ttu-id="3c7b9-139">string</span><span class="sxs-lookup"><span data-stu-id="3c7b9-139">string</span></span> | <span data-ttu-id="3c7b9-p106">outlook.timezone=“东部标准时间”。可选。使用此选项指定响应中开始时间和结束时间的时区。如果未指定，则按 UTC 时间返回响应。</span><span class="sxs-lookup"><span data-stu-id="3c7b9-p106">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c7b9-144">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c7b9-144">Request body</span></span>
<span data-ttu-id="3c7b9-145">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3c7b9-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c7b9-146">响应</span><span class="sxs-lookup"><span data-stu-id="3c7b9-146">Response</span></span>

<span data-ttu-id="3c7b9-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3c7b9-147">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3c7b9-148">示例</span><span class="sxs-lookup"><span data-stu-id="3c7b9-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c7b9-149">请求</span><span class="sxs-lookup"><span data-stu-id="3c7b9-149">Request</span></span>
<span data-ttu-id="3c7b9-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c7b9-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="3c7b9-151">响应</span><span class="sxs-lookup"><span data-stu-id="3c7b9-151">Response</span></span>
<span data-ttu-id="3c7b9-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3c7b9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
