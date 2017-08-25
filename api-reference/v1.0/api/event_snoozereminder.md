# <a name="event-snoozereminder"></a><span data-ttu-id="fd07c-101">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="fd07c-101">event: snoozeReminder</span></span>

<span data-ttu-id="fd07c-102">将提醒推迟到新时间。</span><span class="sxs-lookup"><span data-stu-id="fd07c-102">Postpone a reminder until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd07c-103">权限</span><span class="sxs-lookup"><span data-stu-id="fd07c-103">Permissions</span></span>
<span data-ttu-id="fd07c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fd07c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fd07c-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd07c-106">Permission type</span></span>      | <span data-ttu-id="fd07c-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fd07c-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="fd07c-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd07c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fd07c-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd07c-109">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="fd07c-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd07c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd07c-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd07c-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="fd07c-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd07c-112">Application</span></span> | <span data-ttu-id="fd07c-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd07c-113">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fd07c-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd07c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/events/{id}/snoozeReminder
POST /groups/{id}/events/{id}/snoozeReminder

POST /me/calendar/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/snoozeReminder
POST /groups/{id}/calendar/events/{id}/snoozeReminder

POST /me/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroup/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
```
## <a name="request-headers"></a><span data-ttu-id="fd07c-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="fd07c-115">Request headers</span></span>
| <span data-ttu-id="fd07c-116">名称</span><span class="sxs-lookup"><span data-stu-id="fd07c-116">Name</span></span>       | <span data-ttu-id="fd07c-117">类型</span><span class="sxs-lookup"><span data-stu-id="fd07c-117">Type</span></span> | <span data-ttu-id="fd07c-118">说明</span><span class="sxs-lookup"><span data-stu-id="fd07c-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fd07c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd07c-119">Authorization</span></span>  | <span data-ttu-id="fd07c-120">string</span><span class="sxs-lookup"><span data-stu-id="fd07c-120">string</span></span>  | <span data-ttu-id="fd07c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fd07c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fd07c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fd07c-123">Content-Type</span></span> | <span data-ttu-id="fd07c-124">string</span><span class="sxs-lookup"><span data-stu-id="fd07c-124">string</span></span>  | <span data-ttu-id="fd07c-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="fd07c-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd07c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd07c-127">Request body</span></span>
<span data-ttu-id="fd07c-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="fd07c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fd07c-129">参数</span><span class="sxs-lookup"><span data-stu-id="fd07c-129">Parameter</span></span>    | <span data-ttu-id="fd07c-130">类型</span><span class="sxs-lookup"><span data-stu-id="fd07c-130">Type</span></span>   |<span data-ttu-id="fd07c-131">说明</span><span class="sxs-lookup"><span data-stu-id="fd07c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd07c-132">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="fd07c-132">newReminderTime</span></span>|<span data-ttu-id="fd07c-133">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="fd07c-133">DateTimeTimeZone</span></span>|<span data-ttu-id="fd07c-134">触发提醒的新日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fd07c-134">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="fd07c-135">响应</span><span class="sxs-lookup"><span data-stu-id="fd07c-135">Response</span></span>

<span data-ttu-id="fd07c-p104">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fd07c-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd07c-138">示例</span><span class="sxs-lookup"><span data-stu-id="fd07c-138">Example</span></span>
<span data-ttu-id="fd07c-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="fd07c-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fd07c-140">请求</span><span class="sxs-lookup"><span data-stu-id="fd07c-140">Request</span></span>
<span data-ttu-id="fd07c-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fd07c-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/snoozeReminder
Content-type: application/json
Content-length: 97

{
  "newReminderTime": {
    "dateTime": "dateTime-value",
    "timeZone": "timeZone-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="fd07c-142">响应</span><span class="sxs-lookup"><span data-stu-id="fd07c-142">Response</span></span>
<span data-ttu-id="fd07c-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fd07c-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
