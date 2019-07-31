---
title: 帖子资源类型
description: 表示 converstaionThread 实体中的单个张贴项。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 9de2bfec6bab126577fa0013a58caac83ad031f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008983"
---
# <a name="post-resource-type"></a><span data-ttu-id="e3668-103">帖子资源类型</span><span class="sxs-lookup"><span data-stu-id="e3668-103">post resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3668-104">表示[converstaionThread](conversationthread.md)实体中的单个张贴项。</span><span class="sxs-lookup"><span data-stu-id="e3668-104">Represents an individual post item within a [converstaionThread](conversationthread.md) entity.</span></span>

<span data-ttu-id="e3668-105">即使无法显式创建帖子，也可以执行以下任一操作来创建帖子：</span><span class="sxs-lookup"><span data-stu-id="e3668-105">Even though you cannot explicitly create a post, doing any of the following would create a post:</span></span>

* [<span data-ttu-id="e3668-106">答复现有帖子</span><span class="sxs-lookup"><span data-stu-id="e3668-106">Reply to an existing post</span></span>](../api/post-reply.md) 
* [<span data-ttu-id="e3668-107">答复现有线程</span><span class="sxs-lookup"><span data-stu-id="e3668-107">Reply to an existing thread</span></span>](../api/conversationthread-reply.md) 
* [<span data-ttu-id="e3668-108">在新对话中创建线程</span><span class="sxs-lookup"><span data-stu-id="e3668-108">Create a thread in a new conversation</span></span>](../api/group-post-threads.md)
* [<span data-ttu-id="e3668-109">创建新对话</span><span class="sxs-lookup"><span data-stu-id="e3668-109">Create a new conversation</span></span>](../api/group-post-conversations.md)

<span data-ttu-id="e3668-110">通过该资源可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="e3668-110">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3668-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3668-111">JSON representation</span></span>

