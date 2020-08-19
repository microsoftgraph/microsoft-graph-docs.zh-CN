---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 聊天消息可以是一个根聊天消息，也可以是由聊天消息中的 **replyToId** 属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 3af846c2af807a19410a4671625ed47d637f35b3
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808786"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="281fd-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="281fd-104">chatMessage resource type</span></span>

<span data-ttu-id="281fd-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="281fd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="281fd-106">表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="281fd-106">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="281fd-107">聊天消息可以是一个根聊天消息，也可以是由聊天消息中的 **replyToId** 属性定义的答复线程的一部分。</span><span class="sxs-lookup"><span data-stu-id="281fd-107">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="281fd-108">方法</span><span class="sxs-lookup"><span data-stu-id="281fd-108">Methods</span></span>

| <span data-ttu-id="281fd-109">方法</span><span class="sxs-lookup"><span data-stu-id="281fd-109">Method</span></span>       | <span data-ttu-id="281fd-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="281fd-110">Return Type</span></span>  |<span data-ttu-id="281fd-111">说明</span><span class="sxs-lookup"><span data-stu-id="281fd-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="281fd-112">**通道邮件**</span><span class="sxs-lookup"><span data-stu-id="281fd-112">**Channel messages**</span></span>| | |
|[<span data-ttu-id="281fd-113">列出频道了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="281fd-113">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="281fd-114">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="281fd-114">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="281fd-115">频道中所有根聊天邮件的列表。</span><span class="sxs-lookup"><span data-stu-id="281fd-115">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="281fd-116">在频道 delta 中获取 Chatmessages 集合</span><span class="sxs-lookup"><span data-stu-id="281fd-116">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="281fd-117">chatMessage</span><span class="sxs-lookup"><span data-stu-id="281fd-117">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="281fd-118">获取通道中的增量聊天消息。</span><span class="sxs-lookup"><span data-stu-id="281fd-118">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="281fd-119">为新的频道消息创建订阅</span><span class="sxs-lookup"><span data-stu-id="281fd-119">Create subscription for new channel messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="281fd-120">订阅</span><span class="sxs-lookup"><span data-stu-id="281fd-120">subscription</span></span>](subscription.md) | <span data-ttu-id="281fd-121">收听新的和编辑的频道消息以及对它们的反应。</span><span class="sxs-lookup"><span data-stu-id="281fd-121">Listen for new and edited channel messages, and reactions to them.</span></span> |
|[<span data-ttu-id="281fd-122">获取频道了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="281fd-122">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="281fd-123">chatMessage</span><span class="sxs-lookup"><span data-stu-id="281fd-123">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="281fd-124">从频道中获取单个根聊天消息。</span><span class="sxs-lookup"><span data-stu-id="281fd-124">Get a single root chat message from a channel.</span></span>|
|[<span data-ttu-id="281fd-125">在频道或聊天中创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="281fd-125">Create chatMessage in a channel or chat</span></span>](../api/chatmessage-post.md) | [<span data-ttu-id="281fd-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="281fd-126">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="281fd-127">在频道中创建新的顶级聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="281fd-127">Create a new top-level chat message in a channel.</span></span>|
|<span data-ttu-id="281fd-128">**频道邮件答复**</span><span class="sxs-lookup"><span data-stu-id="281fd-128">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="281fd-129">列出对了 chatmessage 的答复</span><span class="sxs-lookup"><span data-stu-id="281fd-129">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="281fd-130">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="281fd-130">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="281fd-131">频道中对聊天消息的所有回复的列表。</span><span class="sxs-lookup"><span data-stu-id="281fd-131">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="281fd-132">获取对了 chatmessage 的答复</span><span class="sxs-lookup"><span data-stu-id="281fd-132">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="281fd-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="281fd-133">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="281fd-134">获取频道中的聊天消息的单个答复。</span><span class="sxs-lookup"><span data-stu-id="281fd-134">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="281fd-135">答复频道中的了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="281fd-135">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="281fd-136">chatMessage</span><span class="sxs-lookup"><span data-stu-id="281fd-136">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="281fd-137">在频道中答复现有聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="281fd-137">Reply to an existing chat message in a channel.</span></span>|
|<span data-ttu-id="281fd-138">**1:1 和分组聊天消息**</span><span class="sxs-lookup"><span data-stu-id="281fd-138">**1:1 and group chat messages**</span></span>| | |
|[<span data-ttu-id="281fd-139">在聊天中创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="281fd-139">Create chatMessage in a chat</span></span>](../api/chat-post-message.md) | [<span data-ttu-id="281fd-140">chatMessage</span><span class="sxs-lookup"><span data-stu-id="281fd-140">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="281fd-141">在现有的1:1 或组聊天对话中发送聊天消息。</span><span class="sxs-lookup"><span data-stu-id="281fd-141">Send a chat message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="281fd-142">在聊天中列出 Chatmessages 集合</span><span class="sxs-lookup"><span data-stu-id="281fd-142">List chatMessages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="281fd-143">chatMessage</span><span class="sxs-lookup"><span data-stu-id="281fd-143">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="281fd-144">列出1:1 或组聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="281fd-144">List chat messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="281fd-145">创建新聊天邮件的订阅</span><span class="sxs-lookup"><span data-stu-id="281fd-145">Create subscription for new chat messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="281fd-146">订阅</span><span class="sxs-lookup"><span data-stu-id="281fd-146">subscription</span></span>](subscription.md) | <span data-ttu-id="281fd-147">收听新的和已编辑的聊天消息以及对它们的反应。</span><span class="sxs-lookup"><span data-stu-id="281fd-147">Listen for new and edited chat messages, and reactions to them.</span></span> |
|[<span data-ttu-id="281fd-148">在聊天中获取了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="281fd-148">Get chatMessage in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="281fd-149">chatMessage</span><span class="sxs-lookup"><span data-stu-id="281fd-149">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="281fd-150">在聊天中获取单个聊天消息。</span><span class="sxs-lookup"><span data-stu-id="281fd-150">Get a single chat message in a chat.</span></span> |
|<span data-ttu-id="281fd-151">**托管内容**</span><span class="sxs-lookup"><span data-stu-id="281fd-151">**Hosted content**</span></span>| | |
|[<span data-ttu-id="281fd-152">列出所有已承载的内容</span><span class="sxs-lookup"><span data-stu-id="281fd-152">List all hosted content</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | <span data-ttu-id="281fd-153">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="281fd-153">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection</span></span>| <span data-ttu-id="281fd-154">获取聊天消息中的所有托管内容。</span><span class="sxs-lookup"><span data-stu-id="281fd-154">Get all hosted content in a chat message.</span></span>|
|[<span data-ttu-id="281fd-155">获取托管内容</span><span class="sxs-lookup"><span data-stu-id="281fd-155">Get hosted content</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="281fd-156">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="281fd-156">chatMessageHostedContent</span></span>](../resources/chatmessagehostedcontent.md) | <span data-ttu-id="281fd-157">从聊天消息中获取托管的内容。</span><span class="sxs-lookup"><span data-stu-id="281fd-157">Get hosted content from a chat message.</span></span>|

## <a name="properties"></a><span data-ttu-id="281fd-158">属性</span><span class="sxs-lookup"><span data-stu-id="281fd-158">Properties</span></span>

| <span data-ttu-id="281fd-159">属性</span><span class="sxs-lookup"><span data-stu-id="281fd-159">Property</span></span>   | <span data-ttu-id="281fd-160">类型</span><span class="sxs-lookup"><span data-stu-id="281fd-160">Type</span></span> |<span data-ttu-id="281fd-161">说明</span><span class="sxs-lookup"><span data-stu-id="281fd-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="281fd-162">id</span><span class="sxs-lookup"><span data-stu-id="281fd-162">id</span></span>|<span data-ttu-id="281fd-163">String</span><span class="sxs-lookup"><span data-stu-id="281fd-163">String</span></span>| <span data-ttu-id="281fd-164">只读。</span><span class="sxs-lookup"><span data-stu-id="281fd-164">Read-only.</span></span> <span data-ttu-id="281fd-165">邮件的唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="281fd-165">Unique Id of the message.</span></span>|
|<span data-ttu-id="281fd-166">replyToId</span><span class="sxs-lookup"><span data-stu-id="281fd-166">replyToId</span></span>| <span data-ttu-id="281fd-167">string</span><span class="sxs-lookup"><span data-stu-id="281fd-167">string</span></span> | <span data-ttu-id="281fd-168">只读。</span><span class="sxs-lookup"><span data-stu-id="281fd-168">Read-only.</span></span> <span data-ttu-id="281fd-169">线程的父聊天消息或根聊天消息的 Id。</span><span class="sxs-lookup"><span data-stu-id="281fd-169">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="281fd-170"> (仅适用于频道中不聊天的聊天消息) </span><span class="sxs-lookup"><span data-stu-id="281fd-170">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="281fd-171">from</span><span class="sxs-lookup"><span data-stu-id="281fd-171">from</span></span>|[<span data-ttu-id="281fd-172">identitySet</span><span class="sxs-lookup"><span data-stu-id="281fd-172">identitySet</span></span>](identityset.md)| <span data-ttu-id="281fd-173">只读。</span><span class="sxs-lookup"><span data-stu-id="281fd-173">Read only.</span></span> <span data-ttu-id="281fd-174">聊天消息发件人的详细信息。</span><span class="sxs-lookup"><span data-stu-id="281fd-174">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="281fd-175">etag</span><span class="sxs-lookup"><span data-stu-id="281fd-175">etag</span></span>| <span data-ttu-id="281fd-176">string</span><span class="sxs-lookup"><span data-stu-id="281fd-176">string</span></span> | <span data-ttu-id="281fd-177">只读。</span><span class="sxs-lookup"><span data-stu-id="281fd-177">Read-only.</span></span> <span data-ttu-id="281fd-178">聊天消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="281fd-178">Version number of the chat message.</span></span> |
|<span data-ttu-id="281fd-179">messageType</span><span class="sxs-lookup"><span data-stu-id="281fd-179">messageType</span></span>|<span data-ttu-id="281fd-180">string</span><span class="sxs-lookup"><span data-stu-id="281fd-180">string</span></span>|<span data-ttu-id="281fd-181">聊天消息的类型。</span><span class="sxs-lookup"><span data-stu-id="281fd-181">The type of chat message.</span></span> <span data-ttu-id="281fd-182">可能的值是： `message` 。</span><span class="sxs-lookup"><span data-stu-id="281fd-182">The possible values are: `message`.</span></span>|
|<span data-ttu-id="281fd-183">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="281fd-183">createdDateTime</span></span>|<span data-ttu-id="281fd-184">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="281fd-184">dateTimeOffset</span></span>|<span data-ttu-id="281fd-185">只读。</span><span class="sxs-lookup"><span data-stu-id="281fd-185">Read only.</span></span> <span data-ttu-id="281fd-186">在聊天消息创建时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="281fd-186">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="281fd-187">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="281fd-187">lastModifiedDateTime</span></span>|<span data-ttu-id="281fd-188">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="281fd-188">dateTimeOffset</span></span>|<span data-ttu-id="281fd-189">只读。</span><span class="sxs-lookup"><span data-stu-id="281fd-189">Read only.</span></span> <span data-ttu-id="281fd-190">在创建或编辑聊天消息时的时间戳，包括答复的时间 (如果它是频道中的根聊天消息) 或者添加或删除了反应。</span><span class="sxs-lookup"><span data-stu-id="281fd-190">Timestamp of when the chat message is created or edited, including when a reply is made (if it's a root chat message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="281fd-191">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="281fd-191">deletedDateTime</span></span>|<span data-ttu-id="281fd-192">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="281fd-192">dateTimeOffset</span></span>|<span data-ttu-id="281fd-193">只读。</span><span class="sxs-lookup"><span data-stu-id="281fd-193">Read only.</span></span> <span data-ttu-id="281fd-194">删除聊天邮件的时间戳，如果未删除，则为 null。</span><span class="sxs-lookup"><span data-stu-id="281fd-194">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="281fd-195">subject</span><span class="sxs-lookup"><span data-stu-id="281fd-195">subject</span></span>|<span data-ttu-id="281fd-196">string</span><span class="sxs-lookup"><span data-stu-id="281fd-196">string</span></span>| <span data-ttu-id="281fd-197">聊天消息的主题，以纯文本形式。</span><span class="sxs-lookup"><span data-stu-id="281fd-197">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="281fd-198">body</span><span class="sxs-lookup"><span data-stu-id="281fd-198">body</span></span>|[<span data-ttu-id="281fd-199">itemBody</span><span class="sxs-lookup"><span data-stu-id="281fd-199">itemBody</span></span>](itembody.md)|<span data-ttu-id="281fd-200">聊天消息内容的纯文本/HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="281fd-200">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="281fd-201">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="281fd-201">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="281fd-202">如果聊天消息包含 [chatMessageMention](chatmessagemention.md)，则该内容始终为 HTML。</span><span class="sxs-lookup"><span data-stu-id="281fd-202">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="281fd-203">摘要</span><span class="sxs-lookup"><span data-stu-id="281fd-203">summary</span></span>|<span data-ttu-id="281fd-204">string</span><span class="sxs-lookup"><span data-stu-id="281fd-204">string</span></span>| <span data-ttu-id="281fd-205">可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。</span><span class="sxs-lookup"><span data-stu-id="281fd-205">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="281fd-206">仅适用于频道聊天消息，而不是聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="281fd-206">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="281fd-207">附件</span><span class="sxs-lookup"><span data-stu-id="281fd-207">attachments</span></span>|<span data-ttu-id="281fd-208">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="281fd-208">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="281fd-209">附加文件。</span><span class="sxs-lookup"><span data-stu-id="281fd-209">Attached files.</span></span> <span data-ttu-id="281fd-210">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="281fd-210">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="281fd-211">提及</span><span class="sxs-lookup"><span data-stu-id="281fd-211">mentions</span></span>|<span data-ttu-id="281fd-212">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="281fd-212">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="281fd-213">聊天消息中提及的实体列表。</span><span class="sxs-lookup"><span data-stu-id="281fd-213">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="281fd-214">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="281fd-214">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="281fd-215">重要性</span><span class="sxs-lookup"><span data-stu-id="281fd-215">importance</span></span>|<span data-ttu-id="281fd-216">string</span><span class="sxs-lookup"><span data-stu-id="281fd-216">string</span></span> | <span data-ttu-id="281fd-217">聊天消息的重要性。</span><span class="sxs-lookup"><span data-stu-id="281fd-217">The importance of the chat message.</span></span> <span data-ttu-id="281fd-218">可能的值包括 `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="281fd-218">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="281fd-219">反应</span><span class="sxs-lookup"><span data-stu-id="281fd-219">reactions</span></span>| <span data-ttu-id="281fd-220">[chatMessageReaction](./chatmessagereaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="281fd-220">[chatMessageReaction](./chatmessagereaction.md) collection</span></span> | <span data-ttu-id="281fd-221">此聊天消息的反应 (例如，如) 。</span><span class="sxs-lookup"><span data-stu-id="281fd-221">Reactions for this chat message (for example, Like).</span></span>|
|<span data-ttu-id="281fd-222">区域设置</span><span class="sxs-lookup"><span data-stu-id="281fd-222">locale</span></span>|<span data-ttu-id="281fd-223">string</span><span class="sxs-lookup"><span data-stu-id="281fd-223">string</span></span>|<span data-ttu-id="281fd-224">客户端的聊天消息的区域设置。</span><span class="sxs-lookup"><span data-stu-id="281fd-224">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="281fd-225">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="281fd-225">JSON representation</span></span>

<span data-ttu-id="281fd-226">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="281fd-226">The following is a JSON representation of the resource.</span></span>

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
  "policyViolation": "string",
  "reactions":  "string",
  "locale": "string",
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
