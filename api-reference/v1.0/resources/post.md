---
title: 帖子资源类型
description: 表示 conversationThread 实体中的各个帖子项。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 585d823a7a3e4b6814f06c1613cac66a82a93e65
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851189"
---
# <a name="post-resource-type"></a><span data-ttu-id="a38d4-103">帖子资源类型</span><span class="sxs-lookup"><span data-stu-id="a38d4-103">post resource type</span></span>
<span data-ttu-id="a38d4-104">表示 [conversationThread](conversationthread.md) 实体中的各个帖子项。</span><span class="sxs-lookup"><span data-stu-id="a38d4-104">Represents an individual Post item within a [conversationThread](conversationthread.md) entity.</span></span>

<span data-ttu-id="a38d4-105">即使无法显式创建帖子，也可以执行以下任一操作来创建帖子：</span><span class="sxs-lookup"><span data-stu-id="a38d4-105">Even though you cannot explicitly create a post, doing any of the following would create a post:</span></span>

- [<span data-ttu-id="a38d4-106">答复现有帖子</span><span class="sxs-lookup"><span data-stu-id="a38d4-106">Reply to an existing post</span></span>](../api/post-reply.md) 
- [<span data-ttu-id="a38d4-107">答复现有线程</span><span class="sxs-lookup"><span data-stu-id="a38d4-107">Reply to an existing thread</span></span>](../api/conversationthread-reply.md) 
- [<span data-ttu-id="a38d4-108">在新对话中创建线程</span><span class="sxs-lookup"><span data-stu-id="a38d4-108">Create a thread in a new conversation</span></span>](../api/group-post-threads.md)
- [<span data-ttu-id="a38d4-109">创建新对话</span><span class="sxs-lookup"><span data-stu-id="a38d4-109">Create a new conversation</span></span>](../api/group-post-conversations.md)

<span data-ttu-id="a38d4-110">通过该资源可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="a38d4-110">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="a38d4-111">方法</span><span class="sxs-lookup"><span data-stu-id="a38d4-111">Methods</span></span>

