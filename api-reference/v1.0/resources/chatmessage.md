---
title: chatMessage 资源类型
description: 表示频道或聊天实体中的单个聊天消息。 聊天消息可以是根聊天消息，也可以是由聊天消息中的 **replyToId** 属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: 300d17e32114eece7e1af3f9ab57c8b3af370494
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732187"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="b2b13-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="b2b13-104">chatMessage resource type</span></span>

<span data-ttu-id="b2b13-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2b13-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b2b13-106">表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="b2b13-106">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="b2b13-107">该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。</span><span class="sxs-lookup"><span data-stu-id="b2b13-107">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

> <span data-ttu-id="b2b13-108">**注意**：此资源支持订阅更改 (使用更改通知创建、) 和 [删除更改](../resources/webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="b2b13-108">**Note**: This resource supports subscribing to changes (create, update, and delete) using [change notifications](../resources/webhooks.md).</span></span> <span data-ttu-id="b2b13-109">这使呼叫方可以实时订阅和获取更改。</span><span class="sxs-lookup"><span data-stu-id="b2b13-109">This allows callers to subscribe and get changes in real time.</span></span> <span data-ttu-id="b2b13-110">有关详细信息，请参阅[获取消息通知](/graph/teams-changenotifications-chatMessage)。</span><span class="sxs-lookup"><span data-stu-id="b2b13-110">For details, see [Get notifications for messages](/graph/teams-changenotifications-chatMessage).</span></span>

## <a name="methods"></a><span data-ttu-id="b2b13-111">Methods</span><span class="sxs-lookup"><span data-stu-id="b2b13-111">Methods</span></span>

| <span data-ttu-id="b2b13-112">方法</span><span class="sxs-lookup"><span data-stu-id="b2b13-112">Method</span></span>       | <span data-ttu-id="b2b13-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="b2b13-113">Return Type</span></span>  |<span data-ttu-id="b2b13-114">Description</span><span class="sxs-lookup"><span data-stu-id="b2b13-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2b13-115">**频道消息**</span><span class="sxs-lookup"><span data-stu-id="b2b13-115">**Channel messages**</span></span>| | |
|[<span data-ttu-id="b2b13-116">列出频道中的消息</span><span class="sxs-lookup"><span data-stu-id="b2b13-116">List messages in channel</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="b2b13-117">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b2b13-117">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="b2b13-118">频道中所有根消息的列表。</span><span class="sxs-lookup"><span data-stu-id="b2b13-118">List of all root messages in a channel.</span></span>|
|[<span data-ttu-id="b2b13-119">获取频道中消息的增量</span><span class="sxs-lookup"><span data-stu-id="b2b13-119">Get delta of messages in channel</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="b2b13-120">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b2b13-120">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="b2b13-121">获取频道中的增量消息。</span><span class="sxs-lookup"><span data-stu-id="b2b13-121">Get incremental messages in a channel.</span></span> |
|[<span data-ttu-id="b2b13-122">创建新频道消息的订阅</span><span class="sxs-lookup"><span data-stu-id="b2b13-122">Create subscription for new channel messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="b2b13-123">订阅</span><span class="sxs-lookup"><span data-stu-id="b2b13-123">subscription</span></span>](subscription.md) | <span data-ttu-id="b2b13-124">收听新邮件、已编辑邮件和已删除邮件以及响应消息。</span><span class="sxs-lookup"><span data-stu-id="b2b13-124">Listen for new, edited, and deleted messages, and reactions to them.</span></span> |
|[<span data-ttu-id="b2b13-125">获取频道中的消息</span><span class="sxs-lookup"><span data-stu-id="b2b13-125">Get message in channel</span></span>](../api/chatmessage-get.md) | [<span data-ttu-id="b2b13-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b2b13-126">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="b2b13-127">获取频道中的单个根消息。</span><span class="sxs-lookup"><span data-stu-id="b2b13-127">Get a single root message in a channel.</span></span>|
|[<span data-ttu-id="b2b13-128">在频道中发送消息</span><span class="sxs-lookup"><span data-stu-id="b2b13-128">Send message in channel</span></span>](../api/chatmessage-post.md) | [<span data-ttu-id="b2b13-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b2b13-129">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="b2b13-130">在频道中创建新的根消息。</span><span class="sxs-lookup"><span data-stu-id="b2b13-130">Create a new root message in a channel.</span></span>|
|[<span data-ttu-id="b2b13-131">更新频道中的消息</span><span class="sxs-lookup"><span data-stu-id="b2b13-131">Update message in channel</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="b2b13-132">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b2b13-132">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="b2b13-133">更新 **聊天消息的 policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="b2b13-133">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="b2b13-134">**频道消息回复**</span><span class="sxs-lookup"><span data-stu-id="b2b13-134">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="b2b13-135">列出对邮件的答复</span><span class="sxs-lookup"><span data-stu-id="b2b13-135">List replies to message</span></span>](../api/chatmessage-list-replies.md) | <span data-ttu-id="b2b13-136">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b2b13-136">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="b2b13-137">频道中聊天消息的所有回复列表。</span><span class="sxs-lookup"><span data-stu-id="b2b13-137">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="b2b13-138">获取频道中的回复消息</span><span class="sxs-lookup"><span data-stu-id="b2b13-138">Get reply message in channel</span></span>](../api/chatmessage-get.md) | [<span data-ttu-id="b2b13-139">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b2b13-139">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="b2b13-140">获取频道中的单个回复消息。</span><span class="sxs-lookup"><span data-stu-id="b2b13-140">Get a single reply message in a channel.</span></span>|
|[<span data-ttu-id="b2b13-141">在频道中回复消息</span><span class="sxs-lookup"><span data-stu-id="b2b13-141">Reply to a message in channel</span></span>](../api/chatmessage-post-replies.md) | [<span data-ttu-id="b2b13-142">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b2b13-142">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="b2b13-143">回复频道中的现有聊天消息。</span><span class="sxs-lookup"><span data-stu-id="b2b13-143">Reply to an existing chat message in a channel.</span></span>|
|[<span data-ttu-id="b2b13-144">更新回复邮件</span><span class="sxs-lookup"><span data-stu-id="b2b13-144">Update reply message</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="b2b13-145">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b2b13-145">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="b2b13-146">更新 **聊天消息的 policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="b2b13-146">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="b2b13-147">**聊天消息**</span><span class="sxs-lookup"><span data-stu-id="b2b13-147">**Chat messages**</span></span>| | |
|[<span data-ttu-id="b2b13-148">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="b2b13-148">List messages in chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="b2b13-149">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b2b13-149">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="b2b13-150">列出聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="b2b13-150">List chat messages in a chat.</span></span> |
|[<span data-ttu-id="b2b13-151">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="b2b13-151">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="b2b13-152">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b2b13-152">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="b2b13-153">获取聊天中的单个聊天消息。</span><span class="sxs-lookup"><span data-stu-id="b2b13-153">Get a single chat message in a chat.</span></span> |
|[<span data-ttu-id="b2b13-154">创建新聊天消息的订阅</span><span class="sxs-lookup"><span data-stu-id="b2b13-154">Create subscription for new chat messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="b2b13-155">订阅</span><span class="sxs-lookup"><span data-stu-id="b2b13-155">subscription</span></span>](subscription.md) | <span data-ttu-id="b2b13-156">收听新的、编辑的和删除的聊天消息，以及这些消息的反应。</span><span class="sxs-lookup"><span data-stu-id="b2b13-156">Listen for new, edited, and deleted chat messages, and reactions to them.</span></span> |
|[<span data-ttu-id="b2b13-157">在聊天中发送消息</span><span class="sxs-lookup"><span data-stu-id="b2b13-157">Send message in chat</span></span>](../api/chat-post-messages.md) | [<span data-ttu-id="b2b13-158">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b2b13-158">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="b2b13-159">在现有的一对一或群组聊天对话中发送聊天消息。</span><span class="sxs-lookup"><span data-stu-id="b2b13-159">Send a chat message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="b2b13-160">更新聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="b2b13-160">Update message in chat</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="b2b13-161">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b2b13-161">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="b2b13-162">更新 **聊天消息的 policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="b2b13-162">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="b2b13-163">**托管内容**</span><span class="sxs-lookup"><span data-stu-id="b2b13-163">**Hosted content**</span></span>| | |
|[<span data-ttu-id="b2b13-164">列出所有托管内容</span><span class="sxs-lookup"><span data-stu-id="b2b13-164">List all hosted content</span></span>](../api/chatmessage-list-hostedcontents.md) | <span data-ttu-id="b2b13-165">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b2b13-165">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection</span></span>| <span data-ttu-id="b2b13-166">获取与邮件关联的所有托管内容。</span><span class="sxs-lookup"><span data-stu-id="b2b13-166">Get all hosted contents associated with a message.</span></span>|
|[<span data-ttu-id="b2b13-167">获取托管内容</span><span class="sxs-lookup"><span data-stu-id="b2b13-167">Get hosted content</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="b2b13-168">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="b2b13-168">chatMessageHostedContent</span></span>](../resources/chatmessagehostedcontent.md) | <span data-ttu-id="b2b13-169">获取托管的内容 (其字节数) 消息的字节数。</span><span class="sxs-lookup"><span data-stu-id="b2b13-169">Get hosted content (and its bytes) for a message.</span></span>|


## <a name="properties"></a><span data-ttu-id="b2b13-170">属性</span><span class="sxs-lookup"><span data-stu-id="b2b13-170">Properties</span></span>

| <span data-ttu-id="b2b13-171">属性</span><span class="sxs-lookup"><span data-stu-id="b2b13-171">Property</span></span>   | <span data-ttu-id="b2b13-172">类型</span><span class="sxs-lookup"><span data-stu-id="b2b13-172">Type</span></span> |<span data-ttu-id="b2b13-173">说明</span><span class="sxs-lookup"><span data-stu-id="b2b13-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2b13-174">id</span><span class="sxs-lookup"><span data-stu-id="b2b13-174">id</span></span>|<span data-ttu-id="b2b13-175">String</span><span class="sxs-lookup"><span data-stu-id="b2b13-175">String</span></span>| <span data-ttu-id="b2b13-176">只读。</span><span class="sxs-lookup"><span data-stu-id="b2b13-176">Read-only.</span></span> <span data-ttu-id="b2b13-177">邮件的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="b2b13-177">Unique Id of the message.</span></span>|
|<span data-ttu-id="b2b13-178">replyToId</span><span class="sxs-lookup"><span data-stu-id="b2b13-178">replyToId</span></span>| <span data-ttu-id="b2b13-179">string</span><span class="sxs-lookup"><span data-stu-id="b2b13-179">string</span></span> | <span data-ttu-id="b2b13-180">只读。</span><span class="sxs-lookup"><span data-stu-id="b2b13-180">Read-only.</span></span> <span data-ttu-id="b2b13-181">线程的父聊天消息或根聊天消息的 ID。</span><span class="sxs-lookup"><span data-stu-id="b2b13-181">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="b2b13-182"> (仅适用于频道中的聊天消息，而仅适用于 chats) </span><span class="sxs-lookup"><span data-stu-id="b2b13-182">(Only applies to chat messages in channels, not chats.)</span></span> |
|<span data-ttu-id="b2b13-183">from</span><span class="sxs-lookup"><span data-stu-id="b2b13-183">from</span></span>|[<span data-ttu-id="b2b13-184">identitySet</span><span class="sxs-lookup"><span data-stu-id="b2b13-184">identitySet</span></span>](identityset.md)| <span data-ttu-id="b2b13-185">只读。</span><span class="sxs-lookup"><span data-stu-id="b2b13-185">Read only.</span></span> <span data-ttu-id="b2b13-186">聊天消息的发送者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b2b13-186">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="b2b13-187">etag</span><span class="sxs-lookup"><span data-stu-id="b2b13-187">etag</span></span>| <span data-ttu-id="b2b13-188">string</span><span class="sxs-lookup"><span data-stu-id="b2b13-188">string</span></span> | <span data-ttu-id="b2b13-189">只读。</span><span class="sxs-lookup"><span data-stu-id="b2b13-189">Read-only.</span></span> <span data-ttu-id="b2b13-190">聊天消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="b2b13-190">Version number of the chat message.</span></span> |
|<span data-ttu-id="b2b13-191">messageType</span><span class="sxs-lookup"><span data-stu-id="b2b13-191">messageType</span></span>|<span data-ttu-id="b2b13-192">string</span><span class="sxs-lookup"><span data-stu-id="b2b13-192">string</span></span>|<span data-ttu-id="b2b13-193">聊天消息的类型。</span><span class="sxs-lookup"><span data-stu-id="b2b13-193">The type of chat message.</span></span> <span data-ttu-id="b2b13-194">可能的值是 `message` ：。</span><span class="sxs-lookup"><span data-stu-id="b2b13-194">The possible value is: `message`.</span></span>|
|<span data-ttu-id="b2b13-195">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2b13-195">createdDateTime</span></span>|<span data-ttu-id="b2b13-196">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2b13-196">dateTimeOffset</span></span>|<span data-ttu-id="b2b13-197">创建聊天消息的时间戳。</span><span class="sxs-lookup"><span data-stu-id="b2b13-197">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="b2b13-198">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2b13-198">lastModifiedDateTime</span></span>|<span data-ttu-id="b2b13-199">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2b13-199">dateTimeOffset</span></span>|<span data-ttu-id="b2b13-200">只读。</span><span class="sxs-lookup"><span data-stu-id="b2b13-200">Read only.</span></span> <span data-ttu-id="b2b13-201">创建聊天消息的时间戳 (设置) 修改，包括添加或删除回应时。</span><span class="sxs-lookup"><span data-stu-id="b2b13-201">Timestamp when the chat message is created (initial setting) or modified, including when a reaction is added or removed.</span></span> |
|<span data-ttu-id="b2b13-202">lastEditedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2b13-202">lastEditedDateTime</span></span>|<span data-ttu-id="b2b13-203">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2b13-203">dateTimeOffset</span></span>|<span data-ttu-id="b2b13-204">只读。</span><span class="sxs-lookup"><span data-stu-id="b2b13-204">Read only.</span></span> <span data-ttu-id="b2b13-205">编辑聊天消息的时间戳。</span><span class="sxs-lookup"><span data-stu-id="b2b13-205">Timestamp when edits to the chat message were made.</span></span> <span data-ttu-id="b2b13-206">在用户界面中触发"已编辑Teams标记。</span><span class="sxs-lookup"><span data-stu-id="b2b13-206">Triggers an "Edited" flag in the Teams UI.</span></span> <span data-ttu-id="b2b13-207">如果未进行编辑，则值为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="b2b13-207">If no edits are made the value is `null`.</span></span>|
|<span data-ttu-id="b2b13-208">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2b13-208">deletedDateTime</span></span>|<span data-ttu-id="b2b13-209">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2b13-209">dateTimeOffset</span></span>|<span data-ttu-id="b2b13-210">只读。</span><span class="sxs-lookup"><span data-stu-id="b2b13-210">Read only.</span></span> <span data-ttu-id="b2b13-211">删除聊天消息的时间戳;如果未删除，则返回 null。</span><span class="sxs-lookup"><span data-stu-id="b2b13-211">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="b2b13-212">subject</span><span class="sxs-lookup"><span data-stu-id="b2b13-212">subject</span></span>|<span data-ttu-id="b2b13-213">string</span><span class="sxs-lookup"><span data-stu-id="b2b13-213">string</span></span>| <span data-ttu-id="b2b13-214">纯文本形式的聊天消息的主题。</span><span class="sxs-lookup"><span data-stu-id="b2b13-214">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="b2b13-215">body</span><span class="sxs-lookup"><span data-stu-id="b2b13-215">body</span></span>|[<span data-ttu-id="b2b13-216">itemBody</span><span class="sxs-lookup"><span data-stu-id="b2b13-216">itemBody</span></span>](itembody.md)|<span data-ttu-id="b2b13-217">聊天消息内容的纯文本/HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2b13-217">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="b2b13-218">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="b2b13-218">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="b2b13-219">如果聊天消息包含 [chatMessageMention](chatmessagemention.md)，则内容始终为 HTML 格式。</span><span class="sxs-lookup"><span data-stu-id="b2b13-219">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="b2b13-220">摘要</span><span class="sxs-lookup"><span data-stu-id="b2b13-220">summary</span></span>|<span data-ttu-id="b2b13-221">string</span><span class="sxs-lookup"><span data-stu-id="b2b13-221">string</span></span>| <span data-ttu-id="b2b13-222">可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。</span><span class="sxs-lookup"><span data-stu-id="b2b13-222">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="b2b13-223">仅适用于频道聊天消息，不应用于聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="b2b13-223">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="b2b13-224">附件</span><span class="sxs-lookup"><span data-stu-id="b2b13-224">attachments</span></span>|<span data-ttu-id="b2b13-225">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b2b13-225">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="b2b13-226">附加文件。</span><span class="sxs-lookup"><span data-stu-id="b2b13-226">Attached files.</span></span> <span data-ttu-id="b2b13-227">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="b2b13-227">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="b2b13-228">提及</span><span class="sxs-lookup"><span data-stu-id="b2b13-228">mentions</span></span>|<span data-ttu-id="b2b13-229">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b2b13-229">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="b2b13-230">聊天消息中提到的实体列表。</span><span class="sxs-lookup"><span data-stu-id="b2b13-230">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="b2b13-231">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="b2b13-231">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="b2b13-232">重要性</span><span class="sxs-lookup"><span data-stu-id="b2b13-232">importance</span></span>|<span data-ttu-id="b2b13-233">string</span><span class="sxs-lookup"><span data-stu-id="b2b13-233">string</span></span> | <span data-ttu-id="b2b13-234">聊天消息的重要性。</span><span class="sxs-lookup"><span data-stu-id="b2b13-234">The importance of the chat message.</span></span> <span data-ttu-id="b2b13-235">可能的值包括 `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="b2b13-235">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="b2b13-236">反应</span><span class="sxs-lookup"><span data-stu-id="b2b13-236">reactions</span></span>| <span data-ttu-id="b2b13-237">[chatMessageReaction](chatmessagereaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b2b13-237">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="b2b13-238">此聊天消息的反应 (例如，如) 。</span><span class="sxs-lookup"><span data-stu-id="b2b13-238">Reactions for this chat message (for example, Like).</span></span>|
|<span data-ttu-id="b2b13-239">区域设置</span><span class="sxs-lookup"><span data-stu-id="b2b13-239">locale</span></span>|<span data-ttu-id="b2b13-240">string</span><span class="sxs-lookup"><span data-stu-id="b2b13-240">string</span></span>|<span data-ttu-id="b2b13-241">客户端设置的聊天消息区域设置。</span><span class="sxs-lookup"><span data-stu-id="b2b13-241">Locale of the chat message set by the client.</span></span> <span data-ttu-id="b2b13-242">始终设置为 `en-us`。</span><span class="sxs-lookup"><span data-stu-id="b2b13-242">Always set to `en-us`.</span></span>|
|<span data-ttu-id="b2b13-243">policyViolation</span><span class="sxs-lookup"><span data-stu-id="b2b13-243">policyViolation</span></span> | [<span data-ttu-id="b2b13-244">chatMessagePolicyViolation</span><span class="sxs-lookup"><span data-stu-id="b2b13-244">chatMessagePolicyViolation</span></span>](chatmessagepolicyviolation.md) |<span data-ttu-id="b2b13-245">定义 DLP 应用程序中数据丢失防护设置的策略违反 () 属性。</span><span class="sxs-lookup"><span data-stu-id="b2b13-245">Defines the properties of a policy violation set by a data loss prevention (DLP) application.</span></span>|
|<span data-ttu-id="b2b13-246">chatId</span><span class="sxs-lookup"><span data-stu-id="b2b13-246">chatId</span></span>|<span data-ttu-id="b2b13-247">string</span><span class="sxs-lookup"><span data-stu-id="b2b13-247">string</span></span>|<span data-ttu-id="b2b13-248">如果消息是在聊天中发送的，则代表聊天的标识。</span><span class="sxs-lookup"><span data-stu-id="b2b13-248">If the message was sent in a chat, represents the identity of the chat.</span></span>|
|<span data-ttu-id="b2b13-249">channelIdentity</span><span class="sxs-lookup"><span data-stu-id="b2b13-249">channelIdentity</span></span>|[<span data-ttu-id="b2b13-250">channelIdentity</span><span class="sxs-lookup"><span data-stu-id="b2b13-250">channelIdentity</span></span>](channelidentity.md)|<span data-ttu-id="b2b13-251">如果消息是在频道中发送的，则代表频道的标识。</span><span class="sxs-lookup"><span data-stu-id="b2b13-251">If the message was sent in a channel, represents identity of the channel.</span></span>|
|<span data-ttu-id="b2b13-252">webUrl</span><span class="sxs-lookup"><span data-stu-id="b2b13-252">webUrl</span></span>|<span data-ttu-id="b2b13-253">string</span><span class="sxs-lookup"><span data-stu-id="b2b13-253">string</span></span>|<span data-ttu-id="b2b13-254">只读。</span><span class="sxs-lookup"><span data-stu-id="b2b13-254">Read-only.</span></span> <span data-ttu-id="b2b13-255">指向邮件中Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="b2b13-255">Link to the message in Microsoft Teams.</span></span>|
## <a name="relationships"></a><span data-ttu-id="b2b13-256">关系</span><span class="sxs-lookup"><span data-stu-id="b2b13-256">Relationships</span></span>

| <span data-ttu-id="b2b13-257">关系</span><span class="sxs-lookup"><span data-stu-id="b2b13-257">Relationship</span></span>   | <span data-ttu-id="b2b13-258">类型</span><span class="sxs-lookup"><span data-stu-id="b2b13-258">Type</span></span>    | <span data-ttu-id="b2b13-259">Description</span><span class="sxs-lookup"><span data-stu-id="b2b13-259">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b2b13-260">replies</span><span class="sxs-lookup"><span data-stu-id="b2b13-260">replies</span></span>|[<span data-ttu-id="b2b13-261">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b2b13-261">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="b2b13-262">对指定邮件的答复。</span><span class="sxs-lookup"><span data-stu-id="b2b13-262">Replies for a specified message.</span></span> |
|<span data-ttu-id="b2b13-263">hostedContents</span><span class="sxs-lookup"><span data-stu-id="b2b13-263">hostedContents</span></span>|[<span data-ttu-id="b2b13-264">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="b2b13-264">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md)| <span data-ttu-id="b2b13-265">由用户托管的消息中Microsoft Teams例如图像、代码段等。</span><span class="sxs-lookup"><span data-stu-id="b2b13-265">Content in a message hosted by Microsoft Teams - for example, images, code snippets etc.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b2b13-266">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b2b13-266">JSON representation</span></span>

<span data-ttu-id="b2b13-267">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2b13-267">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "replyToId",
    "lastEditedDateTime",
    "deletedDateTime",
    "subject",
    "summary",
    "attachments",
    "mentions",
    "reactions",
    "policyViolation",
    "chatId",
    "channelIdentity"
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
  "lastEditedDateTime": "string (timestamp)",
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
  "chatId": "string",
  "channelIdentity": {"@odata.type": "microsoft.graph.channelIdentity"},
  "webUrl": "string"
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
