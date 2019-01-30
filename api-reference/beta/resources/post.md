---
title: 帖子资源类型
description: 代表 converstaionThread 实体内的单个公告项目。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 554892bdfed45d0fba9b90a084db67c0bb329486
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643599"
---
# <a name="post-resource-type"></a><span data-ttu-id="0d31e-103">帖子资源类型</span><span class="sxs-lookup"><span data-stu-id="0d31e-103">post resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d31e-104">代表[converstaionThread](conversationthread.md)实体内的单个公告项目。</span><span class="sxs-lookup"><span data-stu-id="0d31e-104">Represents an individual post item within a [converstaionThread](conversationthread.md) entity.</span></span>

<span data-ttu-id="0d31e-105">即使无法显式创建帖子，也可以执行以下任一操作来创建帖子：</span><span class="sxs-lookup"><span data-stu-id="0d31e-105">Even though you cannot explicitly create a post, doing any of the following would create a post:</span></span>

* [<span data-ttu-id="0d31e-106">答复现有帖子</span><span class="sxs-lookup"><span data-stu-id="0d31e-106">Reply to an existing post</span></span>](../api/post-reply.md) 
* [<span data-ttu-id="0d31e-107">答复现有线程</span><span class="sxs-lookup"><span data-stu-id="0d31e-107">Reply to an existing thread</span></span>](../api/conversationthread-reply.md) 
* [<span data-ttu-id="0d31e-108">在新对话中创建线程</span><span class="sxs-lookup"><span data-stu-id="0d31e-108">Create a thread in a new conversation</span></span>](../api/group-post-threads.md)
* [<span data-ttu-id="0d31e-109">创建新对话</span><span class="sxs-lookup"><span data-stu-id="0d31e-109">Create a new conversation</span></span>](../api/group-post-conversations.md)

<span data-ttu-id="0d31e-110">通过该资源可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="0d31e-110">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d31e-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d31e-111">JSON representation</span></span>

<span data-ttu-id="0d31e-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d31e-112">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "extensions",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.post"
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
  "importance": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "newParticipants": [{"@odata.type": "microsoft.graph.recipient"}],
  "receivedDateTime": "String (timestamp)",
  "sender": {"@odata.type": "microsoft.graph.recipient"}
}

