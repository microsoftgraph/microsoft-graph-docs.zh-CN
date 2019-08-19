---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 17b6912312c66bca8b84ccce9d25ac3c83a2edf9
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36460764"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="ac490-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="ac490-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac490-105">表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="ac490-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span>
<span data-ttu-id="ac490-106">该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。</span><span class="sxs-lookup"><span data-stu-id="ac490-106">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="ac490-107">方法</span><span class="sxs-lookup"><span data-stu-id="ac490-107">Methods</span></span>

| <span data-ttu-id="ac490-108">方法</span><span class="sxs-lookup"><span data-stu-id="ac490-108">Method</span></span>       | <span data-ttu-id="ac490-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ac490-109">Return Type</span></span>  |<span data-ttu-id="ac490-110">说明</span><span class="sxs-lookup"><span data-stu-id="ac490-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ac490-111">列出渠道消息</span><span class="sxs-lookup"><span data-stu-id="ac490-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="ac490-112">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ac490-112">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="ac490-113">通道中的所有根邮件的列表。</span><span class="sxs-lookup"><span data-stu-id="ac490-113">List of all root messages in a channel.</span></span>|
|[<span data-ttu-id="ac490-114">获取渠道消息</span><span class="sxs-lookup"><span data-stu-id="ac490-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="ac490-115">chatMessage</span><span class="sxs-lookup"><span data-stu-id="ac490-115">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="ac490-116">获取渠道中的单个根消息。</span><span class="sxs-lookup"><span data-stu-id="ac490-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="ac490-117">列出消息回复</span><span class="sxs-lookup"><span data-stu-id="ac490-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="ac490-118">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ac490-118">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="ac490-119">频道中对邮件的所有回复的列表。</span><span class="sxs-lookup"><span data-stu-id="ac490-119">List of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="ac490-120">获取消息回复</span><span class="sxs-lookup"><span data-stu-id="ac490-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="ac490-121">chatMessage</span><span class="sxs-lookup"><span data-stu-id="ac490-121">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="ac490-122">获取渠道中的单个消息回复。</span><span class="sxs-lookup"><span data-stu-id="ac490-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="ac490-123">在频道中创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="ac490-123">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="ac490-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="ac490-124">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="ac490-125">在渠道中创建新的顶级消息。</span><span class="sxs-lookup"><span data-stu-id="ac490-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="ac490-126">在渠道中回复消息</span><span class="sxs-lookup"><span data-stu-id="ac490-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="ac490-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="ac490-127">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="ac490-128">在渠道中回复现有消息。</span><span class="sxs-lookup"><span data-stu-id="ac490-128">Reply to an existing message in a channel.</span></span>|
|[<span data-ttu-id="ac490-129">在聊天中创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="ac490-129">Create chatMessage in a chat</span></span>](../api/chat-post-messages.md) | [<span data-ttu-id="ac490-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="ac490-130">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="ac490-131">在现有的1:1 或组聊天对话中发送邮件。</span><span class="sxs-lookup"><span data-stu-id="ac490-131">Send a message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="ac490-132">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="ac490-132">List messages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="ac490-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="ac490-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="ac490-134">列出1:1 或组聊天中的邮件。</span><span class="sxs-lookup"><span data-stu-id="ac490-134">List messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="ac490-135">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="ac490-135">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="ac490-136">chatMessage</span><span class="sxs-lookup"><span data-stu-id="ac490-136">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="ac490-137">获取聊天中的单个消息。</span><span class="sxs-lookup"><span data-stu-id="ac490-137">Get a single message in a chat.</span></span> |
|[<span data-ttu-id="ac490-138">列出所有托管图像</span><span class="sxs-lookup"><span data-stu-id="ac490-138">List all hosted images</span></span>](../api/chatmessagehostedimage-list-hostedimages.md) | <span data-ttu-id="ac490-139">[hostedImage](../resources/chatmessagehostedimage.md)集合</span><span class="sxs-lookup"><span data-stu-id="ac490-139">[hostedImage](../resources/chatmessagehostedimage.md) collection</span></span>| <span data-ttu-id="ac490-140">获取邮件中的所有托管图像。</span><span class="sxs-lookup"><span data-stu-id="ac490-140">Get all hosted images in a message.</span></span>|
|[<span data-ttu-id="ac490-141">获取托管图像</span><span class="sxs-lookup"><span data-stu-id="ac490-141">Get hosted image</span></span>](../api/chatmessagehostedimage-get.md) | [<span data-ttu-id="ac490-142">hostedImage</span><span class="sxs-lookup"><span data-stu-id="ac490-142">hostedImage</span></span>](../resources/chatmessagehostedimage.md) | <span data-ttu-id="ac490-143">从邮件中获取承载的图像。</span><span class="sxs-lookup"><span data-stu-id="ac490-143">Get a hosted image from a message.</span></span>|
|[<span data-ttu-id="ac490-144">获取承载的图像字节</span><span class="sxs-lookup"><span data-stu-id="ac490-144">Get hosted image bytes</span></span>](../api/chatmessagehostedimage-getbytes.md) | <span data-ttu-id="ac490-145">二进制图像数据</span><span class="sxs-lookup"><span data-stu-id="ac490-145">binary image data</span></span> | <span data-ttu-id="ac490-146">从邮件中获取托管图像的二进制图像数据。</span><span class="sxs-lookup"><span data-stu-id="ac490-146">Get binary image data of a hosted image from a message.</span></span>|

## <a name="properties"></a><span data-ttu-id="ac490-147">属性</span><span class="sxs-lookup"><span data-stu-id="ac490-147">Properties</span></span>

| <span data-ttu-id="ac490-148">属性</span><span class="sxs-lookup"><span data-stu-id="ac490-148">Property</span></span>   | <span data-ttu-id="ac490-149">类型</span><span class="sxs-lookup"><span data-stu-id="ac490-149">Type</span></span> |<span data-ttu-id="ac490-150">说明</span><span class="sxs-lookup"><span data-stu-id="ac490-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac490-151">id</span><span class="sxs-lookup"><span data-stu-id="ac490-151">id</span></span>|<span data-ttu-id="ac490-152">String</span><span class="sxs-lookup"><span data-stu-id="ac490-152">String</span></span>| <span data-ttu-id="ac490-153">只读。</span><span class="sxs-lookup"><span data-stu-id="ac490-153">Read-only.</span></span> <span data-ttu-id="ac490-154">邮件的唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="ac490-154">Unique Id of the message.</span></span>|
|<span data-ttu-id="ac490-155">replyToId</span><span class="sxs-lookup"><span data-stu-id="ac490-155">replyToId</span></span>| <span data-ttu-id="ac490-156">string</span><span class="sxs-lookup"><span data-stu-id="ac490-156">string</span></span> | <span data-ttu-id="ac490-157">只读。</span><span class="sxs-lookup"><span data-stu-id="ac490-157">Read-only.</span></span> <span data-ttu-id="ac490-158">线程的父级消息/根消息的 Id。</span><span class="sxs-lookup"><span data-stu-id="ac490-158">Id of the parent message/root message of the thread.</span></span> <span data-ttu-id="ac490-159">（仅适用于频道中的消息，不适用于聊天）</span><span class="sxs-lookup"><span data-stu-id="ac490-159">(Only applies to messages in channels not chats)</span></span> |
|<span data-ttu-id="ac490-160">from</span><span class="sxs-lookup"><span data-stu-id="ac490-160">from</span></span>|[<span data-ttu-id="ac490-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="ac490-161">identitySet</span></span>](identityset.md)| <span data-ttu-id="ac490-162">只读。</span><span class="sxs-lookup"><span data-stu-id="ac490-162">Read only.</span></span> <span data-ttu-id="ac490-163">消息发送者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ac490-163">Details of the sender of the message.</span></span>|
|<span data-ttu-id="ac490-164">etag</span><span class="sxs-lookup"><span data-stu-id="ac490-164">etag</span></span>| <span data-ttu-id="ac490-165">string</span><span class="sxs-lookup"><span data-stu-id="ac490-165">string</span></span> | <span data-ttu-id="ac490-166">只读。</span><span class="sxs-lookup"><span data-stu-id="ac490-166">Read-only.</span></span> <span data-ttu-id="ac490-167">消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="ac490-167">Version number of the message.</span></span> |
|<span data-ttu-id="ac490-168">messageType</span><span class="sxs-lookup"><span data-stu-id="ac490-168">messageType</span></span>|<span data-ttu-id="ac490-169">chatMessageType</span><span class="sxs-lookup"><span data-stu-id="ac490-169">chatMessageType</span></span>|<span data-ttu-id="ac490-170">邮件类型。</span><span class="sxs-lookup"><span data-stu-id="ac490-170">The type of message.</span></span> <span data-ttu-id="ac490-171">可能的值是: `message`。</span><span class="sxs-lookup"><span data-stu-id="ac490-171">The possible values are: `message`.</span></span>|
|<span data-ttu-id="ac490-172">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac490-172">createdDateTime</span></span>|<span data-ttu-id="ac490-173">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac490-173">dateTimeOffset</span></span>|<span data-ttu-id="ac490-174">只读。</span><span class="sxs-lookup"><span data-stu-id="ac490-174">Read only.</span></span> <span data-ttu-id="ac490-175">创建消息时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="ac490-175">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="ac490-176">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac490-176">lastModifiedDateTime</span></span>|<span data-ttu-id="ac490-177">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac490-177">dateTimeOffset</span></span>|<span data-ttu-id="ac490-178">只读。</span><span class="sxs-lookup"><span data-stu-id="ac490-178">Read only.</span></span> <span data-ttu-id="ac490-179">创建或编辑邮件的时间戳, 包括在何时进行答复 (如果是通道中的根邮件) 或添加或删除反应。</span><span class="sxs-lookup"><span data-stu-id="ac490-179">Timestamp of when the message is created or edited, including when a reply is made (if it's a root message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="ac490-180">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac490-180">deletedDateTime</span></span>|<span data-ttu-id="ac490-181">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac490-181">dateTimeOffset</span></span>|<span data-ttu-id="ac490-182">只读。</span><span class="sxs-lookup"><span data-stu-id="ac490-182">Read only.</span></span> <span data-ttu-id="ac490-183">删除消息时的时间戳，如果未删除则为 null。</span><span class="sxs-lookup"><span data-stu-id="ac490-183">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="ac490-184">subject</span><span class="sxs-lookup"><span data-stu-id="ac490-184">subject</span></span>|<span data-ttu-id="ac490-185">string</span><span class="sxs-lookup"><span data-stu-id="ac490-185">string</span></span>| <span data-ttu-id="ac490-186">消息的主题（纯文本）。</span><span class="sxs-lookup"><span data-stu-id="ac490-186">The subject of the message, in plaintext.</span></span>|
|<span data-ttu-id="ac490-187">正文</span><span class="sxs-lookup"><span data-stu-id="ac490-187">body</span></span>|[<span data-ttu-id="ac490-188">itemBody</span><span class="sxs-lookup"><span data-stu-id="ac490-188">itemBody</span></span>](itembody.md)|<span data-ttu-id="ac490-189">消息内容的纯文本/HTML 表示。</span><span class="sxs-lookup"><span data-stu-id="ac490-189">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="ac490-190">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="ac490-190">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="ac490-191">如果消息包含 [chatMessageMention](chatmessagemention.md)，则内容始终采用 HTML 格式。</span><span class="sxs-lookup"><span data-stu-id="ac490-191">The content is always in HTML if the message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="ac490-192">摘要</span><span class="sxs-lookup"><span data-stu-id="ac490-192">summary</span></span>|<span data-ttu-id="ac490-193">string</span><span class="sxs-lookup"><span data-stu-id="ac490-193">string</span></span>| <span data-ttu-id="ac490-194">可用于推送通知的消息摘要文本和摘要视图或回退视图。</span><span class="sxs-lookup"><span data-stu-id="ac490-194">Summary text of the message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="ac490-195">仅适用于频道消息，不适用于聊天消息。</span><span class="sxs-lookup"><span data-stu-id="ac490-195">Only applies to channel messages, not chat messages.</span></span> |
|<span data-ttu-id="ac490-196">附件</span><span class="sxs-lookup"><span data-stu-id="ac490-196">attachments</span></span>|<span data-ttu-id="ac490-197">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ac490-197">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="ac490-198">附加文件。</span><span class="sxs-lookup"><span data-stu-id="ac490-198">Attached files.</span></span> <span data-ttu-id="ac490-199">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="ac490-199">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="ac490-200">提及</span><span class="sxs-lookup"><span data-stu-id="ac490-200">mentions</span></span>|<span data-ttu-id="ac490-201">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ac490-201">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="ac490-202">消息中提到的实体列表。</span><span class="sxs-lookup"><span data-stu-id="ac490-202">List of entities mentioned in the message.</span></span> <span data-ttu-id="ac490-203">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="ac490-203">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="ac490-204">重要性</span><span class="sxs-lookup"><span data-stu-id="ac490-204">importance</span></span>| <span data-ttu-id="ac490-205">chatMessageImportance</span><span class="sxs-lookup"><span data-stu-id="ac490-205">chatMessageImportance</span></span> | <span data-ttu-id="ac490-206">邮件的重要性。</span><span class="sxs-lookup"><span data-stu-id="ac490-206">The importance of the message.</span></span> <span data-ttu-id="ac490-207">可能的值包括 `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="ac490-207">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="ac490-208">反应</span><span class="sxs-lookup"><span data-stu-id="ac490-208">reactions</span></span>| <span data-ttu-id="ac490-209">[chatMessageReaction](chatmessagereaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ac490-209">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="ac490-210">此消息的反应（例如点赞）。</span><span class="sxs-lookup"><span data-stu-id="ac490-210">Reactions for this message (for example, Like).</span></span>|
|<span data-ttu-id="ac490-211">区域设置</span><span class="sxs-lookup"><span data-stu-id="ac490-211">locale</span></span>|<span data-ttu-id="ac490-212">string</span><span class="sxs-lookup"><span data-stu-id="ac490-212">string</span></span>|<span data-ttu-id="ac490-213">客户端设置的消息区域设置。</span><span class="sxs-lookup"><span data-stu-id="ac490-213">Locale of the message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac490-214">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ac490-214">JSON representation</span></span>

<span data-ttu-id="ac490-215">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac490-215">The following is a JSON representation of the resource.</span></span>

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
