# <a name="message-forward"></a><span data-ttu-id="2d142-101">邮件：转发</span><span class="sxs-lookup"><span data-stu-id="2d142-101">message: forward</span></span>

<span data-ttu-id="2d142-p101">转发邮件。邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="2d142-p101">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d142-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="2d142-104">Prerequisites</span></span>
<span data-ttu-id="2d142-105">要执行此 API，需要以下**范围**之一：*Mail.Send*</span><span class="sxs-lookup"><span data-stu-id="2d142-105">One of the following **scopes** is required to execute this API: *Mail.Send*</span></span>
## <a name="http-request"></a><span data-ttu-id="2d142-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d142-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="2d142-107">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d142-107">Request headers</span></span>
| <span data-ttu-id="2d142-108">名称</span><span class="sxs-lookup"><span data-stu-id="2d142-108">Name</span></span>       | <span data-ttu-id="2d142-109">类型</span><span class="sxs-lookup"><span data-stu-id="2d142-109">Type</span></span> | <span data-ttu-id="2d142-110">说明</span><span class="sxs-lookup"><span data-stu-id="2d142-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2d142-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d142-111">Authorization</span></span>  | <span data-ttu-id="2d142-112">string</span><span class="sxs-lookup"><span data-stu-id="2d142-112">string</span></span>  | <span data-ttu-id="2d142-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2d142-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2d142-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d142-115">Content-Type</span></span> | <span data-ttu-id="2d142-116">string</span><span class="sxs-lookup"><span data-stu-id="2d142-116">string</span></span>  | <span data-ttu-id="2d142-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="2d142-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d142-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d142-119">Request body</span></span>
<span data-ttu-id="2d142-120">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2d142-120">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2d142-121">参数</span><span class="sxs-lookup"><span data-stu-id="2d142-121">Parameter</span></span>    | <span data-ttu-id="2d142-122">类型</span><span class="sxs-lookup"><span data-stu-id="2d142-122">Type</span></span>   |<span data-ttu-id="2d142-123">说明</span><span class="sxs-lookup"><span data-stu-id="2d142-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d142-124">注释</span><span class="sxs-lookup"><span data-stu-id="2d142-124">comment</span></span>|<span data-ttu-id="2d142-125">String</span><span class="sxs-lookup"><span data-stu-id="2d142-125">String</span></span>|<span data-ttu-id="2d142-p104">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="2d142-p104">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="2d142-128">toRecipients</span><span class="sxs-lookup"><span data-stu-id="2d142-128">toRecipients</span></span>|<span data-ttu-id="2d142-129">[Recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="2d142-129">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="2d142-130">收件人列表</span><span class="sxs-lookup"><span data-stu-id="2d142-130">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="2d142-131">响应</span><span class="sxs-lookup"><span data-stu-id="2d142-131">Response</span></span>

<span data-ttu-id="2d142-p105">如果成功，此方法返回 `202, Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2d142-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d142-134">示例</span><span class="sxs-lookup"><span data-stu-id="2d142-134">Example</span></span>
<span data-ttu-id="2d142-135">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2d142-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2d142-136">请求</span><span class="sxs-lookup"><span data-stu-id="2d142-136">Request</span></span>
<span data-ttu-id="2d142-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2d142-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="2d142-138">响应</span><span class="sxs-lookup"><span data-stu-id="2d142-138">Response</span></span>
##### <a name="response"></a><span data-ttu-id="2d142-139">响应</span><span class="sxs-lookup"><span data-stu-id="2d142-139">Response</span></span>
<span data-ttu-id="2d142-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2d142-140">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
