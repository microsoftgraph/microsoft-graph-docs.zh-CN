---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 聊天消息可以是根聊天消息，或者是聊天消息中的 **replyToId** 属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 8099efac4132a070bfcf8443ef290989305d6737
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626129"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="a9c93-104">chatMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9c93-104">chatMessage resource type</span></span>

<span data-ttu-id="a9c93-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9c93-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a9c93-106">表示在 beta ([聊天中](./channel.md) 频道或) [单个聊天消息](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="a9c93-106">Represents an individual chat message within a [channel](./channel.md) or (in beta) [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="a9c93-107">聊天消息可以是根聊天消息或聊天消息中的 **replyToId** 属性定义的回复线程的一部分。</span><span class="sxs-lookup"><span data-stu-id="a9c93-107">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="a9c93-108">方法</span><span class="sxs-lookup"><span data-stu-id="a9c93-108">Methods</span></span>

| <span data-ttu-id="a9c93-109">方法</span><span class="sxs-lookup"><span data-stu-id="a9c93-109">Method</span></span>       | <span data-ttu-id="a9c93-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a9c93-110">Return Type</span></span>  |<span data-ttu-id="a9c93-111">说明</span><span class="sxs-lookup"><span data-stu-id="a9c93-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9c93-112">**频道消息**</span><span class="sxs-lookup"><span data-stu-id="a9c93-112">**Channel messages**</span></span>| | |
|[<span data-ttu-id="a9c93-113">列出频道 chatMessage</span><span class="sxs-lookup"><span data-stu-id="a9c93-113">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="a9c93-114">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a9c93-114">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="a9c93-115">频道中所有根聊天消息的列表。</span><span class="sxs-lookup"><span data-stu-id="a9c93-115">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="a9c93-116">获取通道增量中的 chatMessages</span><span class="sxs-lookup"><span data-stu-id="a9c93-116">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="a9c93-117">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a9c93-117">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="a9c93-118">获取频道中的增量聊天消息。</span><span class="sxs-lookup"><span data-stu-id="a9c93-118">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="a9c93-119">创建新频道消息的订阅</span><span class="sxs-lookup"><span data-stu-id="a9c93-119">Create subscription for new channel messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="a9c93-120">订阅</span><span class="sxs-lookup"><span data-stu-id="a9c93-120">subscription</span></span>](subscription.md) | <span data-ttu-id="a9c93-121">收听新的和编辑的频道消息，并回应它们。</span><span class="sxs-lookup"><span data-stu-id="a9c93-121">Listen for new and edited channel messages, and reactions to them.</span></span> |
|[<span data-ttu-id="a9c93-122">获取频道 chatMessage</span><span class="sxs-lookup"><span data-stu-id="a9c93-122">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="a9c93-123">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a9c93-123">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="a9c93-124">从频道获取单个根聊天消息。</span><span class="sxs-lookup"><span data-stu-id="a9c93-124">Get a single root chat message from a channel.</span></span>|
|[<span data-ttu-id="a9c93-125">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="a9c93-125">Create chatMessage in a channel</span></span>](../api/channel-post-message.md) | [<span data-ttu-id="a9c93-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a9c93-126">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="a9c93-127">向频道发送消息。</span><span class="sxs-lookup"><span data-stu-id="a9c93-127">Send a message to a channel.</span></span> |
|[<span data-ttu-id="a9c93-128">更新 chatMessage</span><span class="sxs-lookup"><span data-stu-id="a9c93-128">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="a9c93-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a9c93-129">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="a9c93-130">更新 **聊天消息的 policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="a9c93-130">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="a9c93-131">**频道消息回复**</span><span class="sxs-lookup"><span data-stu-id="a9c93-131">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="a9c93-132">列出对 chatMessage 的答复</span><span class="sxs-lookup"><span data-stu-id="a9c93-132">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="a9c93-133">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a9c93-133">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="a9c93-134">频道中聊天消息的所有回复列表。</span><span class="sxs-lookup"><span data-stu-id="a9c93-134">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="a9c93-135">获取 chatMessage 回复</span><span class="sxs-lookup"><span data-stu-id="a9c93-135">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="a9c93-136">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a9c93-136">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="a9c93-137">获取频道中聊天消息的单个回复。</span><span class="sxs-lookup"><span data-stu-id="a9c93-137">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="a9c93-138">回复频道中的 chatMessage</span><span class="sxs-lookup"><span data-stu-id="a9c93-138">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="a9c93-139">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a9c93-139">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="a9c93-140">回复频道中的现有聊天消息。</span><span class="sxs-lookup"><span data-stu-id="a9c93-140">Reply to an existing chat message in a channel.</span></span>|
|[<span data-ttu-id="a9c93-141">更新 chatMessage</span><span class="sxs-lookup"><span data-stu-id="a9c93-141">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="a9c93-142">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a9c93-142">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="a9c93-143">更新 **聊天消息的 policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="a9c93-143">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="a9c93-144">**托管内容**</span><span class="sxs-lookup"><span data-stu-id="a9c93-144">**Hosted content**</span></span>| | |
|[<span data-ttu-id="a9c93-145">列出所有托管内容</span><span class="sxs-lookup"><span data-stu-id="a9c93-145">List all hosted content</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | <span data-ttu-id="a9c93-146">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a9c93-146">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection</span></span>| <span data-ttu-id="a9c93-147">获取聊天消息中所有托管的内容。</span><span class="sxs-lookup"><span data-stu-id="a9c93-147">Get all hosted content in a chat message.</span></span>|
|[<span data-ttu-id="a9c93-148">获取托管内容</span><span class="sxs-lookup"><span data-stu-id="a9c93-148">Get hosted content</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="a9c93-149">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="a9c93-149">chatMessageHostedContent</span></span>](../resources/chatmessagehostedcontent.md) | <span data-ttu-id="a9c93-150">从聊天消息获取托管内容。</span><span class="sxs-lookup"><span data-stu-id="a9c93-150">Get hosted content from a chat message.</span></span>|

## <a name="properties"></a><span data-ttu-id="a9c93-151">属性</span><span class="sxs-lookup"><span data-stu-id="a9c93-151">Properties</span></span>

| <span data-ttu-id="a9c93-152">属性</span><span class="sxs-lookup"><span data-stu-id="a9c93-152">Property</span></span>   | <span data-ttu-id="a9c93-153">类型</span><span class="sxs-lookup"><span data-stu-id="a9c93-153">Type</span></span> |<span data-ttu-id="a9c93-154">说明</span><span class="sxs-lookup"><span data-stu-id="a9c93-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9c93-155">id</span><span class="sxs-lookup"><span data-stu-id="a9c93-155">id</span></span>|<span data-ttu-id="a9c93-156">String</span><span class="sxs-lookup"><span data-stu-id="a9c93-156">String</span></span>| <span data-ttu-id="a9c93-157">只读。</span><span class="sxs-lookup"><span data-stu-id="a9c93-157">Read-only.</span></span> <span data-ttu-id="a9c93-158">邮件的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="a9c93-158">Unique Id of the message.</span></span>|
|<span data-ttu-id="a9c93-159">replyToId</span><span class="sxs-lookup"><span data-stu-id="a9c93-159">replyToId</span></span>| <span data-ttu-id="a9c93-160">string</span><span class="sxs-lookup"><span data-stu-id="a9c93-160">string</span></span> | <span data-ttu-id="a9c93-161">只读。</span><span class="sxs-lookup"><span data-stu-id="a9c93-161">Read-only.</span></span> <span data-ttu-id="a9c93-162">线程的父聊天消息或根聊天消息的 ID。</span><span class="sxs-lookup"><span data-stu-id="a9c93-162">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="a9c93-163"> (仅适用于频道中的聊天消息，不应用于聊天) </span><span class="sxs-lookup"><span data-stu-id="a9c93-163">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="a9c93-164">from</span><span class="sxs-lookup"><span data-stu-id="a9c93-164">from</span></span>|[<span data-ttu-id="a9c93-165">identitySet</span><span class="sxs-lookup"><span data-stu-id="a9c93-165">identitySet</span></span>](identityset.md)| <span data-ttu-id="a9c93-166">只读。</span><span class="sxs-lookup"><span data-stu-id="a9c93-166">Read only.</span></span> <span data-ttu-id="a9c93-167">聊天消息的发件人的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a9c93-167">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="a9c93-168">etag</span><span class="sxs-lookup"><span data-stu-id="a9c93-168">etag</span></span>| <span data-ttu-id="a9c93-169">string</span><span class="sxs-lookup"><span data-stu-id="a9c93-169">string</span></span> | <span data-ttu-id="a9c93-170">只读。</span><span class="sxs-lookup"><span data-stu-id="a9c93-170">Read-only.</span></span> <span data-ttu-id="a9c93-171">聊天消息的版本号。</span><span class="sxs-lookup"><span data-stu-id="a9c93-171">Version number of the chat message.</span></span> |
|<span data-ttu-id="a9c93-172">messageType</span><span class="sxs-lookup"><span data-stu-id="a9c93-172">messageType</span></span>|<span data-ttu-id="a9c93-173">string</span><span class="sxs-lookup"><span data-stu-id="a9c93-173">string</span></span>|<span data-ttu-id="a9c93-174">聊天消息的类型。</span><span class="sxs-lookup"><span data-stu-id="a9c93-174">The type of chat message.</span></span> <span data-ttu-id="a9c93-175">可能的值是： `message` .</span><span class="sxs-lookup"><span data-stu-id="a9c93-175">The possible values are: `message`.</span></span>|
|<span data-ttu-id="a9c93-176">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9c93-176">createdDateTime</span></span>|<span data-ttu-id="a9c93-177">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9c93-177">dateTimeOffset</span></span>|<span data-ttu-id="a9c93-178">只读。</span><span class="sxs-lookup"><span data-stu-id="a9c93-178">Read only.</span></span> <span data-ttu-id="a9c93-179">创建聊天消息的时间戳。</span><span class="sxs-lookup"><span data-stu-id="a9c93-179">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="a9c93-180">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9c93-180">lastModifiedDateTime</span></span>|<span data-ttu-id="a9c93-181">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9c93-181">dateTimeOffset</span></span>|<span data-ttu-id="a9c93-182">只读。</span><span class="sxs-lookup"><span data-stu-id="a9c93-182">Read only.</span></span> <span data-ttu-id="a9c93-183">创建聊天消息的时间戳 (设置) 编辑，包括添加或删除反应时。</span><span class="sxs-lookup"><span data-stu-id="a9c93-183">Timestamp when the chat message is created (initial setting) or edited, including when a reaction is added or removed.</span></span> |
|<span data-ttu-id="a9c93-184">lastEditedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9c93-184">lastEditedDateTime</span></span>|<span data-ttu-id="a9c93-185">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9c93-185">dateTimeOffset</span></span>|<span data-ttu-id="a9c93-186">只读。</span><span class="sxs-lookup"><span data-stu-id="a9c93-186">Read only.</span></span> <span data-ttu-id="a9c93-187">编辑聊天消息的时间戳。</span><span class="sxs-lookup"><span data-stu-id="a9c93-187">Timestamp when edits to the chat message were made.</span></span> <span data-ttu-id="a9c93-188">在 Microsoft Teams UI 中触发"已编辑"标志。</span><span class="sxs-lookup"><span data-stu-id="a9c93-188">Triggers an "Edited" flag in the Microsoft Teams UI.</span></span> <span data-ttu-id="a9c93-189">如果未进行编辑，则值为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="a9c93-189">If no edits are made the value is `null`.</span></span>|
|<span data-ttu-id="a9c93-190">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9c93-190">deletedDateTime</span></span>|<span data-ttu-id="a9c93-191">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9c93-191">dateTimeOffset</span></span>|<span data-ttu-id="a9c93-192">只读。</span><span class="sxs-lookup"><span data-stu-id="a9c93-192">Read only.</span></span> <span data-ttu-id="a9c93-193">删除聊天消息的时间戳;如果未删除，则为 null。</span><span class="sxs-lookup"><span data-stu-id="a9c93-193">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="a9c93-194">subject</span><span class="sxs-lookup"><span data-stu-id="a9c93-194">subject</span></span>|<span data-ttu-id="a9c93-195">string</span><span class="sxs-lookup"><span data-stu-id="a9c93-195">string</span></span>| <span data-ttu-id="a9c93-196">纯文本形式的聊天消息的主题。</span><span class="sxs-lookup"><span data-stu-id="a9c93-196">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="a9c93-197">body</span><span class="sxs-lookup"><span data-stu-id="a9c93-197">body</span></span>|[<span data-ttu-id="a9c93-198">itemBody</span><span class="sxs-lookup"><span data-stu-id="a9c93-198">itemBody</span></span>](itembody.md)|<span data-ttu-id="a9c93-199">聊天消息内容的纯文本/HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9c93-199">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="a9c93-200">表示形式由正文中的 contentType 进行指定。</span><span class="sxs-lookup"><span data-stu-id="a9c93-200">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="a9c93-201">如果聊天消息包含 [chatMessageMention，](chatmessagemention.md)则内容始终为 HTML 格式。</span><span class="sxs-lookup"><span data-stu-id="a9c93-201">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="a9c93-202">摘要</span><span class="sxs-lookup"><span data-stu-id="a9c93-202">summary</span></span>|<span data-ttu-id="a9c93-203">string</span><span class="sxs-lookup"><span data-stu-id="a9c93-203">string</span></span>| <span data-ttu-id="a9c93-204">可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。</span><span class="sxs-lookup"><span data-stu-id="a9c93-204">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="a9c93-205">仅适用于频道聊天消息，不应用于聊天中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="a9c93-205">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="a9c93-206">附件</span><span class="sxs-lookup"><span data-stu-id="a9c93-206">attachments</span></span>|<span data-ttu-id="a9c93-207">[chatMessageAttachment](chatmessageattachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a9c93-207">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="a9c93-208">附加文件。</span><span class="sxs-lookup"><span data-stu-id="a9c93-208">Attached files.</span></span> <span data-ttu-id="a9c93-209">附件目前是只读的 – 不支持发送附件。</span><span class="sxs-lookup"><span data-stu-id="a9c93-209">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="a9c93-210">提及</span><span class="sxs-lookup"><span data-stu-id="a9c93-210">mentions</span></span>|<span data-ttu-id="a9c93-211">[chatMessageMention](chatmessagemention.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a9c93-211">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="a9c93-212">聊天消息中提到的实体列表。</span><span class="sxs-lookup"><span data-stu-id="a9c93-212">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="a9c93-213">当前支持用户、机器人、团队、渠道。</span><span class="sxs-lookup"><span data-stu-id="a9c93-213">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="a9c93-214">重要性</span><span class="sxs-lookup"><span data-stu-id="a9c93-214">importance</span></span>| <span data-ttu-id="a9c93-215">string</span><span class="sxs-lookup"><span data-stu-id="a9c93-215">string</span></span> | <span data-ttu-id="a9c93-216">聊天消息的重要性。</span><span class="sxs-lookup"><span data-stu-id="a9c93-216">The importance of the chat message.</span></span> <span data-ttu-id="a9c93-217">可能的值包括 `normal`、`high`、`urgent`。</span><span class="sxs-lookup"><span data-stu-id="a9c93-217">The possible values are: `normal`, `high`, `urgent`.</span></span>|
| <span data-ttu-id="a9c93-218">policyViolation</span><span class="sxs-lookup"><span data-stu-id="a9c93-218">policyViolation</span></span> | [<span data-ttu-id="a9c93-219">chatMessagePolicyViolation</span><span class="sxs-lookup"><span data-stu-id="a9c93-219">chatMessagePolicyViolation</span></span>](../resources/chatmessagepolicyviolation.md) |<span data-ttu-id="a9c93-220">定义 DLP 应用程序数据丢失防护设置 (违反) 的属性。</span><span class="sxs-lookup"><span data-stu-id="a9c93-220">Defines the properties of a policy violation set by a data loss prevention (DLP) application.</span></span>|
|<span data-ttu-id="a9c93-221">区域设置</span><span class="sxs-lookup"><span data-stu-id="a9c93-221">locale</span></span>|<span data-ttu-id="a9c93-222">string</span><span class="sxs-lookup"><span data-stu-id="a9c93-222">string</span></span>|<span data-ttu-id="a9c93-223">客户端设置的聊天消息区域设置。</span><span class="sxs-lookup"><span data-stu-id="a9c93-223">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a9c93-224">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9c93-224">JSON representation</span></span>

<span data-ttu-id="a9c93-225">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9c93-225">The following is a JSON representation of the resource.</span></span>

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
