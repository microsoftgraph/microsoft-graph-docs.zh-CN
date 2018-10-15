# <a name="post-resource-type"></a><span data-ttu-id="d41b2-101">帖子资源类型</span><span class="sxs-lookup"><span data-stu-id="d41b2-101">post resource type</span></span>
<span data-ttu-id="d41b2-102">表示 [conversationThread](conversationthread.md) 实体中的各个帖子项。</span><span class="sxs-lookup"><span data-stu-id="d41b2-102">Represents an individual Post item within a [conversationThread](conversationthread.md) entity.</span></span>

<span data-ttu-id="d41b2-103">即使无法显式创建帖子，也可以执行以下任一操作来创建帖子：</span><span class="sxs-lookup"><span data-stu-id="d41b2-103">Even though you cannot explicitly create a post, doing any of the following would create a post:</span></span>

- [<span data-ttu-id="d41b2-104">答复现有帖子</span><span class="sxs-lookup"><span data-stu-id="d41b2-104">Reply to an existing post</span></span>](../api/post_reply.md) 
- [<span data-ttu-id="d41b2-105">答复现有线程</span><span class="sxs-lookup"><span data-stu-id="d41b2-105">Reply to an existing thread</span></span>](../api/conversationthread_reply.md) 
- [<span data-ttu-id="d41b2-106">在新对话中创建线程</span><span class="sxs-lookup"><span data-stu-id="d41b2-106">Create a thread in a new conversation</span></span>](../api/group_post_threads.md)
- [<span data-ttu-id="d41b2-107">创建新对话</span><span class="sxs-lookup"><span data-stu-id="d41b2-107">Create a new conversation</span></span>](../api/group_post_conversations.md)

