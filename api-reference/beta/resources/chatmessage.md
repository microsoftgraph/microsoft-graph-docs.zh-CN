---
title: chatMessage 资源类型
description: 表示频道或聊天实体中的单个聊天消息。 聊天消息可以是根聊天消息，也可以是由聊天消息中的 **replyToId** 属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: 3c0026f966d84869acca52b18347495d331f230b
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697914"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="078af-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="078af-104">chatMessage resource type</span></span>

<span data-ttu-id="078af-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="078af-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="078af-106">表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="078af-106">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="078af-107">该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。</span><span class="sxs-lookup"><span data-stu-id="078af-107">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

> <span data-ttu-id="078af-108">**注意**：此资源支持订阅更改 (使用更改通知创建、) 和 [删除更改](../resources/webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="078af-108">**Note**: This resource supports subscribing to changes (create, update, and delete) using [change notifications](../resources/webhooks.md).</span></span> <span data-ttu-id="078af-109">这使呼叫方可以实时订阅和获取更改。</span><span class="sxs-lookup"><span data-stu-id="078af-109">This allows callers to subscribe and get changes in real time.</span></span> <span data-ttu-id="078af-110">有关详细信息，请参阅[获取消息通知](/graph/teams-changenotifications-chatMessage)。</span><span class="sxs-lookup"><span data-stu-id="078af-110">For details, see [Get notifications for messages](/graph/teams-changenotifications-chatMessage).</span></span>

## <a name="methods"></a><span data-ttu-id="078af-111">方法</span><span class="sxs-lookup"><span data-stu-id="078af-111">Methods</span></span>

| <span data-ttu-id="078af-112">方法</span><span class="sxs-lookup"><span data-stu-id="078af-112">Method</span></span>       | <span data-ttu-id="078af-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="078af-113">Return Type</span></span>  |<span data-ttu-id="078af-114">说明</span><span class="sxs-lookup"><span data-stu-id="078af-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="078af-115">**频道消息**</span><span class="sxs-lookup"><span data-stu-id="078af-115">**Channel messages**</span></span>| | |
|[<span data-ttu-id="078af-116">列出频道中的消息</span><span class="sxs-lookup"><span data-stu-id="078af-116">List messages in channel</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="078af-117">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="078af-117">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="078af-118">频道中所有根消息的列表。</span><span class="sxs-lookup"><span data-stu-id="078af-118">List of all root messages in a channel.</span></span>|
|[<span data-ttu-id="078af-119">获取频道中消息的增量</span><span class="sxs-lookup"><span data-stu-id="078af-119">Get delta of messages in channel</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="078af-120">chatMessage</span><span class="sxs-lookup"><span data-stu-id="078af-120">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="078af-121">获取频道中的增量消息。</span><span class="sxs-lookup"><span data-stu-id="078af-121">Get incremental messages in a channel.</span></span> |
|[<span data-ttu-id="078af-122">创建新频道消息的订阅</span><span class="sxs-lookup"><span data-stu-id="078af-122">Create subscription for new channel messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="078af-123">订阅</span><span class="sxs-lookup"><span data-stu-id="078af-123">subscription</span></span>](subscription.md) | <span data-ttu-id="078af-124">收听新邮件、已编辑邮件和已删除邮件以及响应消息。</span><span class="sxs-lookup"><span data-stu-id="078af-124">Listen for new, edited, and deleted messages, and reactions to them.</span></span> |
|[<span data-ttu-id="078af-125">获取频道中的消息</span><span class="sxs-lookup"><span data-stu-id="078af-125">Get message in channel</span></span>](../api/chatmessage-get.md) | [<span data-ttu-id="078af-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="078af-126">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="078af-127">获取频道中的单个根消息。</span><span class="sxs-lookup"><span data-stu-id="078af-127">Get a single root message in a channel.</span></span>|
|[<span data-ttu-id="078af-128">在频道中发送消息</span><span class="sxs-lookup"><span data-stu-id="078af-128">Send message in channel</span></span>](../api/chatmessage-post.md) | [<span data-ttu-id="078af-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="078af-129">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="078af-130">在频道中创建新的根消息。</span><span class="sxs-lookup"><span data-stu-id="078af-130">Create a new root message in a channel.</span></span>|
|[<span data-ttu-id="078af-131">更新频道中的消息</span><span class="sxs-lookup"><span data-stu-id="078af-131">Update message in channel</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="078af-132">chatMessage</span><span class="sxs-lookup"><span data-stu-id="078af-132">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="078af-133">更新 **聊天消息的 policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="078af-133">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="078af-134">**频道消息回复**</span><span class="sxs-lookup"><span data-stu-id="078af-134">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="078af-135">列出对邮件的答复</span><span class="sxs-lookup"><span data-stu-id="078af-135">List replies to message</span></span>](../api/chatmessage-list-replies.md) | <span data-ttu-id="078af-136">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="078af-136">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="078af-137">频道中聊天消息的所有回复列表。</span><span class="sxs-lookup"><span data-stu-id="078af-137">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="078af-138">获取频道中的回复消息</span><span class="sxs-lookup"><span data-stu-id="078af-138">Get reply message in channel</span></span>](../api/chatmessage-get.md) | [<span data-ttu-id="078af-139">chatMessage</span><span class="sxs-lookup"><span data-stu-id="078af-139">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="078af-140">获取频道中的单个回复消息。</span><span class="sxs-lookup"><span data-stu-id="078af-140">Get a single reply message in a channel.</span></span>|
|[<span data-ttu-id="078af-141">在频道中回复消息</span><span class="sxs-lookup"><span data-stu-id="078af-141">Reply to a message in channel</span></span>](../api/chatmessage-post-replies.md) | [<span data-ttu-id="078af-142">chatMessage</span><span class="sxs-lookup"><span data-stu-id="078af-142">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="078af-143">回复频道中的现有聊天消息。</span><span class="sxs-lookup"><span data-stu-id="078af-143">Reply to an existing chat message in a channel.</span></span>|
|[<span data-ttu-id="078af-144">更新回复邮件</span><span class="sxs-lookup"><span data-stu-id="078af-144">Update reply message</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="078af-145">chatMessage</span><span class="sxs-lookup"><span data-stu-id="078af-145">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="078af-146">更新 **聊天消息的 policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="078af-146">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="078af-147">**聊天消息**</span><span class="sxs-lookup"><span data-stu-id="078af-147">**Chat messages**</span></span>| | |
|[<span data-ttu-id="078af-148">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="078af-148">List messages in chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="078af-149">chatMessage</span><span class="sxs-lookup"><span data-stu-id="078af-149">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="078af-150">列出聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="078af-150">List chat messages in a chat.</span></span> |
|[<span data-ttu-id="078af-151">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="078af-151">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="078af-152">chatMessage</span><span class="sxs-lookup"><span data-stu-id="078af-152">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="078af-153">获取聊天中的单个聊天消息。</span><span class="sxs-lookup"><span data-stu-id="078af-153">Get a single chat message in a chat.</span></span> |
|[<span data-ttu-id="078af-154">获取用户的所有聊天消息</span><span class="sxs-lookup"><span data-stu-id="078af-154">Get messages across all chats for user</span></span>](../api/chats-getallmessages.md)| <span data-ttu-id="078af-155">[chat](chat.md) 集合</span><span class="sxs-lookup"><span data-stu-id="078af-155">[chat](chat.md) collection</span></span>| <span data-ttu-id="078af-156">从用户参与的所有聊天（包括一对一聊天、群聊和会议聊天）获取消息。</span><span class="sxs-lookup"><span data-stu-id="078af-156">Get messages from all chats that a user is a participant in, including 1:1 chats, group chats, and meeting chats.</span></span> |
|[<span data-ttu-id="078af-157">创建新聊天消息的订阅</span><span class="sxs-lookup"><span data-stu-id="078af-157">Create subscription for new chat messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="078af-158">订阅</span><span class="sxs-lookup"><span data-stu-id="078af-158">subscription</span></span>](subscription.md) | <span data-ttu-id="078af-159">收听新的、编辑的和删除的聊天消息，以及这些消息的反应。</span><span class="sxs-lookup"><span data-stu-id="078af-159">Listen for new, edited, and deleted chat messages, and reactions to them.</span></span> |
|[<span data-ttu-id="078af-160">在聊天中发送消息</span><span class="sxs-lookup"><span data-stu-id="078af-160">Send message in chat</span></span>](../api/chat-post-messages.md) | [<span data-ttu-id="078af-161">chatMessage</span><span class="sxs-lookup"><span data-stu-id="078af-161">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="078af-162">在现有的一对一或群组聊天对话中发送聊天消息。</span><span class="sxs-lookup"><span data-stu-id="078af-162">Send a chat message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="078af-163">更新聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="078af-163">Update message in chat</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="078af-164">chatMessage</span><span class="sxs-lookup"><span data-stu-id="078af-164">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="078af-165">更新 **聊天消息的 policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="078af-165">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="078af-166">**托管内容**</span><span class="sxs-lookup"><span data-stu-id="078af-166">**Hosted content**</span></span>| | |
|[<span data-ttu-id="078af-167">列出所有托管内容</span><span class="sxs-lookup"><span data-stu-id="078af-167">List all hosted content</span></span>](../api/chatmessage-list-hostedcontents.md) | <span data-ttu-id="078af-168">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="078af-168">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection</span></span>| <span data-ttu-id="078af-169">获取与邮件关联的所有托管内容。</span><span class="sxs-lookup"><span data-stu-id="078af-169">Get all hosted contents associated with a message.</span></span>|
|[<span data-ttu-id="078af-170">获取托管内容</span><span class="sxs-lookup"><span data-stu-id="078af-170">Get hosted content</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="078af-171">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="078af-171">chatMessageHostedContent</span></span>](../resources/chatmessagehostedcontent.md) | <span data-ttu-id="078af-172">获取托管的内容 (其字节数) 消息的字节数。</span><span class="sxs-lookup"><span data-stu-id="078af-172">Get hosted content (and its bytes) for a message.</span></span>|


## <a name="properties"></a><span data-ttu-id="078af-173">属性</span><span class="sxs-lookup"><span data-stu-id="078af-173">Properties</span></span>

| <span data-ttu-id="078af-174">属性</span><span class="sxs-lookup"><span data-stu-id="078af-174">Property</span></span>   | <span data-ttu-id="078af-175">类型</span><span class="sxs-lookup"><span data-stu-id="078af-175">Type</span></span> |<span data-ttu-id="078af-176">说明</span><span class="sxs-lookup"><span data-stu-id="078af-176">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="078af-177">id</span><span class="sxs-lookup"><span data-stu-id="078af-177">id</span></span>|<span data-ttu-id="078af-178">String</span><span class="sxs-lookup"><span data-stu-id="078af-178">String</span></span>| <span data-ttu-id="078af-179">只读。</span><span class="sxs-lookup"><span data-stu-id="078af-179">Read-only.</span></span> <span data-ttu-id="078af-180">消息的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="078af-180">Unique ID of the message.</span></span>|
|<span data-ttu-id="078af-181">replyToId</span><span class="sxs-lookup"><span data-stu-id="078af-181">replyToId</span></span>| <span data-ttu-id="078af-182">string</span><span class="sxs-lookup"><span data-stu-id="078af-182">string</span></span> | <span data-ttu-id="078af-183">只读。</span><span class="sxs-lookup"><span data-stu-id="078af-183">Read-only.</span></span> <span data-ttu-id="078af-184">线程的父聊天消息或根聊天消息的 ID。</span><span class="sxs-lookup"><span data-stu-id="078af-184">ID of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="078af-185"> (仅适用于频道中的聊天消息，而仅适用于 chats) </span><span class="sxs-lookup"><span data-stu-id="078af-185">(Only applies to chat messages in channels, not chats.)</span></span> |
|<span data-ttu-id="078af-186">from</span><span class="sxs-lookup"><span data-stu-id="078af-186">from</span></span>|[<span data-ttu-id="078af-187">identitySet</span><span class="sxs-lookup"><span data-stu-id="078af-187">identitySet</span></span>](identityset.md)| <span data-ttu-id="078af-188">只读。</span><span class="sxs-lookup"><span data-stu-id="078af-188">Read only.</span></span> <span data-ttu-id="078af-189">聊天消息的发送者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="078af-189">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="078af-190">etag</span><span class="sxs-lookup"><span data-stu-id="078af-190">etag</span></span>| <span data-ttu-id="078af-191">string</span><span class="sxs-lookup"><span data-stu-id="078af-191">string</span></span> | <span data-ttu-id="078af-192">只读。</span><span class="sxs-lookup"><span data-stu-id="078af-192">Read-only.</span></span> <span data-ttu-id="078af-193">聊天消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="078af-193">Version number of the chat message.</span></span> |
|<span data-ttu-id="078af-194">messageType</span><span class="sxs-lookup"><span data-stu-id="078af-194">messageType</span></span>|<span data-ttu-id="078af-195">字符串</span><span class="sxs-lookup"><span data-stu-id="078af-195">string</span></span>|<span data-ttu-id="078af-196">聊天消息的类型。</span><span class="sxs-lookup"><span data-stu-id="078af-196">The type of chat message.</span></span> <span data-ttu-id="078af-197">可能的值是 `message` ：。</span><span class="sxs-lookup"><span data-stu-id="078af-197">The possible value is: `message`.</span></span>|
|<span data-ttu-id="078af-198">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="078af-198">createdDateTime</span></span>|<span data-ttu-id="078af-199">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="078af-199">dateTimeOffset</span></span>|<span data-ttu-id="078af-200">创建聊天消息的时间戳。</span><span class="sxs-lookup"><span data-stu-id="078af-200">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="078af-201">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="078af-201">lastModifiedDateTime</span></span>|<span data-ttu-id="078af-202">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="078af-202">dateTimeOffset</span></span>|<span data-ttu-id="078af-203">只读。</span><span class="sxs-lookup"><span data-stu-id="078af-203">Read only.</span></span> <span data-ttu-id="078af-204">创建聊天消息的时间戳 (设置) 修改，包括添加或删除回应时。</span><span class="sxs-lookup"><span data-stu-id="078af-204">Timestamp when the chat message is created (initial setting) or modified, including when a reaction is added or removed.</span></span> |
|<span data-ttu-id="078af-205">lastEditedDateTime</span><span class="sxs-lookup"><span data-stu-id="078af-205">lastEditedDateTime</span></span>|<span data-ttu-id="078af-206">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="078af-206">dateTimeOffset</span></span>|<span data-ttu-id="078af-207">只读。</span><span class="sxs-lookup"><span data-stu-id="078af-207">Read only.</span></span> <span data-ttu-id="078af-208">编辑聊天消息的时间戳。</span><span class="sxs-lookup"><span data-stu-id="078af-208">Timestamp when edits to the chat message were made.</span></span> <span data-ttu-id="078af-209">在 Teams UI 中触发"已编辑"标志。</span><span class="sxs-lookup"><span data-stu-id="078af-209">Triggers an "Edited" flag in the Teams UI.</span></span> <span data-ttu-id="078af-210">如果未进行编辑，则值为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="078af-210">If no edits are made the value is `null`.</span></span>|
|<span data-ttu-id="078af-211">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="078af-211">deletedDateTime</span></span>|<span data-ttu-id="078af-212">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="078af-212">dateTimeOffset</span></span>|<span data-ttu-id="078af-213">只读。</span><span class="sxs-lookup"><span data-stu-id="078af-213">Read only.</span></span> <span data-ttu-id="078af-214">删除聊天消息的时间戳;如果未删除，则返回 null。</span><span class="sxs-lookup"><span data-stu-id="078af-214">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="078af-215">subject</span><span class="sxs-lookup"><span data-stu-id="078af-215">subject</span></span>|<span data-ttu-id="078af-216">string</span><span class="sxs-lookup"><span data-stu-id="078af-216">string</span></span>| <span data-ttu-id="078af-217">纯文本形式的聊天消息的主题。</span><span class="sxs-lookup"><span data-stu-id="078af-217">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="078af-218">body</span><span class="sxs-lookup"><span data-stu-id="078af-218">body</span></span>|[<span data-ttu-id="078af-219">itemBody</span><span class="sxs-lookup"><span data-stu-id="078af-219">itemBody</span></span>](itembody.md)|<span data-ttu-id="078af-220">聊天消息内容的纯文本/HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="078af-220">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="078af-221">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="078af-221">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="078af-222">如果聊天消息包含 [chatMessageMention](chatmessagemention.md)，则内容始终为 HTML 格式。</span><span class="sxs-lookup"><span data-stu-id="078af-222">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="078af-223">摘要</span><span class="sxs-lookup"><span data-stu-id="078af-223">summary</span></span>|<span data-ttu-id="078af-224">string</span><span class="sxs-lookup"><span data-stu-id="078af-224">string</span></span>| <span data-ttu-id="078af-225">可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。</span><span class="sxs-lookup"><span data-stu-id="078af-225">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="078af-226">仅适用于频道聊天消息，不应用于聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="078af-226">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="078af-227">附件</span><span class="sxs-lookup"><span data-stu-id="078af-227">attachments</span></span>|<span data-ttu-id="078af-228">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="078af-228">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="078af-229">附加文件。</span><span class="sxs-lookup"><span data-stu-id="078af-229">Attached files.</span></span> <span data-ttu-id="078af-230">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="078af-230">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="078af-231">提及</span><span class="sxs-lookup"><span data-stu-id="078af-231">mentions</span></span>|<span data-ttu-id="078af-232">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="078af-232">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="078af-233">聊天消息中提到的实体列表。</span><span class="sxs-lookup"><span data-stu-id="078af-233">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="078af-234">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="078af-234">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="078af-235">重要性</span><span class="sxs-lookup"><span data-stu-id="078af-235">importance</span></span>|<span data-ttu-id="078af-236">string</span><span class="sxs-lookup"><span data-stu-id="078af-236">string</span></span> | <span data-ttu-id="078af-237">聊天消息的重要性。</span><span class="sxs-lookup"><span data-stu-id="078af-237">The importance of the chat message.</span></span> <span data-ttu-id="078af-238">可能的值包括 `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="078af-238">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="078af-239">反应</span><span class="sxs-lookup"><span data-stu-id="078af-239">reactions</span></span>| <span data-ttu-id="078af-240">[chatMessageReaction](chatmessagereaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="078af-240">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="078af-241">此聊天消息的反应 (例如，如) 。</span><span class="sxs-lookup"><span data-stu-id="078af-241">Reactions for this chat message (for example, Like).</span></span>|
|<span data-ttu-id="078af-242">区域设置</span><span class="sxs-lookup"><span data-stu-id="078af-242">locale</span></span>|<span data-ttu-id="078af-243">string</span><span class="sxs-lookup"><span data-stu-id="078af-243">string</span></span>|<span data-ttu-id="078af-244">客户端设置的聊天消息区域设置。</span><span class="sxs-lookup"><span data-stu-id="078af-244">Locale of the chat message set by the client.</span></span> <span data-ttu-id="078af-245">始终设置为 `en-us`。</span><span class="sxs-lookup"><span data-stu-id="078af-245">Always set to `en-us`.</span></span>|
|<span data-ttu-id="078af-246">policyViolation</span><span class="sxs-lookup"><span data-stu-id="078af-246">policyViolation</span></span> | [<span data-ttu-id="078af-247">chatMessagePolicyViolation</span><span class="sxs-lookup"><span data-stu-id="078af-247">chatMessagePolicyViolation</span></span>](chatmessagepolicyviolation.md) |<span data-ttu-id="078af-248">定义 DLP 应用程序中数据丢失防护设置的策略违反 () 属性。</span><span class="sxs-lookup"><span data-stu-id="078af-248">Defines the properties of a policy violation set by a data loss prevention (DLP) application.</span></span>|
|<span data-ttu-id="078af-249">chatId</span><span class="sxs-lookup"><span data-stu-id="078af-249">chatId</span></span>|<span data-ttu-id="078af-250">字符串</span><span class="sxs-lookup"><span data-stu-id="078af-250">string</span></span>|<span data-ttu-id="078af-251">如果消息是在聊天中发送的，则代表聊天的标识。</span><span class="sxs-lookup"><span data-stu-id="078af-251">If the message was sent in a chat, represents the identity of the chat.</span></span>|
|<span data-ttu-id="078af-252">channelIdentity</span><span class="sxs-lookup"><span data-stu-id="078af-252">channelIdentity</span></span>|[<span data-ttu-id="078af-253">channelIdentity</span><span class="sxs-lookup"><span data-stu-id="078af-253">channelIdentity</span></span>](channelidentity.md)|<span data-ttu-id="078af-254">如果消息是在频道中发送的，则代表频道的标识。</span><span class="sxs-lookup"><span data-stu-id="078af-254">If the message was sent in a channel, represents identity of the channel.</span></span>|
|<span data-ttu-id="078af-255">webUrl</span><span class="sxs-lookup"><span data-stu-id="078af-255">webUrl</span></span>|<span data-ttu-id="078af-256">string</span><span class="sxs-lookup"><span data-stu-id="078af-256">string</span></span>|<span data-ttu-id="078af-257">只读。</span><span class="sxs-lookup"><span data-stu-id="078af-257">Read-only.</span></span> <span data-ttu-id="078af-258">链接到 Microsoft Teams 中的消息。</span><span class="sxs-lookup"><span data-stu-id="078af-258">Link to the message in Microsoft Teams.</span></span>|
## <a name="relationships"></a><span data-ttu-id="078af-259">关系</span><span class="sxs-lookup"><span data-stu-id="078af-259">Relationships</span></span>

| <span data-ttu-id="078af-260">关系</span><span class="sxs-lookup"><span data-stu-id="078af-260">Relationship</span></span>   | <span data-ttu-id="078af-261">类型</span><span class="sxs-lookup"><span data-stu-id="078af-261">Type</span></span>    | <span data-ttu-id="078af-262">说明</span><span class="sxs-lookup"><span data-stu-id="078af-262">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="078af-263">replies</span><span class="sxs-lookup"><span data-stu-id="078af-263">replies</span></span>|[<span data-ttu-id="078af-264">chatMessage</span><span class="sxs-lookup"><span data-stu-id="078af-264">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="078af-265">对指定邮件的答复。</span><span class="sxs-lookup"><span data-stu-id="078af-265">Replies for a specified message.</span></span> |
|<span data-ttu-id="078af-266">hostedContents</span><span class="sxs-lookup"><span data-stu-id="078af-266">hostedContents</span></span>|[<span data-ttu-id="078af-267">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="078af-267">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md)| <span data-ttu-id="078af-268">由 Microsoft Teams 托管的消息中的内容，例如图像、代码段等。</span><span class="sxs-lookup"><span data-stu-id="078af-268">Content in a message hosted by Microsoft Teams e.g., images, code snippets etc.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="078af-269">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="078af-269">JSON representation</span></span>

<span data-ttu-id="078af-270">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="078af-270">The following is a JSON representation of the resource.</span></span>

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
