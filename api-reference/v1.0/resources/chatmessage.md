---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 聊天消息可以是一个根聊天消息，也可以是由聊天消息中的 **replyToId** 属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: af025ad2484757626fec08d9131a870cb345e492
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223210"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="0420f-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="0420f-104">chatMessage resource type</span></span>

<span data-ttu-id="0420f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0420f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0420f-106">代表 beta) [研讨](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)中的[频道](./channel.md)或 (内的单个聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="0420f-106">Represents an individual chat message within a [channel](./channel.md) or (in beta) [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="0420f-107">聊天消息可以是一个根聊天消息，也可以是由聊天消息中的 **replyToId** 属性定义的答复线程的一部分。</span><span class="sxs-lookup"><span data-stu-id="0420f-107">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="0420f-108">方法</span><span class="sxs-lookup"><span data-stu-id="0420f-108">Methods</span></span>

| <span data-ttu-id="0420f-109">方法</span><span class="sxs-lookup"><span data-stu-id="0420f-109">Method</span></span>       | <span data-ttu-id="0420f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0420f-110">Return Type</span></span>  |<span data-ttu-id="0420f-111">说明</span><span class="sxs-lookup"><span data-stu-id="0420f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0420f-112">**通道邮件**</span><span class="sxs-lookup"><span data-stu-id="0420f-112">**Channel messages**</span></span>| | |
|[<span data-ttu-id="0420f-113">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="0420f-113">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="0420f-114">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0420f-114">chatMessage</span></span>](#chatmessage-resource-type)| <span data-ttu-id="0420f-115">在频道中创建新的顶级聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="0420f-115">Create a new top-level chat message in a channel.</span></span>|
|[<span data-ttu-id="0420f-116">更新了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="0420f-116">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="0420f-117">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0420f-117">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="0420f-118">更新聊天邮件的 **policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="0420f-118">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="0420f-119">**频道邮件答复**</span><span class="sxs-lookup"><span data-stu-id="0420f-119">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="0420f-120">答复频道中的了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="0420f-120">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="0420f-121">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0420f-121">chatMessage</span></span>](#chatmessage-resource-type)| <span data-ttu-id="0420f-122">在频道中答复现有聊天邮件。</span><span class="sxs-lookup"><span data-stu-id="0420f-122">Reply to an existing chat message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="0420f-123">属性</span><span class="sxs-lookup"><span data-stu-id="0420f-123">Properties</span></span>

| <span data-ttu-id="0420f-124">属性</span><span class="sxs-lookup"><span data-stu-id="0420f-124">Property</span></span>   | <span data-ttu-id="0420f-125">类型</span><span class="sxs-lookup"><span data-stu-id="0420f-125">Type</span></span> |<span data-ttu-id="0420f-126">说明</span><span class="sxs-lookup"><span data-stu-id="0420f-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0420f-127">id</span><span class="sxs-lookup"><span data-stu-id="0420f-127">id</span></span>|<span data-ttu-id="0420f-128">字符串</span><span class="sxs-lookup"><span data-stu-id="0420f-128">String</span></span>| <span data-ttu-id="0420f-129">只读。</span><span class="sxs-lookup"><span data-stu-id="0420f-129">Read-only.</span></span> <span data-ttu-id="0420f-130">邮件的唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="0420f-130">Unique Id of the message.</span></span>|
|<span data-ttu-id="0420f-131">replyToId</span><span class="sxs-lookup"><span data-stu-id="0420f-131">replyToId</span></span>| <span data-ttu-id="0420f-132">string</span><span class="sxs-lookup"><span data-stu-id="0420f-132">string</span></span> | <span data-ttu-id="0420f-133">只读。</span><span class="sxs-lookup"><span data-stu-id="0420f-133">Read-only.</span></span> <span data-ttu-id="0420f-134">线程的父聊天消息或根聊天消息的 Id。</span><span class="sxs-lookup"><span data-stu-id="0420f-134">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="0420f-135"> (仅适用于频道中不聊天的聊天消息) </span><span class="sxs-lookup"><span data-stu-id="0420f-135">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="0420f-136">from</span><span class="sxs-lookup"><span data-stu-id="0420f-136">from</span></span>|[<span data-ttu-id="0420f-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="0420f-137">identitySet</span></span>](identityset.md)| <span data-ttu-id="0420f-138">只读。</span><span class="sxs-lookup"><span data-stu-id="0420f-138">Read only.</span></span> <span data-ttu-id="0420f-139">聊天消息发件人的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0420f-139">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="0420f-140">etag</span><span class="sxs-lookup"><span data-stu-id="0420f-140">etag</span></span>| <span data-ttu-id="0420f-141">string</span><span class="sxs-lookup"><span data-stu-id="0420f-141">string</span></span> | <span data-ttu-id="0420f-142">只读。</span><span class="sxs-lookup"><span data-stu-id="0420f-142">Read-only.</span></span> <span data-ttu-id="0420f-143">聊天消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="0420f-143">Version number of the chat message.</span></span> |
|<span data-ttu-id="0420f-144">messageType</span><span class="sxs-lookup"><span data-stu-id="0420f-144">messageType</span></span>|<span data-ttu-id="0420f-145">string</span><span class="sxs-lookup"><span data-stu-id="0420f-145">string</span></span>|<span data-ttu-id="0420f-146">聊天消息的类型。</span><span class="sxs-lookup"><span data-stu-id="0420f-146">The type of chat message.</span></span> <span data-ttu-id="0420f-147">可能的值是： `message` 。</span><span class="sxs-lookup"><span data-stu-id="0420f-147">The possible values are: `message`.</span></span>|
|<span data-ttu-id="0420f-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0420f-148">createdDateTime</span></span>|<span data-ttu-id="0420f-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0420f-149">dateTimeOffset</span></span>|<span data-ttu-id="0420f-150">只读。</span><span class="sxs-lookup"><span data-stu-id="0420f-150">Read only.</span></span> <span data-ttu-id="0420f-151">在聊天消息创建时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="0420f-151">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="0420f-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0420f-152">lastModifiedDateTime</span></span>|<span data-ttu-id="0420f-153">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0420f-153">dateTimeOffset</span></span>|<span data-ttu-id="0420f-154">只读。</span><span class="sxs-lookup"><span data-stu-id="0420f-154">Read only.</span></span> <span data-ttu-id="0420f-155">在 (初始设置) 或编辑时（包括添加或删除反应时）创建聊天邮件时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="0420f-155">Timestamp when the chat message is created (initial setting) or edited, including when a reaction is added or removed.</span></span> |
|<span data-ttu-id="0420f-156">lastEditedDateTime</span><span class="sxs-lookup"><span data-stu-id="0420f-156">lastEditedDateTime</span></span>|<span data-ttu-id="0420f-157">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0420f-157">dateTimeOffset</span></span>|<span data-ttu-id="0420f-158">只读。</span><span class="sxs-lookup"><span data-stu-id="0420f-158">Read only.</span></span> <span data-ttu-id="0420f-159">在对聊天消息进行编辑时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="0420f-159">Timestamp when edits to the chat message were made.</span></span> <span data-ttu-id="0420f-160">触发 Microsoft 团队 UI 中的 "编辑" 标志。</span><span class="sxs-lookup"><span data-stu-id="0420f-160">Triggers an "Edited" flag in the Microsoft Teams UI.</span></span> <span data-ttu-id="0420f-161">如果未进行任何编辑，则该值为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="0420f-161">If no edits are made the value is `null`.</span></span>|
|<span data-ttu-id="0420f-162">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="0420f-162">deletedDateTime</span></span>|<span data-ttu-id="0420f-163">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0420f-163">dateTimeOffset</span></span>|<span data-ttu-id="0420f-164">只读。</span><span class="sxs-lookup"><span data-stu-id="0420f-164">Read only.</span></span> <span data-ttu-id="0420f-165">删除聊天邮件的时间戳，如果未删除，则为 null。</span><span class="sxs-lookup"><span data-stu-id="0420f-165">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="0420f-166">subject</span><span class="sxs-lookup"><span data-stu-id="0420f-166">subject</span></span>|<span data-ttu-id="0420f-167">string</span><span class="sxs-lookup"><span data-stu-id="0420f-167">string</span></span>| <span data-ttu-id="0420f-168">聊天消息的主题，以纯文本形式。</span><span class="sxs-lookup"><span data-stu-id="0420f-168">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="0420f-169">body</span><span class="sxs-lookup"><span data-stu-id="0420f-169">body</span></span>|[<span data-ttu-id="0420f-170">itemBody</span><span class="sxs-lookup"><span data-stu-id="0420f-170">itemBody</span></span>](itembody.md)|<span data-ttu-id="0420f-171">聊天消息内容的纯文本/HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0420f-171">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="0420f-172">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="0420f-172">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="0420f-173">如果聊天消息包含 [chatMessageMention](chatmessagemention.md)，则该内容始终为 HTML。</span><span class="sxs-lookup"><span data-stu-id="0420f-173">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="0420f-174">摘要</span><span class="sxs-lookup"><span data-stu-id="0420f-174">summary</span></span>|<span data-ttu-id="0420f-175">string</span><span class="sxs-lookup"><span data-stu-id="0420f-175">string</span></span>| <span data-ttu-id="0420f-176">可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。</span><span class="sxs-lookup"><span data-stu-id="0420f-176">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="0420f-177">仅适用于频道聊天消息，而不是聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="0420f-177">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="0420f-178">附件</span><span class="sxs-lookup"><span data-stu-id="0420f-178">attachments</span></span>|<span data-ttu-id="0420f-179">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0420f-179">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="0420f-180">附加文件。</span><span class="sxs-lookup"><span data-stu-id="0420f-180">Attached files.</span></span> <span data-ttu-id="0420f-181">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="0420f-181">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="0420f-182">提及</span><span class="sxs-lookup"><span data-stu-id="0420f-182">mentions</span></span>|<span data-ttu-id="0420f-183">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0420f-183">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="0420f-184">聊天消息中提及的实体列表。</span><span class="sxs-lookup"><span data-stu-id="0420f-184">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="0420f-185">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="0420f-185">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="0420f-186">重要性</span><span class="sxs-lookup"><span data-stu-id="0420f-186">importance</span></span>| <span data-ttu-id="0420f-187">string</span><span class="sxs-lookup"><span data-stu-id="0420f-187">string</span></span> | <span data-ttu-id="0420f-188">聊天消息的重要性。</span><span class="sxs-lookup"><span data-stu-id="0420f-188">The importance of the chat message.</span></span> <span data-ttu-id="0420f-189">可能的值包括 `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="0420f-189">The possible values are: `normal`, `high`, `urgent`.</span></span>|
| <span data-ttu-id="0420f-190">policyViolation</span><span class="sxs-lookup"><span data-stu-id="0420f-190">policyViolation</span></span> | [<span data-ttu-id="0420f-191">chatMessagePolicyViolation</span><span class="sxs-lookup"><span data-stu-id="0420f-191">chatMessagePolicyViolation</span></span>](../resources/chatmessagepolicyviolation.md) |<span data-ttu-id="0420f-192">定义由数据丢失防护 (DLP) 应用程序设置的策略违规属性。</span><span class="sxs-lookup"><span data-stu-id="0420f-192">Defines the properties of a policy violation set by a data loss prevention (DLP) application.</span></span>|
|<span data-ttu-id="0420f-193">区域设置</span><span class="sxs-lookup"><span data-stu-id="0420f-193">locale</span></span>|<span data-ttu-id="0420f-194">string</span><span class="sxs-lookup"><span data-stu-id="0420f-194">string</span></span>|<span data-ttu-id="0420f-195">客户端的聊天消息的区域设置。</span><span class="sxs-lookup"><span data-stu-id="0420f-195">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0420f-196">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0420f-196">JSON representation</span></span>

<span data-ttu-id="0420f-197">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0420f-197">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "deleted",
    "deletedDateTime",
    "attachments",
    "importance",
    "mentions",
    "subject",
    "summary",
    "policyViolation",
    "locale"
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
  "policyViolation": {"@odata.type": "microsoft.graph.chatMessagePolicyViolation"},
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
