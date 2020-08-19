---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 聊天消息可以是一个根聊天消息，也可以是由聊天消息中的 **replyToId** 属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 2b5c06b8b664c10483c8d4a6767a981f1a5551be
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812342"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="32b8a-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="32b8a-104">chatMessage resource type</span></span>

<span data-ttu-id="32b8a-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32b8a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="32b8a-106">代表 beta) [研讨](/graph/api/resources/chat?view=graph-rest-beta)中的[频道](./channel.md)或 (内的单个聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="32b8a-106">Represents an individual chat message within a [channel](./channel.md) or (in beta) [chat](/graph/api/resources/chat?view=graph-rest-beta).</span></span> <span data-ttu-id="32b8a-107">聊天消息可以是一个根聊天消息，也可以是由聊天消息中的 **replyToId** 属性定义的答复线程的一部分。</span><span class="sxs-lookup"><span data-stu-id="32b8a-107">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="32b8a-108">方法</span><span class="sxs-lookup"><span data-stu-id="32b8a-108">Methods</span></span>

| <span data-ttu-id="32b8a-109">方法</span><span class="sxs-lookup"><span data-stu-id="32b8a-109">Method</span></span>       | <span data-ttu-id="32b8a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="32b8a-110">Return Type</span></span>  |<span data-ttu-id="32b8a-111">说明</span><span class="sxs-lookup"><span data-stu-id="32b8a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32b8a-112">**通道邮件**</span><span class="sxs-lookup"><span data-stu-id="32b8a-112">**Channel messages**</span></span>| | |
|[<span data-ttu-id="32b8a-113">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="32b8a-113">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="32b8a-114">chatMessage</span><span class="sxs-lookup"><span data-stu-id="32b8a-114">chatMessage</span></span>](#chatmessage-resource-type)| <span data-ttu-id="32b8a-115">在频道中创建新的顶级聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="32b8a-115">Create a new top-level chat message in a channel.</span></span>|
|<span data-ttu-id="32b8a-116">**频道邮件答复**</span><span class="sxs-lookup"><span data-stu-id="32b8a-116">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="32b8a-117">答复频道中的了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="32b8a-117">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="32b8a-118">chatMessage</span><span class="sxs-lookup"><span data-stu-id="32b8a-118">chatMessage</span></span>](#chatmessage-resource-type)| <span data-ttu-id="32b8a-119">在频道中答复现有聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="32b8a-119">Reply to an existing chat message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="32b8a-120">属性</span><span class="sxs-lookup"><span data-stu-id="32b8a-120">Properties</span></span>

| <span data-ttu-id="32b8a-121">属性</span><span class="sxs-lookup"><span data-stu-id="32b8a-121">Property</span></span>   | <span data-ttu-id="32b8a-122">类型</span><span class="sxs-lookup"><span data-stu-id="32b8a-122">Type</span></span> |<span data-ttu-id="32b8a-123">说明</span><span class="sxs-lookup"><span data-stu-id="32b8a-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32b8a-124">id</span><span class="sxs-lookup"><span data-stu-id="32b8a-124">id</span></span>|<span data-ttu-id="32b8a-125">String</span><span class="sxs-lookup"><span data-stu-id="32b8a-125">String</span></span>| <span data-ttu-id="32b8a-126">只读。</span><span class="sxs-lookup"><span data-stu-id="32b8a-126">Read-only.</span></span> <span data-ttu-id="32b8a-127">邮件的唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="32b8a-127">Unique Id of the message.</span></span>|
|<span data-ttu-id="32b8a-128">replyToId</span><span class="sxs-lookup"><span data-stu-id="32b8a-128">replyToId</span></span>| <span data-ttu-id="32b8a-129">string</span><span class="sxs-lookup"><span data-stu-id="32b8a-129">string</span></span> | <span data-ttu-id="32b8a-130">只读。</span><span class="sxs-lookup"><span data-stu-id="32b8a-130">Read-only.</span></span> <span data-ttu-id="32b8a-131">线程的父聊天消息或根聊天消息的 Id。</span><span class="sxs-lookup"><span data-stu-id="32b8a-131">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="32b8a-132"> (仅适用于频道中不聊天的聊天消息) </span><span class="sxs-lookup"><span data-stu-id="32b8a-132">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="32b8a-133">from</span><span class="sxs-lookup"><span data-stu-id="32b8a-133">from</span></span>|[<span data-ttu-id="32b8a-134">identitySet</span><span class="sxs-lookup"><span data-stu-id="32b8a-134">identitySet</span></span>](identityset.md)| <span data-ttu-id="32b8a-135">只读。</span><span class="sxs-lookup"><span data-stu-id="32b8a-135">Read only.</span></span> <span data-ttu-id="32b8a-136">聊天消息发件人的详细信息。</span><span class="sxs-lookup"><span data-stu-id="32b8a-136">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="32b8a-137">etag</span><span class="sxs-lookup"><span data-stu-id="32b8a-137">etag</span></span>| <span data-ttu-id="32b8a-138">string</span><span class="sxs-lookup"><span data-stu-id="32b8a-138">string</span></span> | <span data-ttu-id="32b8a-139">只读。</span><span class="sxs-lookup"><span data-stu-id="32b8a-139">Read-only.</span></span> <span data-ttu-id="32b8a-140">聊天消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="32b8a-140">Version number of the chat message.</span></span> |
|<span data-ttu-id="32b8a-141">messageType</span><span class="sxs-lookup"><span data-stu-id="32b8a-141">messageType</span></span>|<span data-ttu-id="32b8a-142">string</span><span class="sxs-lookup"><span data-stu-id="32b8a-142">string</span></span>|<span data-ttu-id="32b8a-143">聊天消息的类型。</span><span class="sxs-lookup"><span data-stu-id="32b8a-143">The type of chat message.</span></span> <span data-ttu-id="32b8a-144">可能的值是： `message` 。</span><span class="sxs-lookup"><span data-stu-id="32b8a-144">The possible values are: `message`.</span></span>|
|<span data-ttu-id="32b8a-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32b8a-145">createdDateTime</span></span>|<span data-ttu-id="32b8a-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32b8a-146">dateTimeOffset</span></span>|<span data-ttu-id="32b8a-147">只读。</span><span class="sxs-lookup"><span data-stu-id="32b8a-147">Read only.</span></span> <span data-ttu-id="32b8a-148">在聊天消息创建时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="32b8a-148">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="32b8a-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32b8a-149">lastModifiedDateTime</span></span>|<span data-ttu-id="32b8a-150">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32b8a-150">dateTimeOffset</span></span>|<span data-ttu-id="32b8a-151">只读。</span><span class="sxs-lookup"><span data-stu-id="32b8a-151">Read only.</span></span> <span data-ttu-id="32b8a-152">在创建或编辑聊天消息时的时间戳，包括答复的时间 (如果它是频道中的根聊天消息) 或者添加或删除了反应。</span><span class="sxs-lookup"><span data-stu-id="32b8a-152">Timestamp of when the chat message is created or edited, including when a reply is made (if it's a root chat message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="32b8a-153">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="32b8a-153">deletedDateTime</span></span>|<span data-ttu-id="32b8a-154">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32b8a-154">dateTimeOffset</span></span>|<span data-ttu-id="32b8a-155">只读。</span><span class="sxs-lookup"><span data-stu-id="32b8a-155">Read only.</span></span> <span data-ttu-id="32b8a-156">删除聊天邮件的时间戳，如果未删除，则为 null。</span><span class="sxs-lookup"><span data-stu-id="32b8a-156">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="32b8a-157">subject</span><span class="sxs-lookup"><span data-stu-id="32b8a-157">subject</span></span>|<span data-ttu-id="32b8a-158">string</span><span class="sxs-lookup"><span data-stu-id="32b8a-158">string</span></span>| <span data-ttu-id="32b8a-159">聊天消息的主题，以纯文本形式。</span><span class="sxs-lookup"><span data-stu-id="32b8a-159">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="32b8a-160">body</span><span class="sxs-lookup"><span data-stu-id="32b8a-160">body</span></span>|[<span data-ttu-id="32b8a-161">itemBody</span><span class="sxs-lookup"><span data-stu-id="32b8a-161">itemBody</span></span>](itembody.md)|<span data-ttu-id="32b8a-162">聊天消息内容的纯文本/HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32b8a-162">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="32b8a-163">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="32b8a-163">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="32b8a-164">如果聊天消息包含 [chatMessageMention](chatmessagemention.md)，则该内容始终为 HTML。</span><span class="sxs-lookup"><span data-stu-id="32b8a-164">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="32b8a-165">摘要</span><span class="sxs-lookup"><span data-stu-id="32b8a-165">summary</span></span>|<span data-ttu-id="32b8a-166">string</span><span class="sxs-lookup"><span data-stu-id="32b8a-166">string</span></span>| <span data-ttu-id="32b8a-167">可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。</span><span class="sxs-lookup"><span data-stu-id="32b8a-167">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="32b8a-168">仅适用于频道聊天消息，而不是聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="32b8a-168">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="32b8a-169">附件</span><span class="sxs-lookup"><span data-stu-id="32b8a-169">attachments</span></span>|<span data-ttu-id="32b8a-170">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="32b8a-170">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="32b8a-171">附加文件。</span><span class="sxs-lookup"><span data-stu-id="32b8a-171">Attached files.</span></span> <span data-ttu-id="32b8a-172">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="32b8a-172">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="32b8a-173">提及</span><span class="sxs-lookup"><span data-stu-id="32b8a-173">mentions</span></span>|<span data-ttu-id="32b8a-174">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="32b8a-174">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="32b8a-175">聊天消息中提及的实体列表。</span><span class="sxs-lookup"><span data-stu-id="32b8a-175">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="32b8a-176">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="32b8a-176">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="32b8a-177">重要性</span><span class="sxs-lookup"><span data-stu-id="32b8a-177">importance</span></span>| <span data-ttu-id="32b8a-178">string</span><span class="sxs-lookup"><span data-stu-id="32b8a-178">string</span></span> | <span data-ttu-id="32b8a-179">聊天消息的重要性。</span><span class="sxs-lookup"><span data-stu-id="32b8a-179">The importance of the chat message.</span></span> <span data-ttu-id="32b8a-180">可能的值包括 `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="32b8a-180">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="32b8a-181">区域设置</span><span class="sxs-lookup"><span data-stu-id="32b8a-181">locale</span></span>|<span data-ttu-id="32b8a-182">string</span><span class="sxs-lookup"><span data-stu-id="32b8a-182">string</span></span>|<span data-ttu-id="32b8a-183">客户端的聊天消息的区域设置。</span><span class="sxs-lookup"><span data-stu-id="32b8a-183">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32b8a-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32b8a-184">JSON representation</span></span>

<span data-ttu-id="32b8a-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32b8a-185">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
