# <a name="event-accept"></a><span data-ttu-id="53a9a-101">event: accept</span><span class="sxs-lookup"><span data-stu-id="53a9a-101">event: accept</span></span>

<span data-ttu-id="53a9a-102">接受指定的事件。</span><span class="sxs-lookup"><span data-stu-id="53a9a-102">Accept the specified event.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53a9a-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="53a9a-103">Prerequisites</span></span>
<span data-ttu-id="53a9a-104">要执行此 API，需要以下**范围**之一：*Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="53a9a-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="53a9a-105">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53a9a-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/accept
POST /users/{id | userPrincipalName}/events/{id}/accept
POST /groups/{id}/events/{id}/accept

POST /me/calendar/events/{id}/accept
POST /users/{id | userPrincipalName}/calendar/events/{id}/accept
POST /groups/{id}/calendar/events/{id}/accept

POST /me/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/accept

POST /me/calendargroup/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/accept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/accept
```
## <a name="request-headers"></a><span data-ttu-id="53a9a-106">请求标头</span><span class="sxs-lookup"><span data-stu-id="53a9a-106">Request headers</span></span>
| <span data-ttu-id="53a9a-107">名称</span><span class="sxs-lookup"><span data-stu-id="53a9a-107">Name</span></span>       | <span data-ttu-id="53a9a-108">类型</span><span class="sxs-lookup"><span data-stu-id="53a9a-108">Type</span></span> | <span data-ttu-id="53a9a-109">说明</span><span class="sxs-lookup"><span data-stu-id="53a9a-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="53a9a-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="53a9a-110">Authorization</span></span>  | <span data-ttu-id="53a9a-111">string</span><span class="sxs-lookup"><span data-stu-id="53a9a-111">string</span></span>  | <span data-ttu-id="53a9a-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53a9a-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53a9a-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53a9a-114">Content-Type</span></span> | <span data-ttu-id="53a9a-115">string</span><span class="sxs-lookup"><span data-stu-id="53a9a-115">string</span></span>  | <span data-ttu-id="53a9a-p102">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="53a9a-p102">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53a9a-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="53a9a-118">Request body</span></span>
<span data-ttu-id="53a9a-119">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="53a9a-119">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="53a9a-120">参数</span><span class="sxs-lookup"><span data-stu-id="53a9a-120">Parameter</span></span>    | <span data-ttu-id="53a9a-121">类型</span><span class="sxs-lookup"><span data-stu-id="53a9a-121">Type</span></span>   |<span data-ttu-id="53a9a-122">说明</span><span class="sxs-lookup"><span data-stu-id="53a9a-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53a9a-123">注释</span><span class="sxs-lookup"><span data-stu-id="53a9a-123">comment</span></span>|<span data-ttu-id="53a9a-124">String</span><span class="sxs-lookup"><span data-stu-id="53a9a-124">String</span></span>|<span data-ttu-id="53a9a-p103">响应中包含的文本。可选。</span><span class="sxs-lookup"><span data-stu-id="53a9a-p103">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="53a9a-127">sendResponse</span><span class="sxs-lookup"><span data-stu-id="53a9a-127">sendResponse</span></span>|<span data-ttu-id="53a9a-128">布尔</span><span class="sxs-lookup"><span data-stu-id="53a9a-128">Boolean</span></span>|<span data-ttu-id="53a9a-p104">如果将响应发送给组织者，则值为 `true`；否则为 `false`。可选。默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="53a9a-p104">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="53a9a-132">响应</span><span class="sxs-lookup"><span data-stu-id="53a9a-132">Response</span></span>

<span data-ttu-id="53a9a-p105">如果成功，此方法返回 `202, Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="53a9a-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53a9a-135">示例</span><span class="sxs-lookup"><span data-stu-id="53a9a-135">Example</span></span>
<span data-ttu-id="53a9a-136">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="53a9a-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="53a9a-137">请求</span><span class="sxs-lookup"><span data-stu-id="53a9a-137">Request</span></span>
<span data-ttu-id="53a9a-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53a9a-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_accept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/accept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <a name="response"></a><span data-ttu-id="53a9a-139">响应</span><span class="sxs-lookup"><span data-stu-id="53a9a-139">Response</span></span>
<span data-ttu-id="53a9a-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="53a9a-140">Here is an example of the response.</span></span>
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
  "description": "event: accept",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