```
## <a name="properties"></a><span data-ttu-id="0d31e-113">属性</span><span class="sxs-lookup"><span data-stu-id="0d31e-113">Properties</span></span>
| <span data-ttu-id="0d31e-114">属性</span><span class="sxs-lookup"><span data-stu-id="0d31e-114">Property</span></span>     | <span data-ttu-id="0d31e-115">类型</span><span class="sxs-lookup"><span data-stu-id="0d31e-115">Type</span></span>   |<span data-ttu-id="0d31e-116">说明</span><span class="sxs-lookup"><span data-stu-id="0d31e-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d31e-117">正文</span><span class="sxs-lookup"><span data-stu-id="0d31e-117">body</span></span>|[<span data-ttu-id="0d31e-118">itemBody</span><span class="sxs-lookup"><span data-stu-id="0d31e-118">itemBody</span></span>](itembody.md)|<span data-ttu-id="0d31e-p101">帖子的内容。这是默认属性。此属性可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="0d31e-p101">The contents of the post. This is a default property. This property can be null.</span></span>|
|<span data-ttu-id="0d31e-122">类别</span><span class="sxs-lookup"><span data-stu-id="0d31e-122">categories</span></span>|<span data-ttu-id="0d31e-123">String collection</span><span class="sxs-lookup"><span data-stu-id="0d31e-123">String collection</span></span>|<span data-ttu-id="0d31e-124">与帖子关联的类别。</span><span class="sxs-lookup"><span data-stu-id="0d31e-124">The categories associated with the post.</span></span> <span data-ttu-id="0d31e-125">每个类别对应于已为用户定义[outlookCategory](outlookcategory.md)的**displayName**属性。</span><span class="sxs-lookup"><span data-stu-id="0d31e-125">Each category corresponds to the **displayName** property of an [outlookCategory](outlookcategory.md) that has been defined for a user.</span></span>|
|<span data-ttu-id="0d31e-126">changeKey</span><span class="sxs-lookup"><span data-stu-id="0d31e-126">changeKey</span></span>|<span data-ttu-id="0d31e-127">String</span><span class="sxs-lookup"><span data-stu-id="0d31e-127">String</span></span>|<span data-ttu-id="0d31e-p103">标识帖子的版本。每次帖子更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="0d31e-p103">Identifies the version of the post. Every time the post is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="0d31e-131">conversationId</span><span class="sxs-lookup"><span data-stu-id="0d31e-131">conversationId</span></span>|<span data-ttu-id="0d31e-132">String</span><span class="sxs-lookup"><span data-stu-id="0d31e-132">String</span></span>|<span data-ttu-id="0d31e-p104">对话的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="0d31e-p104">Unique ID of the conversation. Read-only.</span></span>|
|<span data-ttu-id="0d31e-135">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="0d31e-135">conversationThreadId</span></span>|<span data-ttu-id="0d31e-136">String</span><span class="sxs-lookup"><span data-stu-id="0d31e-136">String</span></span>|<span data-ttu-id="0d31e-p105">对话线程的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="0d31e-p105">Unique ID of the conversation thread. Read-only.</span></span>|
|<span data-ttu-id="0d31e-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d31e-139">createdDateTime</span></span>|<span data-ttu-id="0d31e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d31e-140">DateTimeOffset</span></span>|<span data-ttu-id="0d31e-p106">创建帖子时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0d31e-p106">Specifies when the post was created. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0d31e-144">from</span><span class="sxs-lookup"><span data-stu-id="0d31e-144">from</span></span>|[<span data-ttu-id="0d31e-145">收件人</span><span class="sxs-lookup"><span data-stu-id="0d31e-145">recipient</span></span>](recipient.md)|<span data-ttu-id="0d31e-p107">在委派访问方案中使用。指示代表另一用户发布了此邮件的帐户。这是默认属性。</span><span class="sxs-lookup"><span data-stu-id="0d31e-p107">Used in delegate access scenarios. Indicates who posted the message on behalf of another user. This is a default property.</span></span>|
|<span data-ttu-id="0d31e-149">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="0d31e-149">hasAttachments</span></span>|<span data-ttu-id="0d31e-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d31e-150">Boolean</span></span>|<span data-ttu-id="0d31e-p108">指示帖子是否具有至少一个附件。这是默认属性。</span><span class="sxs-lookup"><span data-stu-id="0d31e-p108">Indicates whether the post has at least one attachment. This is a default property.</span></span>|
|<span data-ttu-id="0d31e-153">id</span><span class="sxs-lookup"><span data-stu-id="0d31e-153">id</span></span>|<span data-ttu-id="0d31e-154">String</span><span class="sxs-lookup"><span data-stu-id="0d31e-154">String</span></span>| <span data-ttu-id="0d31e-155">只读。</span><span class="sxs-lookup"><span data-stu-id="0d31e-155">Read-only.</span></span>|
|<span data-ttu-id="0d31e-156">重要性</span><span class="sxs-lookup"><span data-stu-id="0d31e-156">importance</span></span> | <span data-ttu-id="0d31e-157">String</span><span class="sxs-lookup"><span data-stu-id="0d31e-157">String</span></span> | <span data-ttu-id="0d31e-158">组文章的重要性： `low`， `normal`， `high`。</span><span class="sxs-lookup"><span data-stu-id="0d31e-158">The importance of a group post: `low`, `normal`, `high`.</span></span> |
|<span data-ttu-id="0d31e-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d31e-159">lastModifiedDateTime</span></span>|<span data-ttu-id="0d31e-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d31e-160">DateTimeOffset</span></span>|<span data-ttu-id="0d31e-p109">帖子上次修改时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0d31e-p109">Specifies when the post was last modified. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0d31e-164">newParticipants</span><span class="sxs-lookup"><span data-stu-id="0d31e-164">newParticipants</span></span>|<span data-ttu-id="0d31e-165">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="0d31e-165">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="0d31e-166">添加到此线程作为帖子一部分的对话参与者。</span><span class="sxs-lookup"><span data-stu-id="0d31e-166">Conversation participants that were added to the thread as part of this post.</span></span>|
|<span data-ttu-id="0d31e-167">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d31e-167">receivedDateTime</span></span>|<span data-ttu-id="0d31e-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d31e-168">DateTimeOffset</span></span>|<span data-ttu-id="0d31e-p110">接收到帖子时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0d31e-p110">Specifies when the post was received. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0d31e-172">sender</span><span class="sxs-lookup"><span data-stu-id="0d31e-172">sender</span></span>|[<span data-ttu-id="0d31e-173">recipient</span><span class="sxs-lookup"><span data-stu-id="0d31e-173">recipient</span></span>](recipient.md)|<span data-ttu-id="0d31e-p111">包含发件人的地址未指定发件人时，发件人的值假定为已经过验证身份的用户的地址。这是默认属性。</span><span class="sxs-lookup"><span data-stu-id="0d31e-p111">Contains the address of the sender. The value of Sender is assumed to be the address of the authenticated user in the case when Sender is not specified. This is a default property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d31e-177">关系</span><span class="sxs-lookup"><span data-stu-id="0d31e-177">Relationships</span></span>
| <span data-ttu-id="0d31e-178">关系</span><span class="sxs-lookup"><span data-stu-id="0d31e-178">Relationship</span></span> | <span data-ttu-id="0d31e-179">类型</span><span class="sxs-lookup"><span data-stu-id="0d31e-179">Type</span></span>   |<span data-ttu-id="0d31e-180">说明</span><span class="sxs-lookup"><span data-stu-id="0d31e-180">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d31e-181">attachments</span><span class="sxs-lookup"><span data-stu-id="0d31e-181">attachments</span></span>|<span data-ttu-id="0d31e-182">[Attachment](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d31e-182">[Attachment](attachment.md) collection</span></span>|<span data-ttu-id="0d31e-183">为公告[fileAttachment](fileattachment.md)和[itemAttachment](itemattachment.md)， [referenceAttachment](referenceattachment.md)附件的集合。</span><span class="sxs-lookup"><span data-stu-id="0d31e-183">The collection of [fileAttachment](fileattachment.md), [itemAttachment](itemattachment.md), and [referenceAttachment](referenceattachment.md) attachments for the post.</span></span> <span data-ttu-id="0d31e-184">只读。</span><span class="sxs-lookup"><span data-stu-id="0d31e-184">Read-only.</span></span> <span data-ttu-id="0d31e-185">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="0d31e-185">Nullable.</span></span>|
|<span data-ttu-id="0d31e-186">extensions</span><span class="sxs-lookup"><span data-stu-id="0d31e-186">extensions</span></span>|<span data-ttu-id="0d31e-187">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="0d31e-187">[Extension](extension.md) collection</span></span>|<span data-ttu-id="0d31e-p113">为帖子定义的开放扩展集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="0d31e-p113">The collection of open extensions defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="0d31e-191">inReplyTo</span><span class="sxs-lookup"><span data-stu-id="0d31e-191">inReplyTo</span></span>|[<span data-ttu-id="0d31e-192">Post</span><span class="sxs-lookup"><span data-stu-id="0d31e-192">Post</span></span>](post.md)|<span data-ttu-id="0d31e-193">此文章答复中[conversationThread](conversationthread.md)早期文章。</span><span class="sxs-lookup"><span data-stu-id="0d31e-193">The earlier post that this post is replying to in the [conversationThread](conversationthread.md).</span></span> <span data-ttu-id="0d31e-194">只读。</span><span class="sxs-lookup"><span data-stu-id="0d31e-194">Read-only.</span></span>|
|<span data-ttu-id="0d31e-195">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="0d31e-195">multiValueExtendedProperties</span></span>|<span data-ttu-id="0d31e-196">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d31e-196">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="0d31e-p115">为帖子定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="0d31e-p115">The collection of multi-value extended properties defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="0d31e-200">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="0d31e-200">singleValueExtendedProperties</span></span>|<span data-ttu-id="0d31e-201">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d31e-201">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="0d31e-p116">为帖子定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="0d31e-p116">The collection of single-value extended properties defined for the post. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="0d31e-205">方法</span><span class="sxs-lookup"><span data-stu-id="0d31e-205">Methods</span></span>

| <span data-ttu-id="0d31e-206">方法</span><span class="sxs-lookup"><span data-stu-id="0d31e-206">Method</span></span>           | <span data-ttu-id="0d31e-207">返回类型</span><span class="sxs-lookup"><span data-stu-id="0d31e-207">Return Type</span></span>    |<span data-ttu-id="0d31e-208">说明</span><span class="sxs-lookup"><span data-stu-id="0d31e-208">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0d31e-209">列出帖子</span><span class="sxs-lookup"><span data-stu-id="0d31e-209">List posts</span></span>](../api/conversationthread-list-posts.md) | [<span data-ttu-id="0d31e-210">帖子</span><span class="sxs-lookup"><span data-stu-id="0d31e-210">post</span></span>](post.md) |<span data-ttu-id="0d31e-211">获取指定线程的帖子。</span><span class="sxs-lookup"><span data-stu-id="0d31e-211">Get the posts of the specified thread.</span></span> |
|[<span data-ttu-id="0d31e-212">获取帖子</span><span class="sxs-lookup"><span data-stu-id="0d31e-212">Get post</span></span>](../api/post-get.md) | [<span data-ttu-id="0d31e-213">帖子</span><span class="sxs-lookup"><span data-stu-id="0d31e-213">post</span></span>](post.md) |<span data-ttu-id="0d31e-214">获取指定的线程中帖子的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0d31e-214">Get the properties and relationships of a post in a specified thread.</span></span>|
|[<span data-ttu-id="0d31e-215">答复</span><span class="sxs-lookup"><span data-stu-id="0d31e-215">Reply</span></span>](../api/post-reply.md)|<span data-ttu-id="0d31e-216">无</span><span class="sxs-lookup"><span data-stu-id="0d31e-216">None</span></span>|<span data-ttu-id="0d31e-217">在组对话中答复帖子，并向指定线程中添加新帖子。</span><span class="sxs-lookup"><span data-stu-id="0d31e-217">Reply to a post and add a new post to the specified thread in a group conversation.</span></span>|
|[<span data-ttu-id="0d31e-218">转发</span><span class="sxs-lookup"><span data-stu-id="0d31e-218">Forward</span></span>](../api/post-forward.md)|<span data-ttu-id="0d31e-219">无</span><span class="sxs-lookup"><span data-stu-id="0d31e-219">None</span></span>|<span data-ttu-id="0d31e-220">将帖子转发给收件人。</span><span class="sxs-lookup"><span data-stu-id="0d31e-220">Forward a post to a recipient.</span></span>|
|<span data-ttu-id="0d31e-221">**Attachments**</span><span class="sxs-lookup"><span data-stu-id="0d31e-221">**Attachments**</span></span>| | |
|[<span data-ttu-id="0d31e-222">列出附件</span><span class="sxs-lookup"><span data-stu-id="0d31e-222">List attachments</span></span>](../api/post-list-attachments.md) |<span data-ttu-id="0d31e-223">[attachment](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d31e-223">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="0d31e-224">获取帖子的所有附件。</span><span class="sxs-lookup"><span data-stu-id="0d31e-224">Get all attachments on a post.</span></span>|
|[<span data-ttu-id="0d31e-225">Add attachment</span><span class="sxs-lookup"><span data-stu-id="0d31e-225">Add attachment</span></span>](../api/post-post-attachments.md) |[<span data-ttu-id="0d31e-226">attachment</span><span class="sxs-lookup"><span data-stu-id="0d31e-226">attachment</span></span>](attachment.md)| <span data-ttu-id="0d31e-227">将附件添加到帖子中。</span><span class="sxs-lookup"><span data-stu-id="0d31e-227">Add an attachment to a post.</span></span> |
|<span data-ttu-id="0d31e-228">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="0d31e-228">**Open extensions**</span></span>| | |
|[<span data-ttu-id="0d31e-229">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="0d31e-229">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="0d31e-230">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="0d31e-230">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="0d31e-231">创建开放扩展，并将自定义属性添加到新资源或现有资源。</span><span class="sxs-lookup"><span data-stu-id="0d31e-231">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="0d31e-232">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="0d31e-232">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="0d31e-233">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d31e-233">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="0d31e-234">获取扩展名称标识的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="0d31e-234">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="0d31e-235">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="0d31e-235">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="0d31e-236">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="0d31e-236">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="0d31e-237">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="0d31e-237">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="0d31e-238">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="0d31e-238">**Extended properties**</span></span>| | |
|[<span data-ttu-id="0d31e-239">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="0d31e-239">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="0d31e-240">帖子</span><span class="sxs-lookup"><span data-stu-id="0d31e-240">post</span></span>](post.md)  |<span data-ttu-id="0d31e-241">在新建或现有帖子中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="0d31e-241">Create one or more single-value extended properties in a new or existing post.</span></span>   |
|[<span data-ttu-id="0d31e-242">获取具有单值扩展属性的帖子</span><span class="sxs-lookup"><span data-stu-id="0d31e-242">Get post with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="0d31e-243">帖子</span><span class="sxs-lookup"><span data-stu-id="0d31e-243">post</span></span>](post.md) | <span data-ttu-id="0d31e-244">通过使用 `$expand` or `$filter` 获取包含单值扩展属性的帖子。</span><span class="sxs-lookup"><span data-stu-id="0d31e-244">Get posts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="0d31e-245">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="0d31e-245">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="0d31e-246">帖子</span><span class="sxs-lookup"><span data-stu-id="0d31e-246">post</span></span>](post.md) | <span data-ttu-id="0d31e-247">在新建或现有的帖子中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="0d31e-247">Create one or more multi-value extended properties in a new or existing post.</span></span>  |
|[<span data-ttu-id="0d31e-248">获取具有多值扩展属性的帖子</span><span class="sxs-lookup"><span data-stu-id="0d31e-248">Get post with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="0d31e-249">帖子</span><span class="sxs-lookup"><span data-stu-id="0d31e-249">post</span></span>](post.md) | <span data-ttu-id="0d31e-250">使用 `$expand` 获取包含一个多值扩展属性的帖子。</span><span class="sxs-lookup"><span data-stu-id="0d31e-250">Get a post that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="see-also"></a><span data-ttu-id="0d31e-251">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0d31e-251">See also</span></span>

- [<span data-ttu-id="0d31e-252">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="0d31e-252">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0d31e-253">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="0d31e-253">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="0d31e-254">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="0d31e-254">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