<span data-ttu-id="e3668-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3668-112">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "extensions",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
## <a name="properties"></a><span data-ttu-id="e3668-113">属性</span><span class="sxs-lookup"><span data-stu-id="e3668-113">Properties</span></span>
| <span data-ttu-id="e3668-114">属性</span><span class="sxs-lookup"><span data-stu-id="e3668-114">Property</span></span>     | <span data-ttu-id="e3668-115">类型</span><span class="sxs-lookup"><span data-stu-id="e3668-115">Type</span></span>   |<span data-ttu-id="e3668-116">说明</span><span class="sxs-lookup"><span data-stu-id="e3668-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3668-117">body</span><span class="sxs-lookup"><span data-stu-id="e3668-117">body</span></span>|[<span data-ttu-id="e3668-118">itemBody</span><span class="sxs-lookup"><span data-stu-id="e3668-118">itemBody</span></span>](itembody.md)|<span data-ttu-id="e3668-p101">帖子的内容。这是默认属性。此属性可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e3668-p101">The contents of the post. This is a default property. This property can be null.</span></span>|
|<span data-ttu-id="e3668-122">categories</span><span class="sxs-lookup"><span data-stu-id="e3668-122">categories</span></span>|<span data-ttu-id="e3668-123">String collection</span><span class="sxs-lookup"><span data-stu-id="e3668-123">String collection</span></span>|<span data-ttu-id="e3668-124">与帖子关联的类别。</span><span class="sxs-lookup"><span data-stu-id="e3668-124">The categories associated with the post.</span></span> <span data-ttu-id="e3668-125">每个类别对应于已为用户定义的[outlookCategory](outlookcategory.md)的**displayName**属性。</span><span class="sxs-lookup"><span data-stu-id="e3668-125">Each category corresponds to the **displayName** property of an [outlookCategory](outlookcategory.md) that has been defined for a user.</span></span>|
|<span data-ttu-id="e3668-126">changeKey</span><span class="sxs-lookup"><span data-stu-id="e3668-126">changeKey</span></span>|<span data-ttu-id="e3668-127">字符串</span><span class="sxs-lookup"><span data-stu-id="e3668-127">String</span></span>|<span data-ttu-id="e3668-p103">标识帖子的版本。每次帖子更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="e3668-p103">Identifies the version of the post. Every time the post is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="e3668-131">conversationId</span><span class="sxs-lookup"><span data-stu-id="e3668-131">conversationId</span></span>|<span data-ttu-id="e3668-132">String</span><span class="sxs-lookup"><span data-stu-id="e3668-132">String</span></span>|<span data-ttu-id="e3668-p104">对话的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="e3668-p104">Unique ID of the conversation. Read-only.</span></span>|
|<span data-ttu-id="e3668-135">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="e3668-135">conversationThreadId</span></span>|<span data-ttu-id="e3668-136">字符串</span><span class="sxs-lookup"><span data-stu-id="e3668-136">String</span></span>|<span data-ttu-id="e3668-p105">对话线程的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="e3668-p105">Unique ID of the conversation thread. Read-only.</span></span>|
|<span data-ttu-id="e3668-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3668-139">createdDateTime</span></span>|<span data-ttu-id="e3668-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3668-140">DateTimeOffset</span></span>|<span data-ttu-id="e3668-p106">创建帖子时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e3668-p106">Specifies when the post was created. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e3668-144">发件人</span><span class="sxs-lookup"><span data-stu-id="e3668-144">from</span></span>|[<span data-ttu-id="e3668-145">recipient</span><span class="sxs-lookup"><span data-stu-id="e3668-145">recipient</span></span>](recipient.md)|<span data-ttu-id="e3668-p107">在委派访问方案中使用。指示代表另一用户发布了此邮件的帐户。这是默认属性。</span><span class="sxs-lookup"><span data-stu-id="e3668-p107">Used in delegate access scenarios. Indicates who posted the message on behalf of another user. This is a default property.</span></span>|
|<span data-ttu-id="e3668-149">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="e3668-149">hasAttachments</span></span>|<span data-ttu-id="e3668-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3668-150">Boolean</span></span>|<span data-ttu-id="e3668-p108">指示帖子是否具有至少一个附件。这是默认属性。</span><span class="sxs-lookup"><span data-stu-id="e3668-p108">Indicates whether the post has at least one attachment. This is a default property.</span></span>|
|<span data-ttu-id="e3668-153">id</span><span class="sxs-lookup"><span data-stu-id="e3668-153">id</span></span>|<span data-ttu-id="e3668-154">String</span><span class="sxs-lookup"><span data-stu-id="e3668-154">String</span></span>| <span data-ttu-id="e3668-155">只读。</span><span class="sxs-lookup"><span data-stu-id="e3668-155">Read-only.</span></span>|
|<span data-ttu-id="e3668-156">importance</span><span class="sxs-lookup"><span data-stu-id="e3668-156">importance</span></span> | <span data-ttu-id="e3668-157">String</span><span class="sxs-lookup"><span data-stu-id="e3668-157">String</span></span> | <span data-ttu-id="e3668-158">组帖子的重要性: `low`、 `normal`、。 `high`</span><span class="sxs-lookup"><span data-stu-id="e3668-158">The importance of a group post: `low`, `normal`, `high`.</span></span> |
|<span data-ttu-id="e3668-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3668-159">lastModifiedDateTime</span></span>|<span data-ttu-id="e3668-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3668-160">DateTimeOffset</span></span>|<span data-ttu-id="e3668-p109">帖子上次修改时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e3668-p109">Specifies when the post was last modified. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e3668-164">newParticipants</span><span class="sxs-lookup"><span data-stu-id="e3668-164">newParticipants</span></span>|<span data-ttu-id="e3668-165">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="e3668-165">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="e3668-166">添加到此线程作为帖子一部分的对话参与者。</span><span class="sxs-lookup"><span data-stu-id="e3668-166">Conversation participants that were added to the thread as part of this post.</span></span>|
|<span data-ttu-id="e3668-167">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3668-167">receivedDateTime</span></span>|<span data-ttu-id="e3668-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3668-168">DateTimeOffset</span></span>|<span data-ttu-id="e3668-p110">接收到帖子时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e3668-p110">Specifies when the post was received. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e3668-172">sender</span><span class="sxs-lookup"><span data-stu-id="e3668-172">sender</span></span>|[<span data-ttu-id="e3668-173">recipient</span><span class="sxs-lookup"><span data-stu-id="e3668-173">recipient</span></span>](recipient.md)|<span data-ttu-id="e3668-p111">包含发件人的地址未指定发件人时，发件人的值假定为已经过验证身份的用户的地址。这是默认属性。</span><span class="sxs-lookup"><span data-stu-id="e3668-p111">Contains the address of the sender. The value of Sender is assumed to be the address of the authenticated user in the case when Sender is not specified. This is a default property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3668-177">关系</span><span class="sxs-lookup"><span data-stu-id="e3668-177">Relationships</span></span>
| <span data-ttu-id="e3668-178">关系</span><span class="sxs-lookup"><span data-stu-id="e3668-178">Relationship</span></span> | <span data-ttu-id="e3668-179">类型</span><span class="sxs-lookup"><span data-stu-id="e3668-179">Type</span></span>   |<span data-ttu-id="e3668-180">说明</span><span class="sxs-lookup"><span data-stu-id="e3668-180">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3668-181">attachments</span><span class="sxs-lookup"><span data-stu-id="e3668-181">attachments</span></span>|<span data-ttu-id="e3668-182">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e3668-182">[Attachment](attachment.md) collection</span></span>|<span data-ttu-id="e3668-183">张贴内容的[fileAttachment](fileattachment.md)、 [itemAttachment](itemattachment.md)和[referenceAttachment](referenceattachment.md)附件的集合。</span><span class="sxs-lookup"><span data-stu-id="e3668-183">The collection of [fileAttachment](fileattachment.md), [itemAttachment](itemattachment.md), and [referenceAttachment](referenceattachment.md) attachments for the post.</span></span> <span data-ttu-id="e3668-184">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="e3668-184">Read-only.</span></span> <span data-ttu-id="e3668-185">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e3668-185">Nullable.</span></span>|
|<span data-ttu-id="e3668-186">extensions</span><span class="sxs-lookup"><span data-stu-id="e3668-186">extensions</span></span>|<span data-ttu-id="e3668-187">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="e3668-187">[Extension](extension.md) collection</span></span>|<span data-ttu-id="e3668-p113">为帖子定义的开放扩展集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e3668-p113">The collection of open extensions defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e3668-191">inReplyTo</span><span class="sxs-lookup"><span data-stu-id="e3668-191">inReplyTo</span></span>|[<span data-ttu-id="e3668-192">Post</span><span class="sxs-lookup"><span data-stu-id="e3668-192">Post</span></span>](post.md)|<span data-ttu-id="e3668-193">此文章在[conversationThread](conversationthread.md)中答复的早期帖子。</span><span class="sxs-lookup"><span data-stu-id="e3668-193">The earlier post that this post is replying to in the [conversationThread](conversationthread.md).</span></span> <span data-ttu-id="e3668-194">只读。</span><span class="sxs-lookup"><span data-stu-id="e3668-194">Read-only.</span></span>|
|<span data-ttu-id="e3668-195">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="e3668-195">multiValueExtendedProperties</span></span>|<span data-ttu-id="e3668-196">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e3668-196">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="e3668-p115">为帖子定义的多值扩展属性的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e3668-p115">The collection of multi-value extended properties defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e3668-200">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="e3668-200">singleValueExtendedProperties</span></span>|<span data-ttu-id="e3668-201">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="e3668-201">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="e3668-p116">为帖子定义的单值扩展属性的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e3668-p116">The collection of single-value extended properties defined for the post. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="e3668-205">方法</span><span class="sxs-lookup"><span data-stu-id="e3668-205">Methods</span></span>

