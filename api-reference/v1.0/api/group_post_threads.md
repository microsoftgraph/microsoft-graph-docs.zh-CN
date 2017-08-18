# <a name="create-conversation-thread"></a><span data-ttu-id="bbcb3-101">创建对话线程</span><span class="sxs-lookup"><span data-stu-id="bbcb3-101">Create conversation thread</span></span>

<span data-ttu-id="bbcb3-102">首先，通过创建线程来启动新的组对话。</span><span class="sxs-lookup"><span data-stu-id="bbcb3-102">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="bbcb3-p101">创建新会话、会话线程，然后可在组中创建帖子。使用 [回复线程](conversationthread_reply.md) 或 [回复帖子](post_reply.md) 进一步发布到该线程。</span><span class="sxs-lookup"><span data-stu-id="bbcb3-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread_reply.md) or [reply post](post_reply.md) to further post to that thread.</span></span>

<span data-ttu-id="bbcb3-105">注意：你还可以 [在现有会话中启动新线程](conversation_post_threads.md)。</span><span class="sxs-lookup"><span data-stu-id="bbcb3-105">Note: You can also [start a new thread in an existing conversation](conversation_post_threads.md).</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="bbcb3-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="bbcb3-106">Prerequisites</span></span>
<span data-ttu-id="bbcb3-107">要执行此 API，需要以下**范围**之一：*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="bbcb3-107">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="bbcb3-108">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bbcb3-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="bbcb3-109">请求标头</span><span class="sxs-lookup"><span data-stu-id="bbcb3-109">Request headers</span></span>
| <span data-ttu-id="bbcb3-110">标头</span><span class="sxs-lookup"><span data-stu-id="bbcb3-110">Header</span></span>       | <span data-ttu-id="bbcb3-111">值</span><span class="sxs-lookup"><span data-stu-id="bbcb3-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bbcb3-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbcb3-112">Authorization</span></span>  | <span data-ttu-id="bbcb3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bbcb3-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bbcb3-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bbcb3-115">Content-Type</span></span>  | <span data-ttu-id="bbcb3-116">application/json</span><span class="sxs-lookup"><span data-stu-id="bbcb3-116">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bbcb3-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="bbcb3-117">Request body</span></span>
<span data-ttu-id="bbcb3-118">在请求正文中，提供代表包括 [帖子](../resources/post.md) 的 [conversationThread](../resources/conversationthread.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bbcb3-118">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="bbcb3-119">响应</span><span class="sxs-lookup"><span data-stu-id="bbcb3-119">Response</span></span>

<span data-ttu-id="bbcb3-120">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [conversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bbcb3-120">If successful, this method returns `201, Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbcb3-121">示例</span><span class="sxs-lookup"><span data-stu-id="bbcb3-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bbcb3-122">请求</span><span class="sxs-lookup"><span data-stu-id="bbcb3-122">Request</span></span>
<span data-ttu-id="bbcb3-123">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bbcb3-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads
Content-type: application/json

{
  "topic": "New Conversation Thread Topic",
  "posts": [{
    "body": {
      "contentType": "html",
      "content": "this is body content"
    },
    "newParticipants": [{
      "emailAddress": {
        "name": "Alex Darrow",
        "address": "alexd@contoso.com"
      }
    }]
  }]
}
```
##### <a name="response"></a><span data-ttu-id="bbcb3-124">响应</span><span class="sxs-lookup"><span data-stu-id="bbcb3-124">Response</span></span>
<span data-ttu-id="bbcb3-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bbcb3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
