# <a name="conversationthread-reply"></a><span data-ttu-id="2cc3a-101">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="2cc3a-101">conversationThread: reply</span></span>

<span data-ttu-id="2cc3a-p101">回复组对话中的线程并向其添加新帖子。可以在请求中指定父对话，也可以指定线程，而不指定父对话。</span><span class="sxs-lookup"><span data-stu-id="2cc3a-p101">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="2cc3a-104">权限</span><span class="sxs-lookup"><span data-stu-id="2cc3a-104">Permissions</span></span>
<span data-ttu-id="2cc3a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2cc3a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2cc3a-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="2cc3a-107">Permission type</span></span>      | <span data-ttu-id="2cc3a-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2cc3a-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2cc3a-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2cc3a-109">Delegated (work or school account)</span></span> | <span data-ttu-id="2cc3a-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cc3a-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2cc3a-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2cc3a-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2cc3a-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="2cc3a-112">Not supported.</span></span>    |
|<span data-ttu-id="2cc3a-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="2cc3a-113">Application</span></span> | <span data-ttu-id="2cc3a-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cc3a-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2cc3a-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2cc3a-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="2cc3a-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="2cc3a-116">Request headers</span></span>
| <span data-ttu-id="2cc3a-117">标头</span><span class="sxs-lookup"><span data-stu-id="2cc3a-117">Header</span></span>       | <span data-ttu-id="2cc3a-118">值</span><span class="sxs-lookup"><span data-stu-id="2cc3a-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2cc3a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cc3a-119">Authorization</span></span>  | <span data-ttu-id="2cc3a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2cc3a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2cc3a-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2cc3a-122">Content-Type</span></span>  | <span data-ttu-id="2cc3a-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2cc3a-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2cc3a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2cc3a-125">Request body</span></span>
<span data-ttu-id="2cc3a-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2cc3a-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2cc3a-127">参数</span><span class="sxs-lookup"><span data-stu-id="2cc3a-127">Parameter</span></span>    | <span data-ttu-id="2cc3a-128">类型</span><span class="sxs-lookup"><span data-stu-id="2cc3a-128">Type</span></span>   |<span data-ttu-id="2cc3a-129">说明</span><span class="sxs-lookup"><span data-stu-id="2cc3a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2cc3a-130">帖子</span><span class="sxs-lookup"><span data-stu-id="2cc3a-130">post</span></span>|[<span data-ttu-id="2cc3a-131">帖子</span><span class="sxs-lookup"><span data-stu-id="2cc3a-131">post</span></span>](../resources/post.md)|<span data-ttu-id="2cc3a-132">正在回复的新帖子。</span><span class="sxs-lookup"><span data-stu-id="2cc3a-132">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="2cc3a-133">响应</span><span class="sxs-lookup"><span data-stu-id="2cc3a-133">Response</span></span>

<span data-ttu-id="2cc3a-p105">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2cc3a-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cc3a-136">示例</span><span class="sxs-lookup"><span data-stu-id="2cc3a-136">Example</span></span>
<span data-ttu-id="2cc3a-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2cc3a-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2cc3a-138">请求</span><span class="sxs-lookup"><span data-stu-id="2cc3a-138">Request</span></span>
<span data-ttu-id="2cc3a-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2cc3a-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="2cc3a-140">响应</span><span class="sxs-lookup"><span data-stu-id="2cc3a-140">Response</span></span>
<span data-ttu-id="2cc3a-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2cc3a-141">Here is an example of the response.</span></span>
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
