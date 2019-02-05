---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。
localization_priority: Priority
ms.openlocfilehash: ef91281eff0cc61f992f659bd33debec03841bb4
ms.sourcegitcommit: a1f1e59ee568340bfabdb524e01cff7860bcc862
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2019
ms.locfileid: "29735577"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="286e2-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="286e2-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="286e2-105">表示 [渠道](channel.md)或聊天实体内的单个聊天信息。</span><span class="sxs-lookup"><span data-stu-id="286e2-105">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="286e2-106">该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。</span><span class="sxs-lookup"><span data-stu-id="286e2-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="286e2-107">方法</span><span class="sxs-lookup"><span data-stu-id="286e2-107">Methods</span></span>

| <span data-ttu-id="286e2-108">方法</span><span class="sxs-lookup"><span data-stu-id="286e2-108">Method</span></span>       | <span data-ttu-id="286e2-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="286e2-109">Return Type</span></span>  |<span data-ttu-id="286e2-110">说明</span><span class="sxs-lookup"><span data-stu-id="286e2-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="286e2-111">列出渠道消息</span><span class="sxs-lookup"><span data-stu-id="286e2-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="286e2-112">[chatmessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="286e2-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="286e2-113">获取渠道中的所有根消息列表。</span><span class="sxs-lookup"><span data-stu-id="286e2-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="286e2-114">获取渠道消息</span><span class="sxs-lookup"><span data-stu-id="286e2-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="286e2-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="286e2-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="286e2-116">获取渠道中的单个根消息。</span><span class="sxs-lookup"><span data-stu-id="286e2-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="286e2-117">列出消息回复</span><span class="sxs-lookup"><span data-stu-id="286e2-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="286e2-118">[chatmessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="286e2-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="286e2-119">获取渠道中的所有消息回复列表。</span><span class="sxs-lookup"><span data-stu-id="286e2-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="286e2-120">获取消息回复</span><span class="sxs-lookup"><span data-stu-id="286e2-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="286e2-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="286e2-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="286e2-122">获取渠道中的单个消息回复。</span><span class="sxs-lookup"><span data-stu-id="286e2-122">Get a single reply to a message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="286e2-123">属性</span><span class="sxs-lookup"><span data-stu-id="286e2-123">Properties</span></span>
| <span data-ttu-id="286e2-124">属性</span><span class="sxs-lookup"><span data-stu-id="286e2-124">Property</span></span>     | <span data-ttu-id="286e2-125">类型</span><span class="sxs-lookup"><span data-stu-id="286e2-125">Type</span></span>   |<span data-ttu-id="286e2-126">说明</span><span class="sxs-lookup"><span data-stu-id="286e2-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="286e2-127">id</span><span class="sxs-lookup"><span data-stu-id="286e2-127">id</span></span>|<span data-ttu-id="286e2-128">String</span><span class="sxs-lookup"><span data-stu-id="286e2-128">String</span></span>| <span data-ttu-id="286e2-129">只读。</span><span class="sxs-lookup"><span data-stu-id="286e2-129">Read-only.</span></span> <span data-ttu-id="286e2-130">消息的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="286e2-130">Unique ID of the message.</span></span>|
|<span data-ttu-id="286e2-131">replyToId</span><span class="sxs-lookup"><span data-stu-id="286e2-131">replyToId</span></span>| <span data-ttu-id="286e2-132">string</span><span class="sxs-lookup"><span data-stu-id="286e2-132">string</span></span> | <span data-ttu-id="286e2-133">线程的父级消息/根消息的 Id</span><span class="sxs-lookup"><span data-stu-id="286e2-133">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="286e2-134">from</span><span class="sxs-lookup"><span data-stu-id="286e2-134">from</span></span>|[<span data-ttu-id="286e2-135">identitySet</span><span class="sxs-lookup"><span data-stu-id="286e2-135">identitySet</span></span>](identityset.md)| <span data-ttu-id="286e2-136">消息发送者的详细信息</span><span class="sxs-lookup"><span data-stu-id="286e2-136">Details of the sender of the message</span></span>|
|<span data-ttu-id="286e2-137">etag</span><span class="sxs-lookup"><span data-stu-id="286e2-137">etag</span></span>| <span data-ttu-id="286e2-138">string</span><span class="sxs-lookup"><span data-stu-id="286e2-138">string</span></span> | <span data-ttu-id="286e2-139">消息的版本号</span><span class="sxs-lookup"><span data-stu-id="286e2-139">Version number of the message</span></span> |
|<span data-ttu-id="286e2-140">messageType</span><span class="sxs-lookup"><span data-stu-id="286e2-140">messageType</span></span>|<span data-ttu-id="286e2-141">String</span><span class="sxs-lookup"><span data-stu-id="286e2-141">String</span></span>|<span data-ttu-id="286e2-142">消息类型，当前支持的值包括：message、chatEvent、Typing</span><span class="sxs-lookup"><span data-stu-id="286e2-142">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="286e2-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="286e2-143">createdDateTime</span></span>|<span data-ttu-id="286e2-144">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="286e2-144">dateTimeOffset</span></span>|<span data-ttu-id="286e2-145">只读。</span><span class="sxs-lookup"><span data-stu-id="286e2-145">Read only.</span></span> <span data-ttu-id="286e2-146">创建消息时的时间戳</span><span class="sxs-lookup"><span data-stu-id="286e2-146">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="286e2-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="286e2-147">lastModifiedDateTime</span></span>|<span data-ttu-id="286e2-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="286e2-148">dateTimeOffset</span></span>|<span data-ttu-id="286e2-149">只读。</span><span class="sxs-lookup"><span data-stu-id="286e2-149">Read only.</span></span> <span data-ttu-id="286e2-150">编辑/更新消息时的时间戳</span><span class="sxs-lookup"><span data-stu-id="286e2-150">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="286e2-151">deleted</span><span class="sxs-lookup"><span data-stu-id="286e2-151">deleted</span></span>|<span data-ttu-id="286e2-152">布尔值</span><span class="sxs-lookup"><span data-stu-id="286e2-152">Boolean</span></span>|<span data-ttu-id="286e2-153">指示消息是否已被软删除</span><span class="sxs-lookup"><span data-stu-id="286e2-153">Represents if a message has been soft deleted</span></span>|
|<span data-ttu-id="286e2-154">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="286e2-154">deletedDateTime</span></span>|<span data-ttu-id="286e2-155">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="286e2-155">dateTimeOffset</span></span>|<span data-ttu-id="286e2-156">只读。</span><span class="sxs-lookup"><span data-stu-id="286e2-156">Read only.</span></span> <span data-ttu-id="286e2-157">删除消息时的时间戳</span><span class="sxs-lookup"><span data-stu-id="286e2-157">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="286e2-158">主题</span><span class="sxs-lookup"><span data-stu-id="286e2-158">subject</span></span>|<span data-ttu-id="286e2-159">string</span><span class="sxs-lookup"><span data-stu-id="286e2-159">string</span></span>|<span data-ttu-id="286e2-160">消息主题行。</span><span class="sxs-lookup"><span data-stu-id="286e2-160">Message subject line.</span></span> <span data-ttu-id="286e2-161">可选</span><span class="sxs-lookup"><span data-stu-id="286e2-161">Optional</span></span>|
|<span data-ttu-id="286e2-162">正文</span><span class="sxs-lookup"><span data-stu-id="286e2-162">body</span></span>|[<span data-ttu-id="286e2-163">itemBody</span><span class="sxs-lookup"><span data-stu-id="286e2-163">itemBody</span></span>](itembody.md)|<span data-ttu-id="286e2-164">消息内容的纯文本/HTML 表示。</span><span class="sxs-lookup"><span data-stu-id="286e2-164">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="286e2-165">默认返回纯文本，应用程序可选择 HTML 作为查询参数的一部分</span><span class="sxs-lookup"><span data-stu-id="286e2-165">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="286e2-166">摘要</span><span class="sxs-lookup"><span data-stu-id="286e2-166">summary</span></span>|<span data-ttu-id="286e2-167">string</span><span class="sxs-lookup"><span data-stu-id="286e2-167">string</span></span>|<span data-ttu-id="286e2-168">可用于推送通知的消息摘要文本和摘要视图或回退视图</span><span class="sxs-lookup"><span data-stu-id="286e2-168">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="286e2-169">提及</span><span class="sxs-lookup"><span data-stu-id="286e2-169">mentions</span></span>|<span data-ttu-id="286e2-170">[chatMessageMention](chatmention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="286e2-170">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="286e2-171">消息中提到的实体列表。</span><span class="sxs-lookup"><span data-stu-id="286e2-171">List of entities mentioned in the message.</span></span> <span data-ttu-id="286e2-172">当前支持用户、机器人、团队、渠道</span><span class="sxs-lookup"><span data-stu-id="286e2-172">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="286e2-173">重要性</span><span class="sxs-lookup"><span data-stu-id="286e2-173">importance</span></span>| <span data-ttu-id="286e2-174">string</span><span class="sxs-lookup"><span data-stu-id="286e2-174">string</span></span> | <span data-ttu-id="286e2-175">消息重要性包括：正常、高</span><span class="sxs-lookup"><span data-stu-id="286e2-175">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="286e2-176">反应</span><span class="sxs-lookup"><span data-stu-id="286e2-176">reactions</span></span>| <span data-ttu-id="286e2-177">[chatMessageReaction](chatreaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="286e2-177">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="286e2-178">此消息的反应（例如，赞）</span><span class="sxs-lookup"><span data-stu-id="286e2-178">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="286e2-179">区域设置</span><span class="sxs-lookup"><span data-stu-id="286e2-179">locale</span></span>|<span data-ttu-id="286e2-180">string</span><span class="sxs-lookup"><span data-stu-id="286e2-180">string</span></span>|<span data-ttu-id="286e2-181">客户设置的消息区域设置</span><span class="sxs-lookup"><span data-stu-id="286e2-181">Locale of the message set by the client</span></span>|
|<span data-ttu-id="286e2-182">附件</span><span class="sxs-lookup"><span data-stu-id="286e2-182">attachments</span></span>|<span data-ttu-id="286e2-183">[chatMessageAttachment](chatattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="286e2-183">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="286e2-184">附加文件</span><span class="sxs-lookup"><span data-stu-id="286e2-184">Attached files</span></span>|


## <a name="json-representation"></a><span data-ttu-id="286e2-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="286e2-185">JSON representation</span></span>

<span data-ttu-id="286e2-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="286e2-186">The following is a JSON representation of the resource.</span></span>

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
