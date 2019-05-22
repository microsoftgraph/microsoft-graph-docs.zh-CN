---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 0639fd0b5317abd4814123b500ec0548f78d05ac
ms.sourcegitcommit: abca7fcefeaa74b50f4600b35d816b626ba08468
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2019
ms.locfileid: "34311159"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="be608-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="be608-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be608-105">表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="be608-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="be608-106">该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。</span><span class="sxs-lookup"><span data-stu-id="be608-106">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="be608-107">方法</span><span class="sxs-lookup"><span data-stu-id="be608-107">Methods</span></span>

| <span data-ttu-id="be608-108">方法</span><span class="sxs-lookup"><span data-stu-id="be608-108">Method</span></span>       | <span data-ttu-id="be608-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="be608-109">Return Type</span></span>  |<span data-ttu-id="be608-110">说明</span><span class="sxs-lookup"><span data-stu-id="be608-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="be608-111">列出渠道消息</span><span class="sxs-lookup"><span data-stu-id="be608-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="be608-112">[chatmessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be608-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="be608-113">获取渠道中的所有根消息列表。</span><span class="sxs-lookup"><span data-stu-id="be608-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="be608-114">获取渠道消息</span><span class="sxs-lookup"><span data-stu-id="be608-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="be608-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="be608-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="be608-116">获取渠道中的单个根消息。</span><span class="sxs-lookup"><span data-stu-id="be608-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="be608-117">列出消息回复</span><span class="sxs-lookup"><span data-stu-id="be608-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="be608-118">[chatmessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be608-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="be608-119">获取渠道中的所有消息回复列表。</span><span class="sxs-lookup"><span data-stu-id="be608-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="be608-120">获取消息回复</span><span class="sxs-lookup"><span data-stu-id="be608-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="be608-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="be608-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="be608-122">获取渠道中的单个消息回复。</span><span class="sxs-lookup"><span data-stu-id="be608-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="be608-123">在渠道中发送消息</span><span class="sxs-lookup"><span data-stu-id="be608-123">Send a message in a channel</span></span>](../api/channel-post-chatmessage.md) | [<span data-ttu-id="be608-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="be608-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="be608-125">在渠道中创建新的顶级消息。</span><span class="sxs-lookup"><span data-stu-id="be608-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="be608-126">在渠道中回复消息</span><span class="sxs-lookup"><span data-stu-id="be608-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="be608-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="be608-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="be608-128">在渠道中回复现有消息。</span><span class="sxs-lookup"><span data-stu-id="be608-128">Reply to an existing message in a channel.</span></span>|
|[<span data-ttu-id="be608-129">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="be608-129">List messages in a chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="be608-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="be608-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="be608-131">获取一对一聊天或群组聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="be608-131">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="be608-132">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="be608-132">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="be608-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="be608-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="be608-134">获取聊天中的单个消息。</span><span class="sxs-lookup"><span data-stu-id="be608-134">Get a single message in a chat.</span></span> |


## <a name="properties"></a><span data-ttu-id="be608-135">属性</span><span class="sxs-lookup"><span data-stu-id="be608-135">Properties</span></span>
| <span data-ttu-id="be608-136">属性</span><span class="sxs-lookup"><span data-stu-id="be608-136">Property</span></span>     | <span data-ttu-id="be608-137">类型</span><span class="sxs-lookup"><span data-stu-id="be608-137">Type</span></span>   |<span data-ttu-id="be608-138">说明</span><span class="sxs-lookup"><span data-stu-id="be608-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be608-139">id</span><span class="sxs-lookup"><span data-stu-id="be608-139">id</span></span>|<span data-ttu-id="be608-140">String</span><span class="sxs-lookup"><span data-stu-id="be608-140">String</span></span>| <span data-ttu-id="be608-141">只读。</span><span class="sxs-lookup"><span data-stu-id="be608-141">Read-only.</span></span> <span data-ttu-id="be608-142">消息的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="be608-142">Unique ID of the message.</span></span>|
|<span data-ttu-id="be608-143">replyToId</span><span class="sxs-lookup"><span data-stu-id="be608-143">replyToId</span></span>| <span data-ttu-id="be608-144">string</span><span class="sxs-lookup"><span data-stu-id="be608-144">string</span></span> | <span data-ttu-id="be608-145">线程的父级消息/根消息的 Id。</span><span class="sxs-lookup"><span data-stu-id="be608-145">Id of the parent message/root message of the thread.</span></span> <span data-ttu-id="be608-146">（仅适用于频道中的消息，不适用于聊天）</span><span class="sxs-lookup"><span data-stu-id="be608-146">(Only applies to messages in channels not chats)</span></span> |
|<span data-ttu-id="be608-147">from</span><span class="sxs-lookup"><span data-stu-id="be608-147">from</span></span>|[<span data-ttu-id="be608-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="be608-148">identitySet</span></span>](identityset.md)| <span data-ttu-id="be608-149">只读。</span><span class="sxs-lookup"><span data-stu-id="be608-149">Read only.</span></span> <span data-ttu-id="be608-150">消息发送者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="be608-150">Details of the sender of the message.</span></span>|
|<span data-ttu-id="be608-151">etag</span><span class="sxs-lookup"><span data-stu-id="be608-151">etag</span></span>| <span data-ttu-id="be608-152">string</span><span class="sxs-lookup"><span data-stu-id="be608-152">string</span></span> | <span data-ttu-id="be608-153">消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="be608-153">Version number of the message.</span></span> |
|<span data-ttu-id="be608-154">messageType</span><span class="sxs-lookup"><span data-stu-id="be608-154">messageType</span></span>|<span data-ttu-id="be608-155">String</span><span class="sxs-lookup"><span data-stu-id="be608-155">String</span></span>|<span data-ttu-id="be608-156">消息类型，当前支持的值包括：message、chatEvent、Typing。</span><span class="sxs-lookup"><span data-stu-id="be608-156">The type of message, current supported values are: message, chatEvent, Typing.</span></span>|
|<span data-ttu-id="be608-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be608-157">createdDateTime</span></span>|<span data-ttu-id="be608-158">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be608-158">dateTimeOffset</span></span>|<span data-ttu-id="be608-159">只读。</span><span class="sxs-lookup"><span data-stu-id="be608-159">Read only.</span></span> <span data-ttu-id="be608-160">创建消息时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="be608-160">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="be608-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be608-161">lastModifiedDateTime</span></span>|<span data-ttu-id="be608-162">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be608-162">dateTimeOffset</span></span>|<span data-ttu-id="be608-163">只读。</span><span class="sxs-lookup"><span data-stu-id="be608-163">Read only.</span></span> <span data-ttu-id="be608-164">编辑/更新消息时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="be608-164">Timestamp of when the message was edited/updated.</span></span>|
|<span data-ttu-id="be608-165">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="be608-165">deletedDateTime</span></span>|<span data-ttu-id="be608-166">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be608-166">dateTimeOffset</span></span>|<span data-ttu-id="be608-167">只读。</span><span class="sxs-lookup"><span data-stu-id="be608-167">Read only.</span></span> <span data-ttu-id="be608-168">删除消息时的时间戳，如果未删除则为 null。</span><span class="sxs-lookup"><span data-stu-id="be608-168">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="be608-169">subject</span><span class="sxs-lookup"><span data-stu-id="be608-169">subject</span></span>|<span data-ttu-id="be608-170">string</span><span class="sxs-lookup"><span data-stu-id="be608-170">string</span></span>| <span data-ttu-id="be608-171">消息的主题（纯文本）。</span><span class="sxs-lookup"><span data-stu-id="be608-171">The subject of the message, in plaintext.</span></span>|
|<span data-ttu-id="be608-172">正文</span><span class="sxs-lookup"><span data-stu-id="be608-172">body</span></span>|[<span data-ttu-id="be608-173">itemBody</span><span class="sxs-lookup"><span data-stu-id="be608-173">itemBody</span></span>](itembody.md)|<span data-ttu-id="be608-174">消息内容的纯文本/HTML 表示。</span><span class="sxs-lookup"><span data-stu-id="be608-174">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="be608-175">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="be608-175">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="be608-176">如果消息包含 [chatMessageMention](chatmessagemention.md)，则内容始终采用 HTML 格式。</span><span class="sxs-lookup"><span data-stu-id="be608-176">The content is always in HTML if the message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="be608-177">摘要</span><span class="sxs-lookup"><span data-stu-id="be608-177">summary</span></span>|<span data-ttu-id="be608-178">string</span><span class="sxs-lookup"><span data-stu-id="be608-178">string</span></span>| <span data-ttu-id="be608-179">可用于推送通知的消息摘要文本和摘要视图或回退视图。</span><span class="sxs-lookup"><span data-stu-id="be608-179">Summary text of the message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="be608-180">仅适用于频道消息，不适用于聊天消息。</span><span class="sxs-lookup"><span data-stu-id="be608-180">Only applies to channel messages, not chat messages.</span></span> |
|<span data-ttu-id="be608-181">附件</span><span class="sxs-lookup"><span data-stu-id="be608-181">attachments</span></span>|<span data-ttu-id="be608-182">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be608-182">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="be608-183">附加文件。</span><span class="sxs-lookup"><span data-stu-id="be608-183">Attached files.</span></span> <span data-ttu-id="be608-184">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="be608-184">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="be608-185">提及</span><span class="sxs-lookup"><span data-stu-id="be608-185">mentions</span></span>|<span data-ttu-id="be608-186">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be608-186">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="be608-187">消息中提到的实体列表。</span><span class="sxs-lookup"><span data-stu-id="be608-187">List of entities mentioned in the message.</span></span> <span data-ttu-id="be608-188">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="be608-188">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="be608-189">重要性</span><span class="sxs-lookup"><span data-stu-id="be608-189">importance</span></span>| <span data-ttu-id="be608-190">string</span><span class="sxs-lookup"><span data-stu-id="be608-190">string</span></span> | <span data-ttu-id="be608-191">消息重要性包括：正常、高。</span><span class="sxs-lookup"><span data-stu-id="be608-191">The importance of the message: Normal, High.</span></span>|
|<span data-ttu-id="be608-192">反应</span><span class="sxs-lookup"><span data-stu-id="be608-192">reactions</span></span>| <span data-ttu-id="be608-193">[chatMessageReaction](chatmessagereaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be608-193">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="be608-194">此消息的反应（例如点赞）。</span><span class="sxs-lookup"><span data-stu-id="be608-194">Reactions for this message (for example, Like).</span></span>|
|<span data-ttu-id="be608-195">区域设置</span><span class="sxs-lookup"><span data-stu-id="be608-195">locale</span></span>|<span data-ttu-id="be608-196">string</span><span class="sxs-lookup"><span data-stu-id="be608-196">string</span></span>|<span data-ttu-id="be608-197">客户端设置的消息区域设置。</span><span class="sxs-lookup"><span data-stu-id="be608-197">Locale of the message set by the client.</span></span>|
|<span data-ttu-id="be608-198">webUrl</span><span class="sxs-lookup"><span data-stu-id="be608-198">webUrl</span></span>|<span data-ttu-id="be608-199">string</span><span class="sxs-lookup"><span data-stu-id="be608-199">string</span></span>|<span data-ttu-id="be608-200">导航至 Microsoft Teams 中的频道的超链接。</span><span class="sxs-lookup"><span data-stu-id="be608-200">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="be608-201">在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。</span><span class="sxs-lookup"><span data-stu-id="be608-201">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="be608-202">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="be608-202">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="be608-203">只读。</span><span class="sxs-lookup"><span data-stu-id="be608-203">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be608-204">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be608-204">JSON representation</span></span>

<span data-ttu-id="be608-205">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be608-205">The following is a JSON representation of the resource.</span></span>

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
