# <a name="create-thread"></a><span data-ttu-id="2416a-101">创建线程</span><span class="sxs-lookup"><span data-stu-id="2416a-101">Create thread</span></span>

<span data-ttu-id="2416a-102">在指定会话中创建新线程。</span><span class="sxs-lookup"><span data-stu-id="2416a-102">Create a new thread in the specified conversation.</span></span> 

<span data-ttu-id="2416a-p101">按指定方式创建线程和帖子。使用 [回复线程](conversationthread_reply.md) 进一步发布到该线程。或者，如果你获得帖子 ID，还可以在该线程中 [回复](post_reply.md) 帖子。</span><span class="sxs-lookup"><span data-stu-id="2416a-p101">A thread and post are created as specified. Use [reply thread](conversationthread_reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post_reply.md) to that post in that thread.</span></span>

<span data-ttu-id="2416a-106">注意：还可以 [通过首先创建一个线程启动一个新的对话](group_post_threads.md)</span><span class="sxs-lookup"><span data-stu-id="2416a-106">Note: You can also [start a new conversation by first creating a thread](group_post_threads.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2416a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2416a-107">Prerequisites</span></span>
<span data-ttu-id="2416a-108">要执行此 API，需要以下**范围**：*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="2416a-108">The following **scopes** are required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="2416a-109">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2416a-109">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="2416a-110">请求标头</span><span class="sxs-lookup"><span data-stu-id="2416a-110">Request headers</span></span>
| <span data-ttu-id="2416a-111">名称</span><span class="sxs-lookup"><span data-stu-id="2416a-111">Name</span></span>       | <span data-ttu-id="2416a-112">类型</span><span class="sxs-lookup"><span data-stu-id="2416a-112">Type</span></span> | <span data-ttu-id="2416a-113">说明</span><span class="sxs-lookup"><span data-stu-id="2416a-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2416a-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="2416a-114">Authorization</span></span>  | <span data-ttu-id="2416a-115">string</span><span class="sxs-lookup"><span data-stu-id="2416a-115">string</span></span>  | <span data-ttu-id="2416a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2416a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2416a-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="2416a-118">Request body</span></span>
<span data-ttu-id="2416a-119">在请求正文中，提供 [ConversationThread](../resources/conversationthread.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2416a-119">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2416a-120">响应</span><span class="sxs-lookup"><span data-stu-id="2416a-120">Response</span></span>

<span data-ttu-id="2416a-121">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [ConversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2416a-121">If successful, this method returns `201, Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2416a-122">示例</span><span class="sxs-lookup"><span data-stu-id="2416a-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2416a-123">请求</span><span class="sxs-lookup"><span data-stu-id="2416a-123">Request</span></span>
<span data-ttu-id="2416a-124">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2416a-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_conversation"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
Content-type: application/json

{
  "topic": "topic-value",
  "posts": [{
      "body": {
        "contentType": "html",
        "content": "this is body content"
      }
  }]
}
```
<span data-ttu-id="2416a-125">在请求正文中，提供 [ConversationThread](../resources/conversationthread.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2416a-125">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2416a-126">响应</span><span class="sxs-lookup"><span data-stu-id="2416a-126">Response</span></span>

<span data-ttu-id="2416a-p103">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和新线程的 `id`。下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2416a-p103">If successful, this method returns `201, Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 346

{
  "id": "thread-id-value"
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
