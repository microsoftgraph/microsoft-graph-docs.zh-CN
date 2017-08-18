# <a name="conversationthread-reply"></a><span data-ttu-id="53788-101">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="53788-101">conversationThread: reply</span></span>

<span data-ttu-id="53788-p101">回复组对话中的线程并向其添加新帖子。可以在请求中指定父对话，也可以指定线程，而不指定父对话。</span><span class="sxs-lookup"><span data-stu-id="53788-p101">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53788-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="53788-104">Prerequisites</span></span>
<span data-ttu-id="53788-105">要执行此 API，需要以下**范围**之一：*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="53788-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="53788-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53788-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="53788-107">请求标头</span><span class="sxs-lookup"><span data-stu-id="53788-107">Request headers</span></span>
| <span data-ttu-id="53788-108">标头</span><span class="sxs-lookup"><span data-stu-id="53788-108">Header</span></span>       | <span data-ttu-id="53788-109">值</span><span class="sxs-lookup"><span data-stu-id="53788-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="53788-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="53788-110">Authorization</span></span>  | <span data-ttu-id="53788-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53788-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="53788-113">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53788-113">Content-Type</span></span>  | <span data-ttu-id="53788-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="53788-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="53788-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="53788-116">Request body</span></span>
<span data-ttu-id="53788-117">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="53788-117">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="53788-118">参数</span><span class="sxs-lookup"><span data-stu-id="53788-118">Parameter</span></span>    | <span data-ttu-id="53788-119">类型</span><span class="sxs-lookup"><span data-stu-id="53788-119">Type</span></span>   |<span data-ttu-id="53788-120">说明</span><span class="sxs-lookup"><span data-stu-id="53788-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53788-121">帖子</span><span class="sxs-lookup"><span data-stu-id="53788-121">post</span></span>|[<span data-ttu-id="53788-122">帖子</span><span class="sxs-lookup"><span data-stu-id="53788-122">post</span></span>](../resources/post.md)|<span data-ttu-id="53788-123">正在回复的新帖子。</span><span class="sxs-lookup"><span data-stu-id="53788-123">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="53788-124">响应</span><span class="sxs-lookup"><span data-stu-id="53788-124">Response</span></span>

<span data-ttu-id="53788-p104">如果成功，此方法返回 `202, Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="53788-p104">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53788-127">示例</span><span class="sxs-lookup"><span data-stu-id="53788-127">Example</span></span>
<span data-ttu-id="53788-128">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="53788-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="53788-129">请求</span><span class="sxs-lookup"><span data-stu-id="53788-129">Request</span></span>
<span data-ttu-id="53788-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53788-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    }
  }
}
```

##### <a name="response"></a><span data-ttu-id="53788-131">响应</span><span class="sxs-lookup"><span data-stu-id="53788-131">Response</span></span>
<span data-ttu-id="53788-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="53788-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
