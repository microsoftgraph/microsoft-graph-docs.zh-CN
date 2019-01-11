---
title: 帖子资源类型
description: 代表 converstaionThread 实体内的单个公告项目。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 1912917347697a6f78876175e6fe9f9c160869e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834039"
---
# <a name="post-resource-type"></a><span data-ttu-id="b1791-103">帖子资源类型</span><span class="sxs-lookup"><span data-stu-id="b1791-103">post resource type</span></span>

> <span data-ttu-id="b1791-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b1791-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1791-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b1791-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1791-106">代表[converstaionThread](conversationthread.md)实体内的单个公告项目。</span><span class="sxs-lookup"><span data-stu-id="b1791-106">Represents an individual post item within a [converstaionThread](conversationthread.md) entity.</span></span>

<span data-ttu-id="b1791-107">即使无法显式创建帖子，也可以执行以下任一操作来创建帖子：</span><span class="sxs-lookup"><span data-stu-id="b1791-107">Even though you cannot explicitly create a post, doing any of the following would create a post:</span></span>

* [<span data-ttu-id="b1791-108">答复现有帖子</span><span class="sxs-lookup"><span data-stu-id="b1791-108">Reply to an existing post</span></span>](../api/post-reply.md) 
* [<span data-ttu-id="b1791-109">答复现有线程</span><span class="sxs-lookup"><span data-stu-id="b1791-109">Reply to an existing thread</span></span>](../api/conversationthread-reply.md) 
* [<span data-ttu-id="b1791-110">在新对话中创建线程</span><span class="sxs-lookup"><span data-stu-id="b1791-110">Create a thread in a new conversation</span></span>](../api/group-post-threads.md)
* [<span data-ttu-id="b1791-111">创建新对话</span><span class="sxs-lookup"><span data-stu-id="b1791-111">Create a new conversation</span></span>](../api/group-post-conversations.md)

<span data-ttu-id="b1791-112">通过该资源可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="b1791-112">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1791-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1791-113">JSON representation</span></span>

