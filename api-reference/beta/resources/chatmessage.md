---
title: chatMessage 资源类型
description: 代表 "频道" 或 "聊天" 实体中的单个聊天消息。 聊天消息可以是一个根聊天消息，也可以是由聊天消息中的 **replyToId** 属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: f1af347d0c043ec2b0ca2da05ba44331aab925d2
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193461"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="6c97c-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c97c-104">chatMessage resource type</span></span>

<span data-ttu-id="6c97c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c97c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="6c97c-106">表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="6c97c-106">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="6c97c-107">该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。</span><span class="sxs-lookup"><span data-stu-id="6c97c-107">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>


## <a name="methods"></a><span data-ttu-id="6c97c-108">方法</span><span class="sxs-lookup"><span data-stu-id="6c97c-108">Methods</span></span>

| <span data-ttu-id="6c97c-109">方法</span><span class="sxs-lookup"><span data-stu-id="6c97c-109">Method</span></span>       | <span data-ttu-id="6c97c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6c97c-110">Return Type</span></span>  |<span data-ttu-id="6c97c-111">说明</span><span class="sxs-lookup"><span data-stu-id="6c97c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c97c-112">**通道邮件**</span><span class="sxs-lookup"><span data-stu-id="6c97c-112">**Channel messages**</span></span>| | |
|[<span data-ttu-id="6c97c-113">列出频道了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-113">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="6c97c-114">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c97c-114">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="6c97c-115">频道中所有根聊天邮件的列表。</span><span class="sxs-lookup"><span data-stu-id="6c97c-115">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="6c97c-116">在频道 delta 中获取 Chatmessages 集合</span><span class="sxs-lookup"><span data-stu-id="6c97c-116">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="6c97c-117">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-117">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="6c97c-118">获取通道中的增量聊天消息。</span><span class="sxs-lookup"><span data-stu-id="6c97c-118">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="6c97c-119">为新的频道消息创建订阅</span><span class="sxs-lookup"><span data-stu-id="6c97c-119">Create subscription for new channel messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="6c97c-120">订阅</span><span class="sxs-lookup"><span data-stu-id="6c97c-120">subscription</span></span>](subscription.md) | <span data-ttu-id="6c97c-121">收听新的和编辑的频道消息以及对它们的反应。</span><span class="sxs-lookup"><span data-stu-id="6c97c-121">Listen for new and edited channel messages, and reactions to them.</span></span> |
|[<span data-ttu-id="6c97c-122">获取频道了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-122">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="6c97c-123">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-123">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="6c97c-124">从频道中获取单个根聊天消息。</span><span class="sxs-lookup"><span data-stu-id="6c97c-124">Get a single root chat message from a channel.</span></span>|
|[<span data-ttu-id="6c97c-125">在频道或聊天中创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-125">Create chatMessage in a channel or chat</span></span>](../api/chatmessage-post.md) | [<span data-ttu-id="6c97c-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-126">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="6c97c-127">在频道中创建新的顶级聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="6c97c-127">Create a new top-level chat message in a channel.</span></span>|
|[<span data-ttu-id="6c97c-128">更新了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-128">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="6c97c-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-129">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="6c97c-130">更新聊天邮件的 **policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="6c97c-130">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="6c97c-131">**频道邮件答复**</span><span class="sxs-lookup"><span data-stu-id="6c97c-131">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="6c97c-132">列出对了 chatmessage 的答复</span><span class="sxs-lookup"><span data-stu-id="6c97c-132">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="6c97c-133">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c97c-133">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="6c97c-134">频道中对聊天消息的所有回复的列表。</span><span class="sxs-lookup"><span data-stu-id="6c97c-134">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="6c97c-135">获取对了 chatmessage 的答复</span><span class="sxs-lookup"><span data-stu-id="6c97c-135">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="6c97c-136">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-136">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="6c97c-137">获取频道中的聊天消息的单个答复。</span><span class="sxs-lookup"><span data-stu-id="6c97c-137">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="6c97c-138">答复频道中的了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-138">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="6c97c-139">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-139">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="6c97c-140">在频道中答复现有聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="6c97c-140">Reply to an existing chat message in a channel.</span></span>|
|[<span data-ttu-id="6c97c-141">更新了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-141">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="6c97c-142">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-142">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="6c97c-143">更新聊天邮件的 **policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="6c97c-143">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="6c97c-144">**1:1 和分组聊天消息**</span><span class="sxs-lookup"><span data-stu-id="6c97c-144">**1:1 and group chat messages**</span></span>| | |
|[<span data-ttu-id="6c97c-145">在聊天中获取了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-145">Get chatMessage in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="6c97c-146">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-146">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="6c97c-147">在聊天中获取单个聊天消息。</span><span class="sxs-lookup"><span data-stu-id="6c97c-147">Get a single chat message in a chat.</span></span> |
|[<span data-ttu-id="6c97c-148">在聊天中列出 Chatmessages 集合</span><span class="sxs-lookup"><span data-stu-id="6c97c-148">List chatMessages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="6c97c-149">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-149">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="6c97c-150">列出1:1 或组聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="6c97c-150">List chat messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="6c97c-151">创建新聊天邮件的订阅</span><span class="sxs-lookup"><span data-stu-id="6c97c-151">Create subscription for new chat messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="6c97c-152">订阅</span><span class="sxs-lookup"><span data-stu-id="6c97c-152">subscription</span></span>](subscription.md) | <span data-ttu-id="6c97c-153">收听新的和已编辑的聊天消息以及对它们的反应。</span><span class="sxs-lookup"><span data-stu-id="6c97c-153">Listen for new and edited chat messages, and reactions to them.</span></span> |
|[<span data-ttu-id="6c97c-154">在聊天中创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-154">Create chatMessage in a chat</span></span>](../api/chat-post-message.md) | [<span data-ttu-id="6c97c-155">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-155">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="6c97c-156">在现有的1:1 或组聊天对话中发送聊天消息。</span><span class="sxs-lookup"><span data-stu-id="6c97c-156">Send a chat message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="6c97c-157">更新了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-157">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="6c97c-158">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6c97c-158">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="6c97c-159">更新聊天邮件的 **policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="6c97c-159">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="6c97c-160">**托管内容**</span><span class="sxs-lookup"><span data-stu-id="6c97c-160">**Hosted content**</span></span>| | |
|[<span data-ttu-id="6c97c-161">列出所有已承载的内容</span><span class="sxs-lookup"><span data-stu-id="6c97c-161">List all hosted content</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | <span data-ttu-id="6c97c-162">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c97c-162">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection</span></span>| <span data-ttu-id="6c97c-163">获取聊天消息中的所有托管内容。</span><span class="sxs-lookup"><span data-stu-id="6c97c-163">Get all hosted content in a chat message.</span></span>|
|[<span data-ttu-id="6c97c-164">获取托管内容</span><span class="sxs-lookup"><span data-stu-id="6c97c-164">Get hosted content</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="6c97c-165">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="6c97c-165">chatMessageHostedContent</span></span>](../resources/chatmessagehostedcontent.md) | <span data-ttu-id="6c97c-166">从聊天消息中获取托管的内容。</span><span class="sxs-lookup"><span data-stu-id="6c97c-166">Get hosted content from a chat message.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c97c-167">属性</span><span class="sxs-lookup"><span data-stu-id="6c97c-167">Properties</span></span>

| <span data-ttu-id="6c97c-168">属性</span><span class="sxs-lookup"><span data-stu-id="6c97c-168">Property</span></span>   | <span data-ttu-id="6c97c-169">类型</span><span class="sxs-lookup"><span data-stu-id="6c97c-169">Type</span></span> |<span data-ttu-id="6c97c-170">说明</span><span class="sxs-lookup"><span data-stu-id="6c97c-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c97c-171">id</span><span class="sxs-lookup"><span data-stu-id="6c97c-171">id</span></span>|<span data-ttu-id="6c97c-172">字符串</span><span class="sxs-lookup"><span data-stu-id="6c97c-172">String</span></span>| <span data-ttu-id="6c97c-173">只读。</span><span class="sxs-lookup"><span data-stu-id="6c97c-173">Read-only.</span></span> <span data-ttu-id="6c97c-174">消息的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="6c97c-174">Unique ID of the message.</span></span>|
|<span data-ttu-id="6c97c-175">replyToId</span><span class="sxs-lookup"><span data-stu-id="6c97c-175">replyToId</span></span>| <span data-ttu-id="6c97c-176">string</span><span class="sxs-lookup"><span data-stu-id="6c97c-176">string</span></span> | <span data-ttu-id="6c97c-177">只读。</span><span class="sxs-lookup"><span data-stu-id="6c97c-177">Read-only.</span></span> <span data-ttu-id="6c97c-178">线程的父聊天消息或根聊天消息的 ID。</span><span class="sxs-lookup"><span data-stu-id="6c97c-178">ID of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="6c97c-179"> (仅适用于频道中的聊天消息，而不是聊天。 ) </span><span class="sxs-lookup"><span data-stu-id="6c97c-179">(Only applies to chat messages in channels, not chats.)</span></span> |
|<span data-ttu-id="6c97c-180">from</span><span class="sxs-lookup"><span data-stu-id="6c97c-180">from</span></span>|[<span data-ttu-id="6c97c-181">identitySet</span><span class="sxs-lookup"><span data-stu-id="6c97c-181">identitySet</span></span>](identityset.md)| <span data-ttu-id="6c97c-182">只读。</span><span class="sxs-lookup"><span data-stu-id="6c97c-182">Read only.</span></span> <span data-ttu-id="6c97c-183">聊天消息发件人的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6c97c-183">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="6c97c-184">etag</span><span class="sxs-lookup"><span data-stu-id="6c97c-184">etag</span></span>| <span data-ttu-id="6c97c-185">string</span><span class="sxs-lookup"><span data-stu-id="6c97c-185">string</span></span> | <span data-ttu-id="6c97c-186">只读。</span><span class="sxs-lookup"><span data-stu-id="6c97c-186">Read-only.</span></span> <span data-ttu-id="6c97c-187">聊天消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="6c97c-187">Version number of the chat message.</span></span> |
|<span data-ttu-id="6c97c-188">messageType</span><span class="sxs-lookup"><span data-stu-id="6c97c-188">messageType</span></span>|<span data-ttu-id="6c97c-189">string</span><span class="sxs-lookup"><span data-stu-id="6c97c-189">string</span></span>|<span data-ttu-id="6c97c-190">聊天消息的类型。</span><span class="sxs-lookup"><span data-stu-id="6c97c-190">The type of chat message.</span></span> <span data-ttu-id="6c97c-191">可能的值是： `message` 。</span><span class="sxs-lookup"><span data-stu-id="6c97c-191">The possible values are: `message`.</span></span>|
|<span data-ttu-id="6c97c-192">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c97c-192">createdDateTime</span></span>|<span data-ttu-id="6c97c-193">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c97c-193">dateTimeOffset</span></span>|<span data-ttu-id="6c97c-194">只读。</span><span class="sxs-lookup"><span data-stu-id="6c97c-194">Read only.</span></span> <span data-ttu-id="6c97c-195">在聊天消息创建时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="6c97c-195">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="6c97c-196">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c97c-196">lastModifiedDateTime</span></span>|<span data-ttu-id="6c97c-197">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c97c-197">dateTimeOffset</span></span>|<span data-ttu-id="6c97c-198">只读。</span><span class="sxs-lookup"><span data-stu-id="6c97c-198">Read only.</span></span> <span data-ttu-id="6c97c-199"> (初始设置) 或修改，包括添加或删除反应时）中创建聊天邮件时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="6c97c-199">Timestamp when the chat message is created (initial setting) or modified, including when a reaction is added or removed.</span></span> |
|<span data-ttu-id="6c97c-200">lastEditedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c97c-200">lastEditedDateTime</span></span>|<span data-ttu-id="6c97c-201">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c97c-201">dateTimeOffset</span></span>|<span data-ttu-id="6c97c-202">只读。</span><span class="sxs-lookup"><span data-stu-id="6c97c-202">Read only.</span></span> <span data-ttu-id="6c97c-203">在对聊天消息进行编辑时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="6c97c-203">Timestamp when edits to the chat message were made.</span></span> <span data-ttu-id="6c97c-204">触发团队 UI 中的 "编辑" 标志。</span><span class="sxs-lookup"><span data-stu-id="6c97c-204">Triggers an "Edited" flag in the Teams UI.</span></span> <span data-ttu-id="6c97c-205">如果未进行任何编辑，则该值为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="6c97c-205">If no edits are made the value is `null`.</span></span>|
|<span data-ttu-id="6c97c-206">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c97c-206">deletedDateTime</span></span>|<span data-ttu-id="6c97c-207">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c97c-207">dateTimeOffset</span></span>|<span data-ttu-id="6c97c-208">只读。</span><span class="sxs-lookup"><span data-stu-id="6c97c-208">Read only.</span></span> <span data-ttu-id="6c97c-209">删除聊天邮件的时间戳，如果未删除，则为 null。</span><span class="sxs-lookup"><span data-stu-id="6c97c-209">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="6c97c-210">subject</span><span class="sxs-lookup"><span data-stu-id="6c97c-210">subject</span></span>|<span data-ttu-id="6c97c-211">string</span><span class="sxs-lookup"><span data-stu-id="6c97c-211">string</span></span>| <span data-ttu-id="6c97c-212">聊天消息的主题，以纯文本形式。</span><span class="sxs-lookup"><span data-stu-id="6c97c-212">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="6c97c-213">body</span><span class="sxs-lookup"><span data-stu-id="6c97c-213">body</span></span>|[<span data-ttu-id="6c97c-214">itemBody</span><span class="sxs-lookup"><span data-stu-id="6c97c-214">itemBody</span></span>](itembody.md)|<span data-ttu-id="6c97c-215">聊天消息内容的纯文本/HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c97c-215">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="6c97c-216">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="6c97c-216">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="6c97c-217">如果聊天消息包含 [chatMessageMention](chatmessagemention.md)，则该内容始终为 HTML。</span><span class="sxs-lookup"><span data-stu-id="6c97c-217">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="6c97c-218">摘要</span><span class="sxs-lookup"><span data-stu-id="6c97c-218">summary</span></span>|<span data-ttu-id="6c97c-219">string</span><span class="sxs-lookup"><span data-stu-id="6c97c-219">string</span></span>| <span data-ttu-id="6c97c-220">可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。</span><span class="sxs-lookup"><span data-stu-id="6c97c-220">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="6c97c-221">仅适用于频道聊天消息，而不是聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="6c97c-221">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="6c97c-222">附件</span><span class="sxs-lookup"><span data-stu-id="6c97c-222">attachments</span></span>|<span data-ttu-id="6c97c-223">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c97c-223">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="6c97c-224">附加文件。</span><span class="sxs-lookup"><span data-stu-id="6c97c-224">Attached files.</span></span> <span data-ttu-id="6c97c-225">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="6c97c-225">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="6c97c-226">提及</span><span class="sxs-lookup"><span data-stu-id="6c97c-226">mentions</span></span>|<span data-ttu-id="6c97c-227">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c97c-227">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="6c97c-228">聊天消息中提及的实体列表。</span><span class="sxs-lookup"><span data-stu-id="6c97c-228">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="6c97c-229">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="6c97c-229">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="6c97c-230">重要性</span><span class="sxs-lookup"><span data-stu-id="6c97c-230">importance</span></span>|<span data-ttu-id="6c97c-231">string</span><span class="sxs-lookup"><span data-stu-id="6c97c-231">string</span></span> | <span data-ttu-id="6c97c-232">聊天消息的重要性。</span><span class="sxs-lookup"><span data-stu-id="6c97c-232">The importance of the chat message.</span></span> <span data-ttu-id="6c97c-233">可能的值包括 `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="6c97c-233">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="6c97c-234">反应</span><span class="sxs-lookup"><span data-stu-id="6c97c-234">reactions</span></span>| <span data-ttu-id="6c97c-235">[chatMessageReaction](./chatmessagereaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c97c-235">[chatMessageReaction](./chatmessagereaction.md) collection</span></span> | <span data-ttu-id="6c97c-236">此聊天消息的反应 (例如，如) 。</span><span class="sxs-lookup"><span data-stu-id="6c97c-236">Reactions for this chat message (for example, Like).</span></span>|
|<span data-ttu-id="6c97c-237">区域设置</span><span class="sxs-lookup"><span data-stu-id="6c97c-237">locale</span></span>|<span data-ttu-id="6c97c-238">string</span><span class="sxs-lookup"><span data-stu-id="6c97c-238">string</span></span>|<span data-ttu-id="6c97c-239">客户端的聊天消息的区域设置。</span><span class="sxs-lookup"><span data-stu-id="6c97c-239">Locale of the chat message set by the client.</span></span>|
| <span data-ttu-id="6c97c-240">policyViolation</span><span class="sxs-lookup"><span data-stu-id="6c97c-240">policyViolation</span></span> | [<span data-ttu-id="6c97c-241">chatMessagePolicyViolation</span><span class="sxs-lookup"><span data-stu-id="6c97c-241">chatMessagePolicyViolation</span></span>](../resources/chatmessagepolicyviolation.md) |<span data-ttu-id="6c97c-242">定义由数据丢失防护 (DLP) 应用程序设置的策略违规属性。</span><span class="sxs-lookup"><span data-stu-id="6c97c-242">Defines the properties of a policy violation set by a data loss prevention (DLP) application.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c97c-243">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c97c-243">JSON representation</span></span>

<span data-ttu-id="6c97c-244">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c97c-244">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "deleted",
    "deletedDateTime",
    "attachments",
    "importance",
    "reactions",
    "mentions",
    "subject",
    "summary"
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
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string",
  "policyViolation": {"@odata.type": "microsoft.graph.chatMessagePolicyViolation"},
  "deleted": true
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

