# <a name="message-replyall"></a><span data-ttu-id="4ecc6-101">消息：replyAll</span><span class="sxs-lookup"><span data-stu-id="4ecc6-101">message: replyAll</span></span>

<span data-ttu-id="4ecc6-p101">答复邮件的所有收件人。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="4ecc6-p101">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ecc6-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="4ecc6-104">Prerequisites</span></span>
<span data-ttu-id="4ecc6-105">要执行此 API，需要以下**范围**之一：*Mail.Send*</span><span class="sxs-lookup"><span data-stu-id="4ecc6-105">One of the following **scopes** is required to execute this API: *Mail.Send*</span></span>
## <a name="http-request"></a><span data-ttu-id="4ecc6-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ecc6-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="4ecc6-107">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ecc6-107">Request headers</span></span>
| <span data-ttu-id="4ecc6-108">名称</span><span class="sxs-lookup"><span data-stu-id="4ecc6-108">Name</span></span>       | <span data-ttu-id="4ecc6-109">类型</span><span class="sxs-lookup"><span data-stu-id="4ecc6-109">Type</span></span> | <span data-ttu-id="4ecc6-110">说明</span><span class="sxs-lookup"><span data-stu-id="4ecc6-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4ecc6-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ecc6-111">Authorization</span></span>  | <span data-ttu-id="4ecc6-112">string</span><span class="sxs-lookup"><span data-stu-id="4ecc6-112">string</span></span>  | <span data-ttu-id="4ecc6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ecc6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4ecc6-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4ecc6-115">Content-Type</span></span> | <span data-ttu-id="4ecc6-116">string</span><span class="sxs-lookup"><span data-stu-id="4ecc6-116">string</span></span>  | <span data-ttu-id="4ecc6-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="4ecc6-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ecc6-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ecc6-119">Request body</span></span>
<span data-ttu-id="4ecc6-120">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4ecc6-120">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4ecc6-121">参数</span><span class="sxs-lookup"><span data-stu-id="4ecc6-121">Parameter</span></span>    | <span data-ttu-id="4ecc6-122">类型</span><span class="sxs-lookup"><span data-stu-id="4ecc6-122">Type</span></span>   |<span data-ttu-id="4ecc6-123">说明</span><span class="sxs-lookup"><span data-stu-id="4ecc6-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ecc6-124">注释</span><span class="sxs-lookup"><span data-stu-id="4ecc6-124">comment</span></span>|<span data-ttu-id="4ecc6-125">String</span><span class="sxs-lookup"><span data-stu-id="4ecc6-125">String</span></span>|<span data-ttu-id="4ecc6-p104">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="4ecc6-p104">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="4ecc6-128">响应</span><span class="sxs-lookup"><span data-stu-id="4ecc6-128">Response</span></span>

<span data-ttu-id="4ecc6-p105">如果成功，此方法返回 `202, Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4ecc6-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ecc6-131">示例</span><span class="sxs-lookup"><span data-stu-id="4ecc6-131">Example</span></span>
<span data-ttu-id="4ecc6-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="4ecc6-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4ecc6-133">请求</span><span class="sxs-lookup"><span data-stu-id="4ecc6-133">Request</span></span>
<span data-ttu-id="4ecc6-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ecc6-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/replyAll
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```


##### <a name="response"></a><span data-ttu-id="4ecc6-135">响应</span><span class="sxs-lookup"><span data-stu-id="4ecc6-135">Response</span></span>
<span data-ttu-id="4ecc6-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4ecc6-136">Here is an example of the response.</span></span>
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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
