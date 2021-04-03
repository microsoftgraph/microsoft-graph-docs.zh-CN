---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 chatMessages 集合。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 635982c8610bc524de027632dd07c00e1a3d26b1
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582163"
---
# <a name="chat-resource-type"></a><span data-ttu-id="989a4-103">聊天资源类型</span><span class="sxs-lookup"><span data-stu-id="989a4-103">chat resource type</span></span>

<span data-ttu-id="989a4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="989a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="989a4-105">聊天是一个或多个 [参与者之间的 chatMessages](chatmessage.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="989a4-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="989a4-106">参与者可以是用户或应用。</span><span class="sxs-lookup"><span data-stu-id="989a4-106">Participants can be users or apps.</span></span>

> <span data-ttu-id="989a4-107">**注意**：如果聊天与 [onlineMeeting](../resources/onlinemeeting.md) 实例关联，则列出的一些方法将可传递影响会议。</span><span class="sxs-lookup"><span data-stu-id="989a4-107">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then some of the listed methods will transitively impact the meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="989a4-108">方法</span><span class="sxs-lookup"><span data-stu-id="989a4-108">Methods</span></span>

|  <span data-ttu-id="989a4-109">方法</span><span class="sxs-lookup"><span data-stu-id="989a4-109">Method</span></span>       |  <span data-ttu-id="989a4-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="989a4-110">Return Type</span></span>  | <span data-ttu-id="989a4-111">说明</span><span class="sxs-lookup"><span data-stu-id="989a4-111">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="989a4-112">列出聊天</span><span class="sxs-lookup"><span data-stu-id="989a4-112">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="989a4-113">[chat](chat.md) 集合</span><span class="sxs-lookup"><span data-stu-id="989a4-113">[chat](chat.md) collection</span></span> | <span data-ttu-id="989a4-114">获取用户参与的聊天列表。</span><span class="sxs-lookup"><span data-stu-id="989a4-114">Get the list of chats a user is part of.</span></span>| 
|[<span data-ttu-id="989a4-115">创建聊天</span><span class="sxs-lookup"><span data-stu-id="989a4-115">Create chat</span></span>](../api/chat-post.md) | [<span data-ttu-id="989a4-116">聊天</span><span class="sxs-lookup"><span data-stu-id="989a4-116">chat</span></span>](chat.md) | <span data-ttu-id="989a4-117">创建新聊天。</span><span class="sxs-lookup"><span data-stu-id="989a4-117">Create a new chat.</span></span>| 
|[<span data-ttu-id="989a4-118">获取聊天</span><span class="sxs-lookup"><span data-stu-id="989a4-118">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="989a4-119">聊天</span><span class="sxs-lookup"><span data-stu-id="989a4-119">chat</span></span>](chat.md) | <span data-ttu-id="989a4-120">读取聊天的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="989a4-120">Read properties and relationships of the chat.</span></span>| 
|[<span data-ttu-id="989a4-121">更新聊天</span><span class="sxs-lookup"><span data-stu-id="989a4-121">Update chat</span></span>](../api/chat-patch.md) | [<span data-ttu-id="989a4-122">聊天</span><span class="sxs-lookup"><span data-stu-id="989a4-122">chat</span></span>](chat.md) | <span data-ttu-id="989a4-123">更新聊天的属性。</span><span class="sxs-lookup"><span data-stu-id="989a4-123">Update properties of the chat.</span></span>|
|[<span data-ttu-id="989a4-124">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="989a4-124">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="989a4-125">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="989a4-125">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="989a4-126">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="989a4-126">Get the list of all users in the chat.</span></span>| 
|[<span data-ttu-id="989a4-127">添加聊天成员</span><span class="sxs-lookup"><span data-stu-id="989a4-127">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="989a4-128">位置标头</span><span class="sxs-lookup"><span data-stu-id="989a4-128">Location header</span></span> | <span data-ttu-id="989a4-129">向聊天中添加用户。</span><span class="sxs-lookup"><span data-stu-id="989a4-129">Add a user to the chat.</span></span>| 
|[<span data-ttu-id="989a4-130">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="989a4-130">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="989a4-131">conversationMember</span><span class="sxs-lookup"><span data-stu-id="989a4-131">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="989a4-132">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="989a4-132">Get a single user in the chat.</span></span>| 
|[<span data-ttu-id="989a4-133">删除聊天成员</span><span class="sxs-lookup"><span data-stu-id="989a4-133">Remove chat member</span></span>](../api/chat-delete-members.md)|<span data-ttu-id="989a4-134">无</span><span class="sxs-lookup"><span data-stu-id="989a4-134">None</span></span>|<span data-ttu-id="989a4-135">从聊天中删除用户。</span><span class="sxs-lookup"><span data-stu-id="989a4-135">Remove a user from the chat.</span></span>|
|[<span data-ttu-id="989a4-136">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="989a4-136">List messages in chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="989a4-137">chatMessage</span><span class="sxs-lookup"><span data-stu-id="989a4-137">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="989a4-138">获取聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="989a4-138">Get messages in a chat.</span></span> | 
|[<span data-ttu-id="989a4-139">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="989a4-139">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="989a4-140">chatMessage</span><span class="sxs-lookup"><span data-stu-id="989a4-140">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="989a4-141">获取聊天中的单个消息。</span><span class="sxs-lookup"><span data-stu-id="989a4-141">Get a single message in a chat.</span></span> | 
|[<span data-ttu-id="989a4-142">获取用户和应用之间的聊天</span><span class="sxs-lookup"><span data-stu-id="989a4-142">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="989a4-143">聊天</span><span class="sxs-lookup"><span data-stu-id="989a4-143">chat</span></span>](chat.md)| <span data-ttu-id="989a4-144">获取用户与应用之间的一对一聊天</span><span class="sxs-lookup"><span data-stu-id="989a4-144">Get one-on-one chat between user and the app</span></span> |
|[<span data-ttu-id="989a4-145">获取用户的所有聊天消息</span><span class="sxs-lookup"><span data-stu-id="989a4-145">Get messages across all chats for user</span></span>](../api/chats-getallmessages.md)| <span data-ttu-id="989a4-146">[chat](chat.md) 集合</span><span class="sxs-lookup"><span data-stu-id="989a4-146">[chat](chat.md) collection</span></span>| <span data-ttu-id="989a4-147">从用户参与的所有聊天中获取消息。</span><span class="sxs-lookup"><span data-stu-id="989a4-147">Get messages from all chats that a user is a participant in.</span></span> |
|[<span data-ttu-id="989a4-148">列出聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="989a4-148">List apps in chat</span></span>](../api/chat-list-installedapps.md) |<span data-ttu-id="989a4-149">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="989a4-149">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="989a4-150">列出聊天网站中安装 (关联的会议) 。</span><span class="sxs-lookup"><span data-stu-id="989a4-150">List apps installed in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="989a4-151">在聊天中获取应用</span><span class="sxs-lookup"><span data-stu-id="989a4-151">Get app in chat</span></span>](../api/chat-get-installedapps.md) | [<span data-ttu-id="989a4-152">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="989a4-152">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="989a4-153">获取安装在聊天会话和关联会议 (中的特定) 。</span><span class="sxs-lookup"><span data-stu-id="989a4-153">Get a specific app installed in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="989a4-154">在聊天中添加应用</span><span class="sxs-lookup"><span data-stu-id="989a4-154">Add app in chat</span></span>](../api/chat-post-installedapps.md) | | <span data-ttu-id="989a4-155">添加 (在) 会议及其关联会议 (中安装) 。</span><span class="sxs-lookup"><span data-stu-id="989a4-155">Add (install) an app in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="989a4-156">升级聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="989a4-156">Upgrade app in chat</span></span>](../api/chat-teamsappinstallation-upgrade.md) | <span data-ttu-id="989a4-157">无</span><span class="sxs-lookup"><span data-stu-id="989a4-157">None</span></span> | <span data-ttu-id="989a4-158">更新到聊天会话和相关会议 (安装的应用的) 。</span><span class="sxs-lookup"><span data-stu-id="989a4-158">Update to the latest version of the app installed in chat (and associated meeting).</span></span>|
|[<span data-ttu-id="989a4-159">从聊天中卸载应用</span><span class="sxs-lookup"><span data-stu-id="989a4-159">Uninstall app from chat</span></span>](../api/chat-delete-installedapps.md) | <span data-ttu-id="989a4-160">无</span><span class="sxs-lookup"><span data-stu-id="989a4-160">None</span></span> | <span data-ttu-id="989a4-161">从 (和) 会议记录中删除 (卸载) 。</span><span class="sxs-lookup"><span data-stu-id="989a4-161">Remove (uninstall) app from a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="989a4-162">列出聊天中的选项卡</span><span class="sxs-lookup"><span data-stu-id="989a4-162">List tabs in chat</span></span>](../api/chat-list-tabs.md) | [<span data-ttu-id="989a4-163">teamsTab</span><span class="sxs-lookup"><span data-stu-id="989a4-163">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="989a4-164">列出固定到聊天 (关联的会议选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="989a4-164">List tabs pinned to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="989a4-165">在聊天中获取选项卡</span><span class="sxs-lookup"><span data-stu-id="989a4-165">Get tab in chat</span></span>](../api/chat-get-tabs.md) | [<span data-ttu-id="989a4-166">teamsTab</span><span class="sxs-lookup"><span data-stu-id="989a4-166">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="989a4-167">获取固定到聊天组和关联 (的特定选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="989a4-167">Get a specific tab pinned to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="989a4-168">向聊天添加选项卡</span><span class="sxs-lookup"><span data-stu-id="989a4-168">Add tab to chat</span></span>](../api/chat-post-tabs.md) | [<span data-ttu-id="989a4-169">teamsTab</span><span class="sxs-lookup"><span data-stu-id="989a4-169">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="989a4-170">将 (固定) 选项卡添加到聊天 (关联的会议) 。</span><span class="sxs-lookup"><span data-stu-id="989a4-170">Add (pin) a tab to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="989a4-171">聊天中的"更新"选项卡</span><span class="sxs-lookup"><span data-stu-id="989a4-171">Update tab in chat</span></span>](../api/chat-patch-tabs.md) | [<span data-ttu-id="989a4-172">teamsTab</span><span class="sxs-lookup"><span data-stu-id="989a4-172">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="989a4-173">更新聊天记录和相关会议 (选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="989a4-173">Update the properties of a tab in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="989a4-174">从聊天中删除选项卡</span><span class="sxs-lookup"><span data-stu-id="989a4-174">Remove tab from chat</span></span>](../api/chat-delete-tabs.md) | <span data-ttu-id="989a4-175">无</span><span class="sxs-lookup"><span data-stu-id="989a4-175">None</span></span> | <span data-ttu-id="989a4-176">从 (和) 会议记录中删除 (取消固定选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="989a4-176">Remove (unpin) a tab from a chat (and associated meeting).</span></span>|

><span data-ttu-id="989a4-177">**注意：** 使用应用程序权限时，请务必了解如何获取聊天 ID。</span><span class="sxs-lookup"><span data-stu-id="989a4-177">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="989a4-178">由于不支持列出具有应用程序权限的聊天，因此并非所有方案都可行。</span><span class="sxs-lookup"><span data-stu-id="989a4-178">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="989a4-179">可以获取具有委派权限的聊天 ID，以及从具有应用程序权限的 [/chats/getAllMessages](../api/subscription-post-subscriptions.md) 更改通知获取。</span><span class="sxs-lookup"><span data-stu-id="989a4-179">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="989a4-180">属性</span><span class="sxs-lookup"><span data-stu-id="989a4-180">Properties</span></span>

| <span data-ttu-id="989a4-181">属性</span><span class="sxs-lookup"><span data-stu-id="989a4-181">Property</span></span>   | <span data-ttu-id="989a4-182">类型</span><span class="sxs-lookup"><span data-stu-id="989a4-182">Type</span></span> |<span data-ttu-id="989a4-183">说明</span><span class="sxs-lookup"><span data-stu-id="989a4-183">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="989a4-184">id</span><span class="sxs-lookup"><span data-stu-id="989a4-184">id</span></span>| <span data-ttu-id="989a4-185">字符串</span><span class="sxs-lookup"><span data-stu-id="989a4-185">String</span></span>| <span data-ttu-id="989a4-186">聊天的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="989a4-186">The chat's unique identifier.</span></span> <span data-ttu-id="989a4-187">只读。</span><span class="sxs-lookup"><span data-stu-id="989a4-187">Read-only.</span></span>|
| <span data-ttu-id="989a4-188">topic</span><span class="sxs-lookup"><span data-stu-id="989a4-188">topic</span></span>| <span data-ttu-id="989a4-189">String</span><span class="sxs-lookup"><span data-stu-id="989a4-189">String</span></span>|  <span data-ttu-id="989a4-190"> (聊天) 主题或主题。</span><span class="sxs-lookup"><span data-stu-id="989a4-190">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="989a4-191">仅适用于群聊。</span><span class="sxs-lookup"><span data-stu-id="989a4-191">Only available for group chats.</span></span>|
| <span data-ttu-id="989a4-192">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="989a4-192">createdDateTime</span></span>| <span data-ttu-id="989a4-193">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="989a4-193">dateTimeOffset</span></span>|  <span data-ttu-id="989a4-194">创建聊天的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="989a4-194">Date and time at which the chat was created.</span></span> <span data-ttu-id="989a4-195">只读。</span><span class="sxs-lookup"><span data-stu-id="989a4-195">Read-only.</span></span>|
| <span data-ttu-id="989a4-196">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="989a4-196">lastUpdatedDateTime</span></span>| <span data-ttu-id="989a4-197">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="989a4-197">dateTimeOffset</span></span>|  <span data-ttu-id="989a4-198">上次更改聊天的日期和时间或成员列表。</span><span class="sxs-lookup"><span data-stu-id="989a4-198">Date and time at which the chat was renamed or list of members were last changed.</span></span> <span data-ttu-id="989a4-199">只读。</span><span class="sxs-lookup"><span data-stu-id="989a4-199">Read-only.</span></span>|
| <span data-ttu-id="989a4-200">chatType</span><span class="sxs-lookup"><span data-stu-id="989a4-200">chatType</span></span>| [<span data-ttu-id="989a4-201">chatType</span><span class="sxs-lookup"><span data-stu-id="989a4-201">chatType</span></span>](../resources/chat.md#chattype-values) | <span data-ttu-id="989a4-202">指定聊天类型。</span><span class="sxs-lookup"><span data-stu-id="989a4-202">Specifies the type of chat.</span></span> <span data-ttu-id="989a4-203">可能的值是： `group` 和 `oneOnOne` `meeting` 。</span><span class="sxs-lookup"><span data-stu-id="989a4-203">Possible values are:`group`, `oneOnOne` and `meeting`.</span></span>|

### <a name="chattype-values"></a><span data-ttu-id="989a4-204">chatType 值</span><span class="sxs-lookup"><span data-stu-id="989a4-204">chatType values</span></span> 

| <span data-ttu-id="989a4-205">成员</span><span class="sxs-lookup"><span data-stu-id="989a4-205">Member</span></span>             | <span data-ttu-id="989a4-206">值</span><span class="sxs-lookup"><span data-stu-id="989a4-206">Value</span></span> | <span data-ttu-id="989a4-207">说明</span><span class="sxs-lookup"><span data-stu-id="989a4-207">Description</span></span>               |
| :----------------- | :---- | :------------------------ |
|<span data-ttu-id="989a4-208">oneOnOne</span><span class="sxs-lookup"><span data-stu-id="989a4-208">oneOnOne</span></span>            | <span data-ttu-id="989a4-209">0</span><span class="sxs-lookup"><span data-stu-id="989a4-209">0</span></span>     | <span data-ttu-id="989a4-210">指示聊天为一对一聊天。</span><span class="sxs-lookup"><span data-stu-id="989a4-210">Indicates that the chat is a 1:1 chat.</span></span> <span data-ttu-id="989a4-211">对于此类聊天，名单大小是固定的;无法删除/添加成员。</span><span class="sxs-lookup"><span data-stu-id="989a4-211">The roster size is fixed for this type of chat; members cannot be removed/added.</span></span>|
|<span data-ttu-id="989a4-212">group</span><span class="sxs-lookup"><span data-stu-id="989a4-212">group</span></span>               | <span data-ttu-id="989a4-213">1</span><span class="sxs-lookup"><span data-stu-id="989a4-213">1</span></span>     | <span data-ttu-id="989a4-214">指示聊天是群聊。</span><span class="sxs-lookup"><span data-stu-id="989a4-214">Indicates that the chat is a group chat.</span></span> <span data-ttu-id="989a4-215">可以针对 (聊天类型更新至少两) 名单大小。</span><span class="sxs-lookup"><span data-stu-id="989a4-215">The roster size (of at least two people) can be updated for this type of chat.</span></span> <span data-ttu-id="989a4-216">稍后可以删除/添加成员。</span><span class="sxs-lookup"><span data-stu-id="989a4-216">Members can be removed/added later.</span></span>|
|<span data-ttu-id="989a4-217">meeting</span><span class="sxs-lookup"><span data-stu-id="989a4-217">meeting</span></span>             | <span data-ttu-id="989a4-218">2</span><span class="sxs-lookup"><span data-stu-id="989a4-218">2</span></span>     | <span data-ttu-id="989a4-219">指示聊天与联机会议相关联。</span><span class="sxs-lookup"><span data-stu-id="989a4-219">Indicates that the chat is associated with an online meeting.</span></span> <span data-ttu-id="989a4-220">此类聊天仅在创建联机会议时创建。</span><span class="sxs-lookup"><span data-stu-id="989a4-220">This type of chat is only created as part of the creation of an online meeting.</span></span>|
|<span data-ttu-id="989a4-221">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="989a4-221">unknownFutureValue</span></span>  | <span data-ttu-id="989a4-222">3</span><span class="sxs-lookup"><span data-stu-id="989a4-222">3</span></span>     | <span data-ttu-id="989a4-223">Sentinel 值，用于指示未来值。</span><span class="sxs-lookup"><span data-stu-id="989a4-223">Sentinel value to indicate future values.</span></span> |

## <a name="relationships"></a><span data-ttu-id="989a4-224">关系</span><span class="sxs-lookup"><span data-stu-id="989a4-224">Relationships</span></span>

| <span data-ttu-id="989a4-225">关系</span><span class="sxs-lookup"><span data-stu-id="989a4-225">Relationship</span></span> | <span data-ttu-id="989a4-226">类型</span><span class="sxs-lookup"><span data-stu-id="989a4-226">Type</span></span> |<span data-ttu-id="989a4-227">说明</span><span class="sxs-lookup"><span data-stu-id="989a4-227">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="989a4-228">installedApps</span><span class="sxs-lookup"><span data-stu-id="989a4-228">installedApps</span></span> | <span data-ttu-id="989a4-229">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="989a4-229">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="989a4-230">聊天中所有应用的集合。</span><span class="sxs-lookup"><span data-stu-id="989a4-230">A collection of all the apps in the chat.</span></span> <span data-ttu-id="989a4-231">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="989a4-231">Nullable.</span></span> |
| <span data-ttu-id="989a4-232">members</span><span class="sxs-lookup"><span data-stu-id="989a4-232">members</span></span> | <span data-ttu-id="989a4-233">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="989a4-233">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="989a4-234">聊天中所有成员的集合。</span><span class="sxs-lookup"><span data-stu-id="989a4-234">A collection of all the members in the chat.</span></span> <span data-ttu-id="989a4-235">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="989a4-235">Nullable.</span></span> |
| <span data-ttu-id="989a4-236">messages</span><span class="sxs-lookup"><span data-stu-id="989a4-236">messages</span></span> | <span data-ttu-id="989a4-237">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="989a4-237">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="989a4-238">聊天中所有消息的集合。</span><span class="sxs-lookup"><span data-stu-id="989a4-238">A collection of all the messages in the chat.</span></span> <span data-ttu-id="989a4-239">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="989a4-239">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="989a4-240">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="989a4-240">JSON representation</span></span>

<span data-ttu-id="989a4-241">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="989a4-241">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="989a4-242">另请参阅</span><span class="sxs-lookup"><span data-stu-id="989a4-242">See also</span></span>

- [<span data-ttu-id="989a4-243">频道</span><span class="sxs-lookup"><span data-stu-id="989a4-243">channel</span></span>](channel.md)
- [<span data-ttu-id="989a4-244">chatMessage</span><span class="sxs-lookup"><span data-stu-id="989a4-244">chatMessage</span></span>](chatmessage.md)

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


