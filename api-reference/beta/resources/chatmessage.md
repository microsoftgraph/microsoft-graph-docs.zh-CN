---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 聊天消息可以是一个根聊天消息, 也可以是由聊天消息中的**replyToId**属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: a29afea30f0ea1d75f5c7ce1a0713976f10cc298
ms.sourcegitcommit: cca4f96414aededa03bb45e07e19bb20b7327563
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2019
ms.locfileid: "36677118"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="cd68e-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd68e-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd68e-105">表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="cd68e-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="cd68e-106">聊天消息可以是一个根聊天消息, 也可以是由聊天消息中的**replyToId**属性定义的答复线程的一部分。</span><span class="sxs-lookup"><span data-stu-id="cd68e-106">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="cd68e-107">方法</span><span class="sxs-lookup"><span data-stu-id="cd68e-107">Methods</span></span>

| <span data-ttu-id="cd68e-108">方法</span><span class="sxs-lookup"><span data-stu-id="cd68e-108">Method</span></span>       | <span data-ttu-id="cd68e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="cd68e-109">Return Type</span></span>  |<span data-ttu-id="cd68e-110">说明</span><span class="sxs-lookup"><span data-stu-id="cd68e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cd68e-111">列出频道了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="cd68e-111">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="cd68e-112">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd68e-112">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="cd68e-113">频道中所有根聊天邮件的列表。</span><span class="sxs-lookup"><span data-stu-id="cd68e-113">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="cd68e-114">在频道 delta 中获取 Chatmessages 集合</span><span class="sxs-lookup"><span data-stu-id="cd68e-114">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="cd68e-115">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cd68e-115">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="cd68e-116">获取通道中的增量聊天消息。</span><span class="sxs-lookup"><span data-stu-id="cd68e-116">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="cd68e-117">获取频道了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="cd68e-117">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="cd68e-118">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cd68e-118">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="cd68e-119">从频道中获取单个根聊天消息。</span><span class="sxs-lookup"><span data-stu-id="cd68e-119">Get a single root chat message from a channel.</span></span>|
|[<span data-ttu-id="cd68e-120">列出对了 chatmessage 的答复</span><span class="sxs-lookup"><span data-stu-id="cd68e-120">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="cd68e-121">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd68e-121">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="cd68e-122">频道中对聊天消息的所有回复的列表。</span><span class="sxs-lookup"><span data-stu-id="cd68e-122">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="cd68e-123">获取对了 chatmessage 的答复</span><span class="sxs-lookup"><span data-stu-id="cd68e-123">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="cd68e-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cd68e-124">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="cd68e-125">获取频道中的聊天消息的单个答复。</span><span class="sxs-lookup"><span data-stu-id="cd68e-125">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="cd68e-126">在频道中创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="cd68e-126">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="cd68e-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cd68e-127">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="cd68e-128">在频道中创建新的顶级聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="cd68e-128">Create a new top-level chat message in a channel.</span></span>|
|[<span data-ttu-id="cd68e-129">答复频道中的了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="cd68e-129">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="cd68e-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cd68e-130">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="cd68e-131">在频道中答复现有聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="cd68e-131">Reply to an existing chat message in a channel.</span></span>|
|[<span data-ttu-id="cd68e-132">在聊天中创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="cd68e-132">Create chatMessage in a chat</span></span>](../api/chat-post-messages.md) | [<span data-ttu-id="cd68e-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cd68e-133">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="cd68e-134">在现有的1:1 或组聊天对话中发送聊天消息。</span><span class="sxs-lookup"><span data-stu-id="cd68e-134">Send a chat message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="cd68e-135">在聊天中列出 Chatmessages 集合</span><span class="sxs-lookup"><span data-stu-id="cd68e-135">List chatMessages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="cd68e-136">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cd68e-136">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="cd68e-137">列出1:1 或组聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="cd68e-137">List chat messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="cd68e-138">在聊天中获取了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="cd68e-138">Get chatMessage in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="cd68e-139">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cd68e-139">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="cd68e-140">在聊天中获取单个聊天消息。</span><span class="sxs-lookup"><span data-stu-id="cd68e-140">Get a single chat message in a chat.</span></span> |
|[<span data-ttu-id="cd68e-141">列出所有托管图像</span><span class="sxs-lookup"><span data-stu-id="cd68e-141">List all hosted images</span></span>](../api/chatmessagehostedimage-list-hostedimages.md) | <span data-ttu-id="cd68e-142">[hostedImage](../resources/chatmessagehostedimage.md)集合</span><span class="sxs-lookup"><span data-stu-id="cd68e-142">[hostedImage](../resources/chatmessagehostedimage.md) collection</span></span>| <span data-ttu-id="cd68e-143">获取聊天消息中的所有托管图像。</span><span class="sxs-lookup"><span data-stu-id="cd68e-143">Get all hosted images in a chat message.</span></span>|
|[<span data-ttu-id="cd68e-144">获取托管图像</span><span class="sxs-lookup"><span data-stu-id="cd68e-144">Get hosted image</span></span>](../api/chatmessagehostedimage-get.md) | [<span data-ttu-id="cd68e-145">hostedImage</span><span class="sxs-lookup"><span data-stu-id="cd68e-145">hostedImage</span></span>](../resources/chatmessagehostedimage.md) | <span data-ttu-id="cd68e-146">从聊天消息中获取托管的图像。</span><span class="sxs-lookup"><span data-stu-id="cd68e-146">Get a hosted image from a chat message.</span></span>|
|[<span data-ttu-id="cd68e-147">获取承载的图像字节</span><span class="sxs-lookup"><span data-stu-id="cd68e-147">Get hosted image bytes</span></span>](../api/chatmessagehostedimage-getbytes.md) | <span data-ttu-id="cd68e-148">二进制图像数据</span><span class="sxs-lookup"><span data-stu-id="cd68e-148">binary image data</span></span> | <span data-ttu-id="cd68e-149">从聊天消息中获取托管图像的二进制图像数据。</span><span class="sxs-lookup"><span data-stu-id="cd68e-149">Get binary image data of a hosted image from a chat message.</span></span>|

## <a name="properties"></a><span data-ttu-id="cd68e-150">属性</span><span class="sxs-lookup"><span data-stu-id="cd68e-150">Properties</span></span>

| <span data-ttu-id="cd68e-151">属性</span><span class="sxs-lookup"><span data-stu-id="cd68e-151">Property</span></span>   | <span data-ttu-id="cd68e-152">类型</span><span class="sxs-lookup"><span data-stu-id="cd68e-152">Type</span></span> |<span data-ttu-id="cd68e-153">说明</span><span class="sxs-lookup"><span data-stu-id="cd68e-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd68e-154">id</span><span class="sxs-lookup"><span data-stu-id="cd68e-154">id</span></span>|<span data-ttu-id="cd68e-155">String</span><span class="sxs-lookup"><span data-stu-id="cd68e-155">String</span></span>| <span data-ttu-id="cd68e-156">只读。</span><span class="sxs-lookup"><span data-stu-id="cd68e-156">Read-only.</span></span> <span data-ttu-id="cd68e-157">邮件的唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="cd68e-157">Unique Id of the message.</span></span>|
|<span data-ttu-id="cd68e-158">replyToId</span><span class="sxs-lookup"><span data-stu-id="cd68e-158">replyToId</span></span>| <span data-ttu-id="cd68e-159">string</span><span class="sxs-lookup"><span data-stu-id="cd68e-159">string</span></span> | <span data-ttu-id="cd68e-160">只读。</span><span class="sxs-lookup"><span data-stu-id="cd68e-160">Read-only.</span></span> <span data-ttu-id="cd68e-161">线程的父聊天消息或根聊天消息的 Id。</span><span class="sxs-lookup"><span data-stu-id="cd68e-161">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="cd68e-162">(仅适用于通道中不聊天的聊天邮件)</span><span class="sxs-lookup"><span data-stu-id="cd68e-162">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="cd68e-163">from</span><span class="sxs-lookup"><span data-stu-id="cd68e-163">from</span></span>|[<span data-ttu-id="cd68e-164">identitySet</span><span class="sxs-lookup"><span data-stu-id="cd68e-164">identitySet</span></span>](identityset.md)| <span data-ttu-id="cd68e-165">只读。</span><span class="sxs-lookup"><span data-stu-id="cd68e-165">Read only.</span></span> <span data-ttu-id="cd68e-166">聊天消息发件人的详细信息。</span><span class="sxs-lookup"><span data-stu-id="cd68e-166">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="cd68e-167">etag</span><span class="sxs-lookup"><span data-stu-id="cd68e-167">etag</span></span>| <span data-ttu-id="cd68e-168">string</span><span class="sxs-lookup"><span data-stu-id="cd68e-168">string</span></span> | <span data-ttu-id="cd68e-169">只读。</span><span class="sxs-lookup"><span data-stu-id="cd68e-169">Read-only.</span></span> <span data-ttu-id="cd68e-170">聊天消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="cd68e-170">Version number of the chat message.</span></span> |
|<span data-ttu-id="cd68e-171">messageType</span><span class="sxs-lookup"><span data-stu-id="cd68e-171">messageType</span></span>|<span data-ttu-id="cd68e-172">chatMessageType</span><span class="sxs-lookup"><span data-stu-id="cd68e-172">chatMessageType</span></span>|<span data-ttu-id="cd68e-173">聊天消息的类型。</span><span class="sxs-lookup"><span data-stu-id="cd68e-173">The type of chat message.</span></span> <span data-ttu-id="cd68e-174">可能的值是: `message`。</span><span class="sxs-lookup"><span data-stu-id="cd68e-174">The possible values are: `message`.</span></span>|
|<span data-ttu-id="cd68e-175">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd68e-175">createdDateTime</span></span>|<span data-ttu-id="cd68e-176">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd68e-176">dateTimeOffset</span></span>|<span data-ttu-id="cd68e-177">只读。</span><span class="sxs-lookup"><span data-stu-id="cd68e-177">Read only.</span></span> <span data-ttu-id="cd68e-178">在聊天消息创建时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="cd68e-178">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="cd68e-179">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd68e-179">lastModifiedDateTime</span></span>|<span data-ttu-id="cd68e-180">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd68e-180">dateTimeOffset</span></span>|<span data-ttu-id="cd68e-181">只读。</span><span class="sxs-lookup"><span data-stu-id="cd68e-181">Read only.</span></span> <span data-ttu-id="cd68e-182">在创建或编辑聊天消息时的时间戳, 包括答复的时间 (如果是频道中的根聊天邮件) 或添加或删除了反应。</span><span class="sxs-lookup"><span data-stu-id="cd68e-182">Timestamp of when the chat message is created or edited, including when a reply is made (if it's a root chat message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="cd68e-183">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd68e-183">deletedDateTime</span></span>|<span data-ttu-id="cd68e-184">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd68e-184">dateTimeOffset</span></span>|<span data-ttu-id="cd68e-185">只读。</span><span class="sxs-lookup"><span data-stu-id="cd68e-185">Read only.</span></span> <span data-ttu-id="cd68e-186">删除聊天邮件的时间戳, 如果未删除, 则为 null。</span><span class="sxs-lookup"><span data-stu-id="cd68e-186">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="cd68e-187">subject</span><span class="sxs-lookup"><span data-stu-id="cd68e-187">subject</span></span>|<span data-ttu-id="cd68e-188">string</span><span class="sxs-lookup"><span data-stu-id="cd68e-188">string</span></span>| <span data-ttu-id="cd68e-189">聊天消息的主题, 以纯文本形式。</span><span class="sxs-lookup"><span data-stu-id="cd68e-189">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="cd68e-190">body</span><span class="sxs-lookup"><span data-stu-id="cd68e-190">body</span></span>|[<span data-ttu-id="cd68e-191">itemBody</span><span class="sxs-lookup"><span data-stu-id="cd68e-191">itemBody</span></span>](itembody.md)|<span data-ttu-id="cd68e-192">聊天消息内容的纯文本/HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd68e-192">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="cd68e-193">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="cd68e-193">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="cd68e-194">如果聊天消息包含[chatMessageMention](chatmessagemention.md), 则该内容始终为 HTML。</span><span class="sxs-lookup"><span data-stu-id="cd68e-194">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="cd68e-195">摘要</span><span class="sxs-lookup"><span data-stu-id="cd68e-195">summary</span></span>|<span data-ttu-id="cd68e-196">string</span><span class="sxs-lookup"><span data-stu-id="cd68e-196">string</span></span>| <span data-ttu-id="cd68e-197">可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。</span><span class="sxs-lookup"><span data-stu-id="cd68e-197">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="cd68e-198">仅适用于频道聊天消息, 而不是聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="cd68e-198">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="cd68e-199">附件</span><span class="sxs-lookup"><span data-stu-id="cd68e-199">attachments</span></span>|<span data-ttu-id="cd68e-200">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd68e-200">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="cd68e-201">附加文件。</span><span class="sxs-lookup"><span data-stu-id="cd68e-201">Attached files.</span></span> <span data-ttu-id="cd68e-202">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="cd68e-202">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="cd68e-203">提及</span><span class="sxs-lookup"><span data-stu-id="cd68e-203">mentions</span></span>|<span data-ttu-id="cd68e-204">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd68e-204">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="cd68e-205">聊天消息中提及的实体列表。</span><span class="sxs-lookup"><span data-stu-id="cd68e-205">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="cd68e-206">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="cd68e-206">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="cd68e-207">重要性</span><span class="sxs-lookup"><span data-stu-id="cd68e-207">importance</span></span>| <span data-ttu-id="cd68e-208">chatMessageImportance</span><span class="sxs-lookup"><span data-stu-id="cd68e-208">chatMessageImportance</span></span> | <span data-ttu-id="cd68e-209">聊天消息的重要性。</span><span class="sxs-lookup"><span data-stu-id="cd68e-209">The importance of the chat message.</span></span> <span data-ttu-id="cd68e-210">可能的值包括 `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="cd68e-210">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="cd68e-211">反应</span><span class="sxs-lookup"><span data-stu-id="cd68e-211">reactions</span></span>| <span data-ttu-id="cd68e-212">[chatMessageReaction](chatmessagereaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd68e-212">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="cd68e-213">此聊天消息的反应 (例如, 如)。</span><span class="sxs-lookup"><span data-stu-id="cd68e-213">Reactions for this chat message (for example, Like).</span></span>|
|<span data-ttu-id="cd68e-214">区域设置</span><span class="sxs-lookup"><span data-stu-id="cd68e-214">locale</span></span>|<span data-ttu-id="cd68e-215">string</span><span class="sxs-lookup"><span data-stu-id="cd68e-215">string</span></span>|<span data-ttu-id="cd68e-216">客户端的聊天消息的区域设置。</span><span class="sxs-lookup"><span data-stu-id="cd68e-216">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd68e-217">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd68e-217">JSON representation</span></span>

<span data-ttu-id="cd68e-218">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd68e-218">The following is a JSON representation of the resource.</span></span>

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
