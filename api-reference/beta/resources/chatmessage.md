---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 99e69bd51a661b67fd4cb325fffe80db91214714
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778668"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="37966-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="37966-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37966-105">表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="37966-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span>
<span data-ttu-id="37966-106">该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。</span><span class="sxs-lookup"><span data-stu-id="37966-106">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="37966-107">方法</span><span class="sxs-lookup"><span data-stu-id="37966-107">Methods</span></span>

| <span data-ttu-id="37966-108">方法</span><span class="sxs-lookup"><span data-stu-id="37966-108">Method</span></span>       | <span data-ttu-id="37966-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="37966-109">Return Type</span></span>  |<span data-ttu-id="37966-110">说明</span><span class="sxs-lookup"><span data-stu-id="37966-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="37966-111">列出渠道消息</span><span class="sxs-lookup"><span data-stu-id="37966-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="37966-112">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37966-112">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="37966-113">通道中的所有根邮件的列表。</span><span class="sxs-lookup"><span data-stu-id="37966-113">List of all root messages in a channel.</span></span>|
|[<span data-ttu-id="37966-114">获取渠道消息</span><span class="sxs-lookup"><span data-stu-id="37966-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="37966-115">chatMessage</span><span class="sxs-lookup"><span data-stu-id="37966-115">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="37966-116">获取渠道中的单个根消息。</span><span class="sxs-lookup"><span data-stu-id="37966-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="37966-117">列出消息回复</span><span class="sxs-lookup"><span data-stu-id="37966-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="37966-118">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37966-118">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="37966-119">频道中对邮件的所有回复的列表。</span><span class="sxs-lookup"><span data-stu-id="37966-119">List of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="37966-120">获取消息回复</span><span class="sxs-lookup"><span data-stu-id="37966-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="37966-121">chatMessage</span><span class="sxs-lookup"><span data-stu-id="37966-121">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="37966-122">获取渠道中的单个消息回复。</span><span class="sxs-lookup"><span data-stu-id="37966-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="37966-123">在频道中创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="37966-123">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="37966-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="37966-124">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="37966-125">在渠道中创建新的顶级消息。</span><span class="sxs-lookup"><span data-stu-id="37966-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="37966-126">在渠道中回复消息</span><span class="sxs-lookup"><span data-stu-id="37966-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="37966-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="37966-127">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="37966-128">在渠道中回复现有消息。</span><span class="sxs-lookup"><span data-stu-id="37966-128">Reply to an existing message in a channel.</span></span>|
|[<span data-ttu-id="37966-129">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="37966-129">List messages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="37966-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="37966-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="37966-131">列出1:1 或组聊天中的邮件。</span><span class="sxs-lookup"><span data-stu-id="37966-131">List messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="37966-132">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="37966-132">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="37966-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="37966-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="37966-134">获取聊天中的单个消息。</span><span class="sxs-lookup"><span data-stu-id="37966-134">Get a single message in a chat.</span></span> |
|[<span data-ttu-id="37966-135">列出所有托管图像</span><span class="sxs-lookup"><span data-stu-id="37966-135">List all hosted images</span></span>](../api/chatmessagehostedimage-list-hostedimages.md) | <span data-ttu-id="37966-136">[hostedImage](../resources/chatmessagehostedimage.md)集合</span><span class="sxs-lookup"><span data-stu-id="37966-136">[hostedImage](../resources/chatmessagehostedimage.md) collection</span></span>| <span data-ttu-id="37966-137">获取邮件中的所有托管图像。</span><span class="sxs-lookup"><span data-stu-id="37966-137">Get all hosted images in a message.</span></span>|
|[<span data-ttu-id="37966-138">获取托管图像</span><span class="sxs-lookup"><span data-stu-id="37966-138">Get hosted image</span></span>](../api/chatmessagehostedimage-get.md) | [<span data-ttu-id="37966-139">hostedImage</span><span class="sxs-lookup"><span data-stu-id="37966-139">hostedImage</span></span>](../resources/chatmessagehostedimage.md) | <span data-ttu-id="37966-140">从邮件中获取承载的图像。</span><span class="sxs-lookup"><span data-stu-id="37966-140">Get a hosted image from a message.</span></span>|
|[<span data-ttu-id="37966-141">获取承载的图像字节</span><span class="sxs-lookup"><span data-stu-id="37966-141">Get hosted image bytes</span></span>](../api/chatmessagehostedimage-getbytes.md) | <span data-ttu-id="37966-142">二进制图像数据</span><span class="sxs-lookup"><span data-stu-id="37966-142">binary image data</span></span> | <span data-ttu-id="37966-143">从邮件中获取托管图像的二进制图像数据。</span><span class="sxs-lookup"><span data-stu-id="37966-143">Get binary image data of a hosted image from a message.</span></span>|

## <a name="properties"></a><span data-ttu-id="37966-144">属性</span><span class="sxs-lookup"><span data-stu-id="37966-144">Properties</span></span>

| <span data-ttu-id="37966-145">属性</span><span class="sxs-lookup"><span data-stu-id="37966-145">Property</span></span>   | <span data-ttu-id="37966-146">类型</span><span class="sxs-lookup"><span data-stu-id="37966-146">Type</span></span> |<span data-ttu-id="37966-147">说明</span><span class="sxs-lookup"><span data-stu-id="37966-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37966-148">id</span><span class="sxs-lookup"><span data-stu-id="37966-148">id</span></span>|<span data-ttu-id="37966-149">String</span><span class="sxs-lookup"><span data-stu-id="37966-149">String</span></span>| <span data-ttu-id="37966-150">只读。</span><span class="sxs-lookup"><span data-stu-id="37966-150">Read-only.</span></span> <span data-ttu-id="37966-151">邮件的唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="37966-151">Unique Id of the message.</span></span>|
|<span data-ttu-id="37966-152">replyToId</span><span class="sxs-lookup"><span data-stu-id="37966-152">replyToId</span></span>| <span data-ttu-id="37966-153">string</span><span class="sxs-lookup"><span data-stu-id="37966-153">string</span></span> | <span data-ttu-id="37966-154">只读。</span><span class="sxs-lookup"><span data-stu-id="37966-154">Read-only.</span></span> <span data-ttu-id="37966-155">线程的父级消息/根消息的 Id。</span><span class="sxs-lookup"><span data-stu-id="37966-155">Id of the parent message/root message of the thread.</span></span> <span data-ttu-id="37966-156">（仅适用于频道中的消息，不适用于聊天）</span><span class="sxs-lookup"><span data-stu-id="37966-156">(Only applies to messages in channels not chats)</span></span> |
|<span data-ttu-id="37966-157">from</span><span class="sxs-lookup"><span data-stu-id="37966-157">from</span></span>|[<span data-ttu-id="37966-158">identitySet</span><span class="sxs-lookup"><span data-stu-id="37966-158">identitySet</span></span>](identityset.md)| <span data-ttu-id="37966-159">只读。</span><span class="sxs-lookup"><span data-stu-id="37966-159">Read only.</span></span> <span data-ttu-id="37966-160">消息发送者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="37966-160">Details of the sender of the message.</span></span>|
|<span data-ttu-id="37966-161">etag</span><span class="sxs-lookup"><span data-stu-id="37966-161">etag</span></span>| <span data-ttu-id="37966-162">string</span><span class="sxs-lookup"><span data-stu-id="37966-162">string</span></span> | <span data-ttu-id="37966-163">只读。</span><span class="sxs-lookup"><span data-stu-id="37966-163">Read-only.</span></span> <span data-ttu-id="37966-164">消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="37966-164">Version number of the message.</span></span> |
|<span data-ttu-id="37966-165">messageType</span><span class="sxs-lookup"><span data-stu-id="37966-165">messageType</span></span>|<span data-ttu-id="37966-166">chatMessageType</span><span class="sxs-lookup"><span data-stu-id="37966-166">chatMessageType</span></span>|<span data-ttu-id="37966-167">邮件类型。</span><span class="sxs-lookup"><span data-stu-id="37966-167">The type of message.</span></span> <span data-ttu-id="37966-168">可能的值是: `message`。</span><span class="sxs-lookup"><span data-stu-id="37966-168">The possible values are: `message`.</span></span>|
|<span data-ttu-id="37966-169">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37966-169">createdDateTime</span></span>|<span data-ttu-id="37966-170">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37966-170">dateTimeOffset</span></span>|<span data-ttu-id="37966-171">只读。</span><span class="sxs-lookup"><span data-stu-id="37966-171">Read only.</span></span> <span data-ttu-id="37966-172">创建消息时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="37966-172">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="37966-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37966-173">lastModifiedDateTime</span></span>|<span data-ttu-id="37966-174">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37966-174">dateTimeOffset</span></span>|<span data-ttu-id="37966-175">只读。</span><span class="sxs-lookup"><span data-stu-id="37966-175">Read only.</span></span> <span data-ttu-id="37966-176">创建或编辑邮件的时间戳, 包括在何时进行答复 (如果是通道中的根邮件) 或添加或删除反应。</span><span class="sxs-lookup"><span data-stu-id="37966-176">Timestamp of when the message is created or edited, including when a reply is made (if it's a root message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="37966-177">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="37966-177">deletedDateTime</span></span>|<span data-ttu-id="37966-178">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37966-178">dateTimeOffset</span></span>|<span data-ttu-id="37966-179">只读。</span><span class="sxs-lookup"><span data-stu-id="37966-179">Read only.</span></span> <span data-ttu-id="37966-180">删除消息时的时间戳，如果未删除则为 null。</span><span class="sxs-lookup"><span data-stu-id="37966-180">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="37966-181">subject</span><span class="sxs-lookup"><span data-stu-id="37966-181">subject</span></span>|<span data-ttu-id="37966-182">string</span><span class="sxs-lookup"><span data-stu-id="37966-182">string</span></span>| <span data-ttu-id="37966-183">消息的主题（纯文本）。</span><span class="sxs-lookup"><span data-stu-id="37966-183">The subject of the message, in plaintext.</span></span>|
|<span data-ttu-id="37966-184">正文</span><span class="sxs-lookup"><span data-stu-id="37966-184">body</span></span>|[<span data-ttu-id="37966-185">itemBody</span><span class="sxs-lookup"><span data-stu-id="37966-185">itemBody</span></span>](itembody.md)|<span data-ttu-id="37966-186">消息内容的纯文本/HTML 表示。</span><span class="sxs-lookup"><span data-stu-id="37966-186">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="37966-187">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="37966-187">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="37966-188">如果消息包含 [chatMessageMention](chatmessagemention.md)，则内容始终采用 HTML 格式。</span><span class="sxs-lookup"><span data-stu-id="37966-188">The content is always in HTML if the message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="37966-189">摘要</span><span class="sxs-lookup"><span data-stu-id="37966-189">summary</span></span>|<span data-ttu-id="37966-190">string</span><span class="sxs-lookup"><span data-stu-id="37966-190">string</span></span>| <span data-ttu-id="37966-191">可用于推送通知的消息摘要文本和摘要视图或回退视图。</span><span class="sxs-lookup"><span data-stu-id="37966-191">Summary text of the message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="37966-192">仅适用于频道消息，不适用于聊天消息。</span><span class="sxs-lookup"><span data-stu-id="37966-192">Only applies to channel messages, not chat messages.</span></span> |
|<span data-ttu-id="37966-193">附件</span><span class="sxs-lookup"><span data-stu-id="37966-193">attachments</span></span>|<span data-ttu-id="37966-194">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37966-194">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="37966-195">附加文件。</span><span class="sxs-lookup"><span data-stu-id="37966-195">Attached files.</span></span> <span data-ttu-id="37966-196">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="37966-196">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="37966-197">提及</span><span class="sxs-lookup"><span data-stu-id="37966-197">mentions</span></span>|<span data-ttu-id="37966-198">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37966-198">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="37966-199">消息中提到的实体列表。</span><span class="sxs-lookup"><span data-stu-id="37966-199">List of entities mentioned in the message.</span></span> <span data-ttu-id="37966-200">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="37966-200">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="37966-201">重要性</span><span class="sxs-lookup"><span data-stu-id="37966-201">importance</span></span>| <span data-ttu-id="37966-202">chatMessageImportance</span><span class="sxs-lookup"><span data-stu-id="37966-202">chatMessageImportance</span></span> | <span data-ttu-id="37966-203">邮件的重要性。</span><span class="sxs-lookup"><span data-stu-id="37966-203">The importance of the message.</span></span> <span data-ttu-id="37966-204">可能的值包括 `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="37966-204">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="37966-205">反应</span><span class="sxs-lookup"><span data-stu-id="37966-205">reactions</span></span>| <span data-ttu-id="37966-206">[chatMessageReaction](chatmessagereaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37966-206">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="37966-207">此消息的反应（例如点赞）。</span><span class="sxs-lookup"><span data-stu-id="37966-207">Reactions for this message (for example, Like).</span></span>|
|<span data-ttu-id="37966-208">区域设置</span><span class="sxs-lookup"><span data-stu-id="37966-208">locale</span></span>|<span data-ttu-id="37966-209">string</span><span class="sxs-lookup"><span data-stu-id="37966-209">string</span></span>|<span data-ttu-id="37966-210">客户端设置的消息区域设置。</span><span class="sxs-lookup"><span data-stu-id="37966-210">Locale of the message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37966-211">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37966-211">JSON representation</span></span>

<span data-ttu-id="37966-212">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37966-212">The following is a JSON representation of the resource.</span></span>

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
