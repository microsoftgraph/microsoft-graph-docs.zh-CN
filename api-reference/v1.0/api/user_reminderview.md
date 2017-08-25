# <a name="user-reminderview"></a><span data-ttu-id="01e70-101">user: reminderView</span><span class="sxs-lookup"><span data-stu-id="01e70-101">user: reminderView</span></span>
<span data-ttu-id="01e70-102">返回指定开始时间和结束时间范围内的日历提醒列表。</span><span class="sxs-lookup"><span data-stu-id="01e70-102">Return a list of calendar reminders within the specified start and end times.</span></span> 

## <a name="permissions"></a><span data-ttu-id="01e70-103">权限</span><span class="sxs-lookup"><span data-stu-id="01e70-103">Permissions</span></span>
<span data-ttu-id="01e70-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="01e70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="01e70-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="01e70-106">Permission type</span></span>      | <span data-ttu-id="01e70-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01e70-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="01e70-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01e70-108">Delegated (work or school account)</span></span> | <span data-ttu-id="01e70-109">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01e70-109">Calendars.Read, Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="01e70-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01e70-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01e70-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01e70-111">Calendars.Read, Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="01e70-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="01e70-112">Application</span></span> | <span data-ttu-id="01e70-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01e70-113">Calendars.Read, Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="01e70-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01e70-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a><span data-ttu-id="01e70-115">函数参数</span><span class="sxs-lookup"><span data-stu-id="01e70-115">Function Parameters</span></span>
<span data-ttu-id="01e70-116">在请求 URL 中，提供以下包含值的函数参数。</span><span class="sxs-lookup"><span data-stu-id="01e70-116">In the request URL, provide the following function parameters with values.</span></span>

| <span data-ttu-id="01e70-117">参数</span><span class="sxs-lookup"><span data-stu-id="01e70-117">Parameter</span></span>    | <span data-ttu-id="01e70-118">类型</span><span class="sxs-lookup"><span data-stu-id="01e70-118">Type</span></span>   |<span data-ttu-id="01e70-119">说明</span><span class="sxs-lookup"><span data-stu-id="01e70-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01e70-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="01e70-120">startDateTime</span></span>|<span data-ttu-id="01e70-121">String</span><span class="sxs-lookup"><span data-stu-id="01e70-121">String</span></span>|<span data-ttu-id="01e70-p102">事件（已设置提醒）的开始日期和时间。该值用 ISO 8601 格式表示，例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="01e70-p102">The start date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="01e70-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="01e70-124">endDateTime</span></span>|<span data-ttu-id="01e70-125">String</span><span class="sxs-lookup"><span data-stu-id="01e70-125">String</span></span>|<span data-ttu-id="01e70-p103">事件（已设置提醒）的结束日期和时间。该值用 ISO 8601 格式表示，例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="01e70-p103">The end date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T20:00:00.0000000".</span></span>|


## <a name="request-headers"></a><span data-ttu-id="01e70-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="01e70-128">Request headers</span></span>
| <span data-ttu-id="01e70-129">标头</span><span class="sxs-lookup"><span data-stu-id="01e70-129">Header</span></span>       | <span data-ttu-id="01e70-130">值</span><span class="sxs-lookup"><span data-stu-id="01e70-130">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="01e70-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="01e70-131">Authorization</span></span>  | <span data-ttu-id="01e70-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01e70-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="01e70-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="01e70-134">Content-Type</span></span>   | <span data-ttu-id="01e70-135">application/json</span><span class="sxs-lookup"><span data-stu-id="01e70-135">application/json</span></span> |
| <span data-ttu-id="01e70-136">Prefer</span><span class="sxs-lookup"><span data-stu-id="01e70-136">Prefer</span></span> | <span data-ttu-id="01e70-p105">{Time-zone}。可选，如果缺省，则采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="01e70-p105">{Time-zone}. Optional, UTC assumed if absent.</span></span>| 

## <a name="request-body"></a><span data-ttu-id="01e70-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="01e70-139">Request body</span></span>
<span data-ttu-id="01e70-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="01e70-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01e70-141">响应</span><span class="sxs-lookup"><span data-stu-id="01e70-141">Response</span></span>

<span data-ttu-id="01e70-142">如果成功，此方法在响应正文中返回 `200, OK` 响应代码和 [reminder](../resources/reminder.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="01e70-142">If successful, this method returns `200, OK` response code and [reminder](../resources/reminder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01e70-143">示例</span><span class="sxs-lookup"><span data-stu-id="01e70-143">Example</span></span>
<span data-ttu-id="01e70-144">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="01e70-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="01e70-145">请求</span><span class="sxs-lookup"><span data-stu-id="01e70-145">Request</span></span>
<span data-ttu-id="01e70-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01e70-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')
```

##### <a name="response"></a><span data-ttu-id="01e70-147">响应</span><span class="sxs-lookup"><span data-stu-id="01e70-147">Response</span></span>
<span data-ttu-id="01e70-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="01e70-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reminder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 673

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.reminder)",
    "value": [
        {
            "eventId": "AAMkADNsvAAA=",
            "changeKey": "SuFHwDRP1EeXJUopWbSLlgAAmBvk2g==",
            "eventSubject": "Plan summer company picnic",
            "eventWebLink": "https://outlook.office365.com/owa/?itemid=AAMkADNsvAAA%3D&exvsurl=1&path=/calendar/item",
            "eventStartTime": {
                "dateTime": "2017-06-09T18:00:00.0000000",
                "timeZone": "UTC"
            },
            "eventEndTime": {
                "dateTime": "2017-06-09T19:00:00.0000000",
                "timeZone": "UTC"
            },
            "eventLocation": {
                "displayName": "Conf Room 3"
            },
            "reminderFireTime": {
                "dateTime": "2017-06-09T17:45:00.0000000",
                "timeZone": "UTC"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: reminderView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
