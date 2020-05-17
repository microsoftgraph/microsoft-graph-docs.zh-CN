---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 聊天消息可以是一个根聊天消息，也可以是由聊天消息中的**replyToId**属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 2030a208ed61b7137d22c29eee2743b67556c92d
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272754"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="32033-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="32033-104">chatMessage resource type</span></span>

<span data-ttu-id="32033-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32033-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="32033-106">代表[频道](./channel.md)内或（在 beta 中）[聊天](/graph/api/resources/chat?view=graph-rest-beta)中的单个聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="32033-106">Represents an individual chat message within a [channel](./channel.md) or (in beta) [chat](/graph/api/resources/chat?view=graph-rest-beta).</span></span> <span data-ttu-id="32033-107">聊天消息可以是一个根聊天消息，也可以是由聊天消息中的**replyToId**属性定义的答复线程的一部分。</span><span class="sxs-lookup"><span data-stu-id="32033-107">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="32033-108">Methods</span><span class="sxs-lookup"><span data-stu-id="32033-108">Methods</span></span>

| <span data-ttu-id="32033-109">方法</span><span class="sxs-lookup"><span data-stu-id="32033-109">Method</span></span>       | <span data-ttu-id="32033-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="32033-110">Return Type</span></span>  |<span data-ttu-id="32033-111">说明</span><span class="sxs-lookup"><span data-stu-id="32033-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32033-112">**通道邮件**</span><span class="sxs-lookup"><span data-stu-id="32033-112">**Channel messages**</span></span>| | |
|[<span data-ttu-id="32033-113">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="32033-113">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="32033-114">chatMessage</span><span class="sxs-lookup"><span data-stu-id="32033-114">chatMessage</span></span>](#chatmessage-resource-type)| <span data-ttu-id="32033-115">在频道中创建新的顶级聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="32033-115">Create a new top-level chat message in a channel.</span></span>|
|<span data-ttu-id="32033-116">**频道邮件答复**</span><span class="sxs-lookup"><span data-stu-id="32033-116">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="32033-117">答复频道中的了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="32033-117">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="32033-118">chatMessage</span><span class="sxs-lookup"><span data-stu-id="32033-118">chatMessage</span></span>](#chatmessage-resource-type)| <span data-ttu-id="32033-119">在频道中答复现有聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="32033-119">Reply to an existing chat message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="32033-120">属性</span><span class="sxs-lookup"><span data-stu-id="32033-120">Properties</span></span>

| <span data-ttu-id="32033-121">属性</span><span class="sxs-lookup"><span data-stu-id="32033-121">Property</span></span>   | <span data-ttu-id="32033-122">类型</span><span class="sxs-lookup"><span data-stu-id="32033-122">Type</span></span> |<span data-ttu-id="32033-123">说明</span><span class="sxs-lookup"><span data-stu-id="32033-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32033-124">id</span><span class="sxs-lookup"><span data-stu-id="32033-124">id</span></span>|<span data-ttu-id="32033-125">字符串</span><span class="sxs-lookup"><span data-stu-id="32033-125">String</span></span>| <span data-ttu-id="32033-126">只读。</span><span class="sxs-lookup"><span data-stu-id="32033-126">Read-only.</span></span> <span data-ttu-id="32033-127">邮件的唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="32033-127">Unique Id of the message.</span></span>|
|<span data-ttu-id="32033-128">replyToId</span><span class="sxs-lookup"><span data-stu-id="32033-128">replyToId</span></span>| <span data-ttu-id="32033-129">string</span><span class="sxs-lookup"><span data-stu-id="32033-129">string</span></span> | <span data-ttu-id="32033-130">只读。</span><span class="sxs-lookup"><span data-stu-id="32033-130">Read-only.</span></span> <span data-ttu-id="32033-131">线程的父聊天消息或根聊天消息的 Id。</span><span class="sxs-lookup"><span data-stu-id="32033-131">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="32033-132">（仅适用于通道中不聊天的聊天邮件）</span><span class="sxs-lookup"><span data-stu-id="32033-132">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="32033-133">from</span><span class="sxs-lookup"><span data-stu-id="32033-133">from</span></span>|[<span data-ttu-id="32033-134">identitySet</span><span class="sxs-lookup"><span data-stu-id="32033-134">identitySet</span></span>](identityset.md)| <span data-ttu-id="32033-135">只读。</span><span class="sxs-lookup"><span data-stu-id="32033-135">Read only.</span></span> <span data-ttu-id="32033-136">聊天消息发件人的详细信息。</span><span class="sxs-lookup"><span data-stu-id="32033-136">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="32033-137">etag</span><span class="sxs-lookup"><span data-stu-id="32033-137">etag</span></span>| <span data-ttu-id="32033-138">string</span><span class="sxs-lookup"><span data-stu-id="32033-138">string</span></span> | <span data-ttu-id="32033-139">只读。</span><span class="sxs-lookup"><span data-stu-id="32033-139">Read-only.</span></span> <span data-ttu-id="32033-140">聊天消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="32033-140">Version number of the chat message.</span></span> |
|<span data-ttu-id="32033-141">messageType</span><span class="sxs-lookup"><span data-stu-id="32033-141">messageType</span></span>|<span data-ttu-id="32033-142">string</span><span class="sxs-lookup"><span data-stu-id="32033-142">string</span></span>|<span data-ttu-id="32033-143">聊天消息的类型。</span><span class="sxs-lookup"><span data-stu-id="32033-143">The type of chat message.</span></span> <span data-ttu-id="32033-144">可能的值是： `message` 。</span><span class="sxs-lookup"><span data-stu-id="32033-144">The possible values are: `message`.</span></span>|
|<span data-ttu-id="32033-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32033-145">createdDateTime</span></span>|<span data-ttu-id="32033-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32033-146">dateTimeOffset</span></span>|<span data-ttu-id="32033-147">只读。</span><span class="sxs-lookup"><span data-stu-id="32033-147">Read only.</span></span> <span data-ttu-id="32033-148">在聊天消息创建时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="32033-148">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="32033-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32033-149">lastModifiedDateTime</span></span>|<span data-ttu-id="32033-150">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32033-150">dateTimeOffset</span></span>|<span data-ttu-id="32033-151">只读。</span><span class="sxs-lookup"><span data-stu-id="32033-151">Read only.</span></span> <span data-ttu-id="32033-152">在创建或编辑聊天消息时的时间戳，包括答复的时间（如果是频道中的根聊天邮件）或添加或删除了反应。</span><span class="sxs-lookup"><span data-stu-id="32033-152">Timestamp of when the chat message is created or edited, including when a reply is made (if it's a root chat message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="32033-153">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="32033-153">deletedDateTime</span></span>|<span data-ttu-id="32033-154">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32033-154">dateTimeOffset</span></span>|<span data-ttu-id="32033-155">只读。</span><span class="sxs-lookup"><span data-stu-id="32033-155">Read only.</span></span> <span data-ttu-id="32033-156">删除聊天邮件的时间戳，如果未删除，则为 null。</span><span class="sxs-lookup"><span data-stu-id="32033-156">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="32033-157">subject</span><span class="sxs-lookup"><span data-stu-id="32033-157">subject</span></span>|<span data-ttu-id="32033-158">string</span><span class="sxs-lookup"><span data-stu-id="32033-158">string</span></span>| <span data-ttu-id="32033-159">聊天消息的主题，以纯文本形式。</span><span class="sxs-lookup"><span data-stu-id="32033-159">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="32033-160">body</span><span class="sxs-lookup"><span data-stu-id="32033-160">body</span></span>|[<span data-ttu-id="32033-161">itemBody</span><span class="sxs-lookup"><span data-stu-id="32033-161">itemBody</span></span>](itembody.md)|<span data-ttu-id="32033-162">聊天消息内容的纯文本/HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32033-162">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="32033-163">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="32033-163">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="32033-164">如果聊天消息包含[chatMessageMention](chatmessagemention.md)，则该内容始终为 HTML。</span><span class="sxs-lookup"><span data-stu-id="32033-164">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="32033-165">摘要</span><span class="sxs-lookup"><span data-stu-id="32033-165">summary</span></span>|<span data-ttu-id="32033-166">string</span><span class="sxs-lookup"><span data-stu-id="32033-166">string</span></span>| <span data-ttu-id="32033-167">可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。</span><span class="sxs-lookup"><span data-stu-id="32033-167">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="32033-168">仅适用于频道聊天消息，而不是聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="32033-168">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="32033-169">附件</span><span class="sxs-lookup"><span data-stu-id="32033-169">attachments</span></span>|<span data-ttu-id="32033-170">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="32033-170">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="32033-171">附加文件。</span><span class="sxs-lookup"><span data-stu-id="32033-171">Attached files.</span></span> <span data-ttu-id="32033-172">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="32033-172">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="32033-173">提及</span><span class="sxs-lookup"><span data-stu-id="32033-173">mentions</span></span>|<span data-ttu-id="32033-174">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="32033-174">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="32033-175">聊天消息中提及的实体列表。</span><span class="sxs-lookup"><span data-stu-id="32033-175">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="32033-176">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="32033-176">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="32033-177">重要性</span><span class="sxs-lookup"><span data-stu-id="32033-177">importance</span></span>| <span data-ttu-id="32033-178">string</span><span class="sxs-lookup"><span data-stu-id="32033-178">string</span></span> | <span data-ttu-id="32033-179">聊天消息的重要性。</span><span class="sxs-lookup"><span data-stu-id="32033-179">The importance of the chat message.</span></span> <span data-ttu-id="32033-180">可能的值包括 `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="32033-180">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="32033-181">区域设置</span><span class="sxs-lookup"><span data-stu-id="32033-181">locale</span></span>|<span data-ttu-id="32033-182">string</span><span class="sxs-lookup"><span data-stu-id="32033-182">string</span></span>|<span data-ttu-id="32033-183">客户端的聊天消息的区域设置。</span><span class="sxs-lookup"><span data-stu-id="32033-183">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32033-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32033-184">JSON representation</span></span>

<span data-ttu-id="32033-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32033-185">The following is a JSON representation of the resource.</span></span>

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
  "locale": "string",
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
