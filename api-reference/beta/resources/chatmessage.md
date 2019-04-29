---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 4c2631d0ba4883160c443000fa2ecb0e1853523d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339840"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="c50ff-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="c50ff-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c50ff-105">表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="c50ff-105">Represents an individual chat message within a channel or chat entity.</span></span> <span data-ttu-id="c50ff-106">该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。</span><span class="sxs-lookup"><span data-stu-id="c50ff-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="c50ff-107">方法</span><span class="sxs-lookup"><span data-stu-id="c50ff-107">Methods</span></span>

| <span data-ttu-id="c50ff-108">方法</span><span class="sxs-lookup"><span data-stu-id="c50ff-108">Method</span></span>       | <span data-ttu-id="c50ff-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c50ff-109">Return Type</span></span>  |<span data-ttu-id="c50ff-110">说明</span><span class="sxs-lookup"><span data-stu-id="c50ff-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c50ff-111">列出渠道消息</span><span class="sxs-lookup"><span data-stu-id="c50ff-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="c50ff-112">[chatmessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c50ff-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="c50ff-113">获取渠道中的所有根消息列表。</span><span class="sxs-lookup"><span data-stu-id="c50ff-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="c50ff-114">获取渠道消息</span><span class="sxs-lookup"><span data-stu-id="c50ff-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="c50ff-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="c50ff-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="c50ff-116">获取渠道中的单个根消息。</span><span class="sxs-lookup"><span data-stu-id="c50ff-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="c50ff-117">列出消息回复</span><span class="sxs-lookup"><span data-stu-id="c50ff-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="c50ff-118">[chatmessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c50ff-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="c50ff-119">获取渠道中的所有消息回复列表。</span><span class="sxs-lookup"><span data-stu-id="c50ff-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="c50ff-120">获取消息回复</span><span class="sxs-lookup"><span data-stu-id="c50ff-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="c50ff-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="c50ff-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="c50ff-122">获取渠道中的单个消息回复。</span><span class="sxs-lookup"><span data-stu-id="c50ff-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="c50ff-123">在渠道中发送消息</span><span class="sxs-lookup"><span data-stu-id="c50ff-123">Send a message in a channel</span></span>](../api/channel-post-chatmessage.md) | [<span data-ttu-id="c50ff-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="c50ff-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="c50ff-125">在渠道中创建新的顶级消息。</span><span class="sxs-lookup"><span data-stu-id="c50ff-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="c50ff-126">在渠道中回复消息</span><span class="sxs-lookup"><span data-stu-id="c50ff-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="c50ff-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="c50ff-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="c50ff-128">在渠道中回复现有消息。</span><span class="sxs-lookup"><span data-stu-id="c50ff-128">Reply to an existing message in a channel.</span></span>|
|[<span data-ttu-id="c50ff-129">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="c50ff-129">List messages in a chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="c50ff-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c50ff-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="c50ff-131">获取一对一聊天或群组聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="c50ff-131">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="c50ff-132">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="c50ff-132">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="c50ff-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c50ff-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="c50ff-134">获取聊天中的单个消息。</span><span class="sxs-lookup"><span data-stu-id="c50ff-134">Get a single reply to a message in a channel.</span></span> |


## <a name="properties"></a><span data-ttu-id="c50ff-135">属性</span><span class="sxs-lookup"><span data-stu-id="c50ff-135">Properties</span></span>
| <span data-ttu-id="c50ff-136">属性</span><span class="sxs-lookup"><span data-stu-id="c50ff-136">Property</span></span>     | <span data-ttu-id="c50ff-137">类型</span><span class="sxs-lookup"><span data-stu-id="c50ff-137">Type</span></span>   |<span data-ttu-id="c50ff-138">说明</span><span class="sxs-lookup"><span data-stu-id="c50ff-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c50ff-139">id</span><span class="sxs-lookup"><span data-stu-id="c50ff-139">id</span></span>|<span data-ttu-id="c50ff-140">String</span><span class="sxs-lookup"><span data-stu-id="c50ff-140">String</span></span>| <span data-ttu-id="c50ff-141">只读。</span><span class="sxs-lookup"><span data-stu-id="c50ff-141">Read-only.</span></span> <span data-ttu-id="c50ff-142">消息的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="c50ff-142">Unique ID of the message.</span></span>|
|<span data-ttu-id="c50ff-143">replyToId</span><span class="sxs-lookup"><span data-stu-id="c50ff-143">replyToId</span></span>| <span data-ttu-id="c50ff-144">string</span><span class="sxs-lookup"><span data-stu-id="c50ff-144">string</span></span> | <span data-ttu-id="c50ff-145">线程的父级消息/根消息的 Id。</span><span class="sxs-lookup"><span data-stu-id="c50ff-145">Id of the parent message/root message of the thread.</span></span> <span data-ttu-id="c50ff-146">（仅适用于频道中的消息，不适用于聊天）</span><span class="sxs-lookup"><span data-stu-id="c50ff-146">(Only applies to messages in channels not chats)</span></span> |
|<span data-ttu-id="c50ff-147">from</span><span class="sxs-lookup"><span data-stu-id="c50ff-147">from</span></span>|[<span data-ttu-id="c50ff-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="c50ff-148">identitySet</span></span>](identityset.md)| <span data-ttu-id="c50ff-149">只读。</span><span class="sxs-lookup"><span data-stu-id="c50ff-149">Read only.</span></span> <span data-ttu-id="c50ff-150">消息发送者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c50ff-150">Details of the sender of the message.</span></span>|
|<span data-ttu-id="c50ff-151">etag</span><span class="sxs-lookup"><span data-stu-id="c50ff-151">etag</span></span>| <span data-ttu-id="c50ff-152">string</span><span class="sxs-lookup"><span data-stu-id="c50ff-152">string</span></span> | <span data-ttu-id="c50ff-153">消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="c50ff-153">Version number of the message.</span></span> |
|<span data-ttu-id="c50ff-154">messageType</span><span class="sxs-lookup"><span data-stu-id="c50ff-154">messageType</span></span>|<span data-ttu-id="c50ff-155">String</span><span class="sxs-lookup"><span data-stu-id="c50ff-155">String</span></span>|<span data-ttu-id="c50ff-156">消息类型，当前支持的值包括：message、chatEvent、Typing。</span><span class="sxs-lookup"><span data-stu-id="c50ff-156">The type of message, current supported values are: message, chatEvent, Typing.</span></span>|
|<span data-ttu-id="c50ff-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c50ff-157">createdDateTime</span></span>|<span data-ttu-id="c50ff-158">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c50ff-158">dateTimeOffset</span></span>|<span data-ttu-id="c50ff-159">只读。</span><span class="sxs-lookup"><span data-stu-id="c50ff-159">Read only.</span></span> <span data-ttu-id="c50ff-160">创建消息时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="c50ff-160">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="c50ff-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c50ff-161">lastModifiedDateTime</span></span>|<span data-ttu-id="c50ff-162">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c50ff-162">dateTimeOffset</span></span>|<span data-ttu-id="c50ff-163">只读。</span><span class="sxs-lookup"><span data-stu-id="c50ff-163">Read only.</span></span> <span data-ttu-id="c50ff-164">编辑/更新消息时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="c50ff-164">Timestamp of when the message was edited/updated.</span></span>|
|<span data-ttu-id="c50ff-165">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="c50ff-165">deletedDateTime</span></span>|<span data-ttu-id="c50ff-166">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c50ff-166">dateTimeOffset</span></span>|<span data-ttu-id="c50ff-167">只读。</span><span class="sxs-lookup"><span data-stu-id="c50ff-167">Read only.</span></span> <span data-ttu-id="c50ff-168">删除消息时的时间戳，如果未删除则为 null。</span><span class="sxs-lookup"><span data-stu-id="c50ff-168">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="c50ff-169">subject</span><span class="sxs-lookup"><span data-stu-id="c50ff-169">subject</span></span>|<span data-ttu-id="c50ff-170">string</span><span class="sxs-lookup"><span data-stu-id="c50ff-170">string</span></span>| <span data-ttu-id="c50ff-171">消息的主题（纯文本）。</span><span class="sxs-lookup"><span data-stu-id="c50ff-171">The subject of the message.</span></span>|
|<span data-ttu-id="c50ff-172">正文</span><span class="sxs-lookup"><span data-stu-id="c50ff-172">body</span></span>|[<span data-ttu-id="c50ff-173">itemBody</span><span class="sxs-lookup"><span data-stu-id="c50ff-173">itemBody</span></span>](itembody.md)|<span data-ttu-id="c50ff-174">消息内容的纯文本/HTML 表示。</span><span class="sxs-lookup"><span data-stu-id="c50ff-174">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="c50ff-175">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="c50ff-175">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="c50ff-176">如果消息包含 [chatMessageMention](chatmessagemention.md)，则内容始终采用 HTML 格式。</span><span class="sxs-lookup"><span data-stu-id="c50ff-176">The content is always in HTML if the message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="c50ff-177">摘要</span><span class="sxs-lookup"><span data-stu-id="c50ff-177">summary</span></span>|<span data-ttu-id="c50ff-178">string</span><span class="sxs-lookup"><span data-stu-id="c50ff-178">string</span></span>| <span data-ttu-id="c50ff-179">可用于推送通知的消息摘要文本和摘要视图或回退视图。</span><span class="sxs-lookup"><span data-stu-id="c50ff-179">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span> <span data-ttu-id="c50ff-180">仅适用于频道消息，不适用于聊天消息。</span><span class="sxs-lookup"><span data-stu-id="c50ff-180">Only applies to channel messages, not chat messages.</span></span> |
|<span data-ttu-id="c50ff-181">附件</span><span class="sxs-lookup"><span data-stu-id="c50ff-181">attachments</span></span>|<span data-ttu-id="c50ff-182">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c50ff-182">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="c50ff-183">附加文件。</span><span class="sxs-lookup"><span data-stu-id="c50ff-183">Attached files.</span></span> <span data-ttu-id="c50ff-184">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="c50ff-184">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="c50ff-185">提及</span><span class="sxs-lookup"><span data-stu-id="c50ff-185">mentions</span></span>|<span data-ttu-id="c50ff-186">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c50ff-186">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="c50ff-187">消息中提到的实体列表。</span><span class="sxs-lookup"><span data-stu-id="c50ff-187">List of entities mentioned in the message.</span></span> <span data-ttu-id="c50ff-188">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="c50ff-188">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="c50ff-189">重要性</span><span class="sxs-lookup"><span data-stu-id="c50ff-189">importance</span></span>| <span data-ttu-id="c50ff-190">string</span><span class="sxs-lookup"><span data-stu-id="c50ff-190">string</span></span> | <span data-ttu-id="c50ff-191">消息重要性包括：正常、高。</span><span class="sxs-lookup"><span data-stu-id="c50ff-191">The importance of the message: Normal, High.</span></span>|
|<span data-ttu-id="c50ff-192">反应</span><span class="sxs-lookup"><span data-stu-id="c50ff-192">reactions</span></span>| <span data-ttu-id="c50ff-193">[chatMessageReaction](chatmessagereaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c50ff-193">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="c50ff-194">此消息的反应（例如点赞）。</span><span class="sxs-lookup"><span data-stu-id="c50ff-194">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="c50ff-195">区域设置</span><span class="sxs-lookup"><span data-stu-id="c50ff-195">locale</span></span>|<span data-ttu-id="c50ff-196">string</span><span class="sxs-lookup"><span data-stu-id="c50ff-196">string</span></span>|<span data-ttu-id="c50ff-197">客户端设置的消息区域设置。</span><span class="sxs-lookup"><span data-stu-id="c50ff-197">Locale of the message set by the client</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c50ff-198">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c50ff-198">JSON representation</span></span>

<span data-ttu-id="c50ff-199">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c50ff-199">The following is a JSON representation of the resource.</span></span>

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
