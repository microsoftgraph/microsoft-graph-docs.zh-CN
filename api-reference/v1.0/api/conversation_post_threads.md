# <a name="create-thread"></a><span data-ttu-id="3e87b-101">创建线程</span><span class="sxs-lookup"><span data-stu-id="3e87b-101">Create thread</span></span>

<span data-ttu-id="3e87b-102">在指定会话中创建新线程。</span><span class="sxs-lookup"><span data-stu-id="3e87b-102">Create a new thread in the specified conversation.</span></span> 

<span data-ttu-id="3e87b-p101">按指定方式创建线程和帖子。使用 [回复线程](conversationthread_reply.md) 进一步发布到该线程。或者，如果你获得帖子 ID，还可以在该线程中 [回复](post_reply.md) 帖子。</span><span class="sxs-lookup"><span data-stu-id="3e87b-p101">A thread and post are created as specified. Use [reply thread](conversationthread_reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post_reply.md) to that post in that thread.</span></span>

<span data-ttu-id="3e87b-106">注意：还可以 [通过首先创建一个线程启动一个新的对话](group_post_threads.md)</span><span class="sxs-lookup"><span data-stu-id="3e87b-106">Note: You can also [start a new conversation by first creating a thread](group_post_threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3e87b-107">权限</span><span class="sxs-lookup"><span data-stu-id="3e87b-107">Permissions</span></span>
<span data-ttu-id="3e87b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3e87b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3e87b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e87b-110">Permission type</span></span>      | <span data-ttu-id="3e87b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e87b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e87b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e87b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3e87b-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e87b-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3e87b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e87b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e87b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e87b-115">Not supported.</span></span>    |
|<span data-ttu-id="3e87b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e87b-116">Application</span></span> | <span data-ttu-id="3e87b-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e87b-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e87b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e87b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="3e87b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e87b-119">Request headers</span></span>
| <span data-ttu-id="3e87b-120">名称</span><span class="sxs-lookup"><span data-stu-id="3e87b-120">Name</span></span>       | <span data-ttu-id="3e87b-121">类型</span><span class="sxs-lookup"><span data-stu-id="3e87b-121">Type</span></span> | <span data-ttu-id="3e87b-122">说明</span><span class="sxs-lookup"><span data-stu-id="3e87b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3e87b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e87b-123">Authorization</span></span>  | <span data-ttu-id="3e87b-124">string</span><span class="sxs-lookup"><span data-stu-id="3e87b-124">string</span></span>  | <span data-ttu-id="3e87b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3e87b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e87b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e87b-127">Request body</span></span>
<span data-ttu-id="3e87b-128">在请求正文中，提供 [ConversationThread](../resources/conversationthread.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e87b-128">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3e87b-129">响应</span><span class="sxs-lookup"><span data-stu-id="3e87b-129">Response</span></span>

<span data-ttu-id="3e87b-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [ConversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3e87b-130">If successful, this method returns `201 Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e87b-131">示例</span><span class="sxs-lookup"><span data-stu-id="3e87b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e87b-132">请求</span><span class="sxs-lookup"><span data-stu-id="3e87b-132">Request</span></span>
<span data-ttu-id="3e87b-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3e87b-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="3e87b-134">在请求正文中，提供 [ConversationThread](../resources/conversationthread.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e87b-134">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3e87b-135">响应</span><span class="sxs-lookup"><span data-stu-id="3e87b-135">Response</span></span>

<span data-ttu-id="3e87b-p104">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和新线程的 `id`。下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3e87b-p104">If successful, this method returns `201 Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span> 
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