| <span data-ttu-id="a38d4-112">方法</span><span class="sxs-lookup"><span data-stu-id="a38d4-112">Method</span></span>       | <span data-ttu-id="a38d4-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="a38d4-113">Return Type</span></span>  |<span data-ttu-id="a38d4-114">说明</span><span class="sxs-lookup"><span data-stu-id="a38d4-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a38d4-115">列出帖子</span><span class="sxs-lookup"><span data-stu-id="a38d4-115">List posts</span></span>](../api/conversationthread-list-posts.md) | [<span data-ttu-id="a38d4-116">帖子</span><span class="sxs-lookup"><span data-stu-id="a38d4-116">post</span></span>](post.md) |<span data-ttu-id="a38d4-117">获取指定线程的帖子。</span><span class="sxs-lookup"><span data-stu-id="a38d4-117">Get the posts of the specified thread.</span></span> |
|[<span data-ttu-id="a38d4-118">获取帖子</span><span class="sxs-lookup"><span data-stu-id="a38d4-118">Get post</span></span>](../api/post-get.md) | [<span data-ttu-id="a38d4-119">帖子</span><span class="sxs-lookup"><span data-stu-id="a38d4-119">post</span></span>](post.md) |<span data-ttu-id="a38d4-120">获取指定的线程中帖子的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a38d4-120">Get the properties and relationships of a post in a specified thread.</span></span>|
|[<span data-ttu-id="a38d4-121">答复</span><span class="sxs-lookup"><span data-stu-id="a38d4-121">Reply</span></span>](../api/post-reply.md)|<span data-ttu-id="a38d4-122">无</span><span class="sxs-lookup"><span data-stu-id="a38d4-122">None</span></span>|<span data-ttu-id="a38d4-123">在组对话中答复帖子，并向指定线程中添加新帖子。</span><span class="sxs-lookup"><span data-stu-id="a38d4-123">Reply to a post and add a new post to the specified thread in a group conversation.</span></span>|
|[<span data-ttu-id="a38d4-124">转发</span><span class="sxs-lookup"><span data-stu-id="a38d4-124">Forward</span></span>](../api/post-forward.md)|<span data-ttu-id="a38d4-125">无</span><span class="sxs-lookup"><span data-stu-id="a38d4-125">None</span></span>|<span data-ttu-id="a38d4-126">将帖子转发给收件人。</span><span class="sxs-lookup"><span data-stu-id="a38d4-126">Forward a post to a recipient.</span></span>|
|<span data-ttu-id="a38d4-127">**Attachments**</span><span class="sxs-lookup"><span data-stu-id="a38d4-127">**Attachments**</span></span>| | |
|[<span data-ttu-id="a38d4-128">列出附件</span><span class="sxs-lookup"><span data-stu-id="a38d4-128">List attachments</span></span>](../api/post-list-attachments.md) |<span data-ttu-id="a38d4-129">[attachment](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a38d4-129">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="a38d4-130">获取帖子的所有附件。</span><span class="sxs-lookup"><span data-stu-id="a38d4-130">Get all attachments on a post.</span></span>|
|[<span data-ttu-id="a38d4-131">Add attachment</span><span class="sxs-lookup"><span data-stu-id="a38d4-131">Add attachment</span></span>](../api/post-post-attachments.md) |[<span data-ttu-id="a38d4-132">attachment</span><span class="sxs-lookup"><span data-stu-id="a38d4-132">attachment</span></span>](attachment.md)| <span data-ttu-id="a38d4-133">将附件添加到帖子中。</span><span class="sxs-lookup"><span data-stu-id="a38d4-133">Add an attachment to a post.</span></span> |
|<span data-ttu-id="a38d4-134">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="a38d4-134">**Open extensions**</span></span>| | |
|[<span data-ttu-id="a38d4-135">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="a38d4-135">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="a38d4-136">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="a38d4-136">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="a38d4-137">创建开放扩展，并在新建或现有的资源实例中添加自定义属性。</span><span class="sxs-lookup"><span data-stu-id="a38d4-137">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="a38d4-138">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="a38d4-138">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="a38d4-139">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a38d4-139">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="a38d4-140">获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。</span><span class="sxs-lookup"><span data-stu-id="a38d4-140">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="a38d4-141">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="a38d4-141">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="a38d4-142">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="a38d4-142">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="a38d4-143">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="a38d4-143">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="a38d4-144">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="a38d4-144">**Extended properties**</span></span>| | |
|[<span data-ttu-id="a38d4-145">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="a38d4-145">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="a38d4-146">帖子</span><span class="sxs-lookup"><span data-stu-id="a38d4-146">post</span></span>](post.md)  |<span data-ttu-id="a38d4-147">在新建或现有帖子中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="a38d4-147">Create one or more single-value extended properties in a new or existing post.</span></span>   |
|[<span data-ttu-id="a38d4-148">获取具有单值扩展属性的帖子</span><span class="sxs-lookup"><span data-stu-id="a38d4-148">Get post with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="a38d4-149">帖子</span><span class="sxs-lookup"><span data-stu-id="a38d4-149">post</span></span>](post.md) | <span data-ttu-id="a38d4-150">通过使用 `$expand` or `$filter` 获取包含单值扩展属性的帖子。</span><span class="sxs-lookup"><span data-stu-id="a38d4-150">Get posts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="a38d4-151">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="a38d4-151">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="a38d4-152">帖子</span><span class="sxs-lookup"><span data-stu-id="a38d4-152">post</span></span>](post.md) | <span data-ttu-id="a38d4-153">在新建或现有的帖子中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="a38d4-153">Create one or more multi-value extended properties in a new or existing post.</span></span>  |
|[<span data-ttu-id="a38d4-154">获取具有多值扩展属性的帖子</span><span class="sxs-lookup"><span data-stu-id="a38d4-154">Get post with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="a38d4-155">帖子</span><span class="sxs-lookup"><span data-stu-id="a38d4-155">post</span></span>](post.md) | <span data-ttu-id="a38d4-156">使用 `$expand` 获取包含一个多值扩展属性的帖子。</span><span class="sxs-lookup"><span data-stu-id="a38d4-156">Get a post that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="a38d4-157">属性</span><span class="sxs-lookup"><span data-stu-id="a38d4-157">Properties</span></span>
| <span data-ttu-id="a38d4-158">属性</span><span class="sxs-lookup"><span data-stu-id="a38d4-158">Property</span></span>     | <span data-ttu-id="a38d4-159">类型</span><span class="sxs-lookup"><span data-stu-id="a38d4-159">Type</span></span>   |<span data-ttu-id="a38d4-160">说明</span><span class="sxs-lookup"><span data-stu-id="a38d4-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a38d4-161">body</span><span class="sxs-lookup"><span data-stu-id="a38d4-161">body</span></span>|[<span data-ttu-id="a38d4-162">itemBody</span><span class="sxs-lookup"><span data-stu-id="a38d4-162">itemBody</span></span>](itembody.md)|<span data-ttu-id="a38d4-p101">帖子的内容。这是默认属性。此属性可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="a38d4-p101">The contents of the post. This is a default property. This property can be null.</span></span>|
|<span data-ttu-id="a38d4-166">categories</span><span class="sxs-lookup"><span data-stu-id="a38d4-166">categories</span></span>|<span data-ttu-id="a38d4-167">String collection</span><span class="sxs-lookup"><span data-stu-id="a38d4-167">String collection</span></span>|<span data-ttu-id="a38d4-168">与帖子关联的类别。</span><span class="sxs-lookup"><span data-stu-id="a38d4-168">The categories associated with the post.</span></span>|
|<span data-ttu-id="a38d4-169">changeKey</span><span class="sxs-lookup"><span data-stu-id="a38d4-169">changeKey</span></span>|<span data-ttu-id="a38d4-170">String</span><span class="sxs-lookup"><span data-stu-id="a38d4-170">String</span></span>|<span data-ttu-id="a38d4-p102">标识帖子的版本。每次帖子更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="a38d4-p102">Identifies the version of the post. Every time the post is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="a38d4-174">conversationId</span><span class="sxs-lookup"><span data-stu-id="a38d4-174">conversationId</span></span>|<span data-ttu-id="a38d4-175">String</span><span class="sxs-lookup"><span data-stu-id="a38d4-175">String</span></span>|<span data-ttu-id="a38d4-p103">对话的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="a38d4-p103">Unique ID of the conversation. Read-only.</span></span>|
|<span data-ttu-id="a38d4-178">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="a38d4-178">conversationThreadId</span></span>|<span data-ttu-id="a38d4-179">String</span><span class="sxs-lookup"><span data-stu-id="a38d4-179">String</span></span>|<span data-ttu-id="a38d4-p104">对话线程的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="a38d4-p104">Unique ID of the conversation thread. Read-only.</span></span>|
|<span data-ttu-id="a38d4-182">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a38d4-182">createdDateTime</span></span>|<span data-ttu-id="a38d4-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a38d4-183">DateTimeOffset</span></span>|<span data-ttu-id="a38d4-p105">创建帖子时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a38d4-p105">Specifies when the post was created. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a38d4-187">from</span><span class="sxs-lookup"><span data-stu-id="a38d4-187">from</span></span>|[<span data-ttu-id="a38d4-188">收件人</span><span class="sxs-lookup"><span data-stu-id="a38d4-188">recipient</span></span>](recipient.md)|<span data-ttu-id="a38d4-p106">在委派访问方案中使用。指示代表另一用户发布了此邮件的帐户。这是默认属性。</span><span class="sxs-lookup"><span data-stu-id="a38d4-p106">Used in delegate access scenarios. Indicates who posted the message on behalf of another user. This is a default property.</span></span>|
|<span data-ttu-id="a38d4-192">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="a38d4-192">hasAttachments</span></span>|<span data-ttu-id="a38d4-193">布尔</span><span class="sxs-lookup"><span data-stu-id="a38d4-193">Boolean</span></span>|<span data-ttu-id="a38d4-p107">指示帖子是否具有至少一个附件。这是默认属性。</span><span class="sxs-lookup"><span data-stu-id="a38d4-p107">Indicates whether the post has at least one attachment. This is a default property.</span></span>|
|<span data-ttu-id="a38d4-196">id</span><span class="sxs-lookup"><span data-stu-id="a38d4-196">id</span></span>|<span data-ttu-id="a38d4-197">String</span><span class="sxs-lookup"><span data-stu-id="a38d4-197">String</span></span>| <span data-ttu-id="a38d4-198">只读。</span><span class="sxs-lookup"><span data-stu-id="a38d4-198">Read-only.</span></span>|
|<span data-ttu-id="a38d4-199">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a38d4-199">lastModifiedDateTime</span></span>|<span data-ttu-id="a38d4-200">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a38d4-200">DateTimeOffset</span></span>|<span data-ttu-id="a38d4-p108">帖子上次修改时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a38d4-p108">Specifies when the post was last modified. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a38d4-204">newParticipants</span><span class="sxs-lookup"><span data-stu-id="a38d4-204">newParticipants</span></span>|<span data-ttu-id="a38d4-205">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="a38d4-205">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="a38d4-206">添加到此线程作为帖子一部分的对话参与者。</span><span class="sxs-lookup"><span data-stu-id="a38d4-206">Conversation participants that were added to the thread as part of this post.</span></span>|
|<span data-ttu-id="a38d4-207">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="a38d4-207">receivedDateTime</span></span>|<span data-ttu-id="a38d4-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a38d4-208">DateTimeOffset</span></span>|<span data-ttu-id="a38d4-p109">接收到帖子时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a38d4-p109">Specifies when the post was received. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a38d4-212">sender</span><span class="sxs-lookup"><span data-stu-id="a38d4-212">sender</span></span>|[<span data-ttu-id="a38d4-213">recipient</span><span class="sxs-lookup"><span data-stu-id="a38d4-213">recipient</span></span>](recipient.md)|<span data-ttu-id="a38d4-p110">包含发件人的地址未指定发件人时，发件人的值假定为已经过验证身份的用户的地址。这是默认属性。</span><span class="sxs-lookup"><span data-stu-id="a38d4-p110">Contains the address of the sender. The value of Sender is assumed to be the address of the authenticated user in the case when Sender is not specified. This is a default property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a38d4-217">Relationships</span><span class="sxs-lookup"><span data-stu-id="a38d4-217">Relationships</span></span>
| <span data-ttu-id="a38d4-218">关系</span><span class="sxs-lookup"><span data-stu-id="a38d4-218">Relationship</span></span> | <span data-ttu-id="a38d4-219">类型</span><span class="sxs-lookup"><span data-stu-id="a38d4-219">Type</span></span>   |<span data-ttu-id="a38d4-220">说明</span><span class="sxs-lookup"><span data-stu-id="a38d4-220">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a38d4-221">attachments</span><span class="sxs-lookup"><span data-stu-id="a38d4-221">attachments</span></span>|<span data-ttu-id="a38d4-222">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a38d4-222">[Attachment](attachment.md) collection</span></span>| <span data-ttu-id="a38d4-p111">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="a38d4-p111">Read-only. Nullable.</span></span>|
|<span data-ttu-id="a38d4-225">extensions</span><span class="sxs-lookup"><span data-stu-id="a38d4-225">extensions</span></span>|<span data-ttu-id="a38d4-226">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="a38d4-226">[Extension](extension.md) collection</span></span>|<span data-ttu-id="a38d4-p112">为帖子定义的开放扩展集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="a38d4-p112">The collection of open extensions defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="a38d4-230">inReplyTo</span><span class="sxs-lookup"><span data-stu-id="a38d4-230">inReplyTo</span></span>|[<span data-ttu-id="a38d4-231">帖子</span><span class="sxs-lookup"><span data-stu-id="a38d4-231">post</span></span>](post.md)| <span data-ttu-id="a38d4-232">只读。</span><span class="sxs-lookup"><span data-stu-id="a38d4-232">Read-only.</span></span>|
|<span data-ttu-id="a38d4-233">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="a38d4-233">multiValueExtendedProperties</span></span>|<span data-ttu-id="a38d4-234">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a38d4-234">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="a38d4-p113">为帖子定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="a38d4-p113">The collection of multi-value extended properties defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="a38d4-238">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="a38d4-238">singleValueExtendedProperties</span></span>|<span data-ttu-id="a38d4-239">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a38d4-239">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="a38d4-p114">为帖子定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="a38d4-p114">The collection of single-value extended properties defined for the post. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a38d4-243">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a38d4-243">JSON representation</span></span>

<span data-ttu-id="a38d4-244">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a38d4-244">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="a38d4-245">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a38d4-245">See also</span></span>

- [<span data-ttu-id="a38d4-246">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="a38d4-246">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a38d4-247">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="a38d4-247">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="a38d4-248">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="a38d4-248">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
