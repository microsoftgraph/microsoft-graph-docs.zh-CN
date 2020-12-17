---
title: chatMessage 资源类型
description: 表示频道或聊天实体中的单个聊天消息。 聊天消息可以是根聊天消息或聊天消息中的 **replyToId** 属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: b942cfe5c4a1ca08c201a2f51f9178d5db592413
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705831"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="374bb-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="374bb-104">chatMessage resource type</span></span>

<span data-ttu-id="374bb-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="374bb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="374bb-106">表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="374bb-106">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="374bb-107">该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。</span><span class="sxs-lookup"><span data-stu-id="374bb-107">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

> <span data-ttu-id="374bb-108">**注意**：此资源支持使用更改通知 (、更新和删除) [更改](../resources/webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="374bb-108">**Note**: This resource supports subscribing to changes (create, update, and delete) using [change notifications](../resources/webhooks.md).</span></span> <span data-ttu-id="374bb-109">这使呼叫方可以实时订阅和获取更改。</span><span class="sxs-lookup"><span data-stu-id="374bb-109">This allows callers to subscribe and get changes in real time.</span></span> <span data-ttu-id="374bb-110">有关详细信息，请参阅[获取消息通知](/graph/teams-changenotifications-chatMessage)。</span><span class="sxs-lookup"><span data-stu-id="374bb-110">For details, see [Get notifications for messages](/graph/teams-changenotifications-chatMessage).</span></span>

## <a name="methods"></a><span data-ttu-id="374bb-111">方法</span><span class="sxs-lookup"><span data-stu-id="374bb-111">Methods</span></span>

| <span data-ttu-id="374bb-112">方法</span><span class="sxs-lookup"><span data-stu-id="374bb-112">Method</span></span>       | <span data-ttu-id="374bb-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="374bb-113">Return Type</span></span>  |<span data-ttu-id="374bb-114">说明</span><span class="sxs-lookup"><span data-stu-id="374bb-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="374bb-115">**频道消息**</span><span class="sxs-lookup"><span data-stu-id="374bb-115">**Channel messages**</span></span>| | |
|[<span data-ttu-id="374bb-116">列出频道 chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-116">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="374bb-117">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="374bb-117">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="374bb-118">频道中所有根聊天消息的列表。</span><span class="sxs-lookup"><span data-stu-id="374bb-118">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="374bb-119">获取通道增量中的 chatMessages</span><span class="sxs-lookup"><span data-stu-id="374bb-119">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="374bb-120">chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-120">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="374bb-121">获取频道中的增量聊天消息。</span><span class="sxs-lookup"><span data-stu-id="374bb-121">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="374bb-122">创建新频道消息的订阅</span><span class="sxs-lookup"><span data-stu-id="374bb-122">Create subscription for new channel messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="374bb-123">订阅</span><span class="sxs-lookup"><span data-stu-id="374bb-123">subscription</span></span>](subscription.md) | <span data-ttu-id="374bb-124">收听新的和编辑的频道消息，并响应这些消息。</span><span class="sxs-lookup"><span data-stu-id="374bb-124">Listen for new and edited channel messages, and reactions to them.</span></span> |
|[<span data-ttu-id="374bb-125">获取频道 chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-125">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="374bb-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-126">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="374bb-127">从频道获取单个根聊天消息。</span><span class="sxs-lookup"><span data-stu-id="374bb-127">Get a single root chat message from a channel.</span></span>|
|[<span data-ttu-id="374bb-128">在频道或聊天中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-128">Create chatMessage in a channel or chat</span></span>](../api/chatmessage-post.md) | [<span data-ttu-id="374bb-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-129">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="374bb-130">在频道中创建新的顶级聊天消息。</span><span class="sxs-lookup"><span data-stu-id="374bb-130">Create a new top-level chat message in a channel.</span></span>|
|[<span data-ttu-id="374bb-131">更新 chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-131">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="374bb-132">chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-132">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="374bb-133">更新 **聊天消息的 policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="374bb-133">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="374bb-134">**频道消息回复**</span><span class="sxs-lookup"><span data-stu-id="374bb-134">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="374bb-135">列出对 chatMessage 的回复</span><span class="sxs-lookup"><span data-stu-id="374bb-135">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="374bb-136">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="374bb-136">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="374bb-137">频道中聊天消息的所有回复列表。</span><span class="sxs-lookup"><span data-stu-id="374bb-137">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="374bb-138">获取 chatMessage 的回复</span><span class="sxs-lookup"><span data-stu-id="374bb-138">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="374bb-139">chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-139">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="374bb-140">获取频道中聊天消息的单个回复。</span><span class="sxs-lookup"><span data-stu-id="374bb-140">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="374bb-141">在频道中回复 chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-141">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="374bb-142">chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-142">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="374bb-143">回复频道中的现有聊天消息。</span><span class="sxs-lookup"><span data-stu-id="374bb-143">Reply to an existing chat message in a channel.</span></span>|
|[<span data-ttu-id="374bb-144">更新 chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-144">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="374bb-145">chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-145">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="374bb-146">更新 **聊天消息的 policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="374bb-146">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="374bb-147">**1：1 和群聊消息**</span><span class="sxs-lookup"><span data-stu-id="374bb-147">**1:1 and group chat messages**</span></span>| | |
|[<span data-ttu-id="374bb-148">获取聊天中的 chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-148">Get chatMessage in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="374bb-149">chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-149">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="374bb-150">获取聊天中的单个聊天消息。</span><span class="sxs-lookup"><span data-stu-id="374bb-150">Get a single chat message in a chat.</span></span> |
|[<span data-ttu-id="374bb-151">列出聊天中的 chatMessages</span><span class="sxs-lookup"><span data-stu-id="374bb-151">List chatMessages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="374bb-152">chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-152">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="374bb-153">列出一对一或群聊中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="374bb-153">List chat messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="374bb-154">创建新聊天消息的订阅</span><span class="sxs-lookup"><span data-stu-id="374bb-154">Create subscription for new chat messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="374bb-155">订阅</span><span class="sxs-lookup"><span data-stu-id="374bb-155">subscription</span></span>](subscription.md) | <span data-ttu-id="374bb-156">收听新的和编辑的聊天消息，并响应它们。</span><span class="sxs-lookup"><span data-stu-id="374bb-156">Listen for new and edited chat messages, and reactions to them.</span></span> |
|[<span data-ttu-id="374bb-157">在聊天中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-157">Create chatMessage in a chat</span></span>](../api/chat-post-message.md) | [<span data-ttu-id="374bb-158">chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-158">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="374bb-159">在现有的一对一或群聊对话中发送聊天消息。</span><span class="sxs-lookup"><span data-stu-id="374bb-159">Send a chat message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="374bb-160">更新 chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-160">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="374bb-161">chatMessage</span><span class="sxs-lookup"><span data-stu-id="374bb-161">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="374bb-162">更新 **聊天消息的 policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="374bb-162">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="374bb-163">**托管内容**</span><span class="sxs-lookup"><span data-stu-id="374bb-163">**Hosted content**</span></span>| | |
|[<span data-ttu-id="374bb-164">列出所有托管内容</span><span class="sxs-lookup"><span data-stu-id="374bb-164">List all hosted content</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | <span data-ttu-id="374bb-165">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="374bb-165">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection</span></span>| <span data-ttu-id="374bb-166">获取聊天消息中所有托管的内容。</span><span class="sxs-lookup"><span data-stu-id="374bb-166">Get all hosted content in a chat message.</span></span>|
|[<span data-ttu-id="374bb-167">获取托管内容</span><span class="sxs-lookup"><span data-stu-id="374bb-167">Get hosted content</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="374bb-168">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="374bb-168">chatMessageHostedContent</span></span>](../resources/chatmessagehostedcontent.md) | <span data-ttu-id="374bb-169">从聊天消息获取托管内容。</span><span class="sxs-lookup"><span data-stu-id="374bb-169">Get hosted content from a chat message.</span></span>|


## <a name="properties"></a><span data-ttu-id="374bb-170">属性</span><span class="sxs-lookup"><span data-stu-id="374bb-170">Properties</span></span>

| <span data-ttu-id="374bb-171">属性</span><span class="sxs-lookup"><span data-stu-id="374bb-171">Property</span></span>   | <span data-ttu-id="374bb-172">类型</span><span class="sxs-lookup"><span data-stu-id="374bb-172">Type</span></span> |<span data-ttu-id="374bb-173">说明</span><span class="sxs-lookup"><span data-stu-id="374bb-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="374bb-174">id</span><span class="sxs-lookup"><span data-stu-id="374bb-174">id</span></span>|<span data-ttu-id="374bb-175">字符串</span><span class="sxs-lookup"><span data-stu-id="374bb-175">String</span></span>| <span data-ttu-id="374bb-176">只读。</span><span class="sxs-lookup"><span data-stu-id="374bb-176">Read-only.</span></span> <span data-ttu-id="374bb-177">消息的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="374bb-177">Unique ID of the message.</span></span>|
|<span data-ttu-id="374bb-178">replyToId</span><span class="sxs-lookup"><span data-stu-id="374bb-178">replyToId</span></span>| <span data-ttu-id="374bb-179">string</span><span class="sxs-lookup"><span data-stu-id="374bb-179">string</span></span> | <span data-ttu-id="374bb-180">只读。</span><span class="sxs-lookup"><span data-stu-id="374bb-180">Read-only.</span></span> <span data-ttu-id="374bb-181">线程的父聊天消息或根聊天消息的 ID。</span><span class="sxs-lookup"><span data-stu-id="374bb-181">ID of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="374bb-182"> (仅适用于频道中的聊天消息，不应用于 chats.) </span><span class="sxs-lookup"><span data-stu-id="374bb-182">(Only applies to chat messages in channels, not chats.)</span></span> |
|<span data-ttu-id="374bb-183">from</span><span class="sxs-lookup"><span data-stu-id="374bb-183">from</span></span>|[<span data-ttu-id="374bb-184">identitySet</span><span class="sxs-lookup"><span data-stu-id="374bb-184">identitySet</span></span>](identityset.md)| <span data-ttu-id="374bb-185">只读。</span><span class="sxs-lookup"><span data-stu-id="374bb-185">Read only.</span></span> <span data-ttu-id="374bb-186">聊天消息的发件人的详细信息。</span><span class="sxs-lookup"><span data-stu-id="374bb-186">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="374bb-187">etag</span><span class="sxs-lookup"><span data-stu-id="374bb-187">etag</span></span>| <span data-ttu-id="374bb-188">string</span><span class="sxs-lookup"><span data-stu-id="374bb-188">string</span></span> | <span data-ttu-id="374bb-189">只读。</span><span class="sxs-lookup"><span data-stu-id="374bb-189">Read-only.</span></span> <span data-ttu-id="374bb-190">聊天消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="374bb-190">Version number of the chat message.</span></span> |
|<span data-ttu-id="374bb-191">messageType</span><span class="sxs-lookup"><span data-stu-id="374bb-191">messageType</span></span>|<span data-ttu-id="374bb-192">string</span><span class="sxs-lookup"><span data-stu-id="374bb-192">string</span></span>|<span data-ttu-id="374bb-193">聊天消息的类型。</span><span class="sxs-lookup"><span data-stu-id="374bb-193">The type of chat message.</span></span> <span data-ttu-id="374bb-194">可能的值是： `message` 。</span><span class="sxs-lookup"><span data-stu-id="374bb-194">The possible values are: `message`.</span></span>|
|<span data-ttu-id="374bb-195">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="374bb-195">createdDateTime</span></span>|<span data-ttu-id="374bb-196">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="374bb-196">dateTimeOffset</span></span>|<span data-ttu-id="374bb-197">只读。</span><span class="sxs-lookup"><span data-stu-id="374bb-197">Read only.</span></span> <span data-ttu-id="374bb-198">创建聊天消息的时间戳。</span><span class="sxs-lookup"><span data-stu-id="374bb-198">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="374bb-199">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="374bb-199">lastModifiedDateTime</span></span>|<span data-ttu-id="374bb-200">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="374bb-200">dateTimeOffset</span></span>|<span data-ttu-id="374bb-201">只读。</span><span class="sxs-lookup"><span data-stu-id="374bb-201">Read only.</span></span> <span data-ttu-id="374bb-202">创建聊天消息的时间戳 (设置) 修改，包括添加或删除反应时。</span><span class="sxs-lookup"><span data-stu-id="374bb-202">Timestamp when the chat message is created (initial setting) or modified, including when a reaction is added or removed.</span></span> |
|<span data-ttu-id="374bb-203">lastEditedDateTime</span><span class="sxs-lookup"><span data-stu-id="374bb-203">lastEditedDateTime</span></span>|<span data-ttu-id="374bb-204">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="374bb-204">dateTimeOffset</span></span>|<span data-ttu-id="374bb-205">只读。</span><span class="sxs-lookup"><span data-stu-id="374bb-205">Read only.</span></span> <span data-ttu-id="374bb-206">编辑聊天消息的时间戳。</span><span class="sxs-lookup"><span data-stu-id="374bb-206">Timestamp when edits to the chat message were made.</span></span> <span data-ttu-id="374bb-207">在 Teams UI 中触发"已编辑"标志。</span><span class="sxs-lookup"><span data-stu-id="374bb-207">Triggers an "Edited" flag in the Teams UI.</span></span> <span data-ttu-id="374bb-208">如果未进行编辑，则值为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="374bb-208">If no edits are made the value is `null`.</span></span>|
|<span data-ttu-id="374bb-209">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="374bb-209">deletedDateTime</span></span>|<span data-ttu-id="374bb-210">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="374bb-210">dateTimeOffset</span></span>|<span data-ttu-id="374bb-211">只读。</span><span class="sxs-lookup"><span data-stu-id="374bb-211">Read only.</span></span> <span data-ttu-id="374bb-212">聊天消息被删除的时间戳;如果未删除，则为 null。</span><span class="sxs-lookup"><span data-stu-id="374bb-212">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="374bb-213">subject</span><span class="sxs-lookup"><span data-stu-id="374bb-213">subject</span></span>|<span data-ttu-id="374bb-214">string</span><span class="sxs-lookup"><span data-stu-id="374bb-214">string</span></span>| <span data-ttu-id="374bb-215">纯文本形式的聊天消息的主题。</span><span class="sxs-lookup"><span data-stu-id="374bb-215">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="374bb-216">body</span><span class="sxs-lookup"><span data-stu-id="374bb-216">body</span></span>|[<span data-ttu-id="374bb-217">itemBody</span><span class="sxs-lookup"><span data-stu-id="374bb-217">itemBody</span></span>](itembody.md)|<span data-ttu-id="374bb-218">聊天消息内容的纯文本/HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="374bb-218">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="374bb-219">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="374bb-219">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="374bb-220">如果聊天消息包含 [chatMessageMention，](chatmessagemention.md)则内容始终为 HTML 格式。</span><span class="sxs-lookup"><span data-stu-id="374bb-220">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="374bb-221">摘要</span><span class="sxs-lookup"><span data-stu-id="374bb-221">summary</span></span>|<span data-ttu-id="374bb-222">string</span><span class="sxs-lookup"><span data-stu-id="374bb-222">string</span></span>| <span data-ttu-id="374bb-223">可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。</span><span class="sxs-lookup"><span data-stu-id="374bb-223">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="374bb-224">仅适用于频道聊天消息，不应用于聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="374bb-224">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="374bb-225">附件</span><span class="sxs-lookup"><span data-stu-id="374bb-225">attachments</span></span>|<span data-ttu-id="374bb-226">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="374bb-226">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="374bb-227">附加文件。</span><span class="sxs-lookup"><span data-stu-id="374bb-227">Attached files.</span></span> <span data-ttu-id="374bb-228">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="374bb-228">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="374bb-229">提及</span><span class="sxs-lookup"><span data-stu-id="374bb-229">mentions</span></span>|<span data-ttu-id="374bb-230">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="374bb-230">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="374bb-231">聊天消息中提到的实体列表。</span><span class="sxs-lookup"><span data-stu-id="374bb-231">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="374bb-232">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="374bb-232">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="374bb-233">重要性</span><span class="sxs-lookup"><span data-stu-id="374bb-233">importance</span></span>|<span data-ttu-id="374bb-234">string</span><span class="sxs-lookup"><span data-stu-id="374bb-234">string</span></span> | <span data-ttu-id="374bb-235">聊天消息的重要性。</span><span class="sxs-lookup"><span data-stu-id="374bb-235">The importance of the chat message.</span></span> <span data-ttu-id="374bb-236">可能的值包括 `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="374bb-236">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="374bb-237">反应</span><span class="sxs-lookup"><span data-stu-id="374bb-237">reactions</span></span>| <span data-ttu-id="374bb-238">[chatMessageReaction](./chatmessagereaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="374bb-238">[chatMessageReaction](./chatmessagereaction.md) collection</span></span> | <span data-ttu-id="374bb-239">此聊天消息的反应 (，例如，) 。</span><span class="sxs-lookup"><span data-stu-id="374bb-239">Reactions for this chat message (for example, Like).</span></span>|
|<span data-ttu-id="374bb-240">区域设置</span><span class="sxs-lookup"><span data-stu-id="374bb-240">locale</span></span>|<span data-ttu-id="374bb-241">string</span><span class="sxs-lookup"><span data-stu-id="374bb-241">string</span></span>|<span data-ttu-id="374bb-242">客户端设置的聊天消息区域设置。</span><span class="sxs-lookup"><span data-stu-id="374bb-242">Locale of the chat message set by the client.</span></span>|
| <span data-ttu-id="374bb-243">policyViolation</span><span class="sxs-lookup"><span data-stu-id="374bb-243">policyViolation</span></span> | [<span data-ttu-id="374bb-244">chatMessagePolicyViolation</span><span class="sxs-lookup"><span data-stu-id="374bb-244">chatMessagePolicyViolation</span></span>](../resources/chatmessagepolicyviolation.md) |<span data-ttu-id="374bb-245">定义 DLP 应用程序数据丢失防护设置的策略违反 (属性) 。</span><span class="sxs-lookup"><span data-stu-id="374bb-245">Defines the properties of a policy violation set by a data loss prevention (DLP) application.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="374bb-246">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="374bb-246">JSON representation</span></span>

<span data-ttu-id="374bb-247">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="374bb-247">The following is a JSON representation of the resource.</span></span>

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
