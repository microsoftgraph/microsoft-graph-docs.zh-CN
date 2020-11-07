---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 聊天消息可以是一个根聊天消息，也可以是由聊天消息中的 **replyToId** 属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 16bcd870ba8d4b97b5951fefab538eb6b6669635
ms.sourcegitcommit: 22d99624036ceaeb1b612538d5196faaa743881f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2020
ms.locfileid: "48932575"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="879be-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="879be-104">chatMessage resource type</span></span>

<span data-ttu-id="879be-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="879be-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="879be-106">代表 beta) [研讨](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)中的[频道](./channel.md)或 (内的单个聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="879be-106">Represents an individual chat message within a [channel](./channel.md) or (in beta) [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="879be-107">聊天消息可以是一个根聊天消息，也可以是由聊天消息中的 **replyToId** 属性定义的答复线程的一部分。</span><span class="sxs-lookup"><span data-stu-id="879be-107">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="879be-108">方法</span><span class="sxs-lookup"><span data-stu-id="879be-108">Methods</span></span>

| <span data-ttu-id="879be-109">方法</span><span class="sxs-lookup"><span data-stu-id="879be-109">Method</span></span>       | <span data-ttu-id="879be-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="879be-110">Return Type</span></span>  |<span data-ttu-id="879be-111">说明</span><span class="sxs-lookup"><span data-stu-id="879be-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="879be-112">**通道邮件**</span><span class="sxs-lookup"><span data-stu-id="879be-112">**Channel messages**</span></span>| | |
|[<span data-ttu-id="879be-113">列出频道了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="879be-113">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="879be-114">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="879be-114">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="879be-115">频道中所有根聊天邮件的列表。</span><span class="sxs-lookup"><span data-stu-id="879be-115">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="879be-116">在频道 delta 中获取 Chatmessages 集合</span><span class="sxs-lookup"><span data-stu-id="879be-116">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="879be-117">chatMessage</span><span class="sxs-lookup"><span data-stu-id="879be-117">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="879be-118">获取通道中的增量聊天消息。</span><span class="sxs-lookup"><span data-stu-id="879be-118">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="879be-119">为新的频道消息创建订阅</span><span class="sxs-lookup"><span data-stu-id="879be-119">Create subscription for new channel messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="879be-120">订阅</span><span class="sxs-lookup"><span data-stu-id="879be-120">subscription</span></span>](subscription.md) | <span data-ttu-id="879be-121">收听新的和编辑的频道消息以及对它们的反应。</span><span class="sxs-lookup"><span data-stu-id="879be-121">Listen for new and edited channel messages, and reactions to them.</span></span> |
|[<span data-ttu-id="879be-122">获取频道了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="879be-122">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="879be-123">chatMessage</span><span class="sxs-lookup"><span data-stu-id="879be-123">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="879be-124">从频道中获取单个根聊天消息。</span><span class="sxs-lookup"><span data-stu-id="879be-124">Get a single root chat message from a channel.</span></span>|
|[<span data-ttu-id="879be-125">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="879be-125">Create chatMessage in a channel</span></span>](../api/channel-post-message.md) | [<span data-ttu-id="879be-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="879be-126">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="879be-127">向频道发送消息。</span><span class="sxs-lookup"><span data-stu-id="879be-127">Send a message to a channel.</span></span> |
|[<span data-ttu-id="879be-128">更新了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="879be-128">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="879be-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="879be-129">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="879be-130">更新聊天邮件的 **policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="879be-130">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="879be-131">**频道邮件答复**</span><span class="sxs-lookup"><span data-stu-id="879be-131">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="879be-132">列出对了 chatmessage 的答复</span><span class="sxs-lookup"><span data-stu-id="879be-132">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="879be-133">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="879be-133">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="879be-134">频道中对聊天消息的所有回复的列表。</span><span class="sxs-lookup"><span data-stu-id="879be-134">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="879be-135">获取对了 chatmessage 的答复</span><span class="sxs-lookup"><span data-stu-id="879be-135">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="879be-136">chatMessage</span><span class="sxs-lookup"><span data-stu-id="879be-136">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="879be-137">获取频道中的聊天消息的单个答复。</span><span class="sxs-lookup"><span data-stu-id="879be-137">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="879be-138">答复频道中的了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="879be-138">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="879be-139">chatMessage</span><span class="sxs-lookup"><span data-stu-id="879be-139">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="879be-140">在频道中答复现有聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="879be-140">Reply to an existing chat message in a channel.</span></span>|
|[<span data-ttu-id="879be-141">更新了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="879be-141">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="879be-142">chatMessage</span><span class="sxs-lookup"><span data-stu-id="879be-142">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="879be-143">更新聊天邮件的 **policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="879be-143">Update the **policyViolation** property of a chat message.</span></span>|

## <a name="properties"></a><span data-ttu-id="879be-144">属性</span><span class="sxs-lookup"><span data-stu-id="879be-144">Properties</span></span>

| <span data-ttu-id="879be-145">属性</span><span class="sxs-lookup"><span data-stu-id="879be-145">Property</span></span>   | <span data-ttu-id="879be-146">类型</span><span class="sxs-lookup"><span data-stu-id="879be-146">Type</span></span> |<span data-ttu-id="879be-147">说明</span><span class="sxs-lookup"><span data-stu-id="879be-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="879be-148">id</span><span class="sxs-lookup"><span data-stu-id="879be-148">id</span></span>|<span data-ttu-id="879be-149">String</span><span class="sxs-lookup"><span data-stu-id="879be-149">String</span></span>| <span data-ttu-id="879be-150">只读。</span><span class="sxs-lookup"><span data-stu-id="879be-150">Read-only.</span></span> <span data-ttu-id="879be-151">邮件的唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="879be-151">Unique Id of the message.</span></span>|
|<span data-ttu-id="879be-152">replyToId</span><span class="sxs-lookup"><span data-stu-id="879be-152">replyToId</span></span>| <span data-ttu-id="879be-153">string</span><span class="sxs-lookup"><span data-stu-id="879be-153">string</span></span> | <span data-ttu-id="879be-154">只读。</span><span class="sxs-lookup"><span data-stu-id="879be-154">Read-only.</span></span> <span data-ttu-id="879be-155">线程的父聊天消息或根聊天消息的 Id。</span><span class="sxs-lookup"><span data-stu-id="879be-155">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="879be-156"> (仅适用于频道中不聊天的聊天消息) </span><span class="sxs-lookup"><span data-stu-id="879be-156">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="879be-157">from</span><span class="sxs-lookup"><span data-stu-id="879be-157">from</span></span>|[<span data-ttu-id="879be-158">identitySet</span><span class="sxs-lookup"><span data-stu-id="879be-158">identitySet</span></span>](identityset.md)| <span data-ttu-id="879be-159">只读。</span><span class="sxs-lookup"><span data-stu-id="879be-159">Read only.</span></span> <span data-ttu-id="879be-160">聊天消息发件人的详细信息。</span><span class="sxs-lookup"><span data-stu-id="879be-160">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="879be-161">etag</span><span class="sxs-lookup"><span data-stu-id="879be-161">etag</span></span>| <span data-ttu-id="879be-162">string</span><span class="sxs-lookup"><span data-stu-id="879be-162">string</span></span> | <span data-ttu-id="879be-163">只读。</span><span class="sxs-lookup"><span data-stu-id="879be-163">Read-only.</span></span> <span data-ttu-id="879be-164">聊天消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="879be-164">Version number of the chat message.</span></span> |
|<span data-ttu-id="879be-165">messageType</span><span class="sxs-lookup"><span data-stu-id="879be-165">messageType</span></span>|<span data-ttu-id="879be-166">string</span><span class="sxs-lookup"><span data-stu-id="879be-166">string</span></span>|<span data-ttu-id="879be-167">聊天消息的类型。</span><span class="sxs-lookup"><span data-stu-id="879be-167">The type of chat message.</span></span> <span data-ttu-id="879be-168">可能的值是： `message` 。</span><span class="sxs-lookup"><span data-stu-id="879be-168">The possible values are: `message`.</span></span>|
|<span data-ttu-id="879be-169">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="879be-169">createdDateTime</span></span>|<span data-ttu-id="879be-170">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="879be-170">dateTimeOffset</span></span>|<span data-ttu-id="879be-171">只读。</span><span class="sxs-lookup"><span data-stu-id="879be-171">Read only.</span></span> <span data-ttu-id="879be-172">在聊天消息创建时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="879be-172">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="879be-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="879be-173">lastModifiedDateTime</span></span>|<span data-ttu-id="879be-174">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="879be-174">dateTimeOffset</span></span>|<span data-ttu-id="879be-175">只读。</span><span class="sxs-lookup"><span data-stu-id="879be-175">Read only.</span></span> <span data-ttu-id="879be-176">在 (初始设置) 或编辑时（包括添加或删除反应时）创建聊天邮件时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="879be-176">Timestamp when the chat message is created (initial setting) or edited, including when a reaction is added or removed.</span></span> |
|<span data-ttu-id="879be-177">lastEditedDateTime</span><span class="sxs-lookup"><span data-stu-id="879be-177">lastEditedDateTime</span></span>|<span data-ttu-id="879be-178">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="879be-178">dateTimeOffset</span></span>|<span data-ttu-id="879be-179">只读。</span><span class="sxs-lookup"><span data-stu-id="879be-179">Read only.</span></span> <span data-ttu-id="879be-180">在对聊天消息进行编辑时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="879be-180">Timestamp when edits to the chat message were made.</span></span> <span data-ttu-id="879be-181">触发 Microsoft 团队 UI 中的 "编辑" 标志。</span><span class="sxs-lookup"><span data-stu-id="879be-181">Triggers an "Edited" flag in the Microsoft Teams UI.</span></span> <span data-ttu-id="879be-182">如果未进行任何编辑，则该值为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="879be-182">If no edits are made the value is `null`.</span></span>|
|<span data-ttu-id="879be-183">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="879be-183">deletedDateTime</span></span>|<span data-ttu-id="879be-184">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="879be-184">dateTimeOffset</span></span>|<span data-ttu-id="879be-185">只读。</span><span class="sxs-lookup"><span data-stu-id="879be-185">Read only.</span></span> <span data-ttu-id="879be-186">删除聊天邮件的时间戳，如果未删除，则为 null。</span><span class="sxs-lookup"><span data-stu-id="879be-186">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="879be-187">subject</span><span class="sxs-lookup"><span data-stu-id="879be-187">subject</span></span>|<span data-ttu-id="879be-188">string</span><span class="sxs-lookup"><span data-stu-id="879be-188">string</span></span>| <span data-ttu-id="879be-189">聊天消息的主题，以纯文本形式。</span><span class="sxs-lookup"><span data-stu-id="879be-189">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="879be-190">body</span><span class="sxs-lookup"><span data-stu-id="879be-190">body</span></span>|[<span data-ttu-id="879be-191">itemBody</span><span class="sxs-lookup"><span data-stu-id="879be-191">itemBody</span></span>](itembody.md)|<span data-ttu-id="879be-192">聊天消息内容的纯文本/HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="879be-192">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="879be-193">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="879be-193">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="879be-194">如果聊天消息包含 [chatMessageMention](chatmessagemention.md)，则该内容始终为 HTML。</span><span class="sxs-lookup"><span data-stu-id="879be-194">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="879be-195">摘要</span><span class="sxs-lookup"><span data-stu-id="879be-195">summary</span></span>|<span data-ttu-id="879be-196">string</span><span class="sxs-lookup"><span data-stu-id="879be-196">string</span></span>| <span data-ttu-id="879be-197">可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。</span><span class="sxs-lookup"><span data-stu-id="879be-197">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="879be-198">仅适用于频道聊天消息，而不是聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="879be-198">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="879be-199">附件</span><span class="sxs-lookup"><span data-stu-id="879be-199">attachments</span></span>|<span data-ttu-id="879be-200">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="879be-200">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="879be-201">附加文件。</span><span class="sxs-lookup"><span data-stu-id="879be-201">Attached files.</span></span> <span data-ttu-id="879be-202">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="879be-202">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="879be-203">提及</span><span class="sxs-lookup"><span data-stu-id="879be-203">mentions</span></span>|<span data-ttu-id="879be-204">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="879be-204">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="879be-205">聊天消息中提及的实体列表。</span><span class="sxs-lookup"><span data-stu-id="879be-205">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="879be-206">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="879be-206">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="879be-207">重要性</span><span class="sxs-lookup"><span data-stu-id="879be-207">importance</span></span>| <span data-ttu-id="879be-208">string</span><span class="sxs-lookup"><span data-stu-id="879be-208">string</span></span> | <span data-ttu-id="879be-209">聊天消息的重要性。</span><span class="sxs-lookup"><span data-stu-id="879be-209">The importance of the chat message.</span></span> <span data-ttu-id="879be-210">可能的值包括 `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="879be-210">The possible values are: `normal`, `high`, `urgent`.</span></span>|
| <span data-ttu-id="879be-211">policyViolation</span><span class="sxs-lookup"><span data-stu-id="879be-211">policyViolation</span></span> | [<span data-ttu-id="879be-212">chatMessagePolicyViolation</span><span class="sxs-lookup"><span data-stu-id="879be-212">chatMessagePolicyViolation</span></span>](../resources/chatmessagepolicyviolation.md) |<span data-ttu-id="879be-213">定义由数据丢失防护 (DLP) 应用程序设置的策略违规属性。</span><span class="sxs-lookup"><span data-stu-id="879be-213">Defines the properties of a policy violation set by a data loss prevention (DLP) application.</span></span>|
|<span data-ttu-id="879be-214">区域设置</span><span class="sxs-lookup"><span data-stu-id="879be-214">locale</span></span>|<span data-ttu-id="879be-215">string</span><span class="sxs-lookup"><span data-stu-id="879be-215">string</span></span>|<span data-ttu-id="879be-216">客户端的聊天消息的区域设置。</span><span class="sxs-lookup"><span data-stu-id="879be-216">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="879be-217">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="879be-217">JSON representation</span></span>

<span data-ttu-id="879be-218">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="879be-218">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "deleted",
    "deletedDateTime",
    "attachments",
    "importance",
    "mentions",
    "subject",
    "summary",
    "policyViolation",
    "locale"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessage"
}-->

```json
{
  "id": "string (identifier)",
  "replyToId": "string (identifier)",
  "from": {"@odata.type": "microsoft.graph.identitySet"},
  "etag": "string",
  "messageType": "string",
  "createdDateTime": "string (timestamp)",
  "lastModifiedDateTime": "string (timestamp)",
  "deletedDateTime": "string (timestamp)",
  "subject": "string",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "summary": "string",
  "attachments": [{"@odata.type": "microsoft.graph.chatMessageAttachment"}],
  "mentions": [{"@odata.type": "microsoft.graph.chatMessageMention"}],
  "importance": "string",
  "policyViolation": {"@odata.type": "microsoft.graph.chatMessagePolicyViolation"},
  "locale": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