<span data-ttu-id="b1791-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1791-114">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="b1791-115">属性</span><span class="sxs-lookup"><span data-stu-id="b1791-115">Properties</span></span>
| <span data-ttu-id="b1791-116">属性</span><span class="sxs-lookup"><span data-stu-id="b1791-116">Property</span></span>     | <span data-ttu-id="b1791-117">类型</span><span class="sxs-lookup"><span data-stu-id="b1791-117">Type</span></span>   |<span data-ttu-id="b1791-118">说明</span><span class="sxs-lookup"><span data-stu-id="b1791-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1791-119">body</span><span class="sxs-lookup"><span data-stu-id="b1791-119">body</span></span>|[<span data-ttu-id="b1791-120">itemBody</span><span class="sxs-lookup"><span data-stu-id="b1791-120">itemBody</span></span>](itembody.md)|<span data-ttu-id="b1791-p102">帖子的内容。这是默认属性。此属性可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="b1791-p102">The contents of the post. This is a default property. This property can be null.</span></span>|
|<span data-ttu-id="b1791-124">categories</span><span class="sxs-lookup"><span data-stu-id="b1791-124">categories</span></span>|<span data-ttu-id="b1791-125">String collection</span><span class="sxs-lookup"><span data-stu-id="b1791-125">String collection</span></span>|<span data-ttu-id="b1791-126">与帖子关联的类别。</span><span class="sxs-lookup"><span data-stu-id="b1791-126">The categories associated with the post.</span></span> <span data-ttu-id="b1791-127">每个类别对应于已为用户定义[outlookCategory](outlookcategory.md)的**displayName**属性。</span><span class="sxs-lookup"><span data-stu-id="b1791-127">Each category corresponds to the **displayName** property of an [outlookCategory](outlookcategory.md) that has been defined for a user.</span></span>|
|<span data-ttu-id="b1791-128">changeKey</span><span class="sxs-lookup"><span data-stu-id="b1791-128">changeKey</span></span>|<span data-ttu-id="b1791-129">String</span><span class="sxs-lookup"><span data-stu-id="b1791-129">String</span></span>|<span data-ttu-id="b1791-p104">标识帖子的版本。每次帖子更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="b1791-p104">Identifies the version of the post. Every time the post is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="b1791-133">conversationId</span><span class="sxs-lookup"><span data-stu-id="b1791-133">conversationId</span></span>|<span data-ttu-id="b1791-134">String</span><span class="sxs-lookup"><span data-stu-id="b1791-134">String</span></span>|<span data-ttu-id="b1791-p105">对话的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="b1791-p105">Unique ID of the conversation. Read-only.</span></span>|
|<span data-ttu-id="b1791-137">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="b1791-137">conversationThreadId</span></span>|<span data-ttu-id="b1791-138">String</span><span class="sxs-lookup"><span data-stu-id="b1791-138">String</span></span>|<span data-ttu-id="b1791-p106">对话线程的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="b1791-p106">Unique ID of the conversation thread. Read-only.</span></span>|
|<span data-ttu-id="b1791-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1791-141">createdDateTime</span></span>|<span data-ttu-id="b1791-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1791-142">DateTimeOffset</span></span>|<span data-ttu-id="b1791-p107">创建帖子时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b1791-p107">Specifies when the post was created. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b1791-146">from</span><span class="sxs-lookup"><span data-stu-id="b1791-146">from</span></span>|[<span data-ttu-id="b1791-147">收件人</span><span class="sxs-lookup"><span data-stu-id="b1791-147">recipient</span></span>](recipient.md)|<span data-ttu-id="b1791-p108">在委派访问方案中使用。指示代表另一用户发布了此邮件的帐户。这是默认属性。</span><span class="sxs-lookup"><span data-stu-id="b1791-p108">Used in delegate access scenarios. Indicates who posted the message on behalf of another user. This is a default property.</span></span>|
|<span data-ttu-id="b1791-151">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="b1791-151">hasAttachments</span></span>|<span data-ttu-id="b1791-152">布尔</span><span class="sxs-lookup"><span data-stu-id="b1791-152">Boolean</span></span>|<span data-ttu-id="b1791-p109">指示帖子是否具有至少一个附件。这是默认属性。</span><span class="sxs-lookup"><span data-stu-id="b1791-p109">Indicates whether the post has at least one attachment. This is a default property.</span></span>|
|<span data-ttu-id="b1791-155">id</span><span class="sxs-lookup"><span data-stu-id="b1791-155">id</span></span>|<span data-ttu-id="b1791-156">String</span><span class="sxs-lookup"><span data-stu-id="b1791-156">String</span></span>| <span data-ttu-id="b1791-157">只读。</span><span class="sxs-lookup"><span data-stu-id="b1791-157">Read-only.</span></span>|
|<span data-ttu-id="b1791-158">importance</span><span class="sxs-lookup"><span data-stu-id="b1791-158">importance</span></span> | <span data-ttu-id="b1791-159">String</span><span class="sxs-lookup"><span data-stu-id="b1791-159">String</span></span> | <span data-ttu-id="b1791-160">组文章的重要性： `low`， `normal`， `high`。</span><span class="sxs-lookup"><span data-stu-id="b1791-160">The importance of a group post: `low`, `normal`, `high`.</span></span> |
|<span data-ttu-id="b1791-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1791-161">lastModifiedDateTime</span></span>|<span data-ttu-id="b1791-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1791-162">DateTimeOffset</span></span>|<span data-ttu-id="b1791-p110">帖子上次修改时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b1791-p110">Specifies when the post was last modified. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b1791-166">newParticipants</span><span class="sxs-lookup"><span data-stu-id="b1791-166">newParticipants</span></span>|<span data-ttu-id="b1791-167">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="b1791-167">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="b1791-168">添加到此线程作为帖子一部分的对话参与者。</span><span class="sxs-lookup"><span data-stu-id="b1791-168">Conversation participants that were added to the thread as part of this post.</span></span>|
|<span data-ttu-id="b1791-169">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1791-169">receivedDateTime</span></span>|<span data-ttu-id="b1791-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1791-170">DateTimeOffset</span></span>|<span data-ttu-id="b1791-p111">接收到帖子时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b1791-p111">Specifies when the post was received. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b1791-174">sender</span><span class="sxs-lookup"><span data-stu-id="b1791-174">sender</span></span>|[<span data-ttu-id="b1791-175">recipient</span><span class="sxs-lookup"><span data-stu-id="b1791-175">recipient</span></span>](recipient.md)|<span data-ttu-id="b1791-p112">包含发件人的地址未指定发件人时，发件人的值假定为已经过验证身份的用户的地址。这是默认属性。</span><span class="sxs-lookup"><span data-stu-id="b1791-p112">Contains the address of the sender. The value of Sender is assumed to be the address of the authenticated user in the case when Sender is not specified. This is a default property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1791-179">Relationships</span><span class="sxs-lookup"><span data-stu-id="b1791-179">Relationships</span></span>
| <span data-ttu-id="b1791-180">关系</span><span class="sxs-lookup"><span data-stu-id="b1791-180">Relationship</span></span> | <span data-ttu-id="b1791-181">类型</span><span class="sxs-lookup"><span data-stu-id="b1791-181">Type</span></span>   |<span data-ttu-id="b1791-182">说明</span><span class="sxs-lookup"><span data-stu-id="b1791-182">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1791-183">attachments</span><span class="sxs-lookup"><span data-stu-id="b1791-183">attachments</span></span>|<span data-ttu-id="b1791-184">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b1791-184">[Attachment](attachment.md) collection</span></span>|<span data-ttu-id="b1791-185">为公告[fileAttachment](fileattachment.md)和[itemAttachment](itemattachment.md)， [referenceAttachment](referenceattachment.md)附件的集合。</span><span class="sxs-lookup"><span data-stu-id="b1791-185">The collection of [fileAttachment](fileattachment.md), [itemAttachment](itemattachment.md), and [referenceAttachment](referenceattachment.md) attachments for the post.</span></span> <span data-ttu-id="b1791-186">只读。</span><span class="sxs-lookup"><span data-stu-id="b1791-186">Read-only.</span></span> <span data-ttu-id="b1791-187">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b1791-187">Nullable.</span></span>|
|<span data-ttu-id="b1791-188">extensions</span><span class="sxs-lookup"><span data-stu-id="b1791-188">extensions</span></span>|<span data-ttu-id="b1791-189">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="b1791-189">[Extension](extension.md) collection</span></span>|<span data-ttu-id="b1791-p114">为帖子定义的开放扩展集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="b1791-p114">The collection of open extensions defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="b1791-193">inReplyTo</span><span class="sxs-lookup"><span data-stu-id="b1791-193">inReplyTo</span></span>|[<span data-ttu-id="b1791-194">Post</span><span class="sxs-lookup"><span data-stu-id="b1791-194">Post</span></span>](post.md)|<span data-ttu-id="b1791-195">此文章答复中[conversationThread](conversationthread.md)早期文章。</span><span class="sxs-lookup"><span data-stu-id="b1791-195">The earlier post that this post is replying to in the [conversationThread](conversationthread.md).</span></span> <span data-ttu-id="b1791-196">只读。</span><span class="sxs-lookup"><span data-stu-id="b1791-196">Read-only.</span></span>|
|<span data-ttu-id="b1791-197">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b1791-197">multiValueExtendedProperties</span></span>|<span data-ttu-id="b1791-198">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b1791-198">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="b1791-p116">为帖子定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b1791-p116">The collection of multi-value extended properties defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="b1791-202">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b1791-202">singleValueExtendedProperties</span></span>|<span data-ttu-id="b1791-203">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b1791-203">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="b1791-p117">为帖子定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b1791-p117">The collection of single-value extended properties defined for the post. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="b1791-207">方法</span><span class="sxs-lookup"><span data-stu-id="b1791-207">Methods</span></span>

