# <a name="list-events"></a><span data-ttu-id="2ec10-101">列出事件</span><span class="sxs-lookup"><span data-stu-id="2ec10-101">List events</span></span>

<span data-ttu-id="2ec10-p101">检索日历中的事件列表。该列表包含单个实例会议和系列主控形状。</span><span class="sxs-lookup"><span data-stu-id="2ec10-p101">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="2ec10-104">要获取扩展的事件实例，可以[获取日历视图](calendar_list_calendarview.md)，或者[获取事件的实例](event_list_instances.md)。</span><span class="sxs-lookup"><span data-stu-id="2ec10-104">To get expanded event instances, you can [get the calendar view](calendar_list_calendarview.md), or [get the instances of an event](event_list_instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2ec10-105">权限</span><span class="sxs-lookup"><span data-stu-id="2ec10-105">Permissions</span></span>
<span data-ttu-id="2ec10-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2ec10-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2ec10-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ec10-108">Permission type</span></span>      | <span data-ttu-id="2ec10-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ec10-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ec10-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ec10-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2ec10-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2ec10-111">Calendars.Read</span></span>    |
|<span data-ttu-id="2ec10-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ec10-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ec10-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2ec10-113">Calendars.Read</span></span>    |
|<span data-ttu-id="2ec10-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ec10-114">Application</span></span> | <span data-ttu-id="2ec10-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2ec10-115">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ec10-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ec10-116">HTTP request</span></span>
<span data-ttu-id="2ec10-117"><!-- { "blockType": "ignored" } -->用户或组的默认[日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="2ec10-117"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="2ec10-118">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="2ec10-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="2ec10-119">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="2ec10-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2ec10-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2ec10-120">Optional query parameters</span></span>
<span data-ttu-id="2ec10-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2ec10-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2ec10-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ec10-122">Request headers</span></span>
| <span data-ttu-id="2ec10-123">名称</span><span class="sxs-lookup"><span data-stu-id="2ec10-123">Name</span></span>       | <span data-ttu-id="2ec10-124">类型</span><span class="sxs-lookup"><span data-stu-id="2ec10-124">Type</span></span> | <span data-ttu-id="2ec10-125">说明</span><span class="sxs-lookup"><span data-stu-id="2ec10-125">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="2ec10-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ec10-126">Authorization</span></span>  | <span data-ttu-id="2ec10-127">string</span><span class="sxs-lookup"><span data-stu-id="2ec10-127">string</span></span> | <span data-ttu-id="2ec10-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ec10-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2ec10-130">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="2ec10-130">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="2ec10-131">string</span><span class="sxs-lookup"><span data-stu-id="2ec10-131">string</span></span> | <span data-ttu-id="2ec10-132">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="2ec10-132">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="2ec10-133">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="2ec10-133">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="2ec10-134">可选。</span><span class="sxs-lookup"><span data-stu-id="2ec10-134">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ec10-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ec10-135">Request body</span></span>
<span data-ttu-id="2ec10-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2ec10-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ec10-137">响应</span><span class="sxs-lookup"><span data-stu-id="2ec10-137">Response</span></span>

<span data-ttu-id="2ec10-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2ec10-138">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2ec10-139">示例</span><span class="sxs-lookup"><span data-stu-id="2ec10-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2ec10-140">请求</span><span class="sxs-lookup"><span data-stu-id="2ec10-140">Request</span></span>
<span data-ttu-id="2ec10-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2ec10-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/events
```
##### <a name="response"></a><span data-ttu-id="2ec10-142">响应</span><span class="sxs-lookup"><span data-stu-id="2ec10-142">Response</span></span>
<span data-ttu-id="2ec10-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2ec10-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