<span data-ttu-id="d41b2-108">通过该资源可以使用[扩展](../../../concepts/extensibility_overview.md)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="d41b2-108">This resource lets you add your own data to custom properties using [extensions](../../../concepts/extensibility_overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d41b2-109">方法</span><span class="sxs-lookup"><span data-stu-id="d41b2-109">Methods</span></span>

| <span data-ttu-id="d41b2-110">方法</span><span class="sxs-lookup"><span data-stu-id="d41b2-110">Method</span></span>       | <span data-ttu-id="d41b2-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="d41b2-111">Return Type</span></span>  |<span data-ttu-id="d41b2-112">说明</span><span class="sxs-lookup"><span data-stu-id="d41b2-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d41b2-113">列出帖子</span><span class="sxs-lookup"><span data-stu-id="d41b2-113">List posts</span></span>](../api/conversationthread_list_posts.md) | [<span data-ttu-id="d41b2-114">帖子</span><span class="sxs-lookup"><span data-stu-id="d41b2-114">post</span></span>](post.md) |<span data-ttu-id="d41b2-115">获取指定线程的帖子。</span><span class="sxs-lookup"><span data-stu-id="d41b2-115">Get the posts of the specified thread.</span></span> |
|[<span data-ttu-id="d41b2-116">获取帖子</span><span class="sxs-lookup"><span data-stu-id="d41b2-116">Get post</span></span>](../api/post_get.md) | [<span data-ttu-id="d41b2-117">帖子</span><span class="sxs-lookup"><span data-stu-id="d41b2-117">post</span></span>](post.md) |<span data-ttu-id="d41b2-118">获取指定的线程中帖子的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d41b2-118">Get the properties and relationships of a post in a specified thread.</span></span>|
|[<span data-ttu-id="d41b2-119">答复</span><span class="sxs-lookup"><span data-stu-id="d41b2-119">Reply</span></span>](../api/post_reply.md)|<span data-ttu-id="d41b2-120">无</span><span class="sxs-lookup"><span data-stu-id="d41b2-120">None</span></span>|<span data-ttu-id="d41b2-121">在组对话中答复帖子，并向指定线程中添加新帖子。</span><span class="sxs-lookup"><span data-stu-id="d41b2-121">Reply to a post and add a new post to the specified thread in a group conversation.</span></span>|
|[<span data-ttu-id="d41b2-122">转发</span><span class="sxs-lookup"><span data-stu-id="d41b2-122">Forward</span></span>](../api/post_forward.md)|<span data-ttu-id="d41b2-123">无</span><span class="sxs-lookup"><span data-stu-id="d41b2-123">None</span></span>|<span data-ttu-id="d41b2-124">将帖子转发给收件人。</span><span class="sxs-lookup"><span data-stu-id="d41b2-124">Forward a post to a recipient.</span></span>|
|<span data-ttu-id="d41b2-125">**附件**</span><span class="sxs-lookup"><span data-stu-id="d41b2-125">**Attachments**</span></span>| | |
|[<span data-ttu-id="d41b2-126">列出附件</span><span class="sxs-lookup"><span data-stu-id="d41b2-126">List attachments</span></span>](../api/post_list_attachments.md) |<span data-ttu-id="d41b2-127">[attachment](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d41b2-127">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="d41b2-128">获取帖子的所有附件。</span><span class="sxs-lookup"><span data-stu-id="d41b2-128">Get all attachments on a post.</span></span>|
|[<span data-ttu-id="d41b2-129">添加附件</span><span class="sxs-lookup"><span data-stu-id="d41b2-129">Add attachment</span></span>](../api/post_post_attachments.md) |[<span data-ttu-id="d41b2-130">附件</span><span class="sxs-lookup"><span data-stu-id="d41b2-130">attachment</span></span>](attachment.md)| <span data-ttu-id="d41b2-131">将附件添加到帖子中。</span><span class="sxs-lookup"><span data-stu-id="d41b2-131">Add an attachment to a post.</span></span> |
|<span data-ttu-id="d41b2-132">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="d41b2-132">**Open extensions**</span></span>| | |
|[<span data-ttu-id="d41b2-133">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="d41b2-133">Create open extension</span></span>](../api/opentypeextension_post_opentypeextension.md) |[<span data-ttu-id="d41b2-134">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="d41b2-134">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="d41b2-135">创建开放扩展，并在新建或现有的资源实例中添加自定义属性。</span><span class="sxs-lookup"><span data-stu-id="d41b2-135">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="d41b2-136">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="d41b2-136">Get open extension</span></span>](../api/opentypeextension_get.md) |<span data-ttu-id="d41b2-137">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d41b2-137">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="d41b2-138">获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。</span><span class="sxs-lookup"><span data-stu-id="d41b2-138">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="d41b2-139">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="d41b2-139">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="d41b2-140">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="d41b2-140">Add schema extension values</span></span>](../../../concepts/extensibility_schema_groups.md) || <span data-ttu-id="d41b2-141">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="d41b2-141">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="d41b2-142">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="d41b2-142">**Extended properties**</span></span>| | |
|[<span data-ttu-id="d41b2-143">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="d41b2-143">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="d41b2-144">帖子</span><span class="sxs-lookup"><span data-stu-id="d41b2-144">post</span></span>](post.md)  |<span data-ttu-id="d41b2-145">在新建或现有帖子中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d41b2-145">Create one or more single-value extended properties in a new or existing post.</span></span>   |
|[<span data-ttu-id="d41b2-146">获取具有单值扩展属性的帖子</span><span class="sxs-lookup"><span data-stu-id="d41b2-146">Get post with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="d41b2-147">帖子</span><span class="sxs-lookup"><span data-stu-id="d41b2-147">post</span></span>](post.md) | <span data-ttu-id="d41b2-148">通过使用 `$expand` or `$filter` 获取包含单值扩展属性的帖子。</span><span class="sxs-lookup"><span data-stu-id="d41b2-148">Get posts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="d41b2-149">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="d41b2-149">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="d41b2-150">帖子</span><span class="sxs-lookup"><span data-stu-id="d41b2-150">post</span></span>](post.md) | <span data-ttu-id="d41b2-151">在新建或现有的帖子中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d41b2-151">Create one or more multi-value extended properties in a new or existing post.</span></span>  |
|[<span data-ttu-id="d41b2-152">获取具有多值扩展属性的帖子</span><span class="sxs-lookup"><span data-stu-id="d41b2-152">Get post with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="d41b2-153">帖子</span><span class="sxs-lookup"><span data-stu-id="d41b2-153">post</span></span>](post.md) | <span data-ttu-id="d41b2-154">使用 `$expand` 获取包含一个多值扩展属性的帖子。</span><span class="sxs-lookup"><span data-stu-id="d41b2-154">Get a post that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="d41b2-155">属性</span><span class="sxs-lookup"><span data-stu-id="d41b2-155">Properties</span></span>
| <span data-ttu-id="d41b2-156">属性</span><span class="sxs-lookup"><span data-stu-id="d41b2-156">Property</span></span>     | <span data-ttu-id="d41b2-157">类型</span><span class="sxs-lookup"><span data-stu-id="d41b2-157">Type</span></span>   |<span data-ttu-id="d41b2-158">说明</span><span class="sxs-lookup"><span data-stu-id="d41b2-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d41b2-159">body</span><span class="sxs-lookup"><span data-stu-id="d41b2-159">body</span></span>|[<span data-ttu-id="d41b2-160">itemBody</span><span class="sxs-lookup"><span data-stu-id="d41b2-160">itemBody</span></span>](itembody.md)|<span data-ttu-id="d41b2-p101">帖子的内容。这是默认属性。此属性可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="d41b2-p101">The contents of the post. This is a default property. This property can be null.</span></span>|
|<span data-ttu-id="d41b2-164">categories</span><span class="sxs-lookup"><span data-stu-id="d41b2-164">categories</span></span>|<span data-ttu-id="d41b2-165">字符串集合</span><span class="sxs-lookup"><span data-stu-id="d41b2-165">String collection</span></span>|<span data-ttu-id="d41b2-166">与帖子关联的类别。</span><span class="sxs-lookup"><span data-stu-id="d41b2-166">The categories associated with the post.</span></span>|
|<span data-ttu-id="d41b2-167">changeKey</span><span class="sxs-lookup"><span data-stu-id="d41b2-167">changeKey</span></span>|<span data-ttu-id="d41b2-168">字符串</span><span class="sxs-lookup"><span data-stu-id="d41b2-168">String</span></span>|<span data-ttu-id="d41b2-p102">标识帖子的版本。每次帖子更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="d41b2-p102">Identifies the version of the post. Every time the post is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="d41b2-172">conversationId</span><span class="sxs-lookup"><span data-stu-id="d41b2-172">conversationId</span></span>|<span data-ttu-id="d41b2-173">字符串</span><span class="sxs-lookup"><span data-stu-id="d41b2-173">String</span></span>|<span data-ttu-id="d41b2-p103">对话的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="d41b2-p103">Unique ID of the conversation. Read-only.</span></span>|
|<span data-ttu-id="d41b2-176">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="d41b2-176">conversationThreadId</span></span>|<span data-ttu-id="d41b2-177">字符串</span><span class="sxs-lookup"><span data-stu-id="d41b2-177">String</span></span>|<span data-ttu-id="d41b2-p104">对话线程的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="d41b2-p104">Unique ID of the conversation thread. Read-only.</span></span>|
|<span data-ttu-id="d41b2-180">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d41b2-180">createdDateTime</span></span>|<span data-ttu-id="d41b2-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d41b2-181">DateTimeOffset</span></span>|<span data-ttu-id="d41b2-p105">创建帖子时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式： `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d41b2-p105">Specifies when the post was created. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d41b2-185">from</span><span class="sxs-lookup"><span data-stu-id="d41b2-185">from</span></span>|[<span data-ttu-id="d41b2-186">收件人</span><span class="sxs-lookup"><span data-stu-id="d41b2-186">recipient</span></span>](recipient.md)|<span data-ttu-id="d41b2-p106">在委派访问方案中使用。指示代表另一用户发布了此邮件的帐户。这是默认属性。</span><span class="sxs-lookup"><span data-stu-id="d41b2-p106">Used in delegate access scenarios. Indicates who posted the message on behalf of another user. This is a default property.</span></span>|
|<span data-ttu-id="d41b2-190">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="d41b2-190">hasAttachments</span></span>|<span data-ttu-id="d41b2-191">布尔</span><span class="sxs-lookup"><span data-stu-id="d41b2-191">Boolean</span></span>|<span data-ttu-id="d41b2-p107">指示帖子是否具有至少一个附件。这是默认属性。</span><span class="sxs-lookup"><span data-stu-id="d41b2-p107">Indicates whether the post has at least one attachment. This is a default property.</span></span>|
|<span data-ttu-id="d41b2-194">id</span><span class="sxs-lookup"><span data-stu-id="d41b2-194">id</span></span>|<span data-ttu-id="d41b2-195">字符串</span><span class="sxs-lookup"><span data-stu-id="d41b2-195">String</span></span>| <span data-ttu-id="d41b2-196">只读。</span><span class="sxs-lookup"><span data-stu-id="d41b2-196">Read-only.</span></span>|
|<span data-ttu-id="d41b2-197">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d41b2-197">lastModifiedDateTime</span></span>|<span data-ttu-id="d41b2-198">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d41b2-198">DateTimeOffset</span></span>|<span data-ttu-id="d41b2-p108">帖子上次修改时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式： `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d41b2-p108">Specifies when the post was last modified. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d41b2-202">newParticipants</span><span class="sxs-lookup"><span data-stu-id="d41b2-202">newParticipants</span></span>|<span data-ttu-id="d41b2-203">[收件人](recipient.md)集合</span><span class="sxs-lookup"><span data-stu-id="d41b2-203">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="d41b2-204">添加到此线程作为帖子一部分的对话参与者。</span><span class="sxs-lookup"><span data-stu-id="d41b2-204">Conversation participants that were added to the thread as part of this post.</span></span>|
|<span data-ttu-id="d41b2-205">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="d41b2-205">receivedDateTime</span></span>|<span data-ttu-id="d41b2-206">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d41b2-206">DateTimeOffset</span></span>|<span data-ttu-id="d41b2-p109">接收到帖子时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式： `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d41b2-p109">Specifies when the post was received. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d41b2-210">sender</span><span class="sxs-lookup"><span data-stu-id="d41b2-210">sender</span></span>|[<span data-ttu-id="d41b2-211">recipient</span><span class="sxs-lookup"><span data-stu-id="d41b2-211">recipient</span></span>](recipient.md)|<span data-ttu-id="d41b2-p110">包含发件人的地址未指定发件人时，发件人的值假定为已经过验证身份的用户的地址。这是默认属性。</span><span class="sxs-lookup"><span data-stu-id="d41b2-p110">Contains the address of the sender. The value of Sender is assumed to be the address of the authenticated user in the case when Sender is not specified. This is a default property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d41b2-215">关系</span><span class="sxs-lookup"><span data-stu-id="d41b2-215">Relationships</span></span>
| <span data-ttu-id="d41b2-216">关系</span><span class="sxs-lookup"><span data-stu-id="d41b2-216">Relationship</span></span> | <span data-ttu-id="d41b2-217">类型</span><span class="sxs-lookup"><span data-stu-id="d41b2-217">Type</span></span>   |<span data-ttu-id="d41b2-218">说明</span><span class="sxs-lookup"><span data-stu-id="d41b2-218">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d41b2-219">attachments</span><span class="sxs-lookup"><span data-stu-id="d41b2-219">attachments</span></span>|<span data-ttu-id="d41b2-220">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d41b2-220">[Attachment](attachment.md) collection</span></span>| <span data-ttu-id="d41b2-p111">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="d41b2-p111">Read-only. Nullable.</span></span>|
|<span data-ttu-id="d41b2-223">extensions</span><span class="sxs-lookup"><span data-stu-id="d41b2-223">extensions</span></span>|<span data-ttu-id="d41b2-224">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="d41b2-224">[Extension](extension.md) collection</span></span>|<span data-ttu-id="d41b2-p112">为帖子定义的开放扩展集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="d41b2-p112">The collection of open extensions defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="d41b2-228">inReplyTo</span><span class="sxs-lookup"><span data-stu-id="d41b2-228">inReplyTo</span></span>|[<span data-ttu-id="d41b2-229">帖子</span><span class="sxs-lookup"><span data-stu-id="d41b2-229">post</span></span>](post.md)| <span data-ttu-id="d41b2-230">只读。</span><span class="sxs-lookup"><span data-stu-id="d41b2-230">Read-only.</span></span>|
|<span data-ttu-id="d41b2-231">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d41b2-231">multiValueExtendedProperties</span></span>|<span data-ttu-id="d41b2-232">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d41b2-232">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d41b2-p113">为帖子定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d41b2-p113">The collection of multi-value extended properties defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="d41b2-236">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d41b2-236">singleValueExtendedProperties</span></span>|<span data-ttu-id="d41b2-237">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d41b2-237">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d41b2-p114">为帖子定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d41b2-p114">The collection of single-value extended properties defined for the post. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d41b2-241">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d41b2-241">JSON representation</span></span>

<span data-ttu-id="d41b2-242">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d41b2-242">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "attachments",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "baseType": "microsoft.graph.outlookItem",
  "@odata.type": "microsoft.graph.post",
  "@odata.annotations": [
    {
      "property": "attachments",
      "capabilities": {
        "changeTracking": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "inReplyTo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["string"],
  "changeKey": "string",
  "conversationId": "string",
  "conversationThreadId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "newParticipants": [{"@odata.type": "microsoft.graph.recipient"}],
  "receivedDateTime": "String (timestamp)",
  "sender": {"@odata.type": "microsoft.graph.recipient"}
}

```

## <a name="see-also"></a><span data-ttu-id="d41b2-243">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d41b2-243">See also</span></span>

- [<span data-ttu-id="d41b2-244">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="d41b2-244">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="d41b2-245">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="d41b2-245">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="d41b2-246">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="d41b2-246">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
