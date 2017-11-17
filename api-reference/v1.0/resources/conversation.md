# <a name="conversation-resource-type"></a><span data-ttu-id="0b945-101">对话资源类型</span><span class="sxs-lookup"><span data-stu-id="0b945-101">conversation resource type</span></span>

<span data-ttu-id="0b945-p101">对话是 [线程](conversationthread.md) 集合，而线程包含相应线程拥有的帖子。对话中的所有线程和帖子共享相同的主题。</span><span class="sxs-lookup"><span data-stu-id="0b945-p101">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

## <a name="methods"></a><span data-ttu-id="0b945-104">方法</span><span class="sxs-lookup"><span data-stu-id="0b945-104">Methods</span></span>

| <span data-ttu-id="0b945-105">方法</span><span class="sxs-lookup"><span data-stu-id="0b945-105">Method</span></span>       | <span data-ttu-id="0b945-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="0b945-106">Return Type</span></span>  |<span data-ttu-id="0b945-107">说明</span><span class="sxs-lookup"><span data-stu-id="0b945-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0b945-108">列出对话</span><span class="sxs-lookup"><span data-stu-id="0b945-108">List conversations</span></span>](../api/group_list_conversations.md) | <span data-ttu-id="0b945-109">[对话](conversation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0b945-109">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="0b945-110">获取此组中的对话列表。</span><span class="sxs-lookup"><span data-stu-id="0b945-110">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="0b945-111">创建</span><span class="sxs-lookup"><span data-stu-id="0b945-111">Create</span></span>](../api/group_post_conversations.md) |[<span data-ttu-id="0b945-112">对话</span><span class="sxs-lookup"><span data-stu-id="0b945-112">conversation</span></span>](conversation.md)| <span data-ttu-id="0b945-113">通过包括线程和帖子创建新对话。</span><span class="sxs-lookup"><span data-stu-id="0b945-113">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="0b945-114">获取对话</span><span class="sxs-lookup"><span data-stu-id="0b945-114">Get conversation</span></span>](../api/conversation_get.md) | [<span data-ttu-id="0b945-115">对话</span><span class="sxs-lookup"><span data-stu-id="0b945-115">conversation</span></span>](conversation.md) |<span data-ttu-id="0b945-116">读取 conversation 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0b945-116">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="0b945-117">删除</span><span class="sxs-lookup"><span data-stu-id="0b945-117">Delete</span></span>](../api/conversation_delete.md) | <span data-ttu-id="0b945-118">无</span><span class="sxs-lookup"><span data-stu-id="0b945-118">None</span></span> |<span data-ttu-id="0b945-119">删除 conversation 对象</span><span class="sxs-lookup"><span data-stu-id="0b945-119">Delete conversation object.</span></span> |
|[<span data-ttu-id="0b945-120">列出对话线程</span><span class="sxs-lookup"><span data-stu-id="0b945-120">List conversation threads</span></span>](../api/conversation_list_threads.md) |<span data-ttu-id="0b945-121">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0b945-121">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="0b945-122">获取组对话中的所有线程。</span><span class="sxs-lookup"><span data-stu-id="0b945-122">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="0b945-123">创建对话线程</span><span class="sxs-lookup"><span data-stu-id="0b945-123">Create conversation thread</span></span>](../api/conversation_post_threads.md) |<span data-ttu-id="0b945-124">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0b945-124">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="0b945-125">在指定会话中创建线程。</span><span class="sxs-lookup"><span data-stu-id="0b945-125">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="0b945-126">属性</span><span class="sxs-lookup"><span data-stu-id="0b945-126">Properties</span></span>
| <span data-ttu-id="0b945-127">属性</span><span class="sxs-lookup"><span data-stu-id="0b945-127">Property</span></span>     | <span data-ttu-id="0b945-128">类型</span><span class="sxs-lookup"><span data-stu-id="0b945-128">Type</span></span>   |<span data-ttu-id="0b945-129">说明</span><span class="sxs-lookup"><span data-stu-id="0b945-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b945-130">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="0b945-130">hasAttachments</span></span>|<span data-ttu-id="0b945-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b945-131">Boolean</span></span>|<span data-ttu-id="0b945-132">指示此对话中的任意帖子是否至少有一个附件。</span><span class="sxs-lookup"><span data-stu-id="0b945-132">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="0b945-133">id</span><span class="sxs-lookup"><span data-stu-id="0b945-133">id</span></span>|<span data-ttu-id="0b945-134">String</span><span class="sxs-lookup"><span data-stu-id="0b945-134">String</span></span>|<span data-ttu-id="0b945-p102">对话的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="0b945-p102">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="0b945-137">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="0b945-137">lastDeliveredDateTime</span></span>|<span data-ttu-id="0b945-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b945-138">DateTimeOffset</span></span>|<span data-ttu-id="0b945-p103">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0b945-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0b945-141">preview</span><span class="sxs-lookup"><span data-stu-id="0b945-141">preview</span></span>|<span data-ttu-id="0b945-142">String</span><span class="sxs-lookup"><span data-stu-id="0b945-142">String</span></span>|<span data-ttu-id="0b945-143">来自此对话中最新帖子的正文的简短摘要。</span><span class="sxs-lookup"><span data-stu-id="0b945-143">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="0b945-144">topic</span><span class="sxs-lookup"><span data-stu-id="0b945-144">topic</span></span>|<span data-ttu-id="0b945-145">String</span><span class="sxs-lookup"><span data-stu-id="0b945-145">String</span></span>|<span data-ttu-id="0b945-p104">对话的主题。在创建对话时可设置此属性，但无法对其进行更新。</span><span class="sxs-lookup"><span data-stu-id="0b945-p104">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="0b945-148">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="0b945-148">uniqueSenders</span></span>|<span data-ttu-id="0b945-149">String collection</span><span class="sxs-lookup"><span data-stu-id="0b945-149">String collection</span></span>|<span data-ttu-id="0b945-150">发送消息到此对话的所有用户。</span><span class="sxs-lookup"><span data-stu-id="0b945-150">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b945-151">关系</span><span class="sxs-lookup"><span data-stu-id="0b945-151">Relationships</span></span>
| <span data-ttu-id="0b945-152">关系</span><span class="sxs-lookup"><span data-stu-id="0b945-152">Relationship</span></span> | <span data-ttu-id="0b945-153">类型</span><span class="sxs-lookup"><span data-stu-id="0b945-153">Type</span></span>   |<span data-ttu-id="0b945-154">说明</span><span class="sxs-lookup"><span data-stu-id="0b945-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b945-155">线程</span><span class="sxs-lookup"><span data-stu-id="0b945-155">threads</span></span>|<span data-ttu-id="0b945-156">[conversationThread](conversationthread.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0b945-156">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="0b945-p105">对话中所有对话线程的集合。一种导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="0b945-p105">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b945-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b945-161">JSON representation</span></span>

<span data-ttu-id="0b945-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b945-162">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversation"
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
