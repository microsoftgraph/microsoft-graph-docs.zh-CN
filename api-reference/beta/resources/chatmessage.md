---
title: chatMessage 资源类型
description: 代表 "频道" 或 "聊天" 实体中的单个聊天消息。 聊天消息可以是一个根聊天消息，也可以是由聊天消息中的 **replyToId** 属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: bfaee36a21ee1f44781ea8ae7fed84b205ac90b4
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000637"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="8d21c-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d21c-104">chatMessage resource type</span></span>

<span data-ttu-id="8d21c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d21c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d21c-106">表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="8d21c-106">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="8d21c-107">该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。</span><span class="sxs-lookup"><span data-stu-id="8d21c-107">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

> <span data-ttu-id="8d21c-108">**注意** ：此资源支持订阅使用 [更改通知](../resources/webhooks.md) (创建、更新和删除) 所做的更改。</span><span class="sxs-lookup"><span data-stu-id="8d21c-108">**Note** : This resource supports subscribing to changes (create, update, and delete) using [change notifications](../resources/webhooks.md).</span></span> <span data-ttu-id="8d21c-109">这允许呼叫者实时订阅和获取更改。</span><span class="sxs-lookup"><span data-stu-id="8d21c-109">This allows callers to subscribe and get changes in real time.</span></span> <span data-ttu-id="8d21c-110">有关详细信息，请参阅 [获取邮件通知](/graph/teams-changenotifications-chatMessage)。</span><span class="sxs-lookup"><span data-stu-id="8d21c-110">For details, see [Get notifications for messages](/graph/teams-changenotifications-chatMessage).</span></span>

## <a name="methods"></a><span data-ttu-id="8d21c-111">方法</span><span class="sxs-lookup"><span data-stu-id="8d21c-111">Methods</span></span>

