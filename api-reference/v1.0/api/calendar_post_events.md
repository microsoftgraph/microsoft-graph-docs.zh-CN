# <a name="create-event"></a><span data-ttu-id="aca80-101">创建事件</span><span class="sxs-lookup"><span data-stu-id="aca80-101">Create Event</span></span>

<span data-ttu-id="aca80-102">使用此 API 在默认或指定的日历中创建新事件。</span><span class="sxs-lookup"><span data-stu-id="aca80-102">Use this API to create a new Event in the default or the specified calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="aca80-103">权限</span><span class="sxs-lookup"><span data-stu-id="aca80-103">Permissions</span></span>
<span data-ttu-id="aca80-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="aca80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aca80-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="aca80-106">Permission type</span></span>      | <span data-ttu-id="aca80-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aca80-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aca80-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aca80-108">Delegated (work or school account)</span></span> | <span data-ttu-id="aca80-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aca80-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="aca80-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aca80-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aca80-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aca80-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="aca80-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="aca80-112">Application</span></span> | <span data-ttu-id="aca80-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aca80-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="aca80-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aca80-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="aca80-115">用户或组的默认 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="aca80-115">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="aca80-116">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="aca80-116">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="aca80-117">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="aca80-117">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="aca80-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="aca80-118">Request headers</span></span>
| <span data-ttu-id="aca80-119">标头</span><span class="sxs-lookup"><span data-stu-id="aca80-119">Header</span></span>       | <span data-ttu-id="aca80-120">值</span><span class="sxs-lookup"><span data-stu-id="aca80-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aca80-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aca80-121">Authorization</span></span>  | <span data-ttu-id="aca80-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aca80-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="aca80-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aca80-124">Content-Type</span></span>  | <span data-ttu-id="aca80-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="aca80-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aca80-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="aca80-127">Request body</span></span>
<span data-ttu-id="aca80-128">在请求正文中，提供 [Event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aca80-128">In the request body, supply a JSON representation of [Event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="aca80-129">响应</span><span class="sxs-lookup"><span data-stu-id="aca80-129">Response</span></span>

<span data-ttu-id="aca80-130">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [Event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aca80-130">If successful, this method returns `201, Created` response code and [Event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aca80-131">示例</span><span class="sxs-lookup"><span data-stu-id="aca80-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aca80-132">请求</span><span class="sxs-lookup"><span data-stu-id="aca80-132">Request</span></span>
<span data-ttu-id="aca80-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aca80-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendar/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="aca80-134">在请求正文中，提供 [Event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aca80-134">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="aca80-135">响应</span><span class="sxs-lookup"><span data-stu-id="aca80-135">Response</span></span>
<span data-ttu-id="aca80-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aca80-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
