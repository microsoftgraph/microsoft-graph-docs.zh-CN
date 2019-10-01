---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 聊天消息可以是一个根聊天消息，也可以是由聊天消息中的**replyToId**属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 0d11230402d95009e414c16962a2eb9b5dce1f58
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333363"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="50fef-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="50fef-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50fef-105">表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="50fef-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="50fef-106">聊天消息可以是一个根聊天消息，也可以是由聊天消息中的**replyToId**属性定义的答复线程的一部分。</span><span class="sxs-lookup"><span data-stu-id="50fef-106">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="50fef-107">方法</span><span class="sxs-lookup"><span data-stu-id="50fef-107">Methods</span></span>

| <span data-ttu-id="50fef-108">方法</span><span class="sxs-lookup"><span data-stu-id="50fef-108">Method</span></span>       | <span data-ttu-id="50fef-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="50fef-109">Return Type</span></span>  |<span data-ttu-id="50fef-110">说明</span><span class="sxs-lookup"><span data-stu-id="50fef-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="50fef-111">列出频道了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="50fef-111">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="50fef-112">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50fef-112">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="50fef-113">频道中所有根聊天邮件的列表。</span><span class="sxs-lookup"><span data-stu-id="50fef-113">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="50fef-114">在频道 delta 中获取 Chatmessages 集合</span><span class="sxs-lookup"><span data-stu-id="50fef-114">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="50fef-115">chatMessage</span><span class="sxs-lookup"><span data-stu-id="50fef-115">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="50fef-116">获取通道中的增量聊天消息。</span><span class="sxs-lookup"><span data-stu-id="50fef-116">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="50fef-117">获取频道了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="50fef-117">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="50fef-118">chatMessage</span><span class="sxs-lookup"><span data-stu-id="50fef-118">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="50fef-119">从频道中获取单个根聊天消息。</span><span class="sxs-lookup"><span data-stu-id="50fef-119">Get a single root chat message from a channel.</span></span>|
|[<span data-ttu-id="50fef-120">列出对了 chatmessage 的答复</span><span class="sxs-lookup"><span data-stu-id="50fef-120">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="50fef-121">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50fef-121">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="50fef-122">频道中对聊天消息的所有回复的列表。</span><span class="sxs-lookup"><span data-stu-id="50fef-122">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="50fef-123">获取对了 chatmessage 的答复</span><span class="sxs-lookup"><span data-stu-id="50fef-123">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="50fef-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="50fef-124">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="50fef-125">获取频道中的聊天消息的单个答复。</span><span class="sxs-lookup"><span data-stu-id="50fef-125">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="50fef-126">在频道中创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="50fef-126">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="50fef-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="50fef-127">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="50fef-128">在频道中创建新的顶级聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="50fef-128">Create a new top-level chat message in a channel.</span></span>|
|[<span data-ttu-id="50fef-129">答复频道中的了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="50fef-129">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="50fef-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="50fef-130">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="50fef-131">在频道中答复现有聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="50fef-131">Reply to an existing chat message in a channel.</span></span>|
|[<span data-ttu-id="50fef-132">在聊天中创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="50fef-132">Create chatMessage in a chat</span></span>](../api/chat-post-messages.md) | [<span data-ttu-id="50fef-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="50fef-133">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="50fef-134">在现有的1:1 或组聊天对话中发送聊天消息。</span><span class="sxs-lookup"><span data-stu-id="50fef-134">Send a chat message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="50fef-135">在聊天中列出 Chatmessages 集合</span><span class="sxs-lookup"><span data-stu-id="50fef-135">List chatMessages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="50fef-136">chatMessage</span><span class="sxs-lookup"><span data-stu-id="50fef-136">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="50fef-137">列出1:1 或组聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="50fef-137">List chat messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="50fef-138">在聊天中获取了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="50fef-138">Get chatMessage in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="50fef-139">chatMessage</span><span class="sxs-lookup"><span data-stu-id="50fef-139">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="50fef-140">在聊天中获取单个聊天消息。</span><span class="sxs-lookup"><span data-stu-id="50fef-140">Get a single chat message in a chat.</span></span> |
|[<span data-ttu-id="50fef-141">列出所有已承载的内容</span><span class="sxs-lookup"><span data-stu-id="50fef-141">List all hosted content</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | <span data-ttu-id="50fef-142">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)集合</span><span class="sxs-lookup"><span data-stu-id="50fef-142">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection</span></span>| <span data-ttu-id="50fef-143">获取聊天消息中的所有托管内容。</span><span class="sxs-lookup"><span data-stu-id="50fef-143">Get all hosted content in a chat message.</span></span>|
|[<span data-ttu-id="50fef-144">获取托管内容</span><span class="sxs-lookup"><span data-stu-id="50fef-144">Get hosted content</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="50fef-145">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="50fef-145">chatMessageHostedContent</span></span>](../resources/chatmessagehostedcontent.md) | <span data-ttu-id="50fef-146">从聊天消息中获取托管的内容。</span><span class="sxs-lookup"><span data-stu-id="50fef-146">Get hosted content from a chat message.</span></span>|

## <a name="properties"></a><span data-ttu-id="50fef-147">属性</span><span class="sxs-lookup"><span data-stu-id="50fef-147">Properties</span></span>

| <span data-ttu-id="50fef-148">属性</span><span class="sxs-lookup"><span data-stu-id="50fef-148">Property</span></span>   | <span data-ttu-id="50fef-149">类型</span><span class="sxs-lookup"><span data-stu-id="50fef-149">Type</span></span> |<span data-ttu-id="50fef-150">说明</span><span class="sxs-lookup"><span data-stu-id="50fef-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50fef-151">id</span><span class="sxs-lookup"><span data-stu-id="50fef-151">id</span></span>|<span data-ttu-id="50fef-152">String</span><span class="sxs-lookup"><span data-stu-id="50fef-152">String</span></span>| <span data-ttu-id="50fef-153">只读。</span><span class="sxs-lookup"><span data-stu-id="50fef-153">Read-only.</span></span> <span data-ttu-id="50fef-154">邮件的唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="50fef-154">Unique Id of the message.</span></span>|
|<span data-ttu-id="50fef-155">replyToId</span><span class="sxs-lookup"><span data-stu-id="50fef-155">replyToId</span></span>| <span data-ttu-id="50fef-156">string</span><span class="sxs-lookup"><span data-stu-id="50fef-156">string</span></span> | <span data-ttu-id="50fef-157">只读。</span><span class="sxs-lookup"><span data-stu-id="50fef-157">Read-only.</span></span> <span data-ttu-id="50fef-158">线程的父聊天消息或根聊天消息的 Id。</span><span class="sxs-lookup"><span data-stu-id="50fef-158">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="50fef-159">（仅适用于通道中不聊天的聊天邮件）</span><span class="sxs-lookup"><span data-stu-id="50fef-159">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="50fef-160">from</span><span class="sxs-lookup"><span data-stu-id="50fef-160">from</span></span>|[<span data-ttu-id="50fef-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="50fef-161">identitySet</span></span>](identityset.md)| <span data-ttu-id="50fef-162">只读。</span><span class="sxs-lookup"><span data-stu-id="50fef-162">Read only.</span></span> <span data-ttu-id="50fef-163">聊天消息发件人的详细信息。</span><span class="sxs-lookup"><span data-stu-id="50fef-163">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="50fef-164">etag</span><span class="sxs-lookup"><span data-stu-id="50fef-164">etag</span></span>| <span data-ttu-id="50fef-165">string</span><span class="sxs-lookup"><span data-stu-id="50fef-165">string</span></span> | <span data-ttu-id="50fef-166">只读。</span><span class="sxs-lookup"><span data-stu-id="50fef-166">Read-only.</span></span> <span data-ttu-id="50fef-167">聊天消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="50fef-167">Version number of the chat message.</span></span> |
|<span data-ttu-id="50fef-168">messageType</span><span class="sxs-lookup"><span data-stu-id="50fef-168">messageType</span></span>|<span data-ttu-id="50fef-169">chatMessageType</span><span class="sxs-lookup"><span data-stu-id="50fef-169">chatMessageType</span></span>|<span data-ttu-id="50fef-170">聊天消息的类型。</span><span class="sxs-lookup"><span data-stu-id="50fef-170">The type of chat message.</span></span> <span data-ttu-id="50fef-171">可能的值是： `message`。</span><span class="sxs-lookup"><span data-stu-id="50fef-171">The possible values are: `message`.</span></span>|
|<span data-ttu-id="50fef-172">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50fef-172">createdDateTime</span></span>|<span data-ttu-id="50fef-173">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50fef-173">dateTimeOffset</span></span>|<span data-ttu-id="50fef-174">只读。</span><span class="sxs-lookup"><span data-stu-id="50fef-174">Read only.</span></span> <span data-ttu-id="50fef-175">在聊天消息创建时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="50fef-175">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="50fef-176">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50fef-176">lastModifiedDateTime</span></span>|<span data-ttu-id="50fef-177">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50fef-177">dateTimeOffset</span></span>|<span data-ttu-id="50fef-178">只读。</span><span class="sxs-lookup"><span data-stu-id="50fef-178">Read only.</span></span> <span data-ttu-id="50fef-179">在创建或编辑聊天消息时的时间戳，包括答复的时间（如果是频道中的根聊天邮件）或添加或删除了反应。</span><span class="sxs-lookup"><span data-stu-id="50fef-179">Timestamp of when the chat message is created or edited, including when a reply is made (if it's a root chat message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="50fef-180">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="50fef-180">deletedDateTime</span></span>|<span data-ttu-id="50fef-181">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50fef-181">dateTimeOffset</span></span>|<span data-ttu-id="50fef-182">只读。</span><span class="sxs-lookup"><span data-stu-id="50fef-182">Read only.</span></span> <span data-ttu-id="50fef-183">删除聊天邮件的时间戳，如果未删除，则为 null。</span><span class="sxs-lookup"><span data-stu-id="50fef-183">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="50fef-184">subject</span><span class="sxs-lookup"><span data-stu-id="50fef-184">subject</span></span>|<span data-ttu-id="50fef-185">string</span><span class="sxs-lookup"><span data-stu-id="50fef-185">string</span></span>| <span data-ttu-id="50fef-186">聊天消息的主题，以纯文本形式。</span><span class="sxs-lookup"><span data-stu-id="50fef-186">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="50fef-187">body</span><span class="sxs-lookup"><span data-stu-id="50fef-187">body</span></span>|[<span data-ttu-id="50fef-188">itemBody</span><span class="sxs-lookup"><span data-stu-id="50fef-188">itemBody</span></span>](itembody.md)|<span data-ttu-id="50fef-189">聊天消息内容的纯文本/HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50fef-189">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="50fef-190">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="50fef-190">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="50fef-191">如果聊天消息包含[chatMessageMention](chatmessagemention.md)，则该内容始终为 HTML。</span><span class="sxs-lookup"><span data-stu-id="50fef-191">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="50fef-192">摘要</span><span class="sxs-lookup"><span data-stu-id="50fef-192">summary</span></span>|<span data-ttu-id="50fef-193">string</span><span class="sxs-lookup"><span data-stu-id="50fef-193">string</span></span>| <span data-ttu-id="50fef-194">可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。</span><span class="sxs-lookup"><span data-stu-id="50fef-194">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="50fef-195">仅适用于频道聊天消息，而不是聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="50fef-195">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="50fef-196">附件</span><span class="sxs-lookup"><span data-stu-id="50fef-196">attachments</span></span>|<span data-ttu-id="50fef-197">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50fef-197">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="50fef-198">附加文件。</span><span class="sxs-lookup"><span data-stu-id="50fef-198">Attached files.</span></span> <span data-ttu-id="50fef-199">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="50fef-199">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="50fef-200">提及</span><span class="sxs-lookup"><span data-stu-id="50fef-200">mentions</span></span>|<span data-ttu-id="50fef-201">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50fef-201">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="50fef-202">聊天消息中提及的实体列表。</span><span class="sxs-lookup"><span data-stu-id="50fef-202">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="50fef-203">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="50fef-203">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="50fef-204">重要性</span><span class="sxs-lookup"><span data-stu-id="50fef-204">importance</span></span>| <span data-ttu-id="50fef-205">chatMessageImportance</span><span class="sxs-lookup"><span data-stu-id="50fef-205">chatMessageImportance</span></span> | <span data-ttu-id="50fef-206">聊天消息的重要性。</span><span class="sxs-lookup"><span data-stu-id="50fef-206">The importance of the chat message.</span></span> <span data-ttu-id="50fef-207">可能的值包括 `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="50fef-207">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="50fef-208">反应</span><span class="sxs-lookup"><span data-stu-id="50fef-208">reactions</span></span>| <span data-ttu-id="50fef-209">[chatMessageReaction](chatmessagereaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50fef-209">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="50fef-210">此聊天消息的反应（例如，如）。</span><span class="sxs-lookup"><span data-stu-id="50fef-210">Reactions for this chat message (for example, Like).</span></span>|
|<span data-ttu-id="50fef-211">区域设置</span><span class="sxs-lookup"><span data-stu-id="50fef-211">locale</span></span>|<span data-ttu-id="50fef-212">string</span><span class="sxs-lookup"><span data-stu-id="50fef-212">string</span></span>|<span data-ttu-id="50fef-213">客户端的聊天消息的区域设置。</span><span class="sxs-lookup"><span data-stu-id="50fef-213">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50fef-214">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50fef-214">JSON representation</span></span>

<span data-ttu-id="50fef-215">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50fef-215">The following is a JSON representation of the resource.</span></span>

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
