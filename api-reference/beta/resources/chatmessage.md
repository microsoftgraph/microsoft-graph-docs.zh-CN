---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。
localization_priority: Priority
ms.openlocfilehash: f61668d8c3892482043dd7531a6699974a964527
ms.sourcegitcommit: d1a9e7c8e1376a99c5a5416257889ec113613a77
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/07/2019
ms.locfileid: "30458657"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="78f59-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="78f59-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78f59-105">表示 [渠道](channel.md)或聊天实体内的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="78f59-105">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="78f59-106">该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。</span><span class="sxs-lookup"><span data-stu-id="78f59-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="78f59-107">方法</span><span class="sxs-lookup"><span data-stu-id="78f59-107">Methods</span></span>

| <span data-ttu-id="78f59-108">方法</span><span class="sxs-lookup"><span data-stu-id="78f59-108">Method</span></span>       | <span data-ttu-id="78f59-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="78f59-109">Return Type</span></span>  |<span data-ttu-id="78f59-110">说明</span><span class="sxs-lookup"><span data-stu-id="78f59-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="78f59-111">列出渠道消息</span><span class="sxs-lookup"><span data-stu-id="78f59-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="78f59-112">[chatmessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="78f59-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="78f59-113">获取渠道中的所有根消息列表。</span><span class="sxs-lookup"><span data-stu-id="78f59-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="78f59-114">获取渠道消息</span><span class="sxs-lookup"><span data-stu-id="78f59-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="78f59-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="78f59-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="78f59-116">获取渠道中的单个根消息。</span><span class="sxs-lookup"><span data-stu-id="78f59-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="78f59-117">列出消息回复</span><span class="sxs-lookup"><span data-stu-id="78f59-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="78f59-118">[chatmessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="78f59-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="78f59-119">获取渠道中的所有消息回复列表。</span><span class="sxs-lookup"><span data-stu-id="78f59-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="78f59-120">获取消息回复</span><span class="sxs-lookup"><span data-stu-id="78f59-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="78f59-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="78f59-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="78f59-122">获取渠道中的单个消息回复。</span><span class="sxs-lookup"><span data-stu-id="78f59-122">Get a single reply to a message in a channel.</span></span>|
|<span data-ttu-id="78f59-123">[在渠道中发送消息](../api/channel-post-chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="78f59-123">Use [Create a message in a channel](../api/channel-post-chatmessage.md) instead.</span></span> | [<span data-ttu-id="78f59-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="78f59-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="78f59-125">在渠道中创建新的顶级消息。</span><span class="sxs-lookup"><span data-stu-id="78f59-125">Use Create a message in a channel instead.</span></span>|
|<span data-ttu-id="78f59-126">[在渠道中回复消息](../api/channel-post-messagereply.md)</span><span class="sxs-lookup"><span data-stu-id="78f59-126">Introduced the [Reply to a message in a channel](../api/channel-post-messagereply.md) API.</span></span> | [<span data-ttu-id="78f59-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="78f59-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="78f59-128">在渠道中回复现有消息。</span><span class="sxs-lookup"><span data-stu-id="78f59-128">Reply to an existing message in a channel.</span></span>|


## <a name="properties"></a><span data-ttu-id="78f59-129">属性</span><span class="sxs-lookup"><span data-stu-id="78f59-129">Properties</span></span>
| <span data-ttu-id="78f59-130">属性</span><span class="sxs-lookup"><span data-stu-id="78f59-130">Property</span></span>     | <span data-ttu-id="78f59-131">类型</span><span class="sxs-lookup"><span data-stu-id="78f59-131">Type</span></span>   |<span data-ttu-id="78f59-132">说明</span><span class="sxs-lookup"><span data-stu-id="78f59-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78f59-133">id</span><span class="sxs-lookup"><span data-stu-id="78f59-133">id</span></span>|<span data-ttu-id="78f59-134">String</span><span class="sxs-lookup"><span data-stu-id="78f59-134">String</span></span>| <span data-ttu-id="78f59-135">只读。</span><span class="sxs-lookup"><span data-stu-id="78f59-135">Read-only.</span></span> <span data-ttu-id="78f59-136">消息的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="78f59-136">Unique ID of the message.</span></span>|
|<span data-ttu-id="78f59-137">replyToId</span><span class="sxs-lookup"><span data-stu-id="78f59-137">replyToId</span></span>| <span data-ttu-id="78f59-138">string</span><span class="sxs-lookup"><span data-stu-id="78f59-138">string</span></span> | <span data-ttu-id="78f59-139">线程的父级消息/根消息的 Id</span><span class="sxs-lookup"><span data-stu-id="78f59-139">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="78f59-140">from</span><span class="sxs-lookup"><span data-stu-id="78f59-140">from</span></span>|[<span data-ttu-id="78f59-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="78f59-141">identitySet</span></span>](identityset.md)| <span data-ttu-id="78f59-142">消息发送者的详细信息</span><span class="sxs-lookup"><span data-stu-id="78f59-142">Details of the sender of the message</span></span>|
|<span data-ttu-id="78f59-143">etag</span><span class="sxs-lookup"><span data-stu-id="78f59-143">etag</span></span>| <span data-ttu-id="78f59-144">string</span><span class="sxs-lookup"><span data-stu-id="78f59-144">string</span></span> | <span data-ttu-id="78f59-145">消息的版本号</span><span class="sxs-lookup"><span data-stu-id="78f59-145">Version number of the message</span></span> |
|<span data-ttu-id="78f59-146">messageType</span><span class="sxs-lookup"><span data-stu-id="78f59-146">messageType</span></span>|<span data-ttu-id="78f59-147">String</span><span class="sxs-lookup"><span data-stu-id="78f59-147">String</span></span>|<span data-ttu-id="78f59-148">消息类型，当前支持的值包括：message、chatEvent、Typing</span><span class="sxs-lookup"><span data-stu-id="78f59-148">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="78f59-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="78f59-149">createdDateTime</span></span>|<span data-ttu-id="78f59-150">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78f59-150">dateTimeOffset</span></span>|<span data-ttu-id="78f59-151">只读。</span><span class="sxs-lookup"><span data-stu-id="78f59-151">Read only.</span></span> <span data-ttu-id="78f59-152">创建消息时的时间戳</span><span class="sxs-lookup"><span data-stu-id="78f59-152">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="78f59-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78f59-153">lastModifiedDateTime</span></span>|<span data-ttu-id="78f59-154">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78f59-154">dateTimeOffset</span></span>|<span data-ttu-id="78f59-155">只读。</span><span class="sxs-lookup"><span data-stu-id="78f59-155">Read only.</span></span> <span data-ttu-id="78f59-156">编辑/更新消息时的时间戳</span><span class="sxs-lookup"><span data-stu-id="78f59-156">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="78f59-157">deleted</span><span class="sxs-lookup"><span data-stu-id="78f59-157">deleted</span></span>|<span data-ttu-id="78f59-158">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f59-158">Boolean</span></span>|<span data-ttu-id="78f59-159">指示消息是否已被软删除</span><span class="sxs-lookup"><span data-stu-id="78f59-159">Indicates whether a message has been soft deleted</span></span>|
|<span data-ttu-id="78f59-160">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="78f59-160">deletedDateTime</span></span>|<span data-ttu-id="78f59-161">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78f59-161">dateTimeOffset</span></span>|<span data-ttu-id="78f59-162">只读。</span><span class="sxs-lookup"><span data-stu-id="78f59-162">Read only.</span></span> <span data-ttu-id="78f59-163">删除消息时的时间戳</span><span class="sxs-lookup"><span data-stu-id="78f59-163">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="78f59-164">主题</span><span class="sxs-lookup"><span data-stu-id="78f59-164">subject</span></span>|<span data-ttu-id="78f59-165">string</span><span class="sxs-lookup"><span data-stu-id="78f59-165">string</span></span>|<span data-ttu-id="78f59-166">消息主题行。</span><span class="sxs-lookup"><span data-stu-id="78f59-166">Message subject line.</span></span> <span data-ttu-id="78f59-167">可选</span><span class="sxs-lookup"><span data-stu-id="78f59-167">Optional</span></span>|
|<span data-ttu-id="78f59-168">正文</span><span class="sxs-lookup"><span data-stu-id="78f59-168">body</span></span>|[<span data-ttu-id="78f59-169">itemBody</span><span class="sxs-lookup"><span data-stu-id="78f59-169">itemBody</span></span>](itembody.md)|<span data-ttu-id="78f59-170">消息内容的纯文本/HTML 表示。</span><span class="sxs-lookup"><span data-stu-id="78f59-170">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="78f59-171">默认返回纯文本，应用程序可选择 HTML 作为查询参数的一部分</span><span class="sxs-lookup"><span data-stu-id="78f59-171">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="78f59-172">摘要</span><span class="sxs-lookup"><span data-stu-id="78f59-172">summary</span></span>|<span data-ttu-id="78f59-173">string</span><span class="sxs-lookup"><span data-stu-id="78f59-173">string</span></span>|<span data-ttu-id="78f59-174">可用于推送通知的消息摘要文本和摘要视图或回退视图</span><span class="sxs-lookup"><span data-stu-id="78f59-174">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="78f59-175">提及</span><span class="sxs-lookup"><span data-stu-id="78f59-175">mentions</span></span>|<span data-ttu-id="78f59-176">[chatMessageMention](chatmention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="78f59-176">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="78f59-177">消息中提到的实体列表。</span><span class="sxs-lookup"><span data-stu-id="78f59-177">List of entities mentioned in the message.</span></span> <span data-ttu-id="78f59-178">当前支持用户、机器人、团队、渠道</span><span class="sxs-lookup"><span data-stu-id="78f59-178">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="78f59-179">重要性</span><span class="sxs-lookup"><span data-stu-id="78f59-179">importance</span></span>| <span data-ttu-id="78f59-180">string</span><span class="sxs-lookup"><span data-stu-id="78f59-180">string</span></span> | <span data-ttu-id="78f59-181">消息重要性包括：正常、高</span><span class="sxs-lookup"><span data-stu-id="78f59-181">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="78f59-182">反应</span><span class="sxs-lookup"><span data-stu-id="78f59-182">reactions</span></span>| <span data-ttu-id="78f59-183">[chatMessageReaction](chatreaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="78f59-183">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="78f59-184">此消息的反应（例如，赞）</span><span class="sxs-lookup"><span data-stu-id="78f59-184">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="78f59-185">区域设置</span><span class="sxs-lookup"><span data-stu-id="78f59-185">locale</span></span>|<span data-ttu-id="78f59-186">string</span><span class="sxs-lookup"><span data-stu-id="78f59-186">string</span></span>|<span data-ttu-id="78f59-187">客户设置的消息区域设置</span><span class="sxs-lookup"><span data-stu-id="78f59-187">Locale of the message set by the client</span></span>|
|<span data-ttu-id="78f59-188">附件</span><span class="sxs-lookup"><span data-stu-id="78f59-188">attachments</span></span>|<span data-ttu-id="78f59-189">[chatMessageAttachment](chatattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="78f59-189">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="78f59-190">附加文件</span><span class="sxs-lookup"><span data-stu-id="78f59-190">Attached files</span></span>|


## <a name="json-representation"></a><span data-ttu-id="78f59-191">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78f59-191">JSON representation</span></span>

<span data-ttu-id="78f59-192">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78f59-192">The following is a JSON representation of the resource.</span></span>

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
