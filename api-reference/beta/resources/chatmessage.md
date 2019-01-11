---
title: chatMessage 资源类型
description: 代表单个聊天消息中的通道或聊天实体。 消息能为根邮件或由**replyToId**属性在消息中定义的线程的一部分。
localization_priority: Priority
ms.openlocfilehash: ad381102f7e93a4dcccd7b68435d0687ed6b4837
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855990"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="e5f63-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5f63-104">chatMessage resource type</span></span>

> <span data-ttu-id="e5f63-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e5f63-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5f63-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e5f63-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5f63-107">代表单个聊天消息中的[通道](channel.md)或聊天实体。</span><span class="sxs-lookup"><span data-stu-id="e5f63-107">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="e5f63-108">消息能为根邮件或由**replyToId**属性在消息中定义的线程的一部分。</span><span class="sxs-lookup"><span data-stu-id="e5f63-108">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="e5f63-109">方法</span><span class="sxs-lookup"><span data-stu-id="e5f63-109">Methods</span></span>

| <span data-ttu-id="e5f63-110">方法</span><span class="sxs-lookup"><span data-stu-id="e5f63-110">Method</span></span>       | <span data-ttu-id="e5f63-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="e5f63-111">Return Type</span></span>  |<span data-ttu-id="e5f63-112">说明</span><span class="sxs-lookup"><span data-stu-id="e5f63-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e5f63-113">列表通道消息</span><span class="sxs-lookup"><span data-stu-id="e5f63-113">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="e5f63-114">[chatmessage](chatmessage.md)集合</span><span class="sxs-lookup"><span data-stu-id="e5f63-114">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="e5f63-115">在通道中获取的所有根邮件的列表。</span><span class="sxs-lookup"><span data-stu-id="e5f63-115">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="e5f63-116">Get 频道消息</span><span class="sxs-lookup"><span data-stu-id="e5f63-116">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="e5f63-117">chatmessage</span><span class="sxs-lookup"><span data-stu-id="e5f63-117">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="e5f63-118">从通道中获取单个根消息。</span><span class="sxs-lookup"><span data-stu-id="e5f63-118">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="e5f63-119">列表回复到一条消息</span><span class="sxs-lookup"><span data-stu-id="e5f63-119">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="e5f63-120">[chatmessage](chatmessage.md)集合</span><span class="sxs-lookup"><span data-stu-id="e5f63-120">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="e5f63-121">在通道中获取所有回复到一条消息的列表。</span><span class="sxs-lookup"><span data-stu-id="e5f63-121">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="e5f63-122">获取邮件答复</span><span class="sxs-lookup"><span data-stu-id="e5f63-122">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="e5f63-123">chatmessage</span><span class="sxs-lookup"><span data-stu-id="e5f63-123">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="e5f63-124">在通道中获取单个邮件答复。</span><span class="sxs-lookup"><span data-stu-id="e5f63-124">Get a single reply to a message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="e5f63-125">属性</span><span class="sxs-lookup"><span data-stu-id="e5f63-125">Properties</span></span>
| <span data-ttu-id="e5f63-126">属性</span><span class="sxs-lookup"><span data-stu-id="e5f63-126">Property</span></span>     | <span data-ttu-id="e5f63-127">类型</span><span class="sxs-lookup"><span data-stu-id="e5f63-127">Type</span></span>   |<span data-ttu-id="e5f63-128">说明</span><span class="sxs-lookup"><span data-stu-id="e5f63-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5f63-129">id</span><span class="sxs-lookup"><span data-stu-id="e5f63-129">id</span></span>|<span data-ttu-id="e5f63-130">String</span><span class="sxs-lookup"><span data-stu-id="e5f63-130">String</span></span>| <span data-ttu-id="e5f63-131">只读。</span><span class="sxs-lookup"><span data-stu-id="e5f63-131">Read-only.</span></span> <span data-ttu-id="e5f63-132">邮件的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="e5f63-132">Unique ID of the message.</span></span>|
|<span data-ttu-id="e5f63-133">replyToId</span><span class="sxs-lookup"><span data-stu-id="e5f63-133">replyToId</span></span>| <span data-ttu-id="e5f63-134">string</span><span class="sxs-lookup"><span data-stu-id="e5f63-134">string</span></span> | <span data-ttu-id="e5f63-135">父消息/根邮件的主题的 id</span><span class="sxs-lookup"><span data-stu-id="e5f63-135">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="e5f63-136">发件人</span><span class="sxs-lookup"><span data-stu-id="e5f63-136">from</span></span>|[<span data-ttu-id="e5f63-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="e5f63-137">identitySet</span></span>](identityset.md)| <span data-ttu-id="e5f63-138">发件人的邮件的详细信息</span><span class="sxs-lookup"><span data-stu-id="e5f63-138">Details of the sender of the message</span></span>|
|<span data-ttu-id="e5f63-139">etag</span><span class="sxs-lookup"><span data-stu-id="e5f63-139">etag</span></span>| <span data-ttu-id="e5f63-140">string</span><span class="sxs-lookup"><span data-stu-id="e5f63-140">string</span></span> | <span data-ttu-id="e5f63-141">邮件的版本号</span><span class="sxs-lookup"><span data-stu-id="e5f63-141">Version number of the message</span></span> |
|<span data-ttu-id="e5f63-142">messageType</span><span class="sxs-lookup"><span data-stu-id="e5f63-142">messageType</span></span>|<span data-ttu-id="e5f63-143">字符串</span><span class="sxs-lookup"><span data-stu-id="e5f63-143">String</span></span>|<span data-ttu-id="e5f63-144">支持的邮件，当前的类型的值为： 消息，chatEvent，键入</span><span class="sxs-lookup"><span data-stu-id="e5f63-144">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="e5f63-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5f63-145">createdDateTime</span></span>|<span data-ttu-id="e5f63-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5f63-146">dateTimeOffset</span></span>|<span data-ttu-id="e5f63-147">只读。</span><span class="sxs-lookup"><span data-stu-id="e5f63-147">Read only.</span></span> <span data-ttu-id="e5f63-148">创建邮件时的时间戳</span><span class="sxs-lookup"><span data-stu-id="e5f63-148">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="e5f63-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5f63-149">lastModifiedDateTime</span></span>|<span data-ttu-id="e5f63-150">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5f63-150">dateTimeOffset</span></span>|<span data-ttu-id="e5f63-151">只读。</span><span class="sxs-lookup"><span data-stu-id="e5f63-151">Read only.</span></span> <span data-ttu-id="e5f63-152">时间戳的邮件时编辑更新</span><span class="sxs-lookup"><span data-stu-id="e5f63-152">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="e5f63-153">被</span><span class="sxs-lookup"><span data-stu-id="e5f63-153">isDeleted</span></span>|<span data-ttu-id="e5f63-154">boolean</span><span class="sxs-lookup"><span data-stu-id="e5f63-154">boolean</span></span>|<span data-ttu-id="e5f63-155">如果已软删除一条消息，表示</span><span class="sxs-lookup"><span data-stu-id="e5f63-155">Represents if a message has been soft deleted</span></span>|
|<span data-ttu-id="e5f63-156">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5f63-156">deletedDateTime</span></span>|<span data-ttu-id="e5f63-157">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5f63-157">dateTimeOffset</span></span>|<span data-ttu-id="e5f63-158">只读。</span><span class="sxs-lookup"><span data-stu-id="e5f63-158">Read only.</span></span> <span data-ttu-id="e5f63-159">邮件已被删除的时间戳</span><span class="sxs-lookup"><span data-stu-id="e5f63-159">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="e5f63-160">subject</span><span class="sxs-lookup"><span data-stu-id="e5f63-160">subject</span></span>|<span data-ttu-id="e5f63-161">string</span><span class="sxs-lookup"><span data-stu-id="e5f63-161">string</span></span>|<span data-ttu-id="e5f63-162">邮件主题行。</span><span class="sxs-lookup"><span data-stu-id="e5f63-162">Message subject line.</span></span> <span data-ttu-id="e5f63-163">可选</span><span class="sxs-lookup"><span data-stu-id="e5f63-163">Optional</span></span>|
|<span data-ttu-id="e5f63-164">body</span><span class="sxs-lookup"><span data-stu-id="e5f63-164">body</span></span>|[<span data-ttu-id="e5f63-165">itemBody</span><span class="sxs-lookup"><span data-stu-id="e5f63-165">itemBody</span></span>](itembody.md)|<span data-ttu-id="e5f63-166">纯文本/HTML 表示形式的消息内容。</span><span class="sxs-lookup"><span data-stu-id="e5f63-166">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="e5f63-167">返回纯文本默认情况下应用程序可以查询参数的一部分选择 HTML</span><span class="sxs-lookup"><span data-stu-id="e5f63-167">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="e5f63-168">摘要</span><span class="sxs-lookup"><span data-stu-id="e5f63-168">summary</span></span>|<span data-ttu-id="e5f63-169">string</span><span class="sxs-lookup"><span data-stu-id="e5f63-169">string</span></span>|<span data-ttu-id="e5f63-170">摘要无法用于推送通知和摘要视图或秋季后视图的消息文本</span><span class="sxs-lookup"><span data-stu-id="e5f63-170">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="e5f63-171">提及</span><span class="sxs-lookup"><span data-stu-id="e5f63-171">mentions</span></span>|<span data-ttu-id="e5f63-172">[chatMessageMention](chatmention.md)集合</span><span class="sxs-lookup"><span data-stu-id="e5f63-172">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="e5f63-173">消息中提到的实体的列表。</span><span class="sxs-lookup"><span data-stu-id="e5f63-173">List of entities mentioned in the message.</span></span> <span data-ttu-id="e5f63-174">当前支持用户、 自动程序、 团队和通道</span><span class="sxs-lookup"><span data-stu-id="e5f63-174">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="e5f63-175">importance</span><span class="sxs-lookup"><span data-stu-id="e5f63-175">importance</span></span>| <span data-ttu-id="e5f63-176">string</span><span class="sxs-lookup"><span data-stu-id="e5f63-176">string</span></span> | <span data-ttu-id="e5f63-177">邮件的重要性： 普通、 高</span><span class="sxs-lookup"><span data-stu-id="e5f63-177">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="e5f63-178">反应的方式</span><span class="sxs-lookup"><span data-stu-id="e5f63-178">reactions</span></span>| <span data-ttu-id="e5f63-179">[chatMessageReaction](chatreaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="e5f63-179">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="e5f63-180">此消息的反应的方式 （例如，如）</span><span class="sxs-lookup"><span data-stu-id="e5f63-180">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="e5f63-181">区域设置</span><span class="sxs-lookup"><span data-stu-id="e5f63-181">locale</span></span>|<span data-ttu-id="e5f63-182">string</span><span class="sxs-lookup"><span data-stu-id="e5f63-182">string</span></span>|<span data-ttu-id="e5f63-183">设置由客户端消息的区域设置</span><span class="sxs-lookup"><span data-stu-id="e5f63-183">Locale of the message set by the client</span></span>|
|<span data-ttu-id="e5f63-184">attachments</span><span class="sxs-lookup"><span data-stu-id="e5f63-184">attachments</span></span>|<span data-ttu-id="e5f63-185">[chatMessageAttachment](chatattachment.md)集合</span><span class="sxs-lookup"><span data-stu-id="e5f63-185">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="e5f63-186">附加的文件</span><span class="sxs-lookup"><span data-stu-id="e5f63-186">Attached files</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e5f63-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5f63-187">JSON representation</span></span>

<span data-ttu-id="e5f63-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5f63-188">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