| <span data-ttu-id="b1791-208">方法</span><span class="sxs-lookup"><span data-stu-id="b1791-208">Method</span></span>           | <span data-ttu-id="b1791-209">返回类型</span><span class="sxs-lookup"><span data-stu-id="b1791-209">Return Type</span></span>    |<span data-ttu-id="b1791-210">说明</span><span class="sxs-lookup"><span data-stu-id="b1791-210">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b1791-211">列出帖子</span><span class="sxs-lookup"><span data-stu-id="b1791-211">List posts</span></span>](../api/conversationthread-list-posts.md) | [<span data-ttu-id="b1791-212">帖子</span><span class="sxs-lookup"><span data-stu-id="b1791-212">post</span></span>](post.md) |<span data-ttu-id="b1791-213">获取指定线程的帖子。</span><span class="sxs-lookup"><span data-stu-id="b1791-213">Get the posts of the specified thread.</span></span> |
|[<span data-ttu-id="b1791-214">获取帖子</span><span class="sxs-lookup"><span data-stu-id="b1791-214">Get post</span></span>](../api/post-get.md) | [<span data-ttu-id="b1791-215">帖子</span><span class="sxs-lookup"><span data-stu-id="b1791-215">post</span></span>](post.md) |<span data-ttu-id="b1791-216">获取指定的线程中帖子的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b1791-216">Get the properties and relationships of a post in a specified thread.</span></span>|
|[<span data-ttu-id="b1791-217">答复</span><span class="sxs-lookup"><span data-stu-id="b1791-217">Reply</span></span>](../api/post-reply.md)|<span data-ttu-id="b1791-218">无</span><span class="sxs-lookup"><span data-stu-id="b1791-218">None</span></span>|<span data-ttu-id="b1791-219">在组对话中答复帖子，并向指定线程中添加新帖子。</span><span class="sxs-lookup"><span data-stu-id="b1791-219">Reply to a post and add a new post to the specified thread in a group conversation.</span></span>|
|[<span data-ttu-id="b1791-220">转发</span><span class="sxs-lookup"><span data-stu-id="b1791-220">Forward</span></span>](../api/post-forward.md)|<span data-ttu-id="b1791-221">无</span><span class="sxs-lookup"><span data-stu-id="b1791-221">None</span></span>|<span data-ttu-id="b1791-222">将帖子转发给收件人。</span><span class="sxs-lookup"><span data-stu-id="b1791-222">Forward a post to a recipient.</span></span>|
|<span data-ttu-id="b1791-223">**Attachments**</span><span class="sxs-lookup"><span data-stu-id="b1791-223">**Attachments**</span></span>| | |
|[<span data-ttu-id="b1791-224">列出附件</span><span class="sxs-lookup"><span data-stu-id="b1791-224">List attachments</span></span>](../api/post-list-attachments.md) |<span data-ttu-id="b1791-225">[attachment](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b1791-225">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="b1791-226">获取帖子的所有附件。</span><span class="sxs-lookup"><span data-stu-id="b1791-226">Get all attachments on a post.</span></span>|
|[<span data-ttu-id="b1791-227">Add attachment</span><span class="sxs-lookup"><span data-stu-id="b1791-227">Add attachment</span></span>](../api/post-post-attachments.md) |[<span data-ttu-id="b1791-228">attachment</span><span class="sxs-lookup"><span data-stu-id="b1791-228">attachment</span></span>](attachment.md)| <span data-ttu-id="b1791-229">将附件添加到帖子中。</span><span class="sxs-lookup"><span data-stu-id="b1791-229">Add an attachment to a post.</span></span> |
|<span data-ttu-id="b1791-230">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="b1791-230">**Open extensions**</span></span>| | |
|[<span data-ttu-id="b1791-231">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="b1791-231">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="b1791-232">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="b1791-232">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="b1791-233">创建开放扩展，并将自定义属性添加到新资源或现有资源。</span><span class="sxs-lookup"><span data-stu-id="b1791-233">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="b1791-234">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="b1791-234">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="b1791-235">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b1791-235">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="b1791-236">获取扩展名称标识的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="b1791-236">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="b1791-237">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="b1791-237">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="b1791-238">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="b1791-238">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="b1791-239">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="b1791-239">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="b1791-240">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="b1791-240">**Extended properties**</span></span>| | |
|[<span data-ttu-id="b1791-241">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="b1791-241">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="b1791-242">帖子</span><span class="sxs-lookup"><span data-stu-id="b1791-242">post</span></span>](post.md)  |<span data-ttu-id="b1791-243">在新建或现有帖子中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b1791-243">Create one or more single-value extended properties in a new or existing post.</span></span>   |
|[<span data-ttu-id="b1791-244">获取具有单值扩展属性的帖子</span><span class="sxs-lookup"><span data-stu-id="b1791-244">Get post with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="b1791-245">帖子</span><span class="sxs-lookup"><span data-stu-id="b1791-245">post</span></span>](post.md) | <span data-ttu-id="b1791-246">通过使用 `$expand` or `$filter` 获取包含单值扩展属性的帖子。</span><span class="sxs-lookup"><span data-stu-id="b1791-246">Get posts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="b1791-247">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="b1791-247">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="b1791-248">帖子</span><span class="sxs-lookup"><span data-stu-id="b1791-248">post</span></span>](post.md) | <span data-ttu-id="b1791-249">在新建或现有的帖子中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b1791-249">Create one or more multi-value extended properties in a new or existing post.</span></span>  |
|[<span data-ttu-id="b1791-250">获取具有多值扩展属性的帖子</span><span class="sxs-lookup"><span data-stu-id="b1791-250">Get post with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="b1791-251">帖子</span><span class="sxs-lookup"><span data-stu-id="b1791-251">post</span></span>](post.md) | <span data-ttu-id="b1791-252">使用 `$expand` 获取包含一个多值扩展属性的帖子。</span><span class="sxs-lookup"><span data-stu-id="b1791-252">Get a post that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="see-also"></a><span data-ttu-id="b1791-253">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b1791-253">See also</span></span>

- [<span data-ttu-id="b1791-254">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b1791-254">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b1791-255">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b1791-255">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="b1791-256">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b1791-256">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
