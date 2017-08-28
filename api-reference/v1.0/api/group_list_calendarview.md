# <a name="list-calendarview"></a><span data-ttu-id="ab3b1-101">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="ab3b1-101">List calendarView</span></span>

<span data-ttu-id="ab3b1-102">从群组的默认日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="ab3b1-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>
## <a name="permissions"></a><span data-ttu-id="ab3b1-103">权限</span><span class="sxs-lookup"><span data-stu-id="ab3b1-103">Permissions</span></span>
<span data-ttu-id="ab3b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ab3b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ab3b1-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab3b1-106">Permission type</span></span>      | <span data-ttu-id="ab3b1-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ab3b1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab3b1-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab3b1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ab3b1-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab3b1-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab3b1-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab3b1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab3b1-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab3b1-111">Not supported.</span></span>    |
|<span data-ttu-id="ab3b1-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab3b1-112">Application</span></span> | <span data-ttu-id="ab3b1-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab3b1-113">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab3b1-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab3b1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="ab3b1-115">查询参数</span><span class="sxs-lookup"><span data-stu-id="ab3b1-115">Query parameters</span></span>

<span data-ttu-id="ab3b1-116">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="ab3b1-116">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="ab3b1-117">参数</span><span class="sxs-lookup"><span data-stu-id="ab3b1-117">Parameter</span></span>    | <span data-ttu-id="ab3b1-118">类型</span><span class="sxs-lookup"><span data-stu-id="ab3b1-118">Type</span></span>   |<span data-ttu-id="ab3b1-119">说明</span><span class="sxs-lookup"><span data-stu-id="ab3b1-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab3b1-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ab3b1-120">startDateTime</span></span>|<span data-ttu-id="ab3b1-121">String</span><span class="sxs-lookup"><span data-stu-id="ab3b1-121">String</span></span>|<span data-ttu-id="ab3b1-p102">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="ab3b1-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="ab3b1-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ab3b1-124">endDateTime</span></span>|<span data-ttu-id="ab3b1-125">String</span><span class="sxs-lookup"><span data-stu-id="ab3b1-125">String</span></span>|<span data-ttu-id="ab3b1-p103">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="ab3b1-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="ab3b1-128">此方法还支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ab3b1-128">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ab3b1-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab3b1-129">Request headers</span></span>
| <span data-ttu-id="ab3b1-130">标头</span><span class="sxs-lookup"><span data-stu-id="ab3b1-130">Header</span></span>       | <span data-ttu-id="ab3b1-131">值</span><span class="sxs-lookup"><span data-stu-id="ab3b1-131">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ab3b1-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab3b1-132">Authorization</span></span>  | <span data-ttu-id="ab3b1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ab3b1-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ab3b1-135">Prefer</span><span class="sxs-lookup"><span data-stu-id="ab3b1-135">Prefer</span></span> | <span data-ttu-id="ab3b1-136">string</span><span class="sxs-lookup"><span data-stu-id="ab3b1-136">string</span></span> | <span data-ttu-id="ab3b1-p105">outlook.timezone=“东部标准时间”。可选。使用此选项指定响应中开始时间和结束时间的时区。如果未指定，则按 UTC 时间返回响应。</span><span class="sxs-lookup"><span data-stu-id="ab3b1-p105">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab3b1-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab3b1-141">Request body</span></span>
<span data-ttu-id="ab3b1-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ab3b1-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab3b1-143">响应</span><span class="sxs-lookup"><span data-stu-id="ab3b1-143">Response</span></span>

<span data-ttu-id="ab3b1-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ab3b1-144">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ab3b1-145">示例</span><span class="sxs-lookup"><span data-stu-id="ab3b1-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab3b1-146">请求</span><span class="sxs-lookup"><span data-stu-id="ab3b1-146">Request</span></span>
<span data-ttu-id="ab3b1-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ab3b1-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/calendarView
```
##### <a name="response"></a><span data-ttu-id="ab3b1-148">响应</span><span class="sxs-lookup"><span data-stu-id="ab3b1-148">Response</span></span>
<span data-ttu-id="ab3b1-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ab3b1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
