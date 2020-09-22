---
title: 帖子资源类型
description: 表示 conversationThread 实体中的各个帖子项。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 7c0a09a2348099392a8e00c176f038e30703a854
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037253"
---
# <a name="post-resource-type"></a><span data-ttu-id="4c98f-103">帖子资源类型</span><span class="sxs-lookup"><span data-stu-id="4c98f-103">post resource type</span></span>

<span data-ttu-id="4c98f-104">命名空间： microsoft. graph 表示 [conversationThread](conversationthread.md) 实体中的单个张贴项。</span><span class="sxs-lookup"><span data-stu-id="4c98f-104">Namespace: microsoft.graph Represents an individual Post item within a [conversationThread](conversationthread.md) entity.</span></span>

<span data-ttu-id="4c98f-105">即使无法显式创建帖子，也可以执行以下任一操作来创建帖子：</span><span class="sxs-lookup"><span data-stu-id="4c98f-105">Even though you cannot explicitly create a post, doing any of the following would create a post:</span></span>

- [<span data-ttu-id="4c98f-106">答复现有帖子</span><span class="sxs-lookup"><span data-stu-id="4c98f-106">Reply to an existing post</span></span>](../api/post-reply.md) 
- [<span data-ttu-id="4c98f-107">答复现有线程</span><span class="sxs-lookup"><span data-stu-id="4c98f-107">Reply to an existing thread</span></span>](../api/conversationthread-reply.md) 
- [<span data-ttu-id="4c98f-108">在新对话中创建线程</span><span class="sxs-lookup"><span data-stu-id="4c98f-108">Create a thread in a new conversation</span></span>](../api/group-post-threads.md)
- [<span data-ttu-id="4c98f-109">创建新对话</span><span class="sxs-lookup"><span data-stu-id="4c98f-109">Create a new conversation</span></span>](../api/group-post-conversations.md)

<span data-ttu-id="4c98f-110">使用此资源，可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="4c98f-110">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="4c98f-111">方法</span><span class="sxs-lookup"><span data-stu-id="4c98f-111">Methods</span></span>

