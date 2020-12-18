---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 chatMessages 集合。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2a5fefdff40c60951c07d26df2962fbba1249a16
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714298"
---
# <a name="chat-resource-type"></a><span data-ttu-id="c9421-103">聊天资源类型</span><span class="sxs-lookup"><span data-stu-id="c9421-103">chat resource type</span></span>

<span data-ttu-id="c9421-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9421-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9421-105">聊天是一个或多个参与者之间的 [chatMessages](chatmessage.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="c9421-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="c9421-106">参与者可以是用户或应用。</span><span class="sxs-lookup"><span data-stu-id="c9421-106">Participants can be users or apps.</span></span>

> <span data-ttu-id="c9421-107">**注意**：如果聊天与 [onlineMeeting](../resources/onlinemeeting.md) 实例关联，则列出的一些方法将可传递地影响会议。</span><span class="sxs-lookup"><span data-stu-id="c9421-107">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then some of the listed methods will transitively impact the meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="c9421-108">方法</span><span class="sxs-lookup"><span data-stu-id="c9421-108">Methods</span></span>

|  <span data-ttu-id="c9421-109">方法</span><span class="sxs-lookup"><span data-stu-id="c9421-109">Method</span></span>       |  <span data-ttu-id="c9421-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c9421-110">Return Type</span></span>  | <span data-ttu-id="c9421-111">说明</span><span class="sxs-lookup"><span data-stu-id="c9421-111">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="c9421-112">列出聊天</span><span class="sxs-lookup"><span data-stu-id="c9421-112">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="c9421-113">[chat](chat.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9421-113">[chat](chat.md) collection</span></span> | <span data-ttu-id="c9421-114">获取用户参与的聊天列表。</span><span class="sxs-lookup"><span data-stu-id="c9421-114">Get the list of chats a user is part of.</span></span>| 
|[<span data-ttu-id="c9421-115">创建聊天</span><span class="sxs-lookup"><span data-stu-id="c9421-115">Create chat</span></span>](../api/chat-post.md) | [<span data-ttu-id="c9421-116">聊天</span><span class="sxs-lookup"><span data-stu-id="c9421-116">chat</span></span>](chat.md) | <span data-ttu-id="c9421-117">创建新聊天。</span><span class="sxs-lookup"><span data-stu-id="c9421-117">Create a new chat.</span></span>| 
|[<span data-ttu-id="c9421-118">获取聊天</span><span class="sxs-lookup"><span data-stu-id="c9421-118">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="c9421-119">聊天</span><span class="sxs-lookup"><span data-stu-id="c9421-119">chat</span></span>](chat.md) | <span data-ttu-id="c9421-120">读取聊天的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c9421-120">Read properties and relationships of the chat.</span></span>| 
|[<span data-ttu-id="c9421-121">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="c9421-121">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="c9421-122">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9421-122">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="c9421-123">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="c9421-123">Get the list of all users in the chat.</span></span>| 
|[<span data-ttu-id="c9421-124">添加聊天成员</span><span class="sxs-lookup"><span data-stu-id="c9421-124">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="c9421-125">位置标头</span><span class="sxs-lookup"><span data-stu-id="c9421-125">Location header</span></span> | <span data-ttu-id="c9421-126">向聊天中添加用户。</span><span class="sxs-lookup"><span data-stu-id="c9421-126">Add a user to the chat.</span></span>| 
|[<span data-ttu-id="c9421-127">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="c9421-127">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="c9421-128">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c9421-128">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="c9421-129">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="c9421-129">Get a single user in the chat.</span></span>| 
|[<span data-ttu-id="c9421-130">删除聊天成员</span><span class="sxs-lookup"><span data-stu-id="c9421-130">Remove chat member</span></span>](../api/chat-delete-members.md)|<span data-ttu-id="c9421-131">无</span><span class="sxs-lookup"><span data-stu-id="c9421-131">None</span></span>|<span data-ttu-id="c9421-132">从聊天中删除用户。</span><span class="sxs-lookup"><span data-stu-id="c9421-132">Remove a user from the chat.</span></span>|
|[<span data-ttu-id="c9421-133">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="c9421-133">List messages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="c9421-134">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c9421-134">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="c9421-135">获取一对一聊天或群组聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="c9421-135">Get messages in a 1:1 or group chat.</span></span> | 
|[<span data-ttu-id="c9421-136">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="c9421-136">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="c9421-137">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c9421-137">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="c9421-138">获取聊天中的单个消息。</span><span class="sxs-lookup"><span data-stu-id="c9421-138">Get a single message in a chat.</span></span> | 
|[<span data-ttu-id="c9421-139">获取用户和应用之间的聊天</span><span class="sxs-lookup"><span data-stu-id="c9421-139">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="c9421-140">聊天</span><span class="sxs-lookup"><span data-stu-id="c9421-140">chat</span></span>](chat.md)| <span data-ttu-id="c9421-141">获取用户与应用之间的一对一聊天</span><span class="sxs-lookup"><span data-stu-id="c9421-141">Get one-on-one chat between user and the app</span></span> |
|[<span data-ttu-id="c9421-142">获取所有聊天消息</span><span class="sxs-lookup"><span data-stu-id="c9421-142">Get all chat messages</span></span>](../api/chats-getallmessages.md)| <span data-ttu-id="c9421-143">[chat](chat.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9421-143">[chat](chat.md) collection</span></span>| <span data-ttu-id="c9421-144">从用户参与的所有聊天（包括一对一聊天、群聊和会议聊天）获取消息。</span><span class="sxs-lookup"><span data-stu-id="c9421-144">Get messages from all chats that a user is a participant in, including one-on-one chats, group chats, and meeting chats.</span></span> |
|[<span data-ttu-id="c9421-145">列出聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="c9421-145">List apps in chat</span></span>](../api/chat-list-installedapps.md) |<span data-ttu-id="c9421-146">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9421-146">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="c9421-147">列出安装在聊天聊天 (关联的会议) 。</span><span class="sxs-lookup"><span data-stu-id="c9421-147">List apps installed in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="c9421-148">获取聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="c9421-148">Get app in chat</span></span>](../api/chat-get-installedapps.md) | [<span data-ttu-id="c9421-149">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c9421-149">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="c9421-150">获取在聊天聊天和关联会议 (安装的特定) 。</span><span class="sxs-lookup"><span data-stu-id="c9421-150">Get a specific app installed in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="c9421-151">在聊天中添加应用</span><span class="sxs-lookup"><span data-stu-id="c9421-151">Add app in chat</span></span>](../api/chat-post-installedapps.md) | | <span data-ttu-id="c9421-152">添加 (在) 和关联的会议 (中安装) 。</span><span class="sxs-lookup"><span data-stu-id="c9421-152">Add (install) an app in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="c9421-153">升级聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="c9421-153">Upgrade app in chat</span></span>](../api/chat-teamsappinstallation-upgrade.md) | <span data-ttu-id="c9421-154">无</span><span class="sxs-lookup"><span data-stu-id="c9421-154">None</span></span> | <span data-ttu-id="c9421-155">更新到安装在聊天会话和相关会议 (应用的) 。</span><span class="sxs-lookup"><span data-stu-id="c9421-155">Update to the latest version of the app installed in chat (and associated meeting).</span></span>|
|[<span data-ttu-id="c9421-156">从聊天中卸载应用</span><span class="sxs-lookup"><span data-stu-id="c9421-156">Uninstall app from chat</span></span>](../api/chat-delete-installedapps.md) | <span data-ttu-id="c9421-157">无</span><span class="sxs-lookup"><span data-stu-id="c9421-157">None</span></span> | <span data-ttu-id="c9421-158">从 (会议) 中删除 (应用程序) 。</span><span class="sxs-lookup"><span data-stu-id="c9421-158">Remove (uninstall) app from a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="c9421-159">列出聊天中的选项卡</span><span class="sxs-lookup"><span data-stu-id="c9421-159">List tabs in chat</span></span>](../api/chat-list-tabs.md) | [<span data-ttu-id="c9421-160">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c9421-160">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="c9421-161">列出固定到聊天聊天 (关联的会议) 。</span><span class="sxs-lookup"><span data-stu-id="c9421-161">List tabs pinned to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="c9421-162">获取聊天中的选项卡</span><span class="sxs-lookup"><span data-stu-id="c9421-162">Get tab in chat</span></span>](../api/chat-get-tabs.md) | [<span data-ttu-id="c9421-163">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c9421-163">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="c9421-164">获取固定到聊天会话和关联 (的特定选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="c9421-164">Get a specific tab pinned to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="c9421-165">向聊天添加选项卡</span><span class="sxs-lookup"><span data-stu-id="c9421-165">Add tab to chat</span></span>](../api/chat-post-tabs.md) | [<span data-ttu-id="c9421-166">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c9421-166">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="c9421-167">将 (固定) 选项卡添加到聊天 (关联的会议) 。</span><span class="sxs-lookup"><span data-stu-id="c9421-167">Add (pin) a tab to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="c9421-168">聊天中的"更新"选项卡</span><span class="sxs-lookup"><span data-stu-id="c9421-168">Update tab in chat</span></span>](../api/chat-patch-tabs.md) | [<span data-ttu-id="c9421-169">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c9421-169">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="c9421-170">更新聊天会话和关联会议 (选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="c9421-170">Update the properties of a tab in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="c9421-171">从聊天中删除选项卡</span><span class="sxs-lookup"><span data-stu-id="c9421-171">Remove tab from chat</span></span>](../api/chat-delete-tabs.md) | <span data-ttu-id="c9421-172">无</span><span class="sxs-lookup"><span data-stu-id="c9421-172">None</span></span> | <span data-ttu-id="c9421-173">从 (活动) 关联的会议选项卡 (取消固定) 。</span><span class="sxs-lookup"><span data-stu-id="c9421-173">Remove (unpin) a tab from a chat (and associated meeting).</span></span>|

><span data-ttu-id="c9421-174">**注意：** 使用应用程序权限时，请确保你了解如何获取聊天 ID。</span><span class="sxs-lookup"><span data-stu-id="c9421-174">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="c9421-175">由于不支持列出具有应用程序权限的聊天，因此并非所有方案都可行。</span><span class="sxs-lookup"><span data-stu-id="c9421-175">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="c9421-176">可以获取具有委派权限的聊天 ID，以及从具有应用程序权限 [的 /chats/getAllMessages](../api/subscription-post-subscriptions.md) 更改通知获取。</span><span class="sxs-lookup"><span data-stu-id="c9421-176">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="c9421-177">属性</span><span class="sxs-lookup"><span data-stu-id="c9421-177">Properties</span></span>

| <span data-ttu-id="c9421-178">属性</span><span class="sxs-lookup"><span data-stu-id="c9421-178">Property</span></span>   | <span data-ttu-id="c9421-179">类型</span><span class="sxs-lookup"><span data-stu-id="c9421-179">Type</span></span> |<span data-ttu-id="c9421-180">说明</span><span class="sxs-lookup"><span data-stu-id="c9421-180">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c9421-181">id</span><span class="sxs-lookup"><span data-stu-id="c9421-181">id</span></span>| <span data-ttu-id="c9421-182">String</span><span class="sxs-lookup"><span data-stu-id="c9421-182">String</span></span>| <span data-ttu-id="c9421-183">聊天的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c9421-183">The chat's unique identifier.</span></span> <span data-ttu-id="c9421-184">只读。</span><span class="sxs-lookup"><span data-stu-id="c9421-184">Read-only.</span></span>|
| <span data-ttu-id="c9421-185">topic</span><span class="sxs-lookup"><span data-stu-id="c9421-185">topic</span></span>| <span data-ttu-id="c9421-186">String</span><span class="sxs-lookup"><span data-stu-id="c9421-186">String</span></span>|  <span data-ttu-id="c9421-187"> (聊天) 主题或主题的可选选项。</span><span class="sxs-lookup"><span data-stu-id="c9421-187">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="c9421-188">仅适用于群聊。</span><span class="sxs-lookup"><span data-stu-id="c9421-188">Only available for group chats.</span></span>|
| <span data-ttu-id="c9421-189">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9421-189">createdDateTime</span></span>| <span data-ttu-id="c9421-190">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9421-190">dateTimeOffset</span></span>|  <span data-ttu-id="c9421-191">创建聊天的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c9421-191">Date and time at which the chat was created.</span></span> <span data-ttu-id="c9421-192">只读。</span><span class="sxs-lookup"><span data-stu-id="c9421-192">Read-only.</span></span>|
| <span data-ttu-id="c9421-193">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9421-193">lastUpdatedDateTime</span></span>| <span data-ttu-id="c9421-194">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9421-194">dateTimeOffset</span></span>|  <span data-ttu-id="c9421-195">上次更改聊天或成员列表的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c9421-195">Date and time at which the chat was renamed or list of members were last changed.</span></span> <span data-ttu-id="c9421-196">只读。</span><span class="sxs-lookup"><span data-stu-id="c9421-196">Read-only.</span></span>|
| <span data-ttu-id="c9421-197">chatType</span><span class="sxs-lookup"><span data-stu-id="c9421-197">chatType</span></span>| [<span data-ttu-id="c9421-198">chatType</span><span class="sxs-lookup"><span data-stu-id="c9421-198">chatType</span></span>](../resources/chat.md#chattype-values) | <span data-ttu-id="c9421-199">指定聊天类型。</span><span class="sxs-lookup"><span data-stu-id="c9421-199">Specifies the type of chat.</span></span> <span data-ttu-id="c9421-200">可能的值是： `group` 和 `oneOnOne` `meeting` 。</span><span class="sxs-lookup"><span data-stu-id="c9421-200">Possible values are:`group`, `oneOnOne` and `meeting`.</span></span>|

### <a name="chattype-values"></a><span data-ttu-id="c9421-201">chatType 值</span><span class="sxs-lookup"><span data-stu-id="c9421-201">chatType values</span></span> 

| <span data-ttu-id="c9421-202">成员</span><span class="sxs-lookup"><span data-stu-id="c9421-202">Member</span></span>             | <span data-ttu-id="c9421-203">值</span><span class="sxs-lookup"><span data-stu-id="c9421-203">Value</span></span> | <span data-ttu-id="c9421-204">说明</span><span class="sxs-lookup"><span data-stu-id="c9421-204">Description</span></span>               |
| :----------------- | :---- | :------------------------ |
|<span data-ttu-id="c9421-205">oneOnOne</span><span class="sxs-lookup"><span data-stu-id="c9421-205">oneOnOne</span></span>            | <span data-ttu-id="c9421-206">0</span><span class="sxs-lookup"><span data-stu-id="c9421-206">0</span></span>     | <span data-ttu-id="c9421-207">指示聊天为一对一聊天。</span><span class="sxs-lookup"><span data-stu-id="c9421-207">Indicates that the chat is a 1:1 chat.</span></span> <span data-ttu-id="c9421-208">对于此类聊天，名单大小是固定的;无法删除/添加成员。</span><span class="sxs-lookup"><span data-stu-id="c9421-208">The roster size is fixed for this type of chat; members cannot be removed/added.</span></span>|
|<span data-ttu-id="c9421-209">group</span><span class="sxs-lookup"><span data-stu-id="c9421-209">group</span></span>               | <span data-ttu-id="c9421-210">1</span><span class="sxs-lookup"><span data-stu-id="c9421-210">1</span></span>     | <span data-ttu-id="c9421-211">指示聊天是群聊。</span><span class="sxs-lookup"><span data-stu-id="c9421-211">Indicates that the chat is a group chat.</span></span> <span data-ttu-id="c9421-212">可以针对 (更新至少两) 用户名单大小。</span><span class="sxs-lookup"><span data-stu-id="c9421-212">The roster size (of at least two people) can be updated for this type of chat.</span></span> <span data-ttu-id="c9421-213">稍后可以删除/添加成员。</span><span class="sxs-lookup"><span data-stu-id="c9421-213">Members can be removed/added later.</span></span>|
|<span data-ttu-id="c9421-214">meeting</span><span class="sxs-lookup"><span data-stu-id="c9421-214">meeting</span></span>             | <span data-ttu-id="c9421-215">2</span><span class="sxs-lookup"><span data-stu-id="c9421-215">2</span></span>     | <span data-ttu-id="c9421-216">指示聊天与联机会议关联。</span><span class="sxs-lookup"><span data-stu-id="c9421-216">Indicates that the chat is associated with an online meeting.</span></span> <span data-ttu-id="c9421-217">此类聊天仅作为联机会议创建的一部分创建。</span><span class="sxs-lookup"><span data-stu-id="c9421-217">This type of chat is only created as part of the creation of an online meeting.</span></span>|
|<span data-ttu-id="c9421-218">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="c9421-218">unknownFutureValue</span></span>  | <span data-ttu-id="c9421-219">3</span><span class="sxs-lookup"><span data-stu-id="c9421-219">3</span></span>     | <span data-ttu-id="c9421-220">指示未来值的 Sentinel 值。</span><span class="sxs-lookup"><span data-stu-id="c9421-220">Sentinel value to indicate future values.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c9421-221">关系</span><span class="sxs-lookup"><span data-stu-id="c9421-221">Relationships</span></span>

| <span data-ttu-id="c9421-222">关系</span><span class="sxs-lookup"><span data-stu-id="c9421-222">Relationship</span></span> | <span data-ttu-id="c9421-223">类型</span><span class="sxs-lookup"><span data-stu-id="c9421-223">Type</span></span> |<span data-ttu-id="c9421-224">说明</span><span class="sxs-lookup"><span data-stu-id="c9421-224">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c9421-225">installedApps</span><span class="sxs-lookup"><span data-stu-id="c9421-225">installedApps</span></span> | <span data-ttu-id="c9421-226">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9421-226">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="c9421-227">聊天中所有应用的集合。</span><span class="sxs-lookup"><span data-stu-id="c9421-227">A collection of all the apps in the chat.</span></span> <span data-ttu-id="c9421-228">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="c9421-228">Nullable.</span></span> |
| <span data-ttu-id="c9421-229">members</span><span class="sxs-lookup"><span data-stu-id="c9421-229">members</span></span> | <span data-ttu-id="c9421-230">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9421-230">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="c9421-231">聊天中所有成员的集合。</span><span class="sxs-lookup"><span data-stu-id="c9421-231">A collection of all the members in the chat.</span></span> <span data-ttu-id="c9421-232">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="c9421-232">Nullable.</span></span> |
| <span data-ttu-id="c9421-233">messages</span><span class="sxs-lookup"><span data-stu-id="c9421-233">messages</span></span> | <span data-ttu-id="c9421-234">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9421-234">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="c9421-235">聊天中所有消息的集合。</span><span class="sxs-lookup"><span data-stu-id="c9421-235">A collection of all the messages in the chat.</span></span> <span data-ttu-id="c9421-236">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="c9421-236">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c9421-237">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9421-237">JSON representation</span></span>

<span data-ttu-id="c9421-238">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9421-238">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chat"
}-->

```json
{
  "id": "string (identifier)",
  "topic": "string",
  "createdDateTime": "dateTimeOffset",
  "lastUpdatedDateTime": "dateTimeOffset",
  "chatType": "String"
}
```

## <a name="see-also"></a><span data-ttu-id="c9421-239">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c9421-239">See also</span></span>

- [<span data-ttu-id="c9421-240">频道</span><span class="sxs-lookup"><span data-stu-id="c9421-240">channel</span></span>](channel.md)
- [<span data-ttu-id="c9421-241">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c9421-241">chatMessage</span></span>](chatmessage.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->


