# <a name="create-conversation"></a><span data-ttu-id="fef9c-101">创建对话</span><span class="sxs-lookup"><span data-stu-id="fef9c-101">Create Conversation</span></span>
<span data-ttu-id="fef9c-102">通过包括线程和帖子来创建新会话。</span><span class="sxs-lookup"><span data-stu-id="fef9c-102">Create a new conversation by including a thread and a post.</span></span> 

<span data-ttu-id="fef9c-103">使用[回复线程](conversationthread_reply.md)或[回复帖子](post_reply.md)进一步发布到该对话。</span><span class="sxs-lookup"><span data-stu-id="fef9c-103">Use [reply thread](conversationthread_reply.md) or [reply post](post_reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="fef9c-104">权限</span><span class="sxs-lookup"><span data-stu-id="fef9c-104">Permissions</span></span>
<span data-ttu-id="fef9c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fef9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fef9c-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="fef9c-107">Permission type</span></span>      | <span data-ttu-id="fef9c-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fef9c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fef9c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fef9c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="fef9c-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fef9c-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fef9c-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fef9c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fef9c-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="fef9c-112">Not supported.</span></span>    |
|<span data-ttu-id="fef9c-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="fef9c-113">Application</span></span> | <span data-ttu-id="fef9c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fef9c-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fef9c-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fef9c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="fef9c-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="fef9c-116">Request headers</span></span>
| <span data-ttu-id="fef9c-117">标头</span><span class="sxs-lookup"><span data-stu-id="fef9c-117">Header</span></span>       | <span data-ttu-id="fef9c-118">值</span><span class="sxs-lookup"><span data-stu-id="fef9c-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fef9c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fef9c-119">Authorization</span></span>  | <span data-ttu-id="fef9c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fef9c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fef9c-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fef9c-122">Content-Type</span></span>  | <span data-ttu-id="fef9c-123">application/json</span><span class="sxs-lookup"><span data-stu-id="fef9c-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fef9c-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="fef9c-124">Request body</span></span>
<span data-ttu-id="fef9c-125">在请求正文中，提供包括 [conversationThread](../resources/conversationThread.md) 和 [帖子](../resources/post.md) 的 [conversation](../resources/conversation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fef9c-125">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationThread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="fef9c-126">响应</span><span class="sxs-lookup"><span data-stu-id="fef9c-126">Response</span></span>
<span data-ttu-id="fef9c-127">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fef9c-127">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fef9c-128">示例</span><span class="sxs-lookup"><span data-stu-id="fef9c-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fef9c-129">请求</span><span class="sxs-lookup"><span data-stu-id="fef9c-129">Request</span></span>
<span data-ttu-id="fef9c-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fef9c-130">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/conversations
Content-type: application/json

{
  "topic": "New Conversation Topic",
  "threads": [{
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
  }]
}
```

#### <a name="response"></a><span data-ttu-id="fef9c-131">响应</span><span class="sxs-lookup"><span data-stu-id="fef9c-131">Response</span></span>
<span data-ttu-id="fef9c-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fef9c-132">Here is an example of the response.</span></span>
><span data-ttu-id="fef9c-133">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fef9c-133">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fef9c-134">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fef9c-134">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->