| <span data-ttu-id="4c98f-112">方法</span><span class="sxs-lookup"><span data-stu-id="4c98f-112">Method</span></span>       | <span data-ttu-id="4c98f-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="4c98f-113">Return Type</span></span>  |<span data-ttu-id="4c98f-114">说明</span><span class="sxs-lookup"><span data-stu-id="4c98f-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4c98f-115">列出帖子</span><span class="sxs-lookup"><span data-stu-id="4c98f-115">List posts</span></span>](../api/conversationthread-list-posts.md) | [<span data-ttu-id="4c98f-116">帖子</span><span class="sxs-lookup"><span data-stu-id="4c98f-116">post</span></span>](post.md) |<span data-ttu-id="4c98f-117">获取指定线程的帖子。</span><span class="sxs-lookup"><span data-stu-id="4c98f-117">Get the posts of the specified thread.</span></span> |
|[<span data-ttu-id="4c98f-118">获取帖子</span><span class="sxs-lookup"><span data-stu-id="4c98f-118">Get post</span></span>](../api/post-get.md) | [<span data-ttu-id="4c98f-119">帖子</span><span class="sxs-lookup"><span data-stu-id="4c98f-119">post</span></span>](post.md) |<span data-ttu-id="4c98f-120">获取指定的线程中帖子的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4c98f-120">Get the properties and relationships of a post in a specified thread.</span></span>|
|[<span data-ttu-id="4c98f-121">答复</span><span class="sxs-lookup"><span data-stu-id="4c98f-121">Reply</span></span>](../api/post-reply.md)|<span data-ttu-id="4c98f-122">无</span><span class="sxs-lookup"><span data-stu-id="4c98f-122">None</span></span>|<span data-ttu-id="4c98f-123">在组对话中答复帖子，并向指定线程中添加新帖子。</span><span class="sxs-lookup"><span data-stu-id="4c98f-123">Reply to a post and add a new post to the specified thread in a group conversation.</span></span>|
|[<span data-ttu-id="4c98f-124">转发</span><span class="sxs-lookup"><span data-stu-id="4c98f-124">Forward</span></span>](../api/post-forward.md)|<span data-ttu-id="4c98f-125">无</span><span class="sxs-lookup"><span data-stu-id="4c98f-125">None</span></span>|<span data-ttu-id="4c98f-126">将帖子转发给收件人。</span><span class="sxs-lookup"><span data-stu-id="4c98f-126">Forward a post to a recipient.</span></span>|
|<span data-ttu-id="4c98f-127">**附件**</span><span class="sxs-lookup"><span data-stu-id="4c98f-127">**Attachments**</span></span>| | |
|[<span data-ttu-id="4c98f-128">列出附件</span><span class="sxs-lookup"><span data-stu-id="4c98f-128">List attachments</span></span>](../api/post-list-attachments.md) |<span data-ttu-id="4c98f-129">[attachment](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4c98f-129">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="4c98f-130">获取帖子的所有附件。</span><span class="sxs-lookup"><span data-stu-id="4c98f-130">Get all attachments on a post.</span></span>|
|[<span data-ttu-id="4c98f-131">添加附件</span><span class="sxs-lookup"><span data-stu-id="4c98f-131">Add attachment</span></span>](../api/post-post-attachments.md) |[<span data-ttu-id="4c98f-132">attachment</span><span class="sxs-lookup"><span data-stu-id="4c98f-132">attachment</span></span>](attachment.md)| <span data-ttu-id="4c98f-133">将附件添加到帖子中。</span><span class="sxs-lookup"><span data-stu-id="4c98f-133">Add an attachment to a post.</span></span> |
|<span data-ttu-id="4c98f-134">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="4c98f-134">**Open extensions**</span></span>| | |
|[<span data-ttu-id="4c98f-135">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="4c98f-135">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="4c98f-136">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="4c98f-136">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="4c98f-137">创建开放扩展，并在新建或现有的资源实例中添加自定义属性。</span><span class="sxs-lookup"><span data-stu-id="4c98f-137">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="4c98f-138">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="4c98f-138">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="4c98f-139">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4c98f-139">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="4c98f-140">获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。</span><span class="sxs-lookup"><span data-stu-id="4c98f-140">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="4c98f-141">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="4c98f-141">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="4c98f-142">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="4c98f-142">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="4c98f-143">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="4c98f-143">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="4c98f-144">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="4c98f-144">**Extended properties**</span></span>| | |
|[<span data-ttu-id="4c98f-145">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="4c98f-145">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="4c98f-146">帖子</span><span class="sxs-lookup"><span data-stu-id="4c98f-146">post</span></span>](post.md)  |<span data-ttu-id="4c98f-147">在新建或现有帖子中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="4c98f-147">Create one or more single-value extended properties in a new or existing post.</span></span>   |
|[<span data-ttu-id="4c98f-148">获取具有单值扩展属性的帖子</span><span class="sxs-lookup"><span data-stu-id="4c98f-148">Get post with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="4c98f-149">帖子</span><span class="sxs-lookup"><span data-stu-id="4c98f-149">post</span></span>](post.md) | <span data-ttu-id="4c98f-150">通过使用 `$expand` or `$filter` 获取包含单值扩展属性的帖子。</span><span class="sxs-lookup"><span data-stu-id="4c98f-150">Get posts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="4c98f-151">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="4c98f-151">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="4c98f-152">帖子</span><span class="sxs-lookup"><span data-stu-id="4c98f-152">post</span></span>](post.md) | <span data-ttu-id="4c98f-153">在新建或现有的帖子中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="4c98f-153">Create one or more multi-value extended properties in a new or existing post.</span></span>  |
|[<span data-ttu-id="4c98f-154">获取具有多值扩展属性的帖子</span><span class="sxs-lookup"><span data-stu-id="4c98f-154">Get post with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="4c98f-155">帖子</span><span class="sxs-lookup"><span data-stu-id="4c98f-155">post</span></span>](post.md) | <span data-ttu-id="4c98f-156">使用 `$expand` 获取包含一个多值扩展属性的帖子。</span><span class="sxs-lookup"><span data-stu-id="4c98f-156">Get a post that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="4c98f-157">属性</span><span class="sxs-lookup"><span data-stu-id="4c98f-157">Properties</span></span>
| <span data-ttu-id="4c98f-158">属性</span><span class="sxs-lookup"><span data-stu-id="4c98f-158">Property</span></span>     | <span data-ttu-id="4c98f-159">类型</span><span class="sxs-lookup"><span data-stu-id="4c98f-159">Type</span></span>   |<span data-ttu-id="4c98f-160">说明</span><span class="sxs-lookup"><span data-stu-id="4c98f-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c98f-161">正文</span><span class="sxs-lookup"><span data-stu-id="4c98f-161">body</span></span>|[<span data-ttu-id="4c98f-162">itemBody</span><span class="sxs-lookup"><span data-stu-id="4c98f-162">itemBody</span></span>](itembody.md)|<span data-ttu-id="4c98f-p101">帖子的内容。这是默认属性。此属性可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="4c98f-p101">The contents of the post. This is a default property. This property can be null.</span></span>|
|<span data-ttu-id="4c98f-166">类别</span><span class="sxs-lookup"><span data-stu-id="4c98f-166">categories</span></span>|<span data-ttu-id="4c98f-167">String collection</span><span class="sxs-lookup"><span data-stu-id="4c98f-167">String collection</span></span>|<span data-ttu-id="4c98f-168">与帖子关联的类别。</span><span class="sxs-lookup"><span data-stu-id="4c98f-168">The categories associated with the post.</span></span>|
|<span data-ttu-id="4c98f-169">changeKey</span><span class="sxs-lookup"><span data-stu-id="4c98f-169">changeKey</span></span>|<span data-ttu-id="4c98f-170">String</span><span class="sxs-lookup"><span data-stu-id="4c98f-170">String</span></span>|<span data-ttu-id="4c98f-p102">标识帖子的版本。每次帖子更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="4c98f-p102">Identifies the version of the post. Every time the post is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="4c98f-174">conversationId</span><span class="sxs-lookup"><span data-stu-id="4c98f-174">conversationId</span></span>|<span data-ttu-id="4c98f-175">String</span><span class="sxs-lookup"><span data-stu-id="4c98f-175">String</span></span>|<span data-ttu-id="4c98f-p103">对话的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="4c98f-p103">Unique ID of the conversation. Read-only.</span></span>|
|<span data-ttu-id="4c98f-178">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="4c98f-178">conversationThreadId</span></span>|<span data-ttu-id="4c98f-179">字符串</span><span class="sxs-lookup"><span data-stu-id="4c98f-179">String</span></span>|<span data-ttu-id="4c98f-p104">对话线程的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="4c98f-p104">Unique ID of the conversation thread. Read-only.</span></span>|
|<span data-ttu-id="4c98f-182">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c98f-182">createdDateTime</span></span>|<span data-ttu-id="4c98f-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c98f-183">DateTimeOffset</span></span>|<span data-ttu-id="4c98f-p105">创建帖子时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4c98f-p105">Specifies when the post was created. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4c98f-187">发件人</span><span class="sxs-lookup"><span data-stu-id="4c98f-187">from</span></span>|[<span data-ttu-id="4c98f-188">recipient</span><span class="sxs-lookup"><span data-stu-id="4c98f-188">recipient</span></span>](recipient.md)|<span data-ttu-id="4c98f-p106">在委派访问方案中使用。指示代表另一用户发布了此邮件的帐户。这是默认属性。</span><span class="sxs-lookup"><span data-stu-id="4c98f-p106">Used in delegate access scenarios. Indicates who posted the message on behalf of another user. This is a default property.</span></span>|
|<span data-ttu-id="4c98f-192">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="4c98f-192">hasAttachments</span></span>|<span data-ttu-id="4c98f-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c98f-193">Boolean</span></span>|<span data-ttu-id="4c98f-p107">指示帖子是否具有至少一个附件。这是默认属性。</span><span class="sxs-lookup"><span data-stu-id="4c98f-p107">Indicates whether the post has at least one attachment. This is a default property.</span></span>|
|<span data-ttu-id="4c98f-196">id</span><span class="sxs-lookup"><span data-stu-id="4c98f-196">id</span></span>|<span data-ttu-id="4c98f-197">String</span><span class="sxs-lookup"><span data-stu-id="4c98f-197">String</span></span>| <span data-ttu-id="4c98f-198">只读。</span><span class="sxs-lookup"><span data-stu-id="4c98f-198">Read-only.</span></span>|
|<span data-ttu-id="4c98f-199">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c98f-199">lastModifiedDateTime</span></span>|<span data-ttu-id="4c98f-200">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c98f-200">DateTimeOffset</span></span>|<span data-ttu-id="4c98f-p108">帖子上次修改时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4c98f-p108">Specifies when the post was last modified. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4c98f-204">newParticipants</span><span class="sxs-lookup"><span data-stu-id="4c98f-204">newParticipants</span></span>|<span data-ttu-id="4c98f-205">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="4c98f-205">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="4c98f-206">添加到此线程作为帖子一部分的对话参与者。</span><span class="sxs-lookup"><span data-stu-id="4c98f-206">Conversation participants that were added to the thread as part of this post.</span></span>|
|<span data-ttu-id="4c98f-207">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c98f-207">receivedDateTime</span></span>|<span data-ttu-id="4c98f-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c98f-208">DateTimeOffset</span></span>|<span data-ttu-id="4c98f-p109">接收到帖子时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4c98f-p109">Specifies when the post was received. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4c98f-212">sender</span><span class="sxs-lookup"><span data-stu-id="4c98f-212">sender</span></span>|[<span data-ttu-id="4c98f-213">recipient</span><span class="sxs-lookup"><span data-stu-id="4c98f-213">recipient</span></span>](recipient.md)|<span data-ttu-id="4c98f-p110">包含发件人的地址未指定发件人时，发件人的值假定为已经过验证身份的用户的地址。这是默认属性。</span><span class="sxs-lookup"><span data-stu-id="4c98f-p110">Contains the address of the sender. The value of Sender is assumed to be the address of the authenticated user in the case when Sender is not specified. This is a default property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c98f-217">关系</span><span class="sxs-lookup"><span data-stu-id="4c98f-217">Relationships</span></span>
| <span data-ttu-id="4c98f-218">关系</span><span class="sxs-lookup"><span data-stu-id="4c98f-218">Relationship</span></span> | <span data-ttu-id="4c98f-219">类型</span><span class="sxs-lookup"><span data-stu-id="4c98f-219">Type</span></span>   |<span data-ttu-id="4c98f-220">说明</span><span class="sxs-lookup"><span data-stu-id="4c98f-220">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c98f-221">attachments</span><span class="sxs-lookup"><span data-stu-id="4c98f-221">attachments</span></span>|<span data-ttu-id="4c98f-222">[Attachment](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4c98f-222">[Attachment](attachment.md) collection</span></span>| <span data-ttu-id="4c98f-p111">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="4c98f-p111">Read-only. Nullable.</span></span>|
|<span data-ttu-id="4c98f-225">extensions</span><span class="sxs-lookup"><span data-stu-id="4c98f-225">extensions</span></span>|<span data-ttu-id="4c98f-226">[Extension](extension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4c98f-226">[Extension](extension.md) collection</span></span>|<span data-ttu-id="4c98f-p112">为帖子定义的开放扩展集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="4c98f-p112">The collection of open extensions defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="4c98f-230">inReplyTo</span><span class="sxs-lookup"><span data-stu-id="4c98f-230">inReplyTo</span></span>|[<span data-ttu-id="4c98f-231">帖子</span><span class="sxs-lookup"><span data-stu-id="4c98f-231">post</span></span>](post.md)| <span data-ttu-id="4c98f-232">只读。</span><span class="sxs-lookup"><span data-stu-id="4c98f-232">Read-only.</span></span>|
|<span data-ttu-id="4c98f-233">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="4c98f-233">multiValueExtendedProperties</span></span>|<span data-ttu-id="4c98f-234">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4c98f-234">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="4c98f-p113">为帖子定义的多值扩展属性的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="4c98f-p113">The collection of multi-value extended properties defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="4c98f-238">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="4c98f-238">singleValueExtendedProperties</span></span>|<span data-ttu-id="4c98f-239">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4c98f-239">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="4c98f-p114">为帖子定义的单值扩展属性的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="4c98f-p114">The collection of single-value extended properties defined for the post. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4c98f-243">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c98f-243">JSON representation</span></span>

<span data-ttu-id="4c98f-244">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c98f-244">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="4c98f-245">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4c98f-245">See also</span></span>

- [<span data-ttu-id="4c98f-246">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="4c98f-246">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4c98f-247">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="4c98f-247">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="4c98f-248">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="4c98f-248">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

