# <a name="post-reply"></a><span data-ttu-id="24ac6-101">post: reply</span><span class="sxs-lookup"><span data-stu-id="24ac6-101">post: reply</span></span>

<span data-ttu-id="24ac6-p101">回复帖子，并向组对话中的指定线程添加新帖子。可以在请求中同时指定父对话和线程，或者仅指定父线程，而不指定父对话。</span><span class="sxs-lookup"><span data-stu-id="24ac6-p101">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="24ac6-104">权限</span><span class="sxs-lookup"><span data-stu-id="24ac6-104">Permissions</span></span>
<span data-ttu-id="24ac6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="24ac6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="24ac6-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="24ac6-107">Permission type</span></span>      | <span data-ttu-id="24ac6-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="24ac6-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24ac6-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24ac6-109">Delegated (work or school account)</span></span> | <span data-ttu-id="24ac6-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24ac6-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="24ac6-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24ac6-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24ac6-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="24ac6-112">Not supported.</span></span>    |
|<span data-ttu-id="24ac6-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="24ac6-113">Application</span></span> | <span data-ttu-id="24ac6-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24ac6-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="24ac6-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24ac6-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="24ac6-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="24ac6-116">Request headers</span></span>
| <span data-ttu-id="24ac6-117">标头</span><span class="sxs-lookup"><span data-stu-id="24ac6-117">Header</span></span>       | <span data-ttu-id="24ac6-118">值</span><span class="sxs-lookup"><span data-stu-id="24ac6-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="24ac6-119">授权</span><span class="sxs-lookup"><span data-stu-id="24ac6-119">Authorization</span></span>  | <span data-ttu-id="24ac6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="24ac6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="24ac6-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="24ac6-122">Request body</span></span>
<span data-ttu-id="24ac6-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="24ac6-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="24ac6-124">参数</span><span class="sxs-lookup"><span data-stu-id="24ac6-124">Parameter</span></span>    | <span data-ttu-id="24ac6-125">类型</span><span class="sxs-lookup"><span data-stu-id="24ac6-125">Type</span></span>   |<span data-ttu-id="24ac6-126">说明</span><span class="sxs-lookup"><span data-stu-id="24ac6-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24ac6-127">帖子</span><span class="sxs-lookup"><span data-stu-id="24ac6-127">post</span></span>|[<span data-ttu-id="24ac6-128">帖子</span><span class="sxs-lookup"><span data-stu-id="24ac6-128">post</span></span>](../resources/post.md)|<span data-ttu-id="24ac6-129">正在回复的新帖子。</span><span class="sxs-lookup"><span data-stu-id="24ac6-129">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="24ac6-130">响应</span><span class="sxs-lookup"><span data-stu-id="24ac6-130">Response</span></span>

<span data-ttu-id="24ac6-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="24ac6-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24ac6-133">示例</span><span class="sxs-lookup"><span data-stu-id="24ac6-133">Example</span></span>
<span data-ttu-id="24ac6-134">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="24ac6-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="24ac6-135">请求</span><span class="sxs-lookup"><span data-stu-id="24ac6-135">Request</span></span>
<span data-ttu-id="24ac6-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24ac6-136">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="24ac6-137">响应</span><span class="sxs-lookup"><span data-stu-id="24ac6-137">Response</span></span>
<span data-ttu-id="24ac6-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="24ac6-138">Here is an example of the response.</span></span>
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
