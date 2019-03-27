---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。
localization_priority: Priority
ms.openlocfilehash: 1f1e38e53a7c7ad1b0452c9facc6d7f97314094e
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/26/2019
ms.locfileid: "30799996"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="c8068-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="c8068-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8068-105">表示 [渠道](channel.md)或聊天实体内的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="c8068-105">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="c8068-106">该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。</span><span class="sxs-lookup"><span data-stu-id="c8068-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="c8068-107">方法</span><span class="sxs-lookup"><span data-stu-id="c8068-107">Methods</span></span>

| <span data-ttu-id="c8068-108">方法</span><span class="sxs-lookup"><span data-stu-id="c8068-108">Method</span></span>       | <span data-ttu-id="c8068-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c8068-109">Return Type</span></span>  |<span data-ttu-id="c8068-110">说明</span><span class="sxs-lookup"><span data-stu-id="c8068-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c8068-111">列出渠道消息</span><span class="sxs-lookup"><span data-stu-id="c8068-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="c8068-112">[chatmessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c8068-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="c8068-113">获取渠道中的所有根消息列表。</span><span class="sxs-lookup"><span data-stu-id="c8068-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="c8068-114">获取渠道消息</span><span class="sxs-lookup"><span data-stu-id="c8068-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="c8068-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="c8068-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="c8068-116">获取渠道中的单个根消息。</span><span class="sxs-lookup"><span data-stu-id="c8068-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="c8068-117">列出消息回复</span><span class="sxs-lookup"><span data-stu-id="c8068-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="c8068-118">[chatmessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c8068-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="c8068-119">获取渠道中的所有消息回复列表。</span><span class="sxs-lookup"><span data-stu-id="c8068-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="c8068-120">获取消息回复</span><span class="sxs-lookup"><span data-stu-id="c8068-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="c8068-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="c8068-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="c8068-122">获取渠道中的单个消息回复。</span><span class="sxs-lookup"><span data-stu-id="c8068-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="c8068-123">在渠道中发送消息</span><span class="sxs-lookup"><span data-stu-id="c8068-123">Send a message in a channel</span></span>](../api/channel-post-chatmessage.md) | [<span data-ttu-id="c8068-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="c8068-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="c8068-125">在渠道中创建新的顶级消息。</span><span class="sxs-lookup"><span data-stu-id="c8068-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="c8068-126">在渠道中回复消息</span><span class="sxs-lookup"><span data-stu-id="c8068-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="c8068-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="c8068-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="c8068-128">在渠道中回复现有消息。</span><span class="sxs-lookup"><span data-stu-id="c8068-128">Reply to an existing message in a channel.</span></span>|


## <a name="properties"></a><span data-ttu-id="c8068-129">属性</span><span class="sxs-lookup"><span data-stu-id="c8068-129">Properties</span></span>
| <span data-ttu-id="c8068-130">属性</span><span class="sxs-lookup"><span data-stu-id="c8068-130">Property</span></span>     | <span data-ttu-id="c8068-131">类型</span><span class="sxs-lookup"><span data-stu-id="c8068-131">Type</span></span>   |<span data-ttu-id="c8068-132">说明</span><span class="sxs-lookup"><span data-stu-id="c8068-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8068-133">id</span><span class="sxs-lookup"><span data-stu-id="c8068-133">id</span></span>|<span data-ttu-id="c8068-134">String</span><span class="sxs-lookup"><span data-stu-id="c8068-134">String</span></span>| <span data-ttu-id="c8068-135">只读。</span><span class="sxs-lookup"><span data-stu-id="c8068-135">Read-only.</span></span> <span data-ttu-id="c8068-136">消息的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="c8068-136">Unique ID of the message.</span></span>|
|<span data-ttu-id="c8068-137">replyToId</span><span class="sxs-lookup"><span data-stu-id="c8068-137">replyToId</span></span>| <span data-ttu-id="c8068-138">string</span><span class="sxs-lookup"><span data-stu-id="c8068-138">string</span></span> | <span data-ttu-id="c8068-139">线程的父级消息/根消息的 Id。</span><span class="sxs-lookup"><span data-stu-id="c8068-139">Id of the parent message/root message of the thread.</span></span> |
|<span data-ttu-id="c8068-140">from</span><span class="sxs-lookup"><span data-stu-id="c8068-140">from</span></span>|[<span data-ttu-id="c8068-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="c8068-141">identitySet</span></span>](identityset.md)| <span data-ttu-id="c8068-142">只读。</span><span class="sxs-lookup"><span data-stu-id="c8068-142">Read only.</span></span> <span data-ttu-id="c8068-143">消息发送者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c8068-143">Details of the sender of the message.</span></span>|
|<span data-ttu-id="c8068-144">etag</span><span class="sxs-lookup"><span data-stu-id="c8068-144">etag</span></span>| <span data-ttu-id="c8068-145">string</span><span class="sxs-lookup"><span data-stu-id="c8068-145">string</span></span> | <span data-ttu-id="c8068-146">消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="c8068-146">Version number of the message.</span></span> |
|<span data-ttu-id="c8068-147">messageType</span><span class="sxs-lookup"><span data-stu-id="c8068-147">messageType</span></span>|<span data-ttu-id="c8068-148">String</span><span class="sxs-lookup"><span data-stu-id="c8068-148">String</span></span>|<span data-ttu-id="c8068-149">消息类型，当前支持的值包括：message、chatEvent、Typing。</span><span class="sxs-lookup"><span data-stu-id="c8068-149">The type of message, current supported values are: message, chatEvent, Typing.</span></span>|
|<span data-ttu-id="c8068-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8068-150">createdDateTime</span></span>|<span data-ttu-id="c8068-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8068-151">dateTimeOffset</span></span>|<span data-ttu-id="c8068-152">只读。</span><span class="sxs-lookup"><span data-stu-id="c8068-152">Read only.</span></span> <span data-ttu-id="c8068-153">创建消息时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="c8068-153">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="c8068-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8068-154">lastModifiedDateTime</span></span>|<span data-ttu-id="c8068-155">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8068-155">dateTimeOffset</span></span>|<span data-ttu-id="c8068-156">只读。</span><span class="sxs-lookup"><span data-stu-id="c8068-156">Read only.</span></span> <span data-ttu-id="c8068-157">编辑/更新消息时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="c8068-157">Timestamp of when the message was edited/updated.</span></span>|
|<span data-ttu-id="c8068-158">deleted</span><span class="sxs-lookup"><span data-stu-id="c8068-158">deleted</span></span>|<span data-ttu-id="c8068-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8068-159">Boolean</span></span>|<span data-ttu-id="c8068-160">指示消息是否已被软删除。</span><span class="sxs-lookup"><span data-stu-id="c8068-160">Indicates whether a message has been soft deleted.</span></span>|
|<span data-ttu-id="c8068-161">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8068-161">deletedDateTime</span></span>|<span data-ttu-id="c8068-162">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8068-162">dateTimeOffset</span></span>|<span data-ttu-id="c8068-163">只读。</span><span class="sxs-lookup"><span data-stu-id="c8068-163">Read only.</span></span> <span data-ttu-id="c8068-164">删除消息时的时间戳，如果未删除则为 null。</span><span class="sxs-lookup"><span data-stu-id="c8068-164">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="c8068-165">正文</span><span class="sxs-lookup"><span data-stu-id="c8068-165">body</span></span>|[<span data-ttu-id="c8068-166">itemBody</span><span class="sxs-lookup"><span data-stu-id="c8068-166">itemBody</span></span>](itembody.md)|<span data-ttu-id="c8068-167">消息内容的纯文本/HTML 表示。</span><span class="sxs-lookup"><span data-stu-id="c8068-167">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="c8068-168">默认返回纯文本，应用程序可选择 HTML 作为查询参数的一部分</span><span class="sxs-lookup"><span data-stu-id="c8068-168">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="c8068-169">摘要</span><span class="sxs-lookup"><span data-stu-id="c8068-169">summary</span></span>|<span data-ttu-id="c8068-170">string</span><span class="sxs-lookup"><span data-stu-id="c8068-170">string</span></span>|<span data-ttu-id="c8068-171">可用于推送通知的消息摘要文本和摘要视图或回退视图</span><span class="sxs-lookup"><span data-stu-id="c8068-171">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="c8068-172">提及</span><span class="sxs-lookup"><span data-stu-id="c8068-172">mentions</span></span>|<span data-ttu-id="c8068-173">[chatMessageMention](chatmention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c8068-173">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="c8068-174">消息中提到的实体列表。</span><span class="sxs-lookup"><span data-stu-id="c8068-174">List of entities mentioned in the message.</span></span> <span data-ttu-id="c8068-175">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="c8068-175">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="c8068-176">重要性</span><span class="sxs-lookup"><span data-stu-id="c8068-176">importance</span></span>| <span data-ttu-id="c8068-177">string</span><span class="sxs-lookup"><span data-stu-id="c8068-177">string</span></span> | <span data-ttu-id="c8068-178">消息重要性包括：正常、高。</span><span class="sxs-lookup"><span data-stu-id="c8068-178">The importance of the message: Normal, High.</span></span>|
|<span data-ttu-id="c8068-179">反应</span><span class="sxs-lookup"><span data-stu-id="c8068-179">reactions</span></span>| <span data-ttu-id="c8068-180">[chatMessageReaction](chatreaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c8068-180">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="c8068-181">此消息的反应（例如，赞）</span><span class="sxs-lookup"><span data-stu-id="c8068-181">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="c8068-182">区域设置</span><span class="sxs-lookup"><span data-stu-id="c8068-182">locale</span></span>|<span data-ttu-id="c8068-183">string</span><span class="sxs-lookup"><span data-stu-id="c8068-183">string</span></span>|<span data-ttu-id="c8068-184">客户设置的消息区域设置</span><span class="sxs-lookup"><span data-stu-id="c8068-184">Locale of the message set by the client</span></span>|
|<span data-ttu-id="c8068-185">附件</span><span class="sxs-lookup"><span data-stu-id="c8068-185">attachments</span></span>|<span data-ttu-id="c8068-186">[chatMessageAttachment](chatattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c8068-186">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="c8068-187">附加文件。</span><span class="sxs-lookup"><span data-stu-id="c8068-187">Attached files.</span></span> <span data-ttu-id="c8068-188">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="c8068-188">Attachments are currently read-only – sending attachments is not supported.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c8068-189">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8068-189">JSON representation</span></span>

<span data-ttu-id="c8068-190">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8068-190">The following is a JSON representation of the resource.</span></span>

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
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
