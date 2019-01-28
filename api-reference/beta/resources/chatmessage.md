---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。
localization_priority: Priority
ms.openlocfilehash: 98b9918d5763d6003a3c9a177057abe2e7b415ec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517965"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="1d6da-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d6da-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d6da-105">表示 [渠道](channel.md)或聊天实体内的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="1d6da-105">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="1d6da-106">该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。</span><span class="sxs-lookup"><span data-stu-id="1d6da-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="1d6da-107">方法</span><span class="sxs-lookup"><span data-stu-id="1d6da-107">Methods</span></span>

| <span data-ttu-id="1d6da-108">方法</span><span class="sxs-lookup"><span data-stu-id="1d6da-108">Method</span></span>       | <span data-ttu-id="1d6da-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1d6da-109">Return Type</span></span>  |<span data-ttu-id="1d6da-110">说明</span><span class="sxs-lookup"><span data-stu-id="1d6da-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1d6da-111">列出渠道消息</span><span class="sxs-lookup"><span data-stu-id="1d6da-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="1d6da-112">[chatmessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1d6da-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="1d6da-113">获取渠道中的所有根消息列表。</span><span class="sxs-lookup"><span data-stu-id="1d6da-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="1d6da-114">获取渠道消息</span><span class="sxs-lookup"><span data-stu-id="1d6da-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="1d6da-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="1d6da-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="1d6da-116">获取渠道中的单个根消息。</span><span class="sxs-lookup"><span data-stu-id="1d6da-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="1d6da-117">列出消息回复</span><span class="sxs-lookup"><span data-stu-id="1d6da-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="1d6da-118">[chatmessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1d6da-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="1d6da-119">获取渠道中的所有消息回复列表。</span><span class="sxs-lookup"><span data-stu-id="1d6da-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="1d6da-120">获取消息回复</span><span class="sxs-lookup"><span data-stu-id="1d6da-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="1d6da-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="1d6da-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="1d6da-122">获取渠道中的单个消息回复。</span><span class="sxs-lookup"><span data-stu-id="1d6da-122">Get a single reply to a message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="1d6da-123">属性</span><span class="sxs-lookup"><span data-stu-id="1d6da-123">Properties</span></span>
| <span data-ttu-id="1d6da-124">属性</span><span class="sxs-lookup"><span data-stu-id="1d6da-124">Property</span></span>     | <span data-ttu-id="1d6da-125">类型</span><span class="sxs-lookup"><span data-stu-id="1d6da-125">Type</span></span>   |<span data-ttu-id="1d6da-126">说明</span><span class="sxs-lookup"><span data-stu-id="1d6da-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d6da-127">id</span><span class="sxs-lookup"><span data-stu-id="1d6da-127">id</span></span>|<span data-ttu-id="1d6da-128">String</span><span class="sxs-lookup"><span data-stu-id="1d6da-128">String</span></span>| <span data-ttu-id="1d6da-129">只读。</span><span class="sxs-lookup"><span data-stu-id="1d6da-129">Read-only.</span></span> <span data-ttu-id="1d6da-130">消息的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="1d6da-130">Unique ID of the message.</span></span>|
|<span data-ttu-id="1d6da-131">replyToId</span><span class="sxs-lookup"><span data-stu-id="1d6da-131">replyToId</span></span>| <span data-ttu-id="1d6da-132">string</span><span class="sxs-lookup"><span data-stu-id="1d6da-132">string</span></span> | <span data-ttu-id="1d6da-133">线程的父级消息/根消息的 Id</span><span class="sxs-lookup"><span data-stu-id="1d6da-133">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="1d6da-134">from</span><span class="sxs-lookup"><span data-stu-id="1d6da-134">from</span></span>|[<span data-ttu-id="1d6da-135">identitySet</span><span class="sxs-lookup"><span data-stu-id="1d6da-135">identitySet</span></span>](identityset.md)| <span data-ttu-id="1d6da-136">消息发送者的详细信息</span><span class="sxs-lookup"><span data-stu-id="1d6da-136">Details of the sender of the message</span></span>|
|<span data-ttu-id="1d6da-137">etag</span><span class="sxs-lookup"><span data-stu-id="1d6da-137">etag</span></span>| <span data-ttu-id="1d6da-138">string</span><span class="sxs-lookup"><span data-stu-id="1d6da-138">string</span></span> | <span data-ttu-id="1d6da-139">消息的版本号</span><span class="sxs-lookup"><span data-stu-id="1d6da-139">Version number of the message</span></span> |
|<span data-ttu-id="1d6da-140">messageType</span><span class="sxs-lookup"><span data-stu-id="1d6da-140">messageType</span></span>|<span data-ttu-id="1d6da-141">String</span><span class="sxs-lookup"><span data-stu-id="1d6da-141">String</span></span>|<span data-ttu-id="1d6da-142">消息类型，当前支持的值包括：message、chatEvent、Typing</span><span class="sxs-lookup"><span data-stu-id="1d6da-142">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="1d6da-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d6da-143">createdDateTime</span></span>|<span data-ttu-id="1d6da-144">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d6da-144">dateTimeOffset</span></span>|<span data-ttu-id="1d6da-145">只读。</span><span class="sxs-lookup"><span data-stu-id="1d6da-145">Read only.</span></span> <span data-ttu-id="1d6da-146">创建消息时的时间戳</span><span class="sxs-lookup"><span data-stu-id="1d6da-146">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="1d6da-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d6da-147">lastModifiedDateTime</span></span>|<span data-ttu-id="1d6da-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d6da-148">dateTimeOffset</span></span>|<span data-ttu-id="1d6da-149">只读。</span><span class="sxs-lookup"><span data-stu-id="1d6da-149">Read only.</span></span> <span data-ttu-id="1d6da-150">编辑/更新消息时的时间戳</span><span class="sxs-lookup"><span data-stu-id="1d6da-150">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="1d6da-151">isDeleted</span><span class="sxs-lookup"><span data-stu-id="1d6da-151">isDeleted</span></span>|<span data-ttu-id="1d6da-152">boolean</span><span class="sxs-lookup"><span data-stu-id="1d6da-152">boolean</span></span>|<span data-ttu-id="1d6da-153">表示消息是否已被软删除</span><span class="sxs-lookup"><span data-stu-id="1d6da-153">Represents if a message has been soft deleted</span></span>|
|<span data-ttu-id="1d6da-154">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d6da-154">deletedDateTime</span></span>|<span data-ttu-id="1d6da-155">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d6da-155">dateTimeOffset</span></span>|<span data-ttu-id="1d6da-156">只读。</span><span class="sxs-lookup"><span data-stu-id="1d6da-156">Read only.</span></span> <span data-ttu-id="1d6da-157">删除消息时的时间戳</span><span class="sxs-lookup"><span data-stu-id="1d6da-157">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="1d6da-158">主题</span><span class="sxs-lookup"><span data-stu-id="1d6da-158">subject</span></span>|<span data-ttu-id="1d6da-159">string</span><span class="sxs-lookup"><span data-stu-id="1d6da-159">string</span></span>|<span data-ttu-id="1d6da-160">消息主题行。</span><span class="sxs-lookup"><span data-stu-id="1d6da-160">Message subject line.</span></span> <span data-ttu-id="1d6da-161">可选</span><span class="sxs-lookup"><span data-stu-id="1d6da-161">Optional</span></span>|
|<span data-ttu-id="1d6da-162">正文</span><span class="sxs-lookup"><span data-stu-id="1d6da-162">body</span></span>|[<span data-ttu-id="1d6da-163">itemBody</span><span class="sxs-lookup"><span data-stu-id="1d6da-163">itemBody</span></span>](itembody.md)|<span data-ttu-id="1d6da-164">消息内容的纯文本/HTML 表示。</span><span class="sxs-lookup"><span data-stu-id="1d6da-164">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="1d6da-165">默认返回纯文本，应用程序可选择 HTML 作为查询参数的一部分</span><span class="sxs-lookup"><span data-stu-id="1d6da-165">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="1d6da-166">摘要</span><span class="sxs-lookup"><span data-stu-id="1d6da-166">summary</span></span>|<span data-ttu-id="1d6da-167">string</span><span class="sxs-lookup"><span data-stu-id="1d6da-167">string</span></span>|<span data-ttu-id="1d6da-168">可用于推送通知的消息摘要文本和摘要视图或回退视图</span><span class="sxs-lookup"><span data-stu-id="1d6da-168">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="1d6da-169">提及</span><span class="sxs-lookup"><span data-stu-id="1d6da-169">mentions</span></span>|<span data-ttu-id="1d6da-170">[chatMessageMention](chatmention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1d6da-170">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="1d6da-171">消息中提到的实体列表。</span><span class="sxs-lookup"><span data-stu-id="1d6da-171">List of entities mentioned in the message.</span></span> <span data-ttu-id="1d6da-172">当前支持用户、机器人、团队、渠道</span><span class="sxs-lookup"><span data-stu-id="1d6da-172">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="1d6da-173">重要性</span><span class="sxs-lookup"><span data-stu-id="1d6da-173">importance</span></span>| <span data-ttu-id="1d6da-174">string</span><span class="sxs-lookup"><span data-stu-id="1d6da-174">string</span></span> | <span data-ttu-id="1d6da-175">消息重要性包括：正常、高</span><span class="sxs-lookup"><span data-stu-id="1d6da-175">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="1d6da-176">反应</span><span class="sxs-lookup"><span data-stu-id="1d6da-176">reactions</span></span>| <span data-ttu-id="1d6da-177">[chatMessageReaction](chatreaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1d6da-177">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="1d6da-178">此消息的反应（例如，赞）</span><span class="sxs-lookup"><span data-stu-id="1d6da-178">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="1d6da-179">区域设置</span><span class="sxs-lookup"><span data-stu-id="1d6da-179">locale</span></span>|<span data-ttu-id="1d6da-180">string</span><span class="sxs-lookup"><span data-stu-id="1d6da-180">string</span></span>|<span data-ttu-id="1d6da-181">客户设置的消息区域设置</span><span class="sxs-lookup"><span data-stu-id="1d6da-181">Locale of the message set by the client</span></span>|
|<span data-ttu-id="1d6da-182">附件</span><span class="sxs-lookup"><span data-stu-id="1d6da-182">attachments</span></span>|<span data-ttu-id="1d6da-183">[chatMessageAttachment](chatattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1d6da-183">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="1d6da-184">附加文件</span><span class="sxs-lookup"><span data-stu-id="1d6da-184">Attached files</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1d6da-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d6da-185">JSON representation</span></span>

<span data-ttu-id="1d6da-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d6da-186">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isDeleted",
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
