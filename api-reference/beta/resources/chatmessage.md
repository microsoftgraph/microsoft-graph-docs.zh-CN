---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: ea21d57134643c83406f449ee7cdad192afc0326
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2019
ms.locfileid: "34709409"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="26299-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="26299-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26299-105">表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="26299-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span>
<span data-ttu-id="26299-106">该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。</span><span class="sxs-lookup"><span data-stu-id="26299-106">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="26299-107">方法</span><span class="sxs-lookup"><span data-stu-id="26299-107">Methods</span></span>

| <span data-ttu-id="26299-108">方法</span><span class="sxs-lookup"><span data-stu-id="26299-108">Method</span></span>       | <span data-ttu-id="26299-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="26299-109">Return Type</span></span>  |<span data-ttu-id="26299-110">说明</span><span class="sxs-lookup"><span data-stu-id="26299-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="26299-111">列出渠道消息</span><span class="sxs-lookup"><span data-stu-id="26299-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="26299-112">[chatmessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26299-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="26299-113">获取渠道中的所有根消息列表。</span><span class="sxs-lookup"><span data-stu-id="26299-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="26299-114">获取渠道消息</span><span class="sxs-lookup"><span data-stu-id="26299-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="26299-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="26299-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="26299-116">获取渠道中的单个根消息。</span><span class="sxs-lookup"><span data-stu-id="26299-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="26299-117">列出消息回复</span><span class="sxs-lookup"><span data-stu-id="26299-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="26299-118">[chatmessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26299-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="26299-119">获取渠道中的所有消息回复列表。</span><span class="sxs-lookup"><span data-stu-id="26299-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="26299-120">获取消息回复</span><span class="sxs-lookup"><span data-stu-id="26299-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="26299-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="26299-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="26299-122">获取渠道中的单个消息回复。</span><span class="sxs-lookup"><span data-stu-id="26299-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="26299-123">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="26299-123">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="26299-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="26299-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="26299-125">在渠道中创建新的顶级消息。</span><span class="sxs-lookup"><span data-stu-id="26299-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="26299-126">在频道中创建 chatMessage 回复</span><span class="sxs-lookup"><span data-stu-id="26299-126">Create chatMessage reply in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="26299-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="26299-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="26299-128">在渠道中回复现有消息。</span><span class="sxs-lookup"><span data-stu-id="26299-128">Reply to an existing message in a channel.</span></span>|
|[<span data-ttu-id="26299-129">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="26299-129">List messages in a chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="26299-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="26299-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="26299-131">获取一对一聊天或群组聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="26299-131">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="26299-132">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="26299-132">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="26299-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="26299-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="26299-134">获取聊天中的单个消息。</span><span class="sxs-lookup"><span data-stu-id="26299-134">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="26299-135">属性</span><span class="sxs-lookup"><span data-stu-id="26299-135">Properties</span></span>

| <span data-ttu-id="26299-136">属性</span><span class="sxs-lookup"><span data-stu-id="26299-136">Property</span></span>   | <span data-ttu-id="26299-137">类型</span><span class="sxs-lookup"><span data-stu-id="26299-137">Type</span></span> |<span data-ttu-id="26299-138">说明</span><span class="sxs-lookup"><span data-stu-id="26299-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26299-139">id</span><span class="sxs-lookup"><span data-stu-id="26299-139">id</span></span>|<span data-ttu-id="26299-140">String</span><span class="sxs-lookup"><span data-stu-id="26299-140">String</span></span>| <span data-ttu-id="26299-141">只读。</span><span class="sxs-lookup"><span data-stu-id="26299-141">Read-only.</span></span> <span data-ttu-id="26299-142">消息的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="26299-142">Unique ID of the message.</span></span>|
|<span data-ttu-id="26299-143">replyToId</span><span class="sxs-lookup"><span data-stu-id="26299-143">replyToId</span></span>| <span data-ttu-id="26299-144">string</span><span class="sxs-lookup"><span data-stu-id="26299-144">string</span></span> | <span data-ttu-id="26299-145">只读。</span><span class="sxs-lookup"><span data-stu-id="26299-145">Read-only.</span></span> <span data-ttu-id="26299-146">线程的父级消息/根消息的 Id。</span><span class="sxs-lookup"><span data-stu-id="26299-146">Id of the parent message/root message of the thread.</span></span> <span data-ttu-id="26299-147">（仅适用于频道中的消息，不适用于聊天）</span><span class="sxs-lookup"><span data-stu-id="26299-147">(Only applies to messages in channels not chats)</span></span> |
|<span data-ttu-id="26299-148">from</span><span class="sxs-lookup"><span data-stu-id="26299-148">from</span></span>|[<span data-ttu-id="26299-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="26299-149">identitySet</span></span>](identityset.md)| <span data-ttu-id="26299-150">只读。</span><span class="sxs-lookup"><span data-stu-id="26299-150">Read only.</span></span> <span data-ttu-id="26299-151">消息发送者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="26299-151">Details of the sender of the message.</span></span>|
|<span data-ttu-id="26299-152">etag</span><span class="sxs-lookup"><span data-stu-id="26299-152">etag</span></span>| <span data-ttu-id="26299-153">string</span><span class="sxs-lookup"><span data-stu-id="26299-153">string</span></span> | <span data-ttu-id="26299-154">只读。</span><span class="sxs-lookup"><span data-stu-id="26299-154">Read-only.</span></span> <span data-ttu-id="26299-155">消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="26299-155">Version number of the message.</span></span> |
|<span data-ttu-id="26299-156">messageType</span><span class="sxs-lookup"><span data-stu-id="26299-156">messageType</span></span>|<span data-ttu-id="26299-157">chatMessageType</span><span class="sxs-lookup"><span data-stu-id="26299-157">chatMessageType</span></span>|<span data-ttu-id="26299-158">邮件类型。</span><span class="sxs-lookup"><span data-stu-id="26299-158">The type of message.</span></span> <span data-ttu-id="26299-159">可取值包括：`message`。</span><span class="sxs-lookup"><span data-stu-id="26299-159">The possible values are: `message`, , .</span></span>|
|<span data-ttu-id="26299-160">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26299-160">createdDateTime</span></span>|<span data-ttu-id="26299-161">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26299-161">dateTimeOffset</span></span>|<span data-ttu-id="26299-162">只读。</span><span class="sxs-lookup"><span data-stu-id="26299-162">Read only.</span></span> <span data-ttu-id="26299-163">创建消息时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="26299-163">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="26299-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26299-164">lastModifiedDateTime</span></span>|<span data-ttu-id="26299-165">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26299-165">dateTimeOffset</span></span>|<span data-ttu-id="26299-166">只读。</span><span class="sxs-lookup"><span data-stu-id="26299-166">Read only.</span></span> <span data-ttu-id="26299-167">编辑/更新消息时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="26299-167">Timestamp of when the message was edited/updated.</span></span>|
|<span data-ttu-id="26299-168">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="26299-168">deletedDateTime</span></span>|<span data-ttu-id="26299-169">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26299-169">dateTimeOffset</span></span>|<span data-ttu-id="26299-170">只读。</span><span class="sxs-lookup"><span data-stu-id="26299-170">Read only.</span></span> <span data-ttu-id="26299-171">删除消息时的时间戳，如果未删除则为 null。</span><span class="sxs-lookup"><span data-stu-id="26299-171">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="26299-172">subject</span><span class="sxs-lookup"><span data-stu-id="26299-172">subject</span></span>|<span data-ttu-id="26299-173">string</span><span class="sxs-lookup"><span data-stu-id="26299-173">string</span></span>| <span data-ttu-id="26299-174">消息的主题（纯文本）。</span><span class="sxs-lookup"><span data-stu-id="26299-174">The subject of the message, in plaintext.</span></span>|
|<span data-ttu-id="26299-175">正文</span><span class="sxs-lookup"><span data-stu-id="26299-175">body</span></span>|[<span data-ttu-id="26299-176">itemBody</span><span class="sxs-lookup"><span data-stu-id="26299-176">itemBody</span></span>](itembody.md)|<span data-ttu-id="26299-177">消息内容的纯文本/HTML 表示。</span><span class="sxs-lookup"><span data-stu-id="26299-177">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="26299-178">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="26299-178">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="26299-179">如果消息包含 [chatMessageMention](chatmessagemention.md)，则内容始终采用 HTML 格式。</span><span class="sxs-lookup"><span data-stu-id="26299-179">The content is always in HTML if the message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="26299-180">摘要</span><span class="sxs-lookup"><span data-stu-id="26299-180">summary</span></span>|<span data-ttu-id="26299-181">string</span><span class="sxs-lookup"><span data-stu-id="26299-181">string</span></span>| <span data-ttu-id="26299-182">可用于推送通知的消息摘要文本和摘要视图或回退视图。</span><span class="sxs-lookup"><span data-stu-id="26299-182">Summary text of the message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="26299-183">仅适用于频道消息，不适用于聊天消息。</span><span class="sxs-lookup"><span data-stu-id="26299-183">Only applies to channel messages, not chat messages.</span></span> |
|<span data-ttu-id="26299-184">附件</span><span class="sxs-lookup"><span data-stu-id="26299-184">attachments</span></span>|<span data-ttu-id="26299-185">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26299-185">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="26299-186">附加文件。</span><span class="sxs-lookup"><span data-stu-id="26299-186">Attached files.</span></span> <span data-ttu-id="26299-187">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="26299-187">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="26299-188">提及</span><span class="sxs-lookup"><span data-stu-id="26299-188">mentions</span></span>|<span data-ttu-id="26299-189">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26299-189">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="26299-190">消息中提到的实体列表。</span><span class="sxs-lookup"><span data-stu-id="26299-190">List of entities mentioned in the message.</span></span> <span data-ttu-id="26299-191">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="26299-191">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="26299-192">importance</span><span class="sxs-lookup"><span data-stu-id="26299-192">importance</span></span>| <span data-ttu-id="26299-193">chatMessageImportance</span><span class="sxs-lookup"><span data-stu-id="26299-193">chatMessageImportance</span></span> | <span data-ttu-id="26299-194">邮件的重要性。</span><span class="sxs-lookup"><span data-stu-id="26299-194">The importance of the message.</span></span> <span data-ttu-id="26299-195">可能的值包括 `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="26299-195">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="26299-196">反应</span><span class="sxs-lookup"><span data-stu-id="26299-196">reactions</span></span>| <span data-ttu-id="26299-197">[chatMessageReaction](chatmessagereaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26299-197">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="26299-198">此消息的反应（例如点赞）。</span><span class="sxs-lookup"><span data-stu-id="26299-198">Reactions for this message (for example, Like).</span></span>|
|<span data-ttu-id="26299-199">区域设置</span><span class="sxs-lookup"><span data-stu-id="26299-199">locale</span></span>|<span data-ttu-id="26299-200">string</span><span class="sxs-lookup"><span data-stu-id="26299-200">string</span></span>|<span data-ttu-id="26299-201">客户端设置的消息区域设置。</span><span class="sxs-lookup"><span data-stu-id="26299-201">Locale of the message set by the client.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="26299-202">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26299-202">JSON representation</span></span>

<span data-ttu-id="26299-203">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26299-203">The following is a JSON representation of the resource.</span></span>

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
