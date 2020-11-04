---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 聊天消息可以是一个根聊天消息，也可以是由聊天消息中的 **replyToId** 属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: a3d994379b3b15170ff490433827eda79c18d4f7
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849191"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="a91c3-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="a91c3-104">chatMessage resource type</span></span>

<span data-ttu-id="a91c3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a91c3-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a91c3-106">代表 beta) [研讨](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)中的[频道](./channel.md)或 (内的单个聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="a91c3-106">Represents an individual chat message within a [channel](./channel.md) or (in beta) [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="a91c3-107">聊天消息可以是一个根聊天消息，也可以是由聊天消息中的 **replyToId** 属性定义的答复线程的一部分。</span><span class="sxs-lookup"><span data-stu-id="a91c3-107">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="a91c3-108">方法</span><span class="sxs-lookup"><span data-stu-id="a91c3-108">Methods</span></span>

| <span data-ttu-id="a91c3-109">方法</span><span class="sxs-lookup"><span data-stu-id="a91c3-109">Method</span></span>       | <span data-ttu-id="a91c3-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a91c3-110">Return Type</span></span>  |<span data-ttu-id="a91c3-111">说明</span><span class="sxs-lookup"><span data-stu-id="a91c3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a91c3-112">**通道邮件**</span><span class="sxs-lookup"><span data-stu-id="a91c3-112">**Channel messages**</span></span>| | |
|[<span data-ttu-id="a91c3-113">列出频道了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="a91c3-113">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="a91c3-114">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a91c3-114">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="a91c3-115">频道中所有根聊天邮件的列表。</span><span class="sxs-lookup"><span data-stu-id="a91c3-115">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="a91c3-116">在频道 delta 中获取 Chatmessages 集合</span><span class="sxs-lookup"><span data-stu-id="a91c3-116">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="a91c3-117">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a91c3-117">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="a91c3-118">获取通道中的增量聊天消息。</span><span class="sxs-lookup"><span data-stu-id="a91c3-118">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="a91c3-119">为新的频道消息创建订阅</span><span class="sxs-lookup"><span data-stu-id="a91c3-119">Create subscription for new channel messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="a91c3-120">订阅</span><span class="sxs-lookup"><span data-stu-id="a91c3-120">subscription</span></span>](subscription.md) | <span data-ttu-id="a91c3-121">收听新的和编辑的频道消息以及对它们的反应。</span><span class="sxs-lookup"><span data-stu-id="a91c3-121">Listen for new and edited channel messages, and reactions to them.</span></span> |
|[<span data-ttu-id="a91c3-122">获取频道了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="a91c3-122">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="a91c3-123">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a91c3-123">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="a91c3-124">从频道中获取单个根聊天消息。</span><span class="sxs-lookup"><span data-stu-id="a91c3-124">Get a single root chat message from a channel.</span></span>|
|[<span data-ttu-id="a91c3-125">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="a91c3-125">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="a91c3-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a91c3-126">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="a91c3-127">向频道发送消息。</span><span class="sxs-lookup"><span data-stu-id="a91c3-127">Send a message to a channel.</span></span> |
|[<span data-ttu-id="a91c3-128">更新了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="a91c3-128">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="a91c3-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a91c3-129">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="a91c3-130">更新聊天邮件的 **policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="a91c3-130">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="a91c3-131">**频道邮件答复**</span><span class="sxs-lookup"><span data-stu-id="a91c3-131">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="a91c3-132">列出对了 chatmessage 的答复</span><span class="sxs-lookup"><span data-stu-id="a91c3-132">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="a91c3-133">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a91c3-133">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="a91c3-134">频道中对聊天消息的所有回复的列表。</span><span class="sxs-lookup"><span data-stu-id="a91c3-134">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="a91c3-135">获取对了 chatmessage 的答复</span><span class="sxs-lookup"><span data-stu-id="a91c3-135">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="a91c3-136">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a91c3-136">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="a91c3-137">获取频道中的聊天消息的单个答复。</span><span class="sxs-lookup"><span data-stu-id="a91c3-137">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="a91c3-138">答复频道中的了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="a91c3-138">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="a91c3-139">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a91c3-139">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="a91c3-140">在频道中答复现有聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="a91c3-140">Reply to an existing chat message in a channel.</span></span>|
|[<span data-ttu-id="a91c3-141">更新了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="a91c3-141">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="a91c3-142">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a91c3-142">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="a91c3-143">更新聊天邮件的 **policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="a91c3-143">Update the **policyViolation** property of a chat message.</span></span>|

## <a name="properties"></a><span data-ttu-id="a91c3-144">属性</span><span class="sxs-lookup"><span data-stu-id="a91c3-144">Properties</span></span>

| <span data-ttu-id="a91c3-145">属性</span><span class="sxs-lookup"><span data-stu-id="a91c3-145">Property</span></span>   | <span data-ttu-id="a91c3-146">类型</span><span class="sxs-lookup"><span data-stu-id="a91c3-146">Type</span></span> |<span data-ttu-id="a91c3-147">说明</span><span class="sxs-lookup"><span data-stu-id="a91c3-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a91c3-148">id</span><span class="sxs-lookup"><span data-stu-id="a91c3-148">id</span></span>|<span data-ttu-id="a91c3-149">String</span><span class="sxs-lookup"><span data-stu-id="a91c3-149">String</span></span>| <span data-ttu-id="a91c3-150">只读。</span><span class="sxs-lookup"><span data-stu-id="a91c3-150">Read-only.</span></span> <span data-ttu-id="a91c3-151">邮件的唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="a91c3-151">Unique Id of the message.</span></span>|
|<span data-ttu-id="a91c3-152">replyToId</span><span class="sxs-lookup"><span data-stu-id="a91c3-152">replyToId</span></span>| <span data-ttu-id="a91c3-153">string</span><span class="sxs-lookup"><span data-stu-id="a91c3-153">string</span></span> | <span data-ttu-id="a91c3-154">只读。</span><span class="sxs-lookup"><span data-stu-id="a91c3-154">Read-only.</span></span> <span data-ttu-id="a91c3-155">线程的父聊天消息或根聊天消息的 Id。</span><span class="sxs-lookup"><span data-stu-id="a91c3-155">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="a91c3-156"> (仅适用于频道中不聊天的聊天消息) </span><span class="sxs-lookup"><span data-stu-id="a91c3-156">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="a91c3-157">from</span><span class="sxs-lookup"><span data-stu-id="a91c3-157">from</span></span>|[<span data-ttu-id="a91c3-158">identitySet</span><span class="sxs-lookup"><span data-stu-id="a91c3-158">identitySet</span></span>](identityset.md)| <span data-ttu-id="a91c3-159">只读。</span><span class="sxs-lookup"><span data-stu-id="a91c3-159">Read only.</span></span> <span data-ttu-id="a91c3-160">聊天消息发件人的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a91c3-160">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="a91c3-161">etag</span><span class="sxs-lookup"><span data-stu-id="a91c3-161">etag</span></span>| <span data-ttu-id="a91c3-162">string</span><span class="sxs-lookup"><span data-stu-id="a91c3-162">string</span></span> | <span data-ttu-id="a91c3-163">只读。</span><span class="sxs-lookup"><span data-stu-id="a91c3-163">Read-only.</span></span> <span data-ttu-id="a91c3-164">聊天消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="a91c3-164">Version number of the chat message.</span></span> |
|<span data-ttu-id="a91c3-165">messageType</span><span class="sxs-lookup"><span data-stu-id="a91c3-165">messageType</span></span>|<span data-ttu-id="a91c3-166">string</span><span class="sxs-lookup"><span data-stu-id="a91c3-166">string</span></span>|<span data-ttu-id="a91c3-167">聊天消息的类型。</span><span class="sxs-lookup"><span data-stu-id="a91c3-167">The type of chat message.</span></span> <span data-ttu-id="a91c3-168">可能的值是： `message` 。</span><span class="sxs-lookup"><span data-stu-id="a91c3-168">The possible values are: `message`.</span></span>|
|<span data-ttu-id="a91c3-169">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a91c3-169">createdDateTime</span></span>|<span data-ttu-id="a91c3-170">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a91c3-170">dateTimeOffset</span></span>|<span data-ttu-id="a91c3-171">只读。</span><span class="sxs-lookup"><span data-stu-id="a91c3-171">Read only.</span></span> <span data-ttu-id="a91c3-172">在聊天消息创建时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="a91c3-172">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="a91c3-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a91c3-173">lastModifiedDateTime</span></span>|<span data-ttu-id="a91c3-174">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a91c3-174">dateTimeOffset</span></span>|<span data-ttu-id="a91c3-175">只读。</span><span class="sxs-lookup"><span data-stu-id="a91c3-175">Read only.</span></span> <span data-ttu-id="a91c3-176">在 (初始设置) 或编辑时（包括添加或删除反应时）创建聊天邮件时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="a91c3-176">Timestamp when the chat message is created (initial setting) or edited, including when a reaction is added or removed.</span></span> |
|<span data-ttu-id="a91c3-177">lastEditedDateTime</span><span class="sxs-lookup"><span data-stu-id="a91c3-177">lastEditedDateTime</span></span>|<span data-ttu-id="a91c3-178">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a91c3-178">dateTimeOffset</span></span>|<span data-ttu-id="a91c3-179">只读。</span><span class="sxs-lookup"><span data-stu-id="a91c3-179">Read only.</span></span> <span data-ttu-id="a91c3-180">在对聊天消息进行编辑时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="a91c3-180">Timestamp when edits to the chat message were made.</span></span> <span data-ttu-id="a91c3-181">触发 Microsoft 团队 UI 中的 "编辑" 标志。</span><span class="sxs-lookup"><span data-stu-id="a91c3-181">Triggers an "Edited" flag in the Microsoft Teams UI.</span></span> <span data-ttu-id="a91c3-182">如果未进行任何编辑，则该值为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="a91c3-182">If no edits are made the value is `null`.</span></span>|
|<span data-ttu-id="a91c3-183">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="a91c3-183">deletedDateTime</span></span>|<span data-ttu-id="a91c3-184">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a91c3-184">dateTimeOffset</span></span>|<span data-ttu-id="a91c3-185">只读。</span><span class="sxs-lookup"><span data-stu-id="a91c3-185">Read only.</span></span> <span data-ttu-id="a91c3-186">删除聊天邮件的时间戳，如果未删除，则为 null。</span><span class="sxs-lookup"><span data-stu-id="a91c3-186">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="a91c3-187">subject</span><span class="sxs-lookup"><span data-stu-id="a91c3-187">subject</span></span>|<span data-ttu-id="a91c3-188">string</span><span class="sxs-lookup"><span data-stu-id="a91c3-188">string</span></span>| <span data-ttu-id="a91c3-189">聊天消息的主题，以纯文本形式。</span><span class="sxs-lookup"><span data-stu-id="a91c3-189">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="a91c3-190">body</span><span class="sxs-lookup"><span data-stu-id="a91c3-190">body</span></span>|[<span data-ttu-id="a91c3-191">itemBody</span><span class="sxs-lookup"><span data-stu-id="a91c3-191">itemBody</span></span>](itembody.md)|<span data-ttu-id="a91c3-192">聊天消息内容的纯文本/HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a91c3-192">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="a91c3-193">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="a91c3-193">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="a91c3-194">如果聊天消息包含 [chatMessageMention](chatmessagemention.md)，则该内容始终为 HTML。</span><span class="sxs-lookup"><span data-stu-id="a91c3-194">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="a91c3-195">摘要</span><span class="sxs-lookup"><span data-stu-id="a91c3-195">summary</span></span>|<span data-ttu-id="a91c3-196">string</span><span class="sxs-lookup"><span data-stu-id="a91c3-196">string</span></span>| <span data-ttu-id="a91c3-197">可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。</span><span class="sxs-lookup"><span data-stu-id="a91c3-197">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="a91c3-198">仅适用于频道聊天消息，而不是聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="a91c3-198">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="a91c3-199">附件</span><span class="sxs-lookup"><span data-stu-id="a91c3-199">attachments</span></span>|<span data-ttu-id="a91c3-200">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a91c3-200">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="a91c3-201">附加文件。</span><span class="sxs-lookup"><span data-stu-id="a91c3-201">Attached files.</span></span> <span data-ttu-id="a91c3-202">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="a91c3-202">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="a91c3-203">提及</span><span class="sxs-lookup"><span data-stu-id="a91c3-203">mentions</span></span>|<span data-ttu-id="a91c3-204">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a91c3-204">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="a91c3-205">聊天消息中提及的实体列表。</span><span class="sxs-lookup"><span data-stu-id="a91c3-205">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="a91c3-206">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="a91c3-206">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="a91c3-207">重要性</span><span class="sxs-lookup"><span data-stu-id="a91c3-207">importance</span></span>| <span data-ttu-id="a91c3-208">string</span><span class="sxs-lookup"><span data-stu-id="a91c3-208">string</span></span> | <span data-ttu-id="a91c3-209">聊天消息的重要性。</span><span class="sxs-lookup"><span data-stu-id="a91c3-209">The importance of the chat message.</span></span> <span data-ttu-id="a91c3-210">可能的值包括 `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="a91c3-210">The possible values are: `normal`, `high`, `urgent`.</span></span>|
| <span data-ttu-id="a91c3-211">policyViolation</span><span class="sxs-lookup"><span data-stu-id="a91c3-211">policyViolation</span></span> | [<span data-ttu-id="a91c3-212">chatMessagePolicyViolation</span><span class="sxs-lookup"><span data-stu-id="a91c3-212">chatMessagePolicyViolation</span></span>](../resources/chatmessagepolicyviolation.md) |<span data-ttu-id="a91c3-213">定义由数据丢失防护 (DLP) 应用程序设置的策略违规属性。</span><span class="sxs-lookup"><span data-stu-id="a91c3-213">Defines the properties of a policy violation set by a data loss prevention (DLP) application.</span></span>|
|<span data-ttu-id="a91c3-214">区域设置</span><span class="sxs-lookup"><span data-stu-id="a91c3-214">locale</span></span>|<span data-ttu-id="a91c3-215">string</span><span class="sxs-lookup"><span data-stu-id="a91c3-215">string</span></span>|<span data-ttu-id="a91c3-216">客户端的聊天消息的区域设置。</span><span class="sxs-lookup"><span data-stu-id="a91c3-216">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a91c3-217">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a91c3-217">JSON representation</span></span>

<span data-ttu-id="a91c3-218">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a91c3-218">The following is a JSON representation of the resource.</span></span>

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
