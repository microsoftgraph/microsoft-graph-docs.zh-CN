---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 chatMessages 集合。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 82512c8b934d76ef83e9f6686dbaca40bbd122b3
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061852"
---
# <a name="chat-resource-type"></a><span data-ttu-id="01f67-103">聊天资源类型</span><span class="sxs-lookup"><span data-stu-id="01f67-103">chat resource type</span></span>

<span data-ttu-id="01f67-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01f67-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="01f67-105">聊天是一个或多个 [参与者之间的 chatMessages](chatmessage.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="01f67-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="01f67-106">参与者可以是用户或应用。</span><span class="sxs-lookup"><span data-stu-id="01f67-106">Participants can be users or apps.</span></span>

> <span data-ttu-id="01f67-107">**注意**：如果聊天与 [onlineMeeting](../resources/onlinemeeting.md) 实例关联，则列出的一些方法将可传递影响会议。</span><span class="sxs-lookup"><span data-stu-id="01f67-107">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then some of the listed methods will transitively impact the meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="01f67-108">方法</span><span class="sxs-lookup"><span data-stu-id="01f67-108">Methods</span></span>

|  <span data-ttu-id="01f67-109">方法</span><span class="sxs-lookup"><span data-stu-id="01f67-109">Method</span></span>       |  <span data-ttu-id="01f67-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="01f67-110">Return Type</span></span>  | <span data-ttu-id="01f67-111">说明</span><span class="sxs-lookup"><span data-stu-id="01f67-111">Description</span></span>| 
|:---------------|:--------|:----------|
| <span data-ttu-id="01f67-112">**聊天管理**</span><span class="sxs-lookup"><span data-stu-id="01f67-112">**Chat management**</span></span> |||
|[<span data-ttu-id="01f67-113">创建聊天</span><span class="sxs-lookup"><span data-stu-id="01f67-113">Create chat</span></span>](../api/chat-post.md) | [<span data-ttu-id="01f67-114">聊天</span><span class="sxs-lookup"><span data-stu-id="01f67-114">chat</span></span>](chat.md) | <span data-ttu-id="01f67-115">创建新聊天。</span><span class="sxs-lookup"><span data-stu-id="01f67-115">Create a new chat.</span></span>| 
|[<span data-ttu-id="01f67-116">获取聊天</span><span class="sxs-lookup"><span data-stu-id="01f67-116">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="01f67-117">聊天</span><span class="sxs-lookup"><span data-stu-id="01f67-117">chat</span></span>](chat.md) | <span data-ttu-id="01f67-118">读取聊天的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="01f67-118">Read properties and relationships of the chat.</span></span>| 
|[<span data-ttu-id="01f67-119">更新聊天</span><span class="sxs-lookup"><span data-stu-id="01f67-119">Update chat</span></span>](../api/chat-patch.md) | [<span data-ttu-id="01f67-120">聊天</span><span class="sxs-lookup"><span data-stu-id="01f67-120">chat</span></span>](chat.md) | <span data-ttu-id="01f67-121">更新聊天的属性。</span><span class="sxs-lookup"><span data-stu-id="01f67-121">Update properties of the chat.</span></span>|
|[<span data-ttu-id="01f67-122">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="01f67-122">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="01f67-123">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="01f67-123">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="01f67-124">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="01f67-124">Get the list of all users in the chat.</span></span>| 
|[<span data-ttu-id="01f67-125">添加聊天成员</span><span class="sxs-lookup"><span data-stu-id="01f67-125">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="01f67-126">位置标头</span><span class="sxs-lookup"><span data-stu-id="01f67-126">Location header</span></span> | <span data-ttu-id="01f67-127">向聊天中添加用户。</span><span class="sxs-lookup"><span data-stu-id="01f67-127">Add a user to the chat.</span></span>| 
|[<span data-ttu-id="01f67-128">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="01f67-128">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="01f67-129">conversationMember</span><span class="sxs-lookup"><span data-stu-id="01f67-129">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="01f67-130">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="01f67-130">Get a single user in the chat.</span></span>| 
|[<span data-ttu-id="01f67-131">删除聊天成员</span><span class="sxs-lookup"><span data-stu-id="01f67-131">Remove chat member</span></span>](../api/chat-delete-members.md)|<span data-ttu-id="01f67-132">无</span><span class="sxs-lookup"><span data-stu-id="01f67-132">None</span></span>|<span data-ttu-id="01f67-133">从聊天中删除用户。</span><span class="sxs-lookup"><span data-stu-id="01f67-133">Remove a user from the chat.</span></span>|
|[<span data-ttu-id="01f67-134">获取用户和应用之间的聊天</span><span class="sxs-lookup"><span data-stu-id="01f67-134">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="01f67-135">聊天</span><span class="sxs-lookup"><span data-stu-id="01f67-135">chat</span></span>](chat.md)| <span data-ttu-id="01f67-136">获取用户与应用之间的一对一聊天</span><span class="sxs-lookup"><span data-stu-id="01f67-136">Get one-on-one chat between user and the app</span></span> |
| <span data-ttu-id="01f67-137">**邮件**</span><span class="sxs-lookup"><span data-stu-id="01f67-137">**Messages**</span></span> |||
|[<span data-ttu-id="01f67-138">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="01f67-138">List messages in chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="01f67-139">chatMessage</span><span class="sxs-lookup"><span data-stu-id="01f67-139">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="01f67-140">获取聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="01f67-140">Get messages in a chat.</span></span> | 
|[<span data-ttu-id="01f67-141">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="01f67-141">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="01f67-142">chatMessage</span><span class="sxs-lookup"><span data-stu-id="01f67-142">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="01f67-143">获取聊天中的单个消息。</span><span class="sxs-lookup"><span data-stu-id="01f67-143">Get a single message in a chat.</span></span> | 
| <span data-ttu-id="01f67-144">**应用**</span><span class="sxs-lookup"><span data-stu-id="01f67-144">**Apps**</span></span> |||
|[<span data-ttu-id="01f67-145">列出聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="01f67-145">List apps in chat</span></span>](../api/chat-list-installedapps.md) |<span data-ttu-id="01f67-146">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="01f67-146">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="01f67-147">列出聊天网站中安装 (关联的会议) 。</span><span class="sxs-lookup"><span data-stu-id="01f67-147">List apps installed in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="01f67-148">在聊天中获取应用</span><span class="sxs-lookup"><span data-stu-id="01f67-148">Get app in chat</span></span>](../api/chat-get-installedapps.md) | [<span data-ttu-id="01f67-149">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="01f67-149">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="01f67-150">获取安装在聊天会话和关联会议 (中的特定) 。</span><span class="sxs-lookup"><span data-stu-id="01f67-150">Get a specific app installed in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="01f67-151">在聊天中添加应用</span><span class="sxs-lookup"><span data-stu-id="01f67-151">Add app in chat</span></span>](../api/chat-post-installedapps.md) | | <span data-ttu-id="01f67-152">添加 (在) 会议及其关联会议 (中安装) 。</span><span class="sxs-lookup"><span data-stu-id="01f67-152">Add (install) an app in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="01f67-153">升级聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="01f67-153">Upgrade app in chat</span></span>](../api/chat-teamsappinstallation-upgrade.md) | <span data-ttu-id="01f67-154">无</span><span class="sxs-lookup"><span data-stu-id="01f67-154">None</span></span> | <span data-ttu-id="01f67-155">更新到聊天会话和相关会议 (安装的应用的) 。</span><span class="sxs-lookup"><span data-stu-id="01f67-155">Update to the latest version of the app installed in chat (and associated meeting).</span></span>|
|[<span data-ttu-id="01f67-156">从聊天中卸载应用</span><span class="sxs-lookup"><span data-stu-id="01f67-156">Uninstall app from chat</span></span>](../api/chat-delete-installedapps.md) | <span data-ttu-id="01f67-157">无</span><span class="sxs-lookup"><span data-stu-id="01f67-157">None</span></span> | <span data-ttu-id="01f67-158">从 (和) 会议记录中删除 (卸载) 。</span><span class="sxs-lookup"><span data-stu-id="01f67-158">Remove (uninstall) app from a chat (and associated meeting).</span></span>|
| <span data-ttu-id="01f67-159">**选项卡**</span><span class="sxs-lookup"><span data-stu-id="01f67-159">**Tabs**</span></span> |||
|[<span data-ttu-id="01f67-160">列出聊天中的选项卡</span><span class="sxs-lookup"><span data-stu-id="01f67-160">List tabs in chat</span></span>](../api/chat-list-tabs.md) | [<span data-ttu-id="01f67-161">teamsTab</span><span class="sxs-lookup"><span data-stu-id="01f67-161">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="01f67-162">列出固定到聊天 (关联的会议选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="01f67-162">List tabs pinned to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="01f67-163">在聊天中获取选项卡</span><span class="sxs-lookup"><span data-stu-id="01f67-163">Get tab in chat</span></span>](../api/chat-get-tabs.md) | [<span data-ttu-id="01f67-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="01f67-164">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="01f67-165">获取固定到聊天组和关联 (的特定选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="01f67-165">Get a specific tab pinned to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="01f67-166">向聊天添加选项卡</span><span class="sxs-lookup"><span data-stu-id="01f67-166">Add tab to chat</span></span>](../api/chat-post-tabs.md) | [<span data-ttu-id="01f67-167">teamsTab</span><span class="sxs-lookup"><span data-stu-id="01f67-167">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="01f67-168">将 (固定) 选项卡添加到聊天 (关联的会议) 。</span><span class="sxs-lookup"><span data-stu-id="01f67-168">Add (pin) a tab to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="01f67-169">聊天中的"更新"选项卡</span><span class="sxs-lookup"><span data-stu-id="01f67-169">Update tab in chat</span></span>](../api/chat-patch-tabs.md) | [<span data-ttu-id="01f67-170">teamsTab</span><span class="sxs-lookup"><span data-stu-id="01f67-170">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="01f67-171">更新聊天记录和相关会议 (选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="01f67-171">Update the properties of a tab in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="01f67-172">从聊天中删除选项卡</span><span class="sxs-lookup"><span data-stu-id="01f67-172">Remove tab from chat</span></span>](../api/chat-delete-tabs.md) | <span data-ttu-id="01f67-173">无</span><span class="sxs-lookup"><span data-stu-id="01f67-173">None</span></span> | <span data-ttu-id="01f67-174">从 (和) 会议记录中删除 (取消固定选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="01f67-174">Remove (unpin) a tab from a chat (and associated meeting).</span></span>|

><span data-ttu-id="01f67-175">**注意：** 使用应用程序权限时，请务必了解如何获取聊天 ID。</span><span class="sxs-lookup"><span data-stu-id="01f67-175">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="01f67-176">由于不支持列出具有应用程序权限的聊天，因此并非所有方案都可行。</span><span class="sxs-lookup"><span data-stu-id="01f67-176">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="01f67-177">可以获取具有委派权限的聊天 ID，以及从具有应用程序权限的 [/chats/getAllMessages](../api/subscription-post-subscriptions.md) 更改通知获取。</span><span class="sxs-lookup"><span data-stu-id="01f67-177">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="01f67-178">属性</span><span class="sxs-lookup"><span data-stu-id="01f67-178">Properties</span></span>

| <span data-ttu-id="01f67-179">属性</span><span class="sxs-lookup"><span data-stu-id="01f67-179">Property</span></span>   | <span data-ttu-id="01f67-180">类型</span><span class="sxs-lookup"><span data-stu-id="01f67-180">Type</span></span> |<span data-ttu-id="01f67-181">说明</span><span class="sxs-lookup"><span data-stu-id="01f67-181">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="01f67-182">id</span><span class="sxs-lookup"><span data-stu-id="01f67-182">id</span></span>| <span data-ttu-id="01f67-183">String</span><span class="sxs-lookup"><span data-stu-id="01f67-183">String</span></span>| <span data-ttu-id="01f67-184">聊天的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="01f67-184">The chat's unique identifier.</span></span> <span data-ttu-id="01f67-185">只读。</span><span class="sxs-lookup"><span data-stu-id="01f67-185">Read-only.</span></span>|
| <span data-ttu-id="01f67-186">topic</span><span class="sxs-lookup"><span data-stu-id="01f67-186">topic</span></span>| <span data-ttu-id="01f67-187">String</span><span class="sxs-lookup"><span data-stu-id="01f67-187">String</span></span>|  <span data-ttu-id="01f67-188"> (聊天) 主题或主题。</span><span class="sxs-lookup"><span data-stu-id="01f67-188">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="01f67-189">仅适用于群聊。</span><span class="sxs-lookup"><span data-stu-id="01f67-189">Only available for group chats.</span></span>|
| <span data-ttu-id="01f67-190">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="01f67-190">createdDateTime</span></span>| <span data-ttu-id="01f67-191">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01f67-191">dateTimeOffset</span></span>|  <span data-ttu-id="01f67-192">创建聊天的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="01f67-192">Date and time at which the chat was created.</span></span> <span data-ttu-id="01f67-193">只读。</span><span class="sxs-lookup"><span data-stu-id="01f67-193">Read-only.</span></span>|
| <span data-ttu-id="01f67-194">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="01f67-194">lastUpdatedDateTime</span></span>| <span data-ttu-id="01f67-195">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01f67-195">dateTimeOffset</span></span>|  <span data-ttu-id="01f67-196">上次更改聊天的日期和时间或成员列表。</span><span class="sxs-lookup"><span data-stu-id="01f67-196">Date and time at which the chat was renamed or list of members were last changed.</span></span> <span data-ttu-id="01f67-197">只读。</span><span class="sxs-lookup"><span data-stu-id="01f67-197">Read-only.</span></span>|
| <span data-ttu-id="01f67-198">chatType</span><span class="sxs-lookup"><span data-stu-id="01f67-198">chatType</span></span>| [<span data-ttu-id="01f67-199">chatType</span><span class="sxs-lookup"><span data-stu-id="01f67-199">chatType</span></span>](../resources/chat.md#chattype-values) | <span data-ttu-id="01f67-200">指定聊天类型。</span><span class="sxs-lookup"><span data-stu-id="01f67-200">Specifies the type of chat.</span></span> <span data-ttu-id="01f67-201">可能的值是： `group` 和 `oneOnOne` `meeting` 。</span><span class="sxs-lookup"><span data-stu-id="01f67-201">Possible values are:`group`, `oneOnOne` and `meeting`.</span></span>|

### <a name="chattype-values"></a><span data-ttu-id="01f67-202">chatType 值</span><span class="sxs-lookup"><span data-stu-id="01f67-202">chatType values</span></span> 

| <span data-ttu-id="01f67-203">成员</span><span class="sxs-lookup"><span data-stu-id="01f67-203">Member</span></span>             | <span data-ttu-id="01f67-204">值</span><span class="sxs-lookup"><span data-stu-id="01f67-204">Value</span></span> | <span data-ttu-id="01f67-205">说明</span><span class="sxs-lookup"><span data-stu-id="01f67-205">Description</span></span>               |
| :----------------- | :---- | :------------------------ |
|<span data-ttu-id="01f67-206">oneOnOne</span><span class="sxs-lookup"><span data-stu-id="01f67-206">oneOnOne</span></span>            | <span data-ttu-id="01f67-207">0</span><span class="sxs-lookup"><span data-stu-id="01f67-207">0</span></span>     | <span data-ttu-id="01f67-208">指示聊天为一对一聊天。</span><span class="sxs-lookup"><span data-stu-id="01f67-208">Indicates that the chat is a 1:1 chat.</span></span> <span data-ttu-id="01f67-209">对于此类聊天，名单大小是固定的;无法删除/添加成员。</span><span class="sxs-lookup"><span data-stu-id="01f67-209">The roster size is fixed for this type of chat; members cannot be removed/added.</span></span>|
|<span data-ttu-id="01f67-210">group</span><span class="sxs-lookup"><span data-stu-id="01f67-210">group</span></span>               | <span data-ttu-id="01f67-211">1</span><span class="sxs-lookup"><span data-stu-id="01f67-211">1</span></span>     | <span data-ttu-id="01f67-212">指示聊天是群聊。</span><span class="sxs-lookup"><span data-stu-id="01f67-212">Indicates that the chat is a group chat.</span></span> <span data-ttu-id="01f67-213">可以针对 (聊天类型更新至少两) 名单大小。</span><span class="sxs-lookup"><span data-stu-id="01f67-213">The roster size (of at least two people) can be updated for this type of chat.</span></span> <span data-ttu-id="01f67-214">稍后可以删除/添加成员。</span><span class="sxs-lookup"><span data-stu-id="01f67-214">Members can be removed/added later.</span></span>|
|<span data-ttu-id="01f67-215">meeting</span><span class="sxs-lookup"><span data-stu-id="01f67-215">meeting</span></span>             | <span data-ttu-id="01f67-216">2</span><span class="sxs-lookup"><span data-stu-id="01f67-216">2</span></span>     | <span data-ttu-id="01f67-217">指示聊天与联机会议相关联。</span><span class="sxs-lookup"><span data-stu-id="01f67-217">Indicates that the chat is associated with an online meeting.</span></span> <span data-ttu-id="01f67-218">此类聊天仅在创建联机会议时创建。</span><span class="sxs-lookup"><span data-stu-id="01f67-218">This type of chat is only created as part of the creation of an online meeting.</span></span>|
|<span data-ttu-id="01f67-219">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="01f67-219">unknownFutureValue</span></span>  | <span data-ttu-id="01f67-220">3</span><span class="sxs-lookup"><span data-stu-id="01f67-220">3</span></span>     | <span data-ttu-id="01f67-221">Sentinel 值，用于指示未来值。</span><span class="sxs-lookup"><span data-stu-id="01f67-221">Sentinel value to indicate future values.</span></span> |

## <a name="relationships"></a><span data-ttu-id="01f67-222">关系</span><span class="sxs-lookup"><span data-stu-id="01f67-222">Relationships</span></span>

| <span data-ttu-id="01f67-223">关系</span><span class="sxs-lookup"><span data-stu-id="01f67-223">Relationship</span></span> | <span data-ttu-id="01f67-224">类型</span><span class="sxs-lookup"><span data-stu-id="01f67-224">Type</span></span> |<span data-ttu-id="01f67-225">说明</span><span class="sxs-lookup"><span data-stu-id="01f67-225">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="01f67-226">installedApps</span><span class="sxs-lookup"><span data-stu-id="01f67-226">installedApps</span></span> | <span data-ttu-id="01f67-227">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="01f67-227">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="01f67-228">聊天中所有应用的集合。</span><span class="sxs-lookup"><span data-stu-id="01f67-228">A collection of all the apps in the chat.</span></span> <span data-ttu-id="01f67-229">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="01f67-229">Nullable.</span></span> |
| <span data-ttu-id="01f67-230">members</span><span class="sxs-lookup"><span data-stu-id="01f67-230">members</span></span> | <span data-ttu-id="01f67-231">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="01f67-231">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="01f67-232">聊天中所有成员的集合。</span><span class="sxs-lookup"><span data-stu-id="01f67-232">A collection of all the members in the chat.</span></span> <span data-ttu-id="01f67-233">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="01f67-233">Nullable.</span></span> |
| <span data-ttu-id="01f67-234">messages</span><span class="sxs-lookup"><span data-stu-id="01f67-234">messages</span></span> | <span data-ttu-id="01f67-235">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="01f67-235">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="01f67-236">聊天中所有消息的集合。</span><span class="sxs-lookup"><span data-stu-id="01f67-236">A collection of all the messages in the chat.</span></span> <span data-ttu-id="01f67-237">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="01f67-237">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="01f67-238">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01f67-238">JSON representation</span></span>

<span data-ttu-id="01f67-239">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01f67-239">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="01f67-240">另请参阅</span><span class="sxs-lookup"><span data-stu-id="01f67-240">See also</span></span>

- [<span data-ttu-id="01f67-241">频道</span><span class="sxs-lookup"><span data-stu-id="01f67-241">channel</span></span>](channel.md)
- [<span data-ttu-id="01f67-242">chatMessage</span><span class="sxs-lookup"><span data-stu-id="01f67-242">chatMessage</span></span>](chatmessage.md)

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


