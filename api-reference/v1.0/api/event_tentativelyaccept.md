# <a name="event-tentativelyaccept"></a><span data-ttu-id="18cc7-101">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="18cc7-101">event: tentativelyAccept</span></span>

<span data-ttu-id="18cc7-102">暂时接受指定的事件。</span><span class="sxs-lookup"><span data-stu-id="18cc7-102">Tentatively accept the specified event.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18cc7-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="18cc7-103">Prerequisites</span></span>
<span data-ttu-id="18cc7-104">要执行此 API，需要以下**范围**之一：*Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="18cc7-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="18cc7-105">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18cc7-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/events/{id}/tentativelyAccept
POST /groups/{id}/events/{id}/tentativelyAccept

POST /me/calendar/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendar/events/{id}/tentativelyAccept
POST /groups/{id}/calendar/events/{id}/tentativelyAccept

POST /me/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroup/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
```
## <a name="request-headers"></a><span data-ttu-id="18cc7-106">请求标头</span><span class="sxs-lookup"><span data-stu-id="18cc7-106">Request headers</span></span>
| <span data-ttu-id="18cc7-107">名称</span><span class="sxs-lookup"><span data-stu-id="18cc7-107">Name</span></span>       | <span data-ttu-id="18cc7-108">类型</span><span class="sxs-lookup"><span data-stu-id="18cc7-108">Type</span></span> | <span data-ttu-id="18cc7-109">说明</span><span class="sxs-lookup"><span data-stu-id="18cc7-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="18cc7-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="18cc7-110">Authorization</span></span>  | <span data-ttu-id="18cc7-111">string</span><span class="sxs-lookup"><span data-stu-id="18cc7-111">string</span></span>  | <span data-ttu-id="18cc7-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="18cc7-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18cc7-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18cc7-114">Content-Type</span></span> | <span data-ttu-id="18cc7-115">string</span><span class="sxs-lookup"><span data-stu-id="18cc7-115">string</span></span>  | <span data-ttu-id="18cc7-p102">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="18cc7-p102">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18cc7-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="18cc7-118">Request body</span></span>
<span data-ttu-id="18cc7-119">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="18cc7-119">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="18cc7-120">参数</span><span class="sxs-lookup"><span data-stu-id="18cc7-120">Parameter</span></span>    | <span data-ttu-id="18cc7-121">类型</span><span class="sxs-lookup"><span data-stu-id="18cc7-121">Type</span></span>   |<span data-ttu-id="18cc7-122">说明</span><span class="sxs-lookup"><span data-stu-id="18cc7-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18cc7-123">注释</span><span class="sxs-lookup"><span data-stu-id="18cc7-123">comment</span></span>|<span data-ttu-id="18cc7-124">String</span><span class="sxs-lookup"><span data-stu-id="18cc7-124">String</span></span>|<span data-ttu-id="18cc7-p103">响应中包含的文本。可选。</span><span class="sxs-lookup"><span data-stu-id="18cc7-p103">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="18cc7-127">sendResponse</span><span class="sxs-lookup"><span data-stu-id="18cc7-127">sendResponse</span></span>|<span data-ttu-id="18cc7-128">布尔</span><span class="sxs-lookup"><span data-stu-id="18cc7-128">Boolean</span></span>|<span data-ttu-id="18cc7-p104">如果将响应发送给组织者，则值为 `true`；否则为 `false`。可选。默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="18cc7-p104">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="18cc7-132">响应</span><span class="sxs-lookup"><span data-stu-id="18cc7-132">Response</span></span>

<span data-ttu-id="18cc7-p105">如果成功，此方法返回 `202, Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="18cc7-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18cc7-135">示例</span><span class="sxs-lookup"><span data-stu-id="18cc7-135">Example</span></span>
<span data-ttu-id="18cc7-136">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="18cc7-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="18cc7-137">请求</span><span class="sxs-lookup"><span data-stu-id="18cc7-137">Request</span></span>
<span data-ttu-id="18cc7-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="18cc7-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/tentativelyAccept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <a name="response"></a><span data-ttu-id="18cc7-139">响应</span><span class="sxs-lookup"><span data-stu-id="18cc7-139">Response</span></span>
##### <a name="response"></a><span data-ttu-id="18cc7-140">响应</span><span class="sxs-lookup"><span data-stu-id="18cc7-140">Response</span></span>
<span data-ttu-id="18cc7-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="18cc7-141">Here is an example of the response.</span></span>
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
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
