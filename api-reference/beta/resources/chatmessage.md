---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 聊天消息可以是一个根聊天消息，也可以是由聊天消息中的**replyToId**属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 895425cd7c5b83661fb55be53cd17cefb0a73103
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844237"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="f6125-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6125-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6125-105">表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="f6125-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="f6125-106">聊天消息可以是一个根聊天消息，也可以是由聊天消息中的**replyToId**属性定义的答复线程的一部分。</span><span class="sxs-lookup"><span data-stu-id="f6125-106">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="f6125-107">方法</span><span class="sxs-lookup"><span data-stu-id="f6125-107">Methods</span></span>

| <span data-ttu-id="f6125-108">方法</span><span class="sxs-lookup"><span data-stu-id="f6125-108">Method</span></span>       | <span data-ttu-id="f6125-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f6125-109">Return Type</span></span>  |<span data-ttu-id="f6125-110">说明</span><span class="sxs-lookup"><span data-stu-id="f6125-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6125-111">**通道邮件**</span><span class="sxs-lookup"><span data-stu-id="f6125-111">**Channel messages**</span></span>| | |
|[<span data-ttu-id="f6125-112">列出频道了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="f6125-112">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="f6125-113">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f6125-113">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="f6125-114">频道中所有根聊天邮件的列表。</span><span class="sxs-lookup"><span data-stu-id="f6125-114">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="f6125-115">在频道 delta 中获取 Chatmessages 集合</span><span class="sxs-lookup"><span data-stu-id="f6125-115">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="f6125-116">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f6125-116">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="f6125-117">获取通道中的增量聊天消息。</span><span class="sxs-lookup"><span data-stu-id="f6125-117">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="f6125-118">为新的频道消息创建订阅</span><span class="sxs-lookup"><span data-stu-id="f6125-118">Create subscription for new channel messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="f6125-119">订阅</span><span class="sxs-lookup"><span data-stu-id="f6125-119">subscription</span></span>](subscription.md) | <span data-ttu-id="f6125-120">收听新的和编辑的频道消息以及对它们的反应。</span><span class="sxs-lookup"><span data-stu-id="f6125-120">Listen for new and edited channel messages, and reactions to them.</span></span> |
|[<span data-ttu-id="f6125-121">获取频道了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="f6125-121">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="f6125-122">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f6125-122">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="f6125-123">从频道中获取单个根聊天消息。</span><span class="sxs-lookup"><span data-stu-id="f6125-123">Get a single root chat message from a channel.</span></span>|
|<span data-ttu-id="f6125-124">**频道邮件答复**</span><span class="sxs-lookup"><span data-stu-id="f6125-124">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="f6125-125">列出对了 chatmessage 的答复</span><span class="sxs-lookup"><span data-stu-id="f6125-125">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="f6125-126">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f6125-126">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="f6125-127">频道中对聊天消息的所有回复的列表。</span><span class="sxs-lookup"><span data-stu-id="f6125-127">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="f6125-128">获取对了 chatmessage 的答复</span><span class="sxs-lookup"><span data-stu-id="f6125-128">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="f6125-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f6125-129">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="f6125-130">获取频道中的聊天消息的单个答复。</span><span class="sxs-lookup"><span data-stu-id="f6125-130">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="f6125-131">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="f6125-131">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="f6125-132">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f6125-132">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="f6125-133">在频道中创建新的顶级聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="f6125-133">Create a new top-level chat message in a channel.</span></span>|
|[<span data-ttu-id="f6125-134">答复频道中的了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="f6125-134">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="f6125-135">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f6125-135">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="f6125-136">在频道中答复现有聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="f6125-136">Reply to an existing chat message in a channel.</span></span>|
|<span data-ttu-id="f6125-137">**1:1 和分组聊天消息**</span><span class="sxs-lookup"><span data-stu-id="f6125-137">**1:1 and group chat messages**</span></span>| | |
|[<span data-ttu-id="f6125-138">在聊天中创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="f6125-138">Create chatMessage in a chat</span></span>](../api/chat-post-messages.md) | [<span data-ttu-id="f6125-139">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f6125-139">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="f6125-140">在现有的1:1 或组聊天对话中发送聊天消息。</span><span class="sxs-lookup"><span data-stu-id="f6125-140">Send a chat message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="f6125-141">在聊天中列出 Chatmessages 集合</span><span class="sxs-lookup"><span data-stu-id="f6125-141">List chatMessages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="f6125-142">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f6125-142">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="f6125-143">列出1:1 或组聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="f6125-143">List chat messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="f6125-144">创建新聊天邮件的订阅</span><span class="sxs-lookup"><span data-stu-id="f6125-144">Create subscription for new chat messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="f6125-145">订阅</span><span class="sxs-lookup"><span data-stu-id="f6125-145">subscription</span></span>](subscription.md) | <span data-ttu-id="f6125-146">收听新的和已编辑的聊天消息以及对它们的反应。</span><span class="sxs-lookup"><span data-stu-id="f6125-146">Listen for new and edited chat messages, and reactions to them.</span></span> |
|[<span data-ttu-id="f6125-147">在聊天中获取了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="f6125-147">Get chatMessage in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="f6125-148">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f6125-148">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="f6125-149">在聊天中获取单个聊天消息。</span><span class="sxs-lookup"><span data-stu-id="f6125-149">Get a single chat message in a chat.</span></span> |
|<span data-ttu-id="f6125-150">**托管内容**</span><span class="sxs-lookup"><span data-stu-id="f6125-150">**Hosted content**</span></span>| | |
|[<span data-ttu-id="f6125-151">列出所有已承载的内容</span><span class="sxs-lookup"><span data-stu-id="f6125-151">List all hosted content</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | <span data-ttu-id="f6125-152">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)集合</span><span class="sxs-lookup"><span data-stu-id="f6125-152">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection</span></span>| <span data-ttu-id="f6125-153">获取聊天消息中的所有托管内容。</span><span class="sxs-lookup"><span data-stu-id="f6125-153">Get all hosted content in a chat message.</span></span>|
|[<span data-ttu-id="f6125-154">获取托管内容</span><span class="sxs-lookup"><span data-stu-id="f6125-154">Get hosted content</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="f6125-155">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="f6125-155">chatMessageHostedContent</span></span>](../resources/chatmessagehostedcontent.md) | <span data-ttu-id="f6125-156">从聊天消息中获取托管的内容。</span><span class="sxs-lookup"><span data-stu-id="f6125-156">Get hosted content from a chat message.</span></span>|

## <a name="properties"></a><span data-ttu-id="f6125-157">属性</span><span class="sxs-lookup"><span data-stu-id="f6125-157">Properties</span></span>

| <span data-ttu-id="f6125-158">属性</span><span class="sxs-lookup"><span data-stu-id="f6125-158">Property</span></span>   | <span data-ttu-id="f6125-159">类型</span><span class="sxs-lookup"><span data-stu-id="f6125-159">Type</span></span> |<span data-ttu-id="f6125-160">说明</span><span class="sxs-lookup"><span data-stu-id="f6125-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6125-161">id</span><span class="sxs-lookup"><span data-stu-id="f6125-161">id</span></span>|<span data-ttu-id="f6125-162">字符串</span><span class="sxs-lookup"><span data-stu-id="f6125-162">String</span></span>| <span data-ttu-id="f6125-163">只读。</span><span class="sxs-lookup"><span data-stu-id="f6125-163">Read-only.</span></span> <span data-ttu-id="f6125-164">邮件的唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="f6125-164">Unique Id of the message.</span></span>|
|<span data-ttu-id="f6125-165">replyToId</span><span class="sxs-lookup"><span data-stu-id="f6125-165">replyToId</span></span>| <span data-ttu-id="f6125-166">string</span><span class="sxs-lookup"><span data-stu-id="f6125-166">string</span></span> | <span data-ttu-id="f6125-167">只读。</span><span class="sxs-lookup"><span data-stu-id="f6125-167">Read-only.</span></span> <span data-ttu-id="f6125-168">线程的父聊天消息或根聊天消息的 Id。</span><span class="sxs-lookup"><span data-stu-id="f6125-168">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="f6125-169">（仅适用于通道中不聊天的聊天邮件）</span><span class="sxs-lookup"><span data-stu-id="f6125-169">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="f6125-170">from</span><span class="sxs-lookup"><span data-stu-id="f6125-170">from</span></span>|[<span data-ttu-id="f6125-171">identitySet</span><span class="sxs-lookup"><span data-stu-id="f6125-171">identitySet</span></span>](identityset.md)| <span data-ttu-id="f6125-172">只读。</span><span class="sxs-lookup"><span data-stu-id="f6125-172">Read only.</span></span> <span data-ttu-id="f6125-173">聊天消息发件人的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f6125-173">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="f6125-174">etag</span><span class="sxs-lookup"><span data-stu-id="f6125-174">etag</span></span>| <span data-ttu-id="f6125-175">string</span><span class="sxs-lookup"><span data-stu-id="f6125-175">string</span></span> | <span data-ttu-id="f6125-176">只读。</span><span class="sxs-lookup"><span data-stu-id="f6125-176">Read-only.</span></span> <span data-ttu-id="f6125-177">聊天消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="f6125-177">Version number of the chat message.</span></span> |
|<span data-ttu-id="f6125-178">messageType</span><span class="sxs-lookup"><span data-stu-id="f6125-178">messageType</span></span>|<span data-ttu-id="f6125-179">chatMessageType</span><span class="sxs-lookup"><span data-stu-id="f6125-179">chatMessageType</span></span>|<span data-ttu-id="f6125-180">聊天消息的类型。</span><span class="sxs-lookup"><span data-stu-id="f6125-180">The type of chat message.</span></span> <span data-ttu-id="f6125-181">可能的值是： `message`。</span><span class="sxs-lookup"><span data-stu-id="f6125-181">The possible values are: `message`.</span></span>|
|<span data-ttu-id="f6125-182">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6125-182">createdDateTime</span></span>|<span data-ttu-id="f6125-183">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6125-183">dateTimeOffset</span></span>|<span data-ttu-id="f6125-184">只读。</span><span class="sxs-lookup"><span data-stu-id="f6125-184">Read only.</span></span> <span data-ttu-id="f6125-185">在聊天消息创建时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="f6125-185">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="f6125-186">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6125-186">lastModifiedDateTime</span></span>|<span data-ttu-id="f6125-187">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6125-187">dateTimeOffset</span></span>|<span data-ttu-id="f6125-188">只读。</span><span class="sxs-lookup"><span data-stu-id="f6125-188">Read only.</span></span> <span data-ttu-id="f6125-189">在创建或编辑聊天消息时的时间戳，包括答复的时间（如果是频道中的根聊天邮件）或添加或删除了反应。</span><span class="sxs-lookup"><span data-stu-id="f6125-189">Timestamp of when the chat message is created or edited, including when a reply is made (if it's a root chat message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="f6125-190">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6125-190">deletedDateTime</span></span>|<span data-ttu-id="f6125-191">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6125-191">dateTimeOffset</span></span>|<span data-ttu-id="f6125-192">只读。</span><span class="sxs-lookup"><span data-stu-id="f6125-192">Read only.</span></span> <span data-ttu-id="f6125-193">删除聊天邮件的时间戳，如果未删除，则为 null。</span><span class="sxs-lookup"><span data-stu-id="f6125-193">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="f6125-194">subject</span><span class="sxs-lookup"><span data-stu-id="f6125-194">subject</span></span>|<span data-ttu-id="f6125-195">string</span><span class="sxs-lookup"><span data-stu-id="f6125-195">string</span></span>| <span data-ttu-id="f6125-196">聊天消息的主题，以纯文本形式。</span><span class="sxs-lookup"><span data-stu-id="f6125-196">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="f6125-197">body</span><span class="sxs-lookup"><span data-stu-id="f6125-197">body</span></span>|[<span data-ttu-id="f6125-198">itemBody</span><span class="sxs-lookup"><span data-stu-id="f6125-198">itemBody</span></span>](itembody.md)|<span data-ttu-id="f6125-199">聊天消息内容的纯文本/HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6125-199">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="f6125-200">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="f6125-200">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="f6125-201">如果聊天消息包含[chatMessageMention](chatmessagemention.md)，则该内容始终为 HTML。</span><span class="sxs-lookup"><span data-stu-id="f6125-201">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="f6125-202">摘要</span><span class="sxs-lookup"><span data-stu-id="f6125-202">summary</span></span>|<span data-ttu-id="f6125-203">string</span><span class="sxs-lookup"><span data-stu-id="f6125-203">string</span></span>| <span data-ttu-id="f6125-204">可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。</span><span class="sxs-lookup"><span data-stu-id="f6125-204">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="f6125-205">仅适用于频道聊天消息，而不是聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="f6125-205">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="f6125-206">附件</span><span class="sxs-lookup"><span data-stu-id="f6125-206">attachments</span></span>|<span data-ttu-id="f6125-207">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f6125-207">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="f6125-208">附加文件。</span><span class="sxs-lookup"><span data-stu-id="f6125-208">Attached files.</span></span> <span data-ttu-id="f6125-209">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="f6125-209">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="f6125-210">提及</span><span class="sxs-lookup"><span data-stu-id="f6125-210">mentions</span></span>|<span data-ttu-id="f6125-211">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f6125-211">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="f6125-212">聊天消息中提及的实体列表。</span><span class="sxs-lookup"><span data-stu-id="f6125-212">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="f6125-213">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="f6125-213">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="f6125-214">重要性</span><span class="sxs-lookup"><span data-stu-id="f6125-214">importance</span></span>| <span data-ttu-id="f6125-215">chatMessageImportance</span><span class="sxs-lookup"><span data-stu-id="f6125-215">chatMessageImportance</span></span> | <span data-ttu-id="f6125-216">聊天消息的重要性。</span><span class="sxs-lookup"><span data-stu-id="f6125-216">The importance of the chat message.</span></span> <span data-ttu-id="f6125-217">可能的值包括 `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="f6125-217">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="f6125-218">反应</span><span class="sxs-lookup"><span data-stu-id="f6125-218">reactions</span></span>| <span data-ttu-id="f6125-219">[chatMessageReaction](chatmessagereaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f6125-219">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="f6125-220">此聊天消息的反应（例如，如）。</span><span class="sxs-lookup"><span data-stu-id="f6125-220">Reactions for this chat message (for example, Like).</span></span>|
|<span data-ttu-id="f6125-221">区域设置</span><span class="sxs-lookup"><span data-stu-id="f6125-221">locale</span></span>|<span data-ttu-id="f6125-222">string</span><span class="sxs-lookup"><span data-stu-id="f6125-222">string</span></span>|<span data-ttu-id="f6125-223">客户端的聊天消息的区域设置。</span><span class="sxs-lookup"><span data-stu-id="f6125-223">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f6125-224">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6125-224">JSON representation</span></span>

<span data-ttu-id="f6125-225">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6125-225">The following is a JSON representation of the resource.</span></span>

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
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
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