| <span data-ttu-id="e3668-206">方法</span><span class="sxs-lookup"><span data-stu-id="e3668-206">Method</span></span>           | <span data-ttu-id="e3668-207">返回类型</span><span class="sxs-lookup"><span data-stu-id="e3668-207">Return Type</span></span>    |<span data-ttu-id="e3668-208">说明</span><span class="sxs-lookup"><span data-stu-id="e3668-208">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e3668-209">列出帖子</span><span class="sxs-lookup"><span data-stu-id="e3668-209">List posts</span></span>](../api/conversationthread-list-posts.md) | [<span data-ttu-id="e3668-210">帖子</span><span class="sxs-lookup"><span data-stu-id="e3668-210">post</span></span>](post.md) |<span data-ttu-id="e3668-211">获取指定线程的帖子。</span><span class="sxs-lookup"><span data-stu-id="e3668-211">Get the posts of the specified thread.</span></span> |
|[<span data-ttu-id="e3668-212">获取帖子</span><span class="sxs-lookup"><span data-stu-id="e3668-212">Get post</span></span>](../api/post-get.md) | [<span data-ttu-id="e3668-213">帖子</span><span class="sxs-lookup"><span data-stu-id="e3668-213">post</span></span>](post.md) |<span data-ttu-id="e3668-214">获取指定的线程中帖子的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e3668-214">Get the properties and relationships of a post in a specified thread.</span></span>|
|[<span data-ttu-id="e3668-215">答复</span><span class="sxs-lookup"><span data-stu-id="e3668-215">Reply</span></span>](../api/post-reply.md)|<span data-ttu-id="e3668-216">无</span><span class="sxs-lookup"><span data-stu-id="e3668-216">None</span></span>|<span data-ttu-id="e3668-217">在组对话中答复帖子，并向指定线程中添加新帖子。</span><span class="sxs-lookup"><span data-stu-id="e3668-217">Reply to a post and add a new post to the specified thread in a group conversation.</span></span>|
|[<span data-ttu-id="e3668-218">转发</span><span class="sxs-lookup"><span data-stu-id="e3668-218">Forward</span></span>](../api/post-forward.md)|<span data-ttu-id="e3668-219">无</span><span class="sxs-lookup"><span data-stu-id="e3668-219">None</span></span>|<span data-ttu-id="e3668-220">将帖子转发给收件人。</span><span class="sxs-lookup"><span data-stu-id="e3668-220">Forward a post to a recipient.</span></span>|
|<span data-ttu-id="e3668-221">**附件**</span><span class="sxs-lookup"><span data-stu-id="e3668-221">**Attachments**</span></span>| | |
|[<span data-ttu-id="e3668-222">列出附件</span><span class="sxs-lookup"><span data-stu-id="e3668-222">List attachments</span></span>](../api/post-list-attachments.md) |<span data-ttu-id="e3668-223">[attachment](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e3668-223">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="e3668-224">获取帖子的所有附件。</span><span class="sxs-lookup"><span data-stu-id="e3668-224">Get all attachments on a post.</span></span>|
|[<span data-ttu-id="e3668-225">Add attachment</span><span class="sxs-lookup"><span data-stu-id="e3668-225">Add attachment</span></span>](../api/post-post-attachments.md) |[<span data-ttu-id="e3668-226">attachment</span><span class="sxs-lookup"><span data-stu-id="e3668-226">attachment</span></span>](attachment.md)| <span data-ttu-id="e3668-227">将附件添加到帖子中。</span><span class="sxs-lookup"><span data-stu-id="e3668-227">Add an attachment to a post.</span></span> |
|<span data-ttu-id="e3668-228">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="e3668-228">**Open extensions**</span></span>| | |
|[<span data-ttu-id="e3668-229">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="e3668-229">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="e3668-230">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="e3668-230">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="e3668-231">创建开放扩展，并将自定义属性添加到新资源或现有资源。</span><span class="sxs-lookup"><span data-stu-id="e3668-231">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="e3668-232">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="e3668-232">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="e3668-233">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e3668-233">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="e3668-234">获取扩展名称标识的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="e3668-234">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="e3668-235">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="e3668-235">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="e3668-236">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="e3668-236">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="e3668-237">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="e3668-237">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="e3668-238">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="e3668-238">**Extended properties**</span></span>| | |
|[<span data-ttu-id="e3668-239">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="e3668-239">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="e3668-240">帖子</span><span class="sxs-lookup"><span data-stu-id="e3668-240">post</span></span>](post.md)  |<span data-ttu-id="e3668-241">在新建或现有帖子中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e3668-241">Create one or more single-value extended properties in a new or existing post.</span></span>   |
|[<span data-ttu-id="e3668-242">获取具有单值扩展属性的帖子</span><span class="sxs-lookup"><span data-stu-id="e3668-242">Get post with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="e3668-243">帖子</span><span class="sxs-lookup"><span data-stu-id="e3668-243">post</span></span>](post.md) | <span data-ttu-id="e3668-244">通过使用 `$expand` or `$filter` 获取包含单值扩展属性的帖子。</span><span class="sxs-lookup"><span data-stu-id="e3668-244">Get posts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="e3668-245">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="e3668-245">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="e3668-246">帖子</span><span class="sxs-lookup"><span data-stu-id="e3668-246">post</span></span>](post.md) | <span data-ttu-id="e3668-247">在新建或现有的帖子中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e3668-247">Create one or more multi-value extended properties in a new or existing post.</span></span>  |
|[<span data-ttu-id="e3668-248">获取具有多值扩展属性的帖子</span><span class="sxs-lookup"><span data-stu-id="e3668-248">Get post with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="e3668-249">帖子</span><span class="sxs-lookup"><span data-stu-id="e3668-249">post</span></span>](post.md) | <span data-ttu-id="e3668-250">使用 `$expand` 获取包含一个多值扩展属性的帖子。</span><span class="sxs-lookup"><span data-stu-id="e3668-250">Get a post that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="see-also"></a><span data-ttu-id="e3668-251">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e3668-251">See also</span></span>

- [<span data-ttu-id="e3668-252">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e3668-252">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e3668-253">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e3668-253">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="e3668-254">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e3668-254">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
