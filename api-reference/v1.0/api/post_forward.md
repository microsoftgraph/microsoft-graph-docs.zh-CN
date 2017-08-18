# <a name="post-forward"></a><span data-ttu-id="b4679-101">帖子：转发</span><span class="sxs-lookup"><span data-stu-id="b4679-101">post: forward</span></span>

<span data-ttu-id="b4679-p101">将帖子转发给收件人。可以在请求中同时指定父对话和线程，或者仅指定父线程，而不指定父对话。</span><span class="sxs-lookup"><span data-stu-id="b4679-p101">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="b4679-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="b4679-104">Prerequisites</span></span>
<span data-ttu-id="b4679-105">要执行此 API，需要以下**范围**之一：</span><span class="sxs-lookup"><span data-stu-id="b4679-105">One of the following **scopes** is required to execute this API:</span></span>

<span data-ttu-id="b4679-106">*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="b4679-106">*Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="b4679-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4679-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="b4679-108">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4679-108">Request headers</span></span>
| <span data-ttu-id="b4679-109">标头</span><span class="sxs-lookup"><span data-stu-id="b4679-109">Header</span></span>       | <span data-ttu-id="b4679-110">值</span><span class="sxs-lookup"><span data-stu-id="b4679-110">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b4679-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4679-111">Authorization</span></span>  | <span data-ttu-id="b4679-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4679-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b4679-114">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4679-114">Request body</span></span>
<span data-ttu-id="b4679-115">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b4679-115">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b4679-116">参数</span><span class="sxs-lookup"><span data-stu-id="b4679-116">Parameter</span></span>    | <span data-ttu-id="b4679-117">类型</span><span class="sxs-lookup"><span data-stu-id="b4679-117">Type</span></span>   |<span data-ttu-id="b4679-118">说明</span><span class="sxs-lookup"><span data-stu-id="b4679-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4679-119">注释</span><span class="sxs-lookup"><span data-stu-id="b4679-119">comment</span></span>|<span data-ttu-id="b4679-120">String</span><span class="sxs-lookup"><span data-stu-id="b4679-120">String</span></span>|<span data-ttu-id="b4679-121">与帖子一起转发的可选注释。</span><span class="sxs-lookup"><span data-stu-id="b4679-121">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="b4679-122">toRecipients</span><span class="sxs-lookup"><span data-stu-id="b4679-122">toRecipients</span></span>|<span data-ttu-id="b4679-123">[收件人](../resources/recipient.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b4679-123">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="b4679-124">线程要转发至的收件人。</span><span class="sxs-lookup"><span data-stu-id="b4679-124">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="b4679-125">响应</span><span class="sxs-lookup"><span data-stu-id="b4679-125">Response</span></span>

<span data-ttu-id="b4679-p103">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b4679-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4679-128">示例</span><span class="sxs-lookup"><span data-stu-id="b4679-128">Example</span></span>
<span data-ttu-id="b4679-129">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="b4679-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b4679-130">请求</span><span class="sxs-lookup"><span data-stu-id="b4679-130">Request</span></span>
<span data-ttu-id="b4679-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b4679-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/forward
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

##### <a name="response"></a><span data-ttu-id="b4679-132">响应</span><span class="sxs-lookup"><span data-stu-id="b4679-132">Response</span></span>
<span data-ttu-id="b4679-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b4679-133">Here is an example of the response.</span></span>
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
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
