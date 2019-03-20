---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。
localization_priority: Priority
ms.openlocfilehash: a74f422c6bf60e1293d8620b440152be77dacdc7
ms.sourcegitcommit: cd4bdb2c6754b1d5658e68909ea6c219466da6df
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2019
ms.locfileid: "30644319"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="186db-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="186db-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="186db-105">表示 [渠道](channel.md)或聊天实体内的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="186db-105">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="186db-106">该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。</span><span class="sxs-lookup"><span data-stu-id="186db-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="186db-107">方法</span><span class="sxs-lookup"><span data-stu-id="186db-107">Methods</span></span>

| <span data-ttu-id="186db-108">方法</span><span class="sxs-lookup"><span data-stu-id="186db-108">Method</span></span>       | <span data-ttu-id="186db-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="186db-109">Return Type</span></span>  |<span data-ttu-id="186db-110">说明</span><span class="sxs-lookup"><span data-stu-id="186db-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="186db-111">列出渠道消息</span><span class="sxs-lookup"><span data-stu-id="186db-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="186db-112">[chatmessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="186db-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="186db-113">获取渠道中的所有根消息列表。</span><span class="sxs-lookup"><span data-stu-id="186db-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="186db-114">获取渠道消息</span><span class="sxs-lookup"><span data-stu-id="186db-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="186db-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="186db-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="186db-116">获取渠道中的单个根消息。</span><span class="sxs-lookup"><span data-stu-id="186db-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="186db-117">列出消息回复</span><span class="sxs-lookup"><span data-stu-id="186db-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="186db-118">[chatmessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="186db-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="186db-119">获取渠道中的所有消息回复列表。</span><span class="sxs-lookup"><span data-stu-id="186db-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="186db-120">获取消息回复</span><span class="sxs-lookup"><span data-stu-id="186db-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="186db-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="186db-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="186db-122">获取渠道中的单个消息回复。</span><span class="sxs-lookup"><span data-stu-id="186db-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="186db-123">在渠道中发送消息</span><span class="sxs-lookup"><span data-stu-id="186db-123">Send a message in a channel</span></span>](../api/channel-post-chatmessage.md) | [<span data-ttu-id="186db-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="186db-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="186db-125">在渠道中创建新的顶级消息。</span><span class="sxs-lookup"><span data-stu-id="186db-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="186db-126">在渠道中回复消息</span><span class="sxs-lookup"><span data-stu-id="186db-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="186db-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="186db-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="186db-128">在渠道中回复现有消息。</span><span class="sxs-lookup"><span data-stu-id="186db-128">Reply to an existing message in a channel.</span></span>|


## <a name="properties"></a><span data-ttu-id="186db-129">属性</span><span class="sxs-lookup"><span data-stu-id="186db-129">Properties</span></span>
| <span data-ttu-id="186db-130">属性</span><span class="sxs-lookup"><span data-stu-id="186db-130">Property</span></span>     | <span data-ttu-id="186db-131">类型</span><span class="sxs-lookup"><span data-stu-id="186db-131">Type</span></span>   |<span data-ttu-id="186db-132">说明</span><span class="sxs-lookup"><span data-stu-id="186db-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="186db-133">id</span><span class="sxs-lookup"><span data-stu-id="186db-133">id</span></span>|<span data-ttu-id="186db-134">String</span><span class="sxs-lookup"><span data-stu-id="186db-134">String</span></span>| <span data-ttu-id="186db-135">只读。</span><span class="sxs-lookup"><span data-stu-id="186db-135">Read-only.</span></span> <span data-ttu-id="186db-136">消息的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="186db-136">Unique ID of the message.</span></span>|
|<span data-ttu-id="186db-137">replyToId</span><span class="sxs-lookup"><span data-stu-id="186db-137">replyToId</span></span>| <span data-ttu-id="186db-138">string</span><span class="sxs-lookup"><span data-stu-id="186db-138">string</span></span> | <span data-ttu-id="186db-139">线程的父级消息/根消息的 Id。</span><span class="sxs-lookup"><span data-stu-id="186db-139">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="186db-140">from</span><span class="sxs-lookup"><span data-stu-id="186db-140">from</span></span>|[<span data-ttu-id="186db-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="186db-141">identitySet</span></span>](identityset.md)| <span data-ttu-id="186db-142">只读。</span><span class="sxs-lookup"><span data-stu-id="186db-142">Read only.</span></span> <span data-ttu-id="186db-143">消息发送者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="186db-143">Details of the sender of the message</span></span>|
|<span data-ttu-id="186db-144">etag</span><span class="sxs-lookup"><span data-stu-id="186db-144">etag</span></span>| <span data-ttu-id="186db-145">string</span><span class="sxs-lookup"><span data-stu-id="186db-145">string</span></span> | <span data-ttu-id="186db-146">消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="186db-146">Version number of the message</span></span> |
|<span data-ttu-id="186db-147">messageType</span><span class="sxs-lookup"><span data-stu-id="186db-147">messageType</span></span>|<span data-ttu-id="186db-148">String</span><span class="sxs-lookup"><span data-stu-id="186db-148">String</span></span>|<span data-ttu-id="186db-149">消息类型，当前支持的值包括：message、chatEvent、Typing。</span><span class="sxs-lookup"><span data-stu-id="186db-149">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="186db-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="186db-150">createdDateTime</span></span>|<span data-ttu-id="186db-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="186db-151">dateTimeOffset</span></span>|<span data-ttu-id="186db-152">只读。</span><span class="sxs-lookup"><span data-stu-id="186db-152">Read only.</span></span> <span data-ttu-id="186db-153">创建消息时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="186db-153">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="186db-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="186db-154">lastModifiedDateTime</span></span>|<span data-ttu-id="186db-155">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="186db-155">dateTimeOffset</span></span>|<span data-ttu-id="186db-156">只读。</span><span class="sxs-lookup"><span data-stu-id="186db-156">Read only.</span></span> <span data-ttu-id="186db-157">编辑/更新消息时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="186db-157">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="186db-158">deleted</span><span class="sxs-lookup"><span data-stu-id="186db-158">deleted</span></span>|<span data-ttu-id="186db-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="186db-159">Boolean</span></span>|<span data-ttu-id="186db-160">指示消息是否已被软删除。</span><span class="sxs-lookup"><span data-stu-id="186db-160">Indicates whether a message has been soft deleted</span></span>|
|<span data-ttu-id="186db-161">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="186db-161">deletedDateTime</span></span>|<span data-ttu-id="186db-162">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="186db-162">dateTimeOffset</span></span>|<span data-ttu-id="186db-163">只读。</span><span class="sxs-lookup"><span data-stu-id="186db-163">Read only.</span></span> <span data-ttu-id="186db-164">删除消息时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="186db-164">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="186db-165">主题</span><span class="sxs-lookup"><span data-stu-id="186db-165">subject</span></span>|<span data-ttu-id="186db-166">string</span><span class="sxs-lookup"><span data-stu-id="186db-166">string</span></span>|<span data-ttu-id="186db-167">消息主题行。</span><span class="sxs-lookup"><span data-stu-id="186db-167">Message subject line.</span></span> <span data-ttu-id="186db-168">可选。</span><span class="sxs-lookup"><span data-stu-id="186db-168">Optional.</span></span>|
|<span data-ttu-id="186db-169">正文</span><span class="sxs-lookup"><span data-stu-id="186db-169">body</span></span>|[<span data-ttu-id="186db-170">itemBody</span><span class="sxs-lookup"><span data-stu-id="186db-170">itemBody</span></span>](itembody.md)|<span data-ttu-id="186db-171">消息内容的纯文本/HTML 表示。</span><span class="sxs-lookup"><span data-stu-id="186db-171">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="186db-172">默认返回纯文本，应用程序可选择 HTML 作为查询参数的一部分</span><span class="sxs-lookup"><span data-stu-id="186db-172">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="186db-173">摘要</span><span class="sxs-lookup"><span data-stu-id="186db-173">summary</span></span>|<span data-ttu-id="186db-174">string</span><span class="sxs-lookup"><span data-stu-id="186db-174">string</span></span>|<span data-ttu-id="186db-175">可用于推送通知的消息摘要文本和摘要视图或回退视图</span><span class="sxs-lookup"><span data-stu-id="186db-175">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="186db-176">提及</span><span class="sxs-lookup"><span data-stu-id="186db-176">mentions</span></span>|<span data-ttu-id="186db-177">[chatMessageMention](chatmention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="186db-177">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="186db-178">消息中提到的实体列表。</span><span class="sxs-lookup"><span data-stu-id="186db-178">List of entities mentioned in the message.</span></span> <span data-ttu-id="186db-179">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="186db-179">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="186db-180">重要性</span><span class="sxs-lookup"><span data-stu-id="186db-180">importance</span></span>| <span data-ttu-id="186db-181">string</span><span class="sxs-lookup"><span data-stu-id="186db-181">string</span></span> | <span data-ttu-id="186db-182">消息重要性包括：正常、高。</span><span class="sxs-lookup"><span data-stu-id="186db-182">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="186db-183">反应</span><span class="sxs-lookup"><span data-stu-id="186db-183">reactions</span></span>| <span data-ttu-id="186db-184">[chatMessageReaction](chatreaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="186db-184">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="186db-185">此消息的反应（例如，赞）</span><span class="sxs-lookup"><span data-stu-id="186db-185">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="186db-186">区域设置</span><span class="sxs-lookup"><span data-stu-id="186db-186">locale</span></span>|<span data-ttu-id="186db-187">string</span><span class="sxs-lookup"><span data-stu-id="186db-187">string</span></span>|<span data-ttu-id="186db-188">客户设置的消息区域设置</span><span class="sxs-lookup"><span data-stu-id="186db-188">Locale of the message set by the client</span></span>|
|<span data-ttu-id="186db-189">附件</span><span class="sxs-lookup"><span data-stu-id="186db-189">attachments</span></span>|<span data-ttu-id="186db-190">[chatMessageAttachment](chatattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="186db-190">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="186db-191">附加文件。</span><span class="sxs-lookup"><span data-stu-id="186db-191">Attached files</span></span> <span data-ttu-id="186db-192">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="186db-192">Attachments are currently read-only – sending attachments is not supported.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="186db-193">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="186db-193">JSON representation</span></span>

<span data-ttu-id="186db-194">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="186db-194">The following is a JSON representation of the resource.</span></span>

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
  "isDeleted": "boolean",
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
