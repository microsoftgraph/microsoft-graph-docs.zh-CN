# <a name="event-accept"></a><span data-ttu-id="26685-101">event: accept</span><span class="sxs-lookup"><span data-stu-id="26685-101">event: accept</span></span>

<span data-ttu-id="26685-102">接受用户[日历](../resources/calendar.md)中指定的[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="26685-102">Accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="26685-103">权限</span><span class="sxs-lookup"><span data-stu-id="26685-103">Permissions</span></span>
<span data-ttu-id="26685-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="26685-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="26685-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="26685-106">Permission type</span></span>      | <span data-ttu-id="26685-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="26685-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26685-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26685-108">Delegated (work or school account)</span></span> | <span data-ttu-id="26685-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26685-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="26685-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26685-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26685-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26685-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="26685-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="26685-112">Application</span></span> | <span data-ttu-id="26685-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26685-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="26685-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26685-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/accept
POST /users/{id | userPrincipalName}/events/{id}/accept

POST /me/calendar/events/{id}/accept
POST /users/{id | userPrincipalName}/calendar/events/{id}/accept

POST /me/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/accept

POST /me/calendargroup/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/accept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/accept
```
## <a name="request-headers"></a><span data-ttu-id="26685-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="26685-115">Request headers</span></span>
| <span data-ttu-id="26685-116">名称</span><span class="sxs-lookup"><span data-stu-id="26685-116">Name</span></span>       | <span data-ttu-id="26685-117">类型</span><span class="sxs-lookup"><span data-stu-id="26685-117">Type</span></span> | <span data-ttu-id="26685-118">说明</span><span class="sxs-lookup"><span data-stu-id="26685-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="26685-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="26685-119">Authorization</span></span>  | <span data-ttu-id="26685-120">字符串</span><span class="sxs-lookup"><span data-stu-id="26685-120">string</span></span>  | <span data-ttu-id="26685-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="26685-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="26685-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26685-123">Content-Type</span></span> | <span data-ttu-id="26685-124">字符串</span><span class="sxs-lookup"><span data-stu-id="26685-124">string</span></span>  | <span data-ttu-id="26685-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="26685-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26685-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="26685-127">Request body</span></span>
<span data-ttu-id="26685-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="26685-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="26685-129">参数</span><span class="sxs-lookup"><span data-stu-id="26685-129">Parameter</span></span>    | <span data-ttu-id="26685-130">类型</span><span class="sxs-lookup"><span data-stu-id="26685-130">Type</span></span>   |<span data-ttu-id="26685-131">说明</span><span class="sxs-lookup"><span data-stu-id="26685-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26685-132">注释</span><span class="sxs-lookup"><span data-stu-id="26685-132">comment</span></span>|<span data-ttu-id="26685-133">字符串</span><span class="sxs-lookup"><span data-stu-id="26685-133">String</span></span>|<span data-ttu-id="26685-p104">响应中包含的文本。可选。</span><span class="sxs-lookup"><span data-stu-id="26685-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="26685-136">sendResponse</span><span class="sxs-lookup"><span data-stu-id="26685-136">sendResponse</span></span>|<span data-ttu-id="26685-137">布尔</span><span class="sxs-lookup"><span data-stu-id="26685-137">Boolean</span></span>|<span data-ttu-id="26685-p105">`true` 如果将响应发送给组织者，则值为 `true`；否则为 `false`。可选。默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="26685-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="26685-141">响应</span><span class="sxs-lookup"><span data-stu-id="26685-141">Response</span></span>

<span data-ttu-id="26685-p106">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="26685-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26685-144">示例</span><span class="sxs-lookup"><span data-stu-id="26685-144">Example</span></span>
<span data-ttu-id="26685-145">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="26685-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="26685-146">请求</span><span class="sxs-lookup"><span data-stu-id="26685-146">Request</span></span>
<span data-ttu-id="26685-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="26685-147">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="26685-148">响应</span><span class="sxs-lookup"><span data-stu-id="26685-148">Response</span></span>
<span data-ttu-id="26685-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="26685-149">Here is an example of the response.</span></span>
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
