# <a name="message-send"></a><span data-ttu-id="95688-101">邮件：发送</span><span class="sxs-lookup"><span data-stu-id="95688-101">message: send</span></span>

<span data-ttu-id="95688-p101">在草稿箱文件夹中发送邮件。邮件草稿可以是新邮件草稿、答复草稿、全部答复草稿或转发草稿。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="95688-p101">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95688-105">先决条件</span><span class="sxs-lookup"><span data-stu-id="95688-105">Prerequisites</span></span>
<span data-ttu-id="95688-106">要执行此 API，需要以下**范围**之一：*Mail.Send*</span><span class="sxs-lookup"><span data-stu-id="95688-106">One of the following **scopes** is required to execute this API: *Mail.Send*</span></span>
## <a name="http-request"></a><span data-ttu-id="95688-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95688-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```
## <a name="request-headers"></a><span data-ttu-id="95688-108">请求标头</span><span class="sxs-lookup"><span data-stu-id="95688-108">Request headers</span></span>
| <span data-ttu-id="95688-109">名称</span><span class="sxs-lookup"><span data-stu-id="95688-109">Name</span></span>       | <span data-ttu-id="95688-110">类型</span><span class="sxs-lookup"><span data-stu-id="95688-110">Type</span></span> | <span data-ttu-id="95688-111">说明</span><span class="sxs-lookup"><span data-stu-id="95688-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="95688-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="95688-112">Authorization</span></span>  | <span data-ttu-id="95688-113">string</span><span class="sxs-lookup"><span data-stu-id="95688-113">string</span></span>  | <span data-ttu-id="95688-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="95688-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95688-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="95688-116">Request body</span></span>

## <a name="response"></a><span data-ttu-id="95688-117">响应</span><span class="sxs-lookup"><span data-stu-id="95688-117">Response</span></span>

<span data-ttu-id="95688-p103">如果成功，此方法返回 `202, Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="95688-p103">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95688-120">示例</span><span class="sxs-lookup"><span data-stu-id="95688-120">Example</span></span>
<span data-ttu-id="95688-121">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="95688-121">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="95688-122">请求</span><span class="sxs-lookup"><span data-stu-id="95688-122">Request</span></span>
<span data-ttu-id="95688-123">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="95688-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="95688-124">响应</span><span class="sxs-lookup"><span data-stu-id="95688-124">Response</span></span>
##### <a name="response"></a><span data-ttu-id="95688-125">响应</span><span class="sxs-lookup"><span data-stu-id="95688-125">Response</span></span>
<span data-ttu-id="95688-126">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="95688-126">Here is an example of the response.</span></span>
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
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
