---
title: chatMessage 资源类型
description: 表示频道或聊天实体中的单个聊天消息。 聊天消息可以是根聊天消息或聊天消息中的 **replyToId** 属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 53c4a22d66ced56a038e89a504f918a184c33a02
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874045"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="030cd-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="030cd-104">chatMessage resource type</span></span>

<span data-ttu-id="030cd-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="030cd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="030cd-106">表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="030cd-106">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="030cd-107">该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。</span><span class="sxs-lookup"><span data-stu-id="030cd-107">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

> <span data-ttu-id="030cd-108">**注意**：此资源支持使用更改通知 (、更新和删除) [更改](../resources/webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="030cd-108">**Note**: This resource supports subscribing to changes (create, update, and delete) using [change notifications](../resources/webhooks.md).</span></span> <span data-ttu-id="030cd-109">这使呼叫方可以实时订阅和获取更改。</span><span class="sxs-lookup"><span data-stu-id="030cd-109">This allows callers to subscribe and get changes in real time.</span></span> <span data-ttu-id="030cd-110">有关详细信息，请参阅[获取消息通知](/graph/teams-changenotifications-chatMessage)。</span><span class="sxs-lookup"><span data-stu-id="030cd-110">For details, see [Get notifications for messages](/graph/teams-changenotifications-chatMessage).</span></span>

## <a name="methods"></a><span data-ttu-id="030cd-111">方法</span><span class="sxs-lookup"><span data-stu-id="030cd-111">Methods</span></span>

| <span data-ttu-id="030cd-112">方法</span><span class="sxs-lookup"><span data-stu-id="030cd-112">Method</span></span>       | <span data-ttu-id="030cd-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="030cd-113">Return Type</span></span>  |<span data-ttu-id="030cd-114">Description</span><span class="sxs-lookup"><span data-stu-id="030cd-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="030cd-115">**频道消息**</span><span class="sxs-lookup"><span data-stu-id="030cd-115">**Channel messages**</span></span>| | |
|[<span data-ttu-id="030cd-116">列出频道 chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-116">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="030cd-117">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="030cd-117">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="030cd-118">频道中所有根聊天消息的列表。</span><span class="sxs-lookup"><span data-stu-id="030cd-118">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="030cd-119">获取通道增量中的 chatMessages</span><span class="sxs-lookup"><span data-stu-id="030cd-119">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="030cd-120">chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-120">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="030cd-121">获取频道中的增量聊天消息。</span><span class="sxs-lookup"><span data-stu-id="030cd-121">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="030cd-122">创建新频道消息的订阅</span><span class="sxs-lookup"><span data-stu-id="030cd-122">Create subscription for new channel messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="030cd-123">订阅</span><span class="sxs-lookup"><span data-stu-id="030cd-123">subscription</span></span>](subscription.md) | <span data-ttu-id="030cd-124">收听新的和编辑的频道消息，并响应这些消息。</span><span class="sxs-lookup"><span data-stu-id="030cd-124">Listen for new and edited channel messages, and reactions to them.</span></span> |
|[<span data-ttu-id="030cd-125">获取频道 chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-125">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="030cd-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-126">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="030cd-127">从频道获取单个根聊天消息。</span><span class="sxs-lookup"><span data-stu-id="030cd-127">Get a single root chat message from a channel.</span></span>|
|[<span data-ttu-id="030cd-128">在频道或聊天中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-128">Create chatMessage in a channel or chat</span></span>](../api/chatmessage-post.md) | [<span data-ttu-id="030cd-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-129">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="030cd-130">在频道中创建新的顶级聊天消息。</span><span class="sxs-lookup"><span data-stu-id="030cd-130">Create a new top-level chat message in a channel.</span></span>|
|[<span data-ttu-id="030cd-131">更新 chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-131">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="030cd-132">chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-132">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="030cd-133">更新 **聊天消息的 policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="030cd-133">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="030cd-134">**频道消息回复**</span><span class="sxs-lookup"><span data-stu-id="030cd-134">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="030cd-135">列出对 chatMessage 的回复</span><span class="sxs-lookup"><span data-stu-id="030cd-135">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="030cd-136">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="030cd-136">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="030cd-137">频道中聊天消息的所有回复列表。</span><span class="sxs-lookup"><span data-stu-id="030cd-137">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="030cd-138">获取 chatMessage 的回复</span><span class="sxs-lookup"><span data-stu-id="030cd-138">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="030cd-139">chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-139">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="030cd-140">获取频道中聊天消息的单个回复。</span><span class="sxs-lookup"><span data-stu-id="030cd-140">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="030cd-141">在频道中回复 chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-141">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="030cd-142">chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-142">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="030cd-143">回复频道中的现有聊天消息。</span><span class="sxs-lookup"><span data-stu-id="030cd-143">Reply to an existing chat message in a channel.</span></span>|
|[<span data-ttu-id="030cd-144">更新 chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-144">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="030cd-145">chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-145">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="030cd-146">更新 **聊天消息的 policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="030cd-146">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="030cd-147">**1：1 和群聊消息**</span><span class="sxs-lookup"><span data-stu-id="030cd-147">**1:1 and group chat messages**</span></span>| | |
|[<span data-ttu-id="030cd-148">获取聊天中的 chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-148">Get chatMessage in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="030cd-149">chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-149">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="030cd-150">获取聊天中的单个聊天消息。</span><span class="sxs-lookup"><span data-stu-id="030cd-150">Get a single chat message in a chat.</span></span> |
|[<span data-ttu-id="030cd-151">列出聊天中的 chatMessages</span><span class="sxs-lookup"><span data-stu-id="030cd-151">List chatMessages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="030cd-152">chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-152">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="030cd-153">列出一对一或群聊中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="030cd-153">List chat messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="030cd-154">获取用户的所有聊天消息</span><span class="sxs-lookup"><span data-stu-id="030cd-154">Get all chat messages for user</span></span>](../api/chats-getallmessages.md)| <span data-ttu-id="030cd-155">[chat](chat.md) 集合</span><span class="sxs-lookup"><span data-stu-id="030cd-155">[chat](chat.md) collection</span></span>| <span data-ttu-id="030cd-156">从用户参与的所有聊天获取消息，包括一对一聊天、群聊和会议聊天。</span><span class="sxs-lookup"><span data-stu-id="030cd-156">Get messages from all chats that a user is a participant in, including 1:1 chats, group chats, and meeting chats.</span></span> |
|[<span data-ttu-id="030cd-157">创建新聊天消息的订阅</span><span class="sxs-lookup"><span data-stu-id="030cd-157">Create subscription for new chat messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="030cd-158">订阅</span><span class="sxs-lookup"><span data-stu-id="030cd-158">subscription</span></span>](subscription.md) | <span data-ttu-id="030cd-159">收听新的和编辑的聊天消息，并响应它们。</span><span class="sxs-lookup"><span data-stu-id="030cd-159">Listen for new and edited chat messages, and reactions to them.</span></span> |
|[<span data-ttu-id="030cd-160">在聊天中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-160">Create chatMessage in a chat</span></span>](../api/chat-post-message.md) | [<span data-ttu-id="030cd-161">chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-161">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="030cd-162">在现有的一对一或群聊对话中发送聊天消息。</span><span class="sxs-lookup"><span data-stu-id="030cd-162">Send a chat message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="030cd-163">更新 chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-163">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="030cd-164">chatMessage</span><span class="sxs-lookup"><span data-stu-id="030cd-164">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="030cd-165">更新 **聊天消息的 policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="030cd-165">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="030cd-166">**托管内容**</span><span class="sxs-lookup"><span data-stu-id="030cd-166">**Hosted content**</span></span>| | |
|[<span data-ttu-id="030cd-167">列出所有托管内容</span><span class="sxs-lookup"><span data-stu-id="030cd-167">List all hosted content</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | <span data-ttu-id="030cd-168">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="030cd-168">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection</span></span>| <span data-ttu-id="030cd-169">获取聊天消息中所有托管的内容。</span><span class="sxs-lookup"><span data-stu-id="030cd-169">Get all hosted content in a chat message.</span></span>|
|[<span data-ttu-id="030cd-170">获取托管内容</span><span class="sxs-lookup"><span data-stu-id="030cd-170">Get hosted content</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="030cd-171">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="030cd-171">chatMessageHostedContent</span></span>](../resources/chatmessagehostedcontent.md) | <span data-ttu-id="030cd-172">从聊天消息获取托管内容。</span><span class="sxs-lookup"><span data-stu-id="030cd-172">Get hosted content from a chat message.</span></span>|


## <a name="properties"></a><span data-ttu-id="030cd-173">属性</span><span class="sxs-lookup"><span data-stu-id="030cd-173">Properties</span></span>

| <span data-ttu-id="030cd-174">属性</span><span class="sxs-lookup"><span data-stu-id="030cd-174">Property</span></span>   | <span data-ttu-id="030cd-175">类型</span><span class="sxs-lookup"><span data-stu-id="030cd-175">Type</span></span> |<span data-ttu-id="030cd-176">说明</span><span class="sxs-lookup"><span data-stu-id="030cd-176">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="030cd-177">id</span><span class="sxs-lookup"><span data-stu-id="030cd-177">id</span></span>|<span data-ttu-id="030cd-178">String</span><span class="sxs-lookup"><span data-stu-id="030cd-178">String</span></span>| <span data-ttu-id="030cd-179">只读。</span><span class="sxs-lookup"><span data-stu-id="030cd-179">Read-only.</span></span> <span data-ttu-id="030cd-180">消息的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="030cd-180">Unique ID of the message.</span></span>|
|<span data-ttu-id="030cd-181">replyToId</span><span class="sxs-lookup"><span data-stu-id="030cd-181">replyToId</span></span>| <span data-ttu-id="030cd-182">string</span><span class="sxs-lookup"><span data-stu-id="030cd-182">string</span></span> | <span data-ttu-id="030cd-183">只读。</span><span class="sxs-lookup"><span data-stu-id="030cd-183">Read-only.</span></span> <span data-ttu-id="030cd-184">线程的父聊天消息或根聊天消息的 ID。</span><span class="sxs-lookup"><span data-stu-id="030cd-184">ID of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="030cd-185"> (仅适用于频道中的聊天消息，不应用于 chats.) </span><span class="sxs-lookup"><span data-stu-id="030cd-185">(Only applies to chat messages in channels, not chats.)</span></span> |
|<span data-ttu-id="030cd-186">from</span><span class="sxs-lookup"><span data-stu-id="030cd-186">from</span></span>|[<span data-ttu-id="030cd-187">identitySet</span><span class="sxs-lookup"><span data-stu-id="030cd-187">identitySet</span></span>](identityset.md)| <span data-ttu-id="030cd-188">只读。</span><span class="sxs-lookup"><span data-stu-id="030cd-188">Read only.</span></span> <span data-ttu-id="030cd-189">聊天消息的发件人的详细信息。</span><span class="sxs-lookup"><span data-stu-id="030cd-189">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="030cd-190">etag</span><span class="sxs-lookup"><span data-stu-id="030cd-190">etag</span></span>| <span data-ttu-id="030cd-191">string</span><span class="sxs-lookup"><span data-stu-id="030cd-191">string</span></span> | <span data-ttu-id="030cd-192">只读。</span><span class="sxs-lookup"><span data-stu-id="030cd-192">Read-only.</span></span> <span data-ttu-id="030cd-193">聊天消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="030cd-193">Version number of the chat message.</span></span> |
|<span data-ttu-id="030cd-194">messageType</span><span class="sxs-lookup"><span data-stu-id="030cd-194">messageType</span></span>|<span data-ttu-id="030cd-195">string</span><span class="sxs-lookup"><span data-stu-id="030cd-195">string</span></span>|<span data-ttu-id="030cd-196">聊天消息的类型。</span><span class="sxs-lookup"><span data-stu-id="030cd-196">The type of chat message.</span></span> <span data-ttu-id="030cd-197">可能的值是： `message` 。</span><span class="sxs-lookup"><span data-stu-id="030cd-197">The possible values are: `message`.</span></span>|
|<span data-ttu-id="030cd-198">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="030cd-198">createdDateTime</span></span>|<span data-ttu-id="030cd-199">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="030cd-199">dateTimeOffset</span></span>|<span data-ttu-id="030cd-200">只读。</span><span class="sxs-lookup"><span data-stu-id="030cd-200">Read only.</span></span> <span data-ttu-id="030cd-201">创建聊天消息的时间戳。</span><span class="sxs-lookup"><span data-stu-id="030cd-201">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="030cd-202">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="030cd-202">lastModifiedDateTime</span></span>|<span data-ttu-id="030cd-203">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="030cd-203">dateTimeOffset</span></span>|<span data-ttu-id="030cd-204">只读。</span><span class="sxs-lookup"><span data-stu-id="030cd-204">Read only.</span></span> <span data-ttu-id="030cd-205">创建聊天消息的时间戳 (设置) 修改，包括添加或删除反应时。</span><span class="sxs-lookup"><span data-stu-id="030cd-205">Timestamp when the chat message is created (initial setting) or modified, including when a reaction is added or removed.</span></span> |
|<span data-ttu-id="030cd-206">lastEditedDateTime</span><span class="sxs-lookup"><span data-stu-id="030cd-206">lastEditedDateTime</span></span>|<span data-ttu-id="030cd-207">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="030cd-207">dateTimeOffset</span></span>|<span data-ttu-id="030cd-208">只读。</span><span class="sxs-lookup"><span data-stu-id="030cd-208">Read only.</span></span> <span data-ttu-id="030cd-209">编辑聊天消息的时间戳。</span><span class="sxs-lookup"><span data-stu-id="030cd-209">Timestamp when edits to the chat message were made.</span></span> <span data-ttu-id="030cd-210">在 Teams UI 中触发"已编辑"标志。</span><span class="sxs-lookup"><span data-stu-id="030cd-210">Triggers an "Edited" flag in the Teams UI.</span></span> <span data-ttu-id="030cd-211">如果未进行编辑，则值为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="030cd-211">If no edits are made the value is `null`.</span></span>|
|<span data-ttu-id="030cd-212">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="030cd-212">deletedDateTime</span></span>|<span data-ttu-id="030cd-213">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="030cd-213">dateTimeOffset</span></span>|<span data-ttu-id="030cd-214">只读。</span><span class="sxs-lookup"><span data-stu-id="030cd-214">Read only.</span></span> <span data-ttu-id="030cd-215">聊天消息被删除的时间戳;如果未删除，则为 null。</span><span class="sxs-lookup"><span data-stu-id="030cd-215">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="030cd-216">subject</span><span class="sxs-lookup"><span data-stu-id="030cd-216">subject</span></span>|<span data-ttu-id="030cd-217">string</span><span class="sxs-lookup"><span data-stu-id="030cd-217">string</span></span>| <span data-ttu-id="030cd-218">纯文本形式的聊天消息的主题。</span><span class="sxs-lookup"><span data-stu-id="030cd-218">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="030cd-219">body</span><span class="sxs-lookup"><span data-stu-id="030cd-219">body</span></span>|[<span data-ttu-id="030cd-220">itemBody</span><span class="sxs-lookup"><span data-stu-id="030cd-220">itemBody</span></span>](itembody.md)|<span data-ttu-id="030cd-221">聊天消息内容的纯文本/HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="030cd-221">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="030cd-222">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="030cd-222">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="030cd-223">如果聊天消息包含 [chatMessageMention，](chatmessagemention.md)则内容始终为 HTML 格式。</span><span class="sxs-lookup"><span data-stu-id="030cd-223">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="030cd-224">摘要</span><span class="sxs-lookup"><span data-stu-id="030cd-224">summary</span></span>|<span data-ttu-id="030cd-225">string</span><span class="sxs-lookup"><span data-stu-id="030cd-225">string</span></span>| <span data-ttu-id="030cd-226">可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。</span><span class="sxs-lookup"><span data-stu-id="030cd-226">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="030cd-227">仅适用于频道聊天消息，不应用于聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="030cd-227">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="030cd-228">附件</span><span class="sxs-lookup"><span data-stu-id="030cd-228">attachments</span></span>|<span data-ttu-id="030cd-229">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="030cd-229">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="030cd-230">附加文件。</span><span class="sxs-lookup"><span data-stu-id="030cd-230">Attached files.</span></span> <span data-ttu-id="030cd-231">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="030cd-231">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="030cd-232">提及</span><span class="sxs-lookup"><span data-stu-id="030cd-232">mentions</span></span>|<span data-ttu-id="030cd-233">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="030cd-233">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="030cd-234">聊天消息中提到的实体列表。</span><span class="sxs-lookup"><span data-stu-id="030cd-234">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="030cd-235">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="030cd-235">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="030cd-236">重要性</span><span class="sxs-lookup"><span data-stu-id="030cd-236">importance</span></span>|<span data-ttu-id="030cd-237">string</span><span class="sxs-lookup"><span data-stu-id="030cd-237">string</span></span> | <span data-ttu-id="030cd-238">聊天消息的重要性。</span><span class="sxs-lookup"><span data-stu-id="030cd-238">The importance of the chat message.</span></span> <span data-ttu-id="030cd-239">可能的值包括 `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="030cd-239">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="030cd-240">反应</span><span class="sxs-lookup"><span data-stu-id="030cd-240">reactions</span></span>| <span data-ttu-id="030cd-241">[chatMessageReaction](./chatmessagereaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="030cd-241">[chatMessageReaction](./chatmessagereaction.md) collection</span></span> | <span data-ttu-id="030cd-242">此聊天消息的反应 (，例如，) 。</span><span class="sxs-lookup"><span data-stu-id="030cd-242">Reactions for this chat message (for example, Like).</span></span>|
|<span data-ttu-id="030cd-243">区域设置</span><span class="sxs-lookup"><span data-stu-id="030cd-243">locale</span></span>|<span data-ttu-id="030cd-244">string</span><span class="sxs-lookup"><span data-stu-id="030cd-244">string</span></span>|<span data-ttu-id="030cd-245">客户端设置的聊天消息区域设置。</span><span class="sxs-lookup"><span data-stu-id="030cd-245">Locale of the chat message set by the client.</span></span>|
| <span data-ttu-id="030cd-246">policyViolation</span><span class="sxs-lookup"><span data-stu-id="030cd-246">policyViolation</span></span> | [<span data-ttu-id="030cd-247">chatMessagePolicyViolation</span><span class="sxs-lookup"><span data-stu-id="030cd-247">chatMessagePolicyViolation</span></span>](../resources/chatmessagepolicyviolation.md) |<span data-ttu-id="030cd-248">定义 DLP 应用程序数据丢失防护设置的策略违反 (属性) 。</span><span class="sxs-lookup"><span data-stu-id="030cd-248">Defines the properties of a policy violation set by a data loss prevention (DLP) application.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="030cd-249">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="030cd-249">JSON representation</span></span>

<span data-ttu-id="030cd-250">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="030cd-250">The following is a JSON representation of the resource.</span></span>

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
