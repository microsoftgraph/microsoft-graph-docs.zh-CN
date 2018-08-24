# <a name="event-dismissreminder"></a><span data-ttu-id="befc4-101">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="befc4-101">event: dismissReminder</span></span>

<span data-ttu-id="befc4-102">忽略关于用户 [日历](../resources/calendar.md)中的 [事件](../resources/event.md)被触发的提醒。</span><span class="sxs-lookup"><span data-stu-id="befc4-102">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="befc4-103">权限</span><span class="sxs-lookup"><span data-stu-id="befc4-103">Permissions</span></span>
<span data-ttu-id="befc4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="befc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="befc4-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="befc4-106">Permission type</span></span>      | <span data-ttu-id="befc4-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="befc4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="befc4-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="befc4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="befc4-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="befc4-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="befc4-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="befc4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="befc4-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="befc4-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="befc4-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="befc4-112">Application</span></span> | <span data-ttu-id="befc4-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="befc4-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="befc4-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="befc4-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/events/{id}/dismissReminder

POST /me/calendar/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/dismissReminder

POST /me/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroup/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="befc4-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="befc4-115">Request headers</span></span>
| <span data-ttu-id="befc4-116">名称</span><span class="sxs-lookup"><span data-stu-id="befc4-116">Name</span></span>       | <span data-ttu-id="befc4-117">类型</span><span class="sxs-lookup"><span data-stu-id="befc4-117">Type</span></span> | <span data-ttu-id="befc4-118">说明</span><span class="sxs-lookup"><span data-stu-id="befc4-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="befc4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="befc4-119">Authorization</span></span>  | <span data-ttu-id="befc4-120">字符串</span><span class="sxs-lookup"><span data-stu-id="befc4-120">string</span></span>  | <span data-ttu-id="befc4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="befc4-p102">Bearer {token}. Required.</span></span> |

<br/>

## <a name="response"></a><span data-ttu-id="befc4-123">响应</span><span class="sxs-lookup"><span data-stu-id="befc4-123">Response</span></span>

<span data-ttu-id="befc4-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="befc4-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="befc4-126">示例</span><span class="sxs-lookup"><span data-stu-id="befc4-126">Example</span></span>

<span data-ttu-id="befc4-127">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="befc4-127">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="befc4-128">请求</span><span class="sxs-lookup"><span data-stu-id="befc4-128">Request</span></span>
<span data-ttu-id="befc4-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="befc4-129">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```

<br/>

### <a name="response"></a><span data-ttu-id="befc4-130">响应</span><span class="sxs-lookup"><span data-stu-id="befc4-130">Response</span></span>
<span data-ttu-id="befc4-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="befc4-131">Here is an example of the response.</span></span>

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
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
