# <a name="post-reply"></a><span data-ttu-id="a9ff0-101">post: reply</span><span class="sxs-lookup"><span data-stu-id="a9ff0-101">post: reply</span></span>

<span data-ttu-id="a9ff0-p101">回复帖子，并向组对话中的指定线程添加新帖子。可以在请求中同时指定父对话和线程，或者仅指定父线程，而不指定父对话。</span><span class="sxs-lookup"><span data-stu-id="a9ff0-p101">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9ff0-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="a9ff0-104">Prerequisites</span></span>
<span data-ttu-id="a9ff0-105">要执行此 API，需要以下**范围**之一：</span><span class="sxs-lookup"><span data-stu-id="a9ff0-105">One of the following **scopes** is required to execute this API:</span></span>

<span data-ttu-id="a9ff0-106">*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="a9ff0-106">*Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="a9ff0-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9ff0-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="a9ff0-108">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9ff0-108">Request headers</span></span>
| <span data-ttu-id="a9ff0-109">标头</span><span class="sxs-lookup"><span data-stu-id="a9ff0-109">Header</span></span>       | <span data-ttu-id="a9ff0-110">值</span><span class="sxs-lookup"><span data-stu-id="a9ff0-110">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a9ff0-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9ff0-111">Authorization</span></span>  | <span data-ttu-id="a9ff0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a9ff0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a9ff0-114">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9ff0-114">Request body</span></span>
<span data-ttu-id="a9ff0-115">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a9ff0-115">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a9ff0-116">参数</span><span class="sxs-lookup"><span data-stu-id="a9ff0-116">Parameter</span></span>    | <span data-ttu-id="a9ff0-117">类型</span><span class="sxs-lookup"><span data-stu-id="a9ff0-117">Type</span></span>   |<span data-ttu-id="a9ff0-118">说明</span><span class="sxs-lookup"><span data-stu-id="a9ff0-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9ff0-119">帖子</span><span class="sxs-lookup"><span data-stu-id="a9ff0-119">post</span></span>|[<span data-ttu-id="a9ff0-120">帖子</span><span class="sxs-lookup"><span data-stu-id="a9ff0-120">post</span></span>](../resources/post.md)|<span data-ttu-id="a9ff0-121">正在回复的新帖子。</span><span class="sxs-lookup"><span data-stu-id="a9ff0-121">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="a9ff0-122">响应</span><span class="sxs-lookup"><span data-stu-id="a9ff0-122">Response</span></span>

<span data-ttu-id="a9ff0-p103">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a9ff0-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9ff0-125">示例</span><span class="sxs-lookup"><span data-stu-id="a9ff0-125">Example</span></span>
<span data-ttu-id="a9ff0-126">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a9ff0-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a9ff0-127">请求</span><span class="sxs-lookup"><span data-stu-id="a9ff0-127">Request</span></span>
<span data-ttu-id="a9ff0-128">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a9ff0-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    },
    "receivedDateTime": "datetime-value",
    "hasAttachments": true,
    "from": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "sender": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "conversationThreadId": "conversationThreadId-value",
    "newParticipants": [
      {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      }
    ],
    "conversationId": "conversationId-value",
    "createdDateTime": "datetime-value",
    "lastModifiedDateTime": "datetime-value",
    "changeKey": "changeKey-value",
    "categories": [
      "categories-value"
    ],
    "id": "id-value",
    "inReplyTo": {
    },
    "attachments": [
      {
        "lastModifiedDateTime": "datetime-value",
        "name": "name-value",
        "contentType": "contentType-value",
        "size": 99,
        "isInline": true,
        "id": "id-value"
      }
    ]
  }
}
```

##### <a name="response"></a><span data-ttu-id="a9ff0-129">响应</span><span class="sxs-lookup"><span data-stu-id="a9ff0-129">Response</span></span>
##### <a name="response"></a><span data-ttu-id="a9ff0-130">响应</span><span class="sxs-lookup"><span data-stu-id="a9ff0-130">Response</span></span>
<span data-ttu-id="a9ff0-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a9ff0-131">Here is an example of the response.</span></span>
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
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