| <span data-ttu-id="8d21c-112">方法</span><span class="sxs-lookup"><span data-stu-id="8d21c-112">Method</span></span>       | <span data-ttu-id="8d21c-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="8d21c-113">Return Type</span></span>  |<span data-ttu-id="8d21c-114">说明</span><span class="sxs-lookup"><span data-stu-id="8d21c-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d21c-115">**通道邮件**</span><span class="sxs-lookup"><span data-stu-id="8d21c-115">**Channel messages**</span></span>| | |
|[<span data-ttu-id="8d21c-116">列出频道了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-116">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="8d21c-117">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d21c-117">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="8d21c-118">频道中所有根聊天邮件的列表。</span><span class="sxs-lookup"><span data-stu-id="8d21c-118">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="8d21c-119">在频道 delta 中获取 Chatmessages 集合</span><span class="sxs-lookup"><span data-stu-id="8d21c-119">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="8d21c-120">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-120">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="8d21c-121">获取通道中的增量聊天消息。</span><span class="sxs-lookup"><span data-stu-id="8d21c-121">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="8d21c-122">为新的频道消息创建订阅</span><span class="sxs-lookup"><span data-stu-id="8d21c-122">Create subscription for new channel messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="8d21c-123">订阅</span><span class="sxs-lookup"><span data-stu-id="8d21c-123">subscription</span></span>](subscription.md) | <span data-ttu-id="8d21c-124">收听新的和编辑的频道消息以及对它们的反应。</span><span class="sxs-lookup"><span data-stu-id="8d21c-124">Listen for new and edited channel messages, and reactions to them.</span></span> |
|[<span data-ttu-id="8d21c-125">获取频道了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-125">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="8d21c-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-126">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="8d21c-127">从频道中获取单个根聊天消息。</span><span class="sxs-lookup"><span data-stu-id="8d21c-127">Get a single root chat message from a channel.</span></span>|
|[<span data-ttu-id="8d21c-128">在频道或聊天中创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-128">Create chatMessage in a channel or chat</span></span>](../api/chatmessage-post.md) | [<span data-ttu-id="8d21c-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-129">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="8d21c-130">在频道中创建新的顶级聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="8d21c-130">Create a new top-level chat message in a channel.</span></span>|
|[<span data-ttu-id="8d21c-131">更新了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-131">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="8d21c-132">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-132">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="8d21c-133">更新聊天邮件的 **policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="8d21c-133">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="8d21c-134">**频道邮件答复**</span><span class="sxs-lookup"><span data-stu-id="8d21c-134">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="8d21c-135">列出对了 chatmessage 的答复</span><span class="sxs-lookup"><span data-stu-id="8d21c-135">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="8d21c-136">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d21c-136">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="8d21c-137">频道中对聊天消息的所有回复的列表。</span><span class="sxs-lookup"><span data-stu-id="8d21c-137">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="8d21c-138">获取对了 chatmessage 的答复</span><span class="sxs-lookup"><span data-stu-id="8d21c-138">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="8d21c-139">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-139">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="8d21c-140">获取频道中的聊天消息的单个答复。</span><span class="sxs-lookup"><span data-stu-id="8d21c-140">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="8d21c-141">答复频道中的了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-141">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="8d21c-142">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-142">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="8d21c-143">在频道中答复现有聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="8d21c-143">Reply to an existing chat message in a channel.</span></span>|
|[<span data-ttu-id="8d21c-144">更新了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-144">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="8d21c-145">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-145">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="8d21c-146">更新聊天邮件的 **policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="8d21c-146">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="8d21c-147">**1:1 和分组聊天消息**</span><span class="sxs-lookup"><span data-stu-id="8d21c-147">**1:1 and group chat messages**</span></span>| | |
|[<span data-ttu-id="8d21c-148">在聊天中获取了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-148">Get chatMessage in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="8d21c-149">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-149">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="8d21c-150">在聊天中获取单个聊天消息。</span><span class="sxs-lookup"><span data-stu-id="8d21c-150">Get a single chat message in a chat.</span></span> |
|[<span data-ttu-id="8d21c-151">在聊天中列出 Chatmessages 集合</span><span class="sxs-lookup"><span data-stu-id="8d21c-151">List chatMessages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="8d21c-152">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-152">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="8d21c-153">列出1:1 或组聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="8d21c-153">List chat messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="8d21c-154">创建新聊天邮件的订阅</span><span class="sxs-lookup"><span data-stu-id="8d21c-154">Create subscription for new chat messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="8d21c-155">订阅</span><span class="sxs-lookup"><span data-stu-id="8d21c-155">subscription</span></span>](subscription.md) | <span data-ttu-id="8d21c-156">收听新的和已编辑的聊天消息以及对它们的反应。</span><span class="sxs-lookup"><span data-stu-id="8d21c-156">Listen for new and edited chat messages, and reactions to them.</span></span> |
|[<span data-ttu-id="8d21c-157">在聊天中创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-157">Create chatMessage in a chat</span></span>](../api/chat-post-message.md) | [<span data-ttu-id="8d21c-158">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-158">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="8d21c-159">在现有的1:1 或组聊天对话中发送聊天消息。</span><span class="sxs-lookup"><span data-stu-id="8d21c-159">Send a chat message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="8d21c-160">更新了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-160">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="8d21c-161">chatMessage</span><span class="sxs-lookup"><span data-stu-id="8d21c-161">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="8d21c-162">更新聊天邮件的 **policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="8d21c-162">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="8d21c-163">**托管内容**</span><span class="sxs-lookup"><span data-stu-id="8d21c-163">**Hosted content**</span></span>| | |
|[<span data-ttu-id="8d21c-164">列出所有已承载的内容</span><span class="sxs-lookup"><span data-stu-id="8d21c-164">List all hosted content</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | <span data-ttu-id="8d21c-165">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d21c-165">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection</span></span>| <span data-ttu-id="8d21c-166">获取聊天消息中的所有托管内容。</span><span class="sxs-lookup"><span data-stu-id="8d21c-166">Get all hosted content in a chat message.</span></span>|
|[<span data-ttu-id="8d21c-167">获取托管内容</span><span class="sxs-lookup"><span data-stu-id="8d21c-167">Get hosted content</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="8d21c-168">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="8d21c-168">chatMessageHostedContent</span></span>](../resources/chatmessagehostedcontent.md) | <span data-ttu-id="8d21c-169">从聊天消息中获取托管的内容。</span><span class="sxs-lookup"><span data-stu-id="8d21c-169">Get hosted content from a chat message.</span></span>|


## <a name="properties"></a><span data-ttu-id="8d21c-170">属性</span><span class="sxs-lookup"><span data-stu-id="8d21c-170">Properties</span></span>

| <span data-ttu-id="8d21c-171">属性</span><span class="sxs-lookup"><span data-stu-id="8d21c-171">Property</span></span>   | <span data-ttu-id="8d21c-172">类型</span><span class="sxs-lookup"><span data-stu-id="8d21c-172">Type</span></span> |<span data-ttu-id="8d21c-173">说明</span><span class="sxs-lookup"><span data-stu-id="8d21c-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d21c-174">id</span><span class="sxs-lookup"><span data-stu-id="8d21c-174">id</span></span>|<span data-ttu-id="8d21c-175">字符串</span><span class="sxs-lookup"><span data-stu-id="8d21c-175">String</span></span>| <span data-ttu-id="8d21c-176">只读。</span><span class="sxs-lookup"><span data-stu-id="8d21c-176">Read-only.</span></span> <span data-ttu-id="8d21c-177">消息的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="8d21c-177">Unique ID of the message.</span></span>|
|<span data-ttu-id="8d21c-178">replyToId</span><span class="sxs-lookup"><span data-stu-id="8d21c-178">replyToId</span></span>| <span data-ttu-id="8d21c-179">string</span><span class="sxs-lookup"><span data-stu-id="8d21c-179">string</span></span> | <span data-ttu-id="8d21c-180">只读。</span><span class="sxs-lookup"><span data-stu-id="8d21c-180">Read-only.</span></span> <span data-ttu-id="8d21c-181">线程的父聊天消息或根聊天消息的 ID。</span><span class="sxs-lookup"><span data-stu-id="8d21c-181">ID of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="8d21c-182"> (仅适用于频道中的聊天消息，而不是聊天。 ) </span><span class="sxs-lookup"><span data-stu-id="8d21c-182">(Only applies to chat messages in channels, not chats.)</span></span> |
|<span data-ttu-id="8d21c-183">from</span><span class="sxs-lookup"><span data-stu-id="8d21c-183">from</span></span>|[<span data-ttu-id="8d21c-184">identitySet</span><span class="sxs-lookup"><span data-stu-id="8d21c-184">identitySet</span></span>](identityset.md)| <span data-ttu-id="8d21c-185">只读。</span><span class="sxs-lookup"><span data-stu-id="8d21c-185">Read only.</span></span> <span data-ttu-id="8d21c-186">聊天消息发件人的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8d21c-186">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="8d21c-187">etag</span><span class="sxs-lookup"><span data-stu-id="8d21c-187">etag</span></span>| <span data-ttu-id="8d21c-188">string</span><span class="sxs-lookup"><span data-stu-id="8d21c-188">string</span></span> | <span data-ttu-id="8d21c-189">只读。</span><span class="sxs-lookup"><span data-stu-id="8d21c-189">Read-only.</span></span> <span data-ttu-id="8d21c-190">聊天消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="8d21c-190">Version number of the chat message.</span></span> |
|<span data-ttu-id="8d21c-191">messageType</span><span class="sxs-lookup"><span data-stu-id="8d21c-191">messageType</span></span>|<span data-ttu-id="8d21c-192">string</span><span class="sxs-lookup"><span data-stu-id="8d21c-192">string</span></span>|<span data-ttu-id="8d21c-193">聊天消息的类型。</span><span class="sxs-lookup"><span data-stu-id="8d21c-193">The type of chat message.</span></span> <span data-ttu-id="8d21c-194">可能的值是： `message` 。</span><span class="sxs-lookup"><span data-stu-id="8d21c-194">The possible values are: `message`.</span></span>|
|<span data-ttu-id="8d21c-195">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d21c-195">createdDateTime</span></span>|<span data-ttu-id="8d21c-196">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d21c-196">dateTimeOffset</span></span>|<span data-ttu-id="8d21c-197">只读。</span><span class="sxs-lookup"><span data-stu-id="8d21c-197">Read only.</span></span> <span data-ttu-id="8d21c-198">在聊天消息创建时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="8d21c-198">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="8d21c-199">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d21c-199">lastModifiedDateTime</span></span>|<span data-ttu-id="8d21c-200">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d21c-200">dateTimeOffset</span></span>|<span data-ttu-id="8d21c-201">只读。</span><span class="sxs-lookup"><span data-stu-id="8d21c-201">Read only.</span></span> <span data-ttu-id="8d21c-202"> (初始设置) 或修改，包括添加或删除反应时）中创建聊天邮件时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="8d21c-202">Timestamp when the chat message is created (initial setting) or modified, including when a reaction is added or removed.</span></span> |
|<span data-ttu-id="8d21c-203">lastEditedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d21c-203">lastEditedDateTime</span></span>|<span data-ttu-id="8d21c-204">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d21c-204">dateTimeOffset</span></span>|<span data-ttu-id="8d21c-205">只读。</span><span class="sxs-lookup"><span data-stu-id="8d21c-205">Read only.</span></span> <span data-ttu-id="8d21c-206">在对聊天消息进行编辑时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="8d21c-206">Timestamp when edits to the chat message were made.</span></span> <span data-ttu-id="8d21c-207">触发团队 UI 中的 "编辑" 标志。</span><span class="sxs-lookup"><span data-stu-id="8d21c-207">Triggers an "Edited" flag in the Teams UI.</span></span> <span data-ttu-id="8d21c-208">如果未进行任何编辑，则该值为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="8d21c-208">If no edits are made the value is `null`.</span></span>|
|<span data-ttu-id="8d21c-209">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d21c-209">deletedDateTime</span></span>|<span data-ttu-id="8d21c-210">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d21c-210">dateTimeOffset</span></span>|<span data-ttu-id="8d21c-211">只读。</span><span class="sxs-lookup"><span data-stu-id="8d21c-211">Read only.</span></span> <span data-ttu-id="8d21c-212">删除聊天邮件的时间戳，如果未删除，则为 null。</span><span class="sxs-lookup"><span data-stu-id="8d21c-212">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="8d21c-213">subject</span><span class="sxs-lookup"><span data-stu-id="8d21c-213">subject</span></span>|<span data-ttu-id="8d21c-214">string</span><span class="sxs-lookup"><span data-stu-id="8d21c-214">string</span></span>| <span data-ttu-id="8d21c-215">聊天消息的主题，以纯文本形式。</span><span class="sxs-lookup"><span data-stu-id="8d21c-215">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="8d21c-216">body</span><span class="sxs-lookup"><span data-stu-id="8d21c-216">body</span></span>|[<span data-ttu-id="8d21c-217">itemBody</span><span class="sxs-lookup"><span data-stu-id="8d21c-217">itemBody</span></span>](itembody.md)|<span data-ttu-id="8d21c-218">聊天消息内容的纯文本/HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d21c-218">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="8d21c-219">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="8d21c-219">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="8d21c-220">如果聊天消息包含 [chatMessageMention](chatmessagemention.md)，则该内容始终为 HTML。</span><span class="sxs-lookup"><span data-stu-id="8d21c-220">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="8d21c-221">摘要</span><span class="sxs-lookup"><span data-stu-id="8d21c-221">summary</span></span>|<span data-ttu-id="8d21c-222">string</span><span class="sxs-lookup"><span data-stu-id="8d21c-222">string</span></span>| <span data-ttu-id="8d21c-223">可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。</span><span class="sxs-lookup"><span data-stu-id="8d21c-223">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="8d21c-224">仅适用于频道聊天消息，而不是聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="8d21c-224">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="8d21c-225">附件</span><span class="sxs-lookup"><span data-stu-id="8d21c-225">attachments</span></span>|<span data-ttu-id="8d21c-226">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d21c-226">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="8d21c-227">附加文件。</span><span class="sxs-lookup"><span data-stu-id="8d21c-227">Attached files.</span></span> <span data-ttu-id="8d21c-228">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="8d21c-228">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="8d21c-229">提及</span><span class="sxs-lookup"><span data-stu-id="8d21c-229">mentions</span></span>|<span data-ttu-id="8d21c-230">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d21c-230">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="8d21c-231">聊天消息中提及的实体列表。</span><span class="sxs-lookup"><span data-stu-id="8d21c-231">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="8d21c-232">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="8d21c-232">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="8d21c-233">重要性</span><span class="sxs-lookup"><span data-stu-id="8d21c-233">importance</span></span>|<span data-ttu-id="8d21c-234">string</span><span class="sxs-lookup"><span data-stu-id="8d21c-234">string</span></span> | <span data-ttu-id="8d21c-235">聊天消息的重要性。</span><span class="sxs-lookup"><span data-stu-id="8d21c-235">The importance of the chat message.</span></span> <span data-ttu-id="8d21c-236">可能的值包括 `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="8d21c-236">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="8d21c-237">反应</span><span class="sxs-lookup"><span data-stu-id="8d21c-237">reactions</span></span>| <span data-ttu-id="8d21c-238">[chatMessageReaction](./chatmessagereaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d21c-238">[chatMessageReaction](./chatmessagereaction.md) collection</span></span> | <span data-ttu-id="8d21c-239">此聊天消息的反应 (例如，如) 。</span><span class="sxs-lookup"><span data-stu-id="8d21c-239">Reactions for this chat message (for example, Like).</span></span>|
|<span data-ttu-id="8d21c-240">区域设置</span><span class="sxs-lookup"><span data-stu-id="8d21c-240">locale</span></span>|<span data-ttu-id="8d21c-241">string</span><span class="sxs-lookup"><span data-stu-id="8d21c-241">string</span></span>|<span data-ttu-id="8d21c-242">客户端的聊天消息的区域设置。</span><span class="sxs-lookup"><span data-stu-id="8d21c-242">Locale of the chat message set by the client.</span></span>|
| <span data-ttu-id="8d21c-243">policyViolation</span><span class="sxs-lookup"><span data-stu-id="8d21c-243">policyViolation</span></span> | [<span data-ttu-id="8d21c-244">chatMessagePolicyViolation</span><span class="sxs-lookup"><span data-stu-id="8d21c-244">chatMessagePolicyViolation</span></span>](../resources/chatmessagepolicyviolation.md) |<span data-ttu-id="8d21c-245">定义由数据丢失防护 (DLP) 应用程序设置的策略违规属性。</span><span class="sxs-lookup"><span data-stu-id="8d21c-245">Defines the properties of a policy violation set by a data loss prevention (DLP) application.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d21c-246">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d21c-246">JSON representation</span></span>

<span data-ttu-id="8d21c-247">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d21c-247">The following is a JSON representation of the resource.</span></span>

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
