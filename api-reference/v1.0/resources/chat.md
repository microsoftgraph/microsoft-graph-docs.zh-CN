---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 chatMessages 集合。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 51980c166652ea2a2d863049e5877b3cc6d632ba
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582786"
---
# <a name="chat-resource-type"></a><span data-ttu-id="16453-103">聊天资源类型</span><span class="sxs-lookup"><span data-stu-id="16453-103">chat resource type</span></span>

<span data-ttu-id="16453-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16453-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16453-105">聊天是一个或多个 [参与者之间的 chatMessages](chatmessage.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="16453-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="16453-106">参与者可以是用户或应用。</span><span class="sxs-lookup"><span data-stu-id="16453-106">Participants can be users or apps.</span></span>

> <span data-ttu-id="16453-107">**注意**：如果聊天与 [onlineMeeting](../resources/onlinemeeting.md) 实例关联，则列出的一些方法将可传递影响会议。</span><span class="sxs-lookup"><span data-stu-id="16453-107">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then some of the listed methods will transitively impact the meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="16453-108">方法</span><span class="sxs-lookup"><span data-stu-id="16453-108">Methods</span></span>

|  <span data-ttu-id="16453-109">方法</span><span class="sxs-lookup"><span data-stu-id="16453-109">Method</span></span>       |  <span data-ttu-id="16453-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="16453-110">Return Type</span></span>  | <span data-ttu-id="16453-111">说明</span><span class="sxs-lookup"><span data-stu-id="16453-111">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="16453-112">创建聊天</span><span class="sxs-lookup"><span data-stu-id="16453-112">Create chat</span></span>](../api/chat-post.md) | [<span data-ttu-id="16453-113">聊天</span><span class="sxs-lookup"><span data-stu-id="16453-113">chat</span></span>](chat.md) | <span data-ttu-id="16453-114">创建新聊天。</span><span class="sxs-lookup"><span data-stu-id="16453-114">Create a new chat.</span></span>| 
|[<span data-ttu-id="16453-115">获取聊天</span><span class="sxs-lookup"><span data-stu-id="16453-115">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="16453-116">聊天</span><span class="sxs-lookup"><span data-stu-id="16453-116">chat</span></span>](chat.md) | <span data-ttu-id="16453-117">读取聊天的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="16453-117">Read properties and relationships of the chat.</span></span>| 
|[<span data-ttu-id="16453-118">更新聊天</span><span class="sxs-lookup"><span data-stu-id="16453-118">Update chat</span></span>](../api/chat-patch.md) | [<span data-ttu-id="16453-119">聊天</span><span class="sxs-lookup"><span data-stu-id="16453-119">chat</span></span>](chat.md) | <span data-ttu-id="16453-120">更新聊天的属性。</span><span class="sxs-lookup"><span data-stu-id="16453-120">Update properties of the chat.</span></span>|
|[<span data-ttu-id="16453-121">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="16453-121">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="16453-122">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16453-122">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="16453-123">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="16453-123">Get the list of all users in the chat.</span></span>| 
|[<span data-ttu-id="16453-124">添加聊天成员</span><span class="sxs-lookup"><span data-stu-id="16453-124">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="16453-125">位置标头</span><span class="sxs-lookup"><span data-stu-id="16453-125">Location header</span></span> | <span data-ttu-id="16453-126">向聊天中添加用户。</span><span class="sxs-lookup"><span data-stu-id="16453-126">Add a user to the chat.</span></span>| 
|[<span data-ttu-id="16453-127">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="16453-127">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="16453-128">conversationMember</span><span class="sxs-lookup"><span data-stu-id="16453-128">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="16453-129">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="16453-129">Get a single user in the chat.</span></span>| 
|[<span data-ttu-id="16453-130">删除聊天成员</span><span class="sxs-lookup"><span data-stu-id="16453-130">Remove chat member</span></span>](../api/chat-delete-members.md)|<span data-ttu-id="16453-131">无</span><span class="sxs-lookup"><span data-stu-id="16453-131">None</span></span>|<span data-ttu-id="16453-132">从聊天中删除用户。</span><span class="sxs-lookup"><span data-stu-id="16453-132">Remove a user from the chat.</span></span>|
|[<span data-ttu-id="16453-133">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="16453-133">List messages in chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="16453-134">chatMessage</span><span class="sxs-lookup"><span data-stu-id="16453-134">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="16453-135">获取聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="16453-135">Get messages in a chat.</span></span> | 
|[<span data-ttu-id="16453-136">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="16453-136">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="16453-137">chatMessage</span><span class="sxs-lookup"><span data-stu-id="16453-137">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="16453-138">获取聊天中的单个消息。</span><span class="sxs-lookup"><span data-stu-id="16453-138">Get a single message in a chat.</span></span> | 
|[<span data-ttu-id="16453-139">获取用户和应用之间的聊天</span><span class="sxs-lookup"><span data-stu-id="16453-139">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="16453-140">聊天</span><span class="sxs-lookup"><span data-stu-id="16453-140">chat</span></span>](chat.md)| <span data-ttu-id="16453-141">获取用户与应用之间的一对一聊天</span><span class="sxs-lookup"><span data-stu-id="16453-141">Get one-on-one chat between user and the app</span></span> |
|[<span data-ttu-id="16453-142">列出聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="16453-142">List apps in chat</span></span>](../api/chat-list-installedapps.md) |<span data-ttu-id="16453-143">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16453-143">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="16453-144">列出聊天网站中安装 (关联的会议) 。</span><span class="sxs-lookup"><span data-stu-id="16453-144">List apps installed in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="16453-145">在聊天中获取应用</span><span class="sxs-lookup"><span data-stu-id="16453-145">Get app in chat</span></span>](../api/chat-get-installedapps.md) | [<span data-ttu-id="16453-146">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="16453-146">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="16453-147">获取安装在聊天会话和关联会议 (中的特定) 。</span><span class="sxs-lookup"><span data-stu-id="16453-147">Get a specific app installed in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="16453-148">在聊天中添加应用</span><span class="sxs-lookup"><span data-stu-id="16453-148">Add app in chat</span></span>](../api/chat-post-installedapps.md) | | <span data-ttu-id="16453-149">添加 (在) 会议及其关联会议 (中安装) 。</span><span class="sxs-lookup"><span data-stu-id="16453-149">Add (install) an app in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="16453-150">升级聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="16453-150">Upgrade app in chat</span></span>](../api/chat-teamsappinstallation-upgrade.md) | <span data-ttu-id="16453-151">无</span><span class="sxs-lookup"><span data-stu-id="16453-151">None</span></span> | <span data-ttu-id="16453-152">更新到聊天会话和相关会议 (安装的应用的) 。</span><span class="sxs-lookup"><span data-stu-id="16453-152">Update to the latest version of the app installed in chat (and associated meeting).</span></span>|
|[<span data-ttu-id="16453-153">从聊天中卸载应用</span><span class="sxs-lookup"><span data-stu-id="16453-153">Uninstall app from chat</span></span>](../api/chat-delete-installedapps.md) | <span data-ttu-id="16453-154">无</span><span class="sxs-lookup"><span data-stu-id="16453-154">None</span></span> | <span data-ttu-id="16453-155">从 (和) 会议记录中删除 (卸载) 。</span><span class="sxs-lookup"><span data-stu-id="16453-155">Remove (uninstall) app from a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="16453-156">列出聊天中的选项卡</span><span class="sxs-lookup"><span data-stu-id="16453-156">List tabs in chat</span></span>](../api/chat-list-tabs.md) | [<span data-ttu-id="16453-157">teamsTab</span><span class="sxs-lookup"><span data-stu-id="16453-157">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="16453-158">列出固定到聊天 (关联的会议选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="16453-158">List tabs pinned to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="16453-159">在聊天中获取选项卡</span><span class="sxs-lookup"><span data-stu-id="16453-159">Get tab in chat</span></span>](../api/chat-get-tabs.md) | [<span data-ttu-id="16453-160">teamsTab</span><span class="sxs-lookup"><span data-stu-id="16453-160">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="16453-161">获取固定到聊天组和关联 (的特定选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="16453-161">Get a specific tab pinned to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="16453-162">向聊天添加选项卡</span><span class="sxs-lookup"><span data-stu-id="16453-162">Add tab to chat</span></span>](../api/chat-post-tabs.md) | [<span data-ttu-id="16453-163">teamsTab</span><span class="sxs-lookup"><span data-stu-id="16453-163">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="16453-164">将 (固定) 选项卡添加到聊天 (关联的会议) 。</span><span class="sxs-lookup"><span data-stu-id="16453-164">Add (pin) a tab to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="16453-165">聊天中的"更新"选项卡</span><span class="sxs-lookup"><span data-stu-id="16453-165">Update tab in chat</span></span>](../api/chat-patch-tabs.md) | [<span data-ttu-id="16453-166">teamsTab</span><span class="sxs-lookup"><span data-stu-id="16453-166">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="16453-167">更新聊天记录和相关会议 (选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="16453-167">Update the properties of a tab in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="16453-168">从聊天中删除选项卡</span><span class="sxs-lookup"><span data-stu-id="16453-168">Remove tab from chat</span></span>](../api/chat-delete-tabs.md) | <span data-ttu-id="16453-169">无</span><span class="sxs-lookup"><span data-stu-id="16453-169">None</span></span> | <span data-ttu-id="16453-170">从 (和) 会议记录中删除 (取消固定选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="16453-170">Remove (unpin) a tab from a chat (and associated meeting).</span></span>|

><span data-ttu-id="16453-171">**注意：** 使用应用程序权限时，请务必了解如何获取聊天 ID。</span><span class="sxs-lookup"><span data-stu-id="16453-171">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="16453-172">由于不支持列出具有应用程序权限的聊天，因此并非所有方案都可行。</span><span class="sxs-lookup"><span data-stu-id="16453-172">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="16453-173">可以获取具有委派权限的聊天 ID，以及从具有应用程序权限的 [/chats/getAllMessages](../api/subscription-post-subscriptions.md) 更改通知获取。</span><span class="sxs-lookup"><span data-stu-id="16453-173">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="16453-174">属性</span><span class="sxs-lookup"><span data-stu-id="16453-174">Properties</span></span>

| <span data-ttu-id="16453-175">属性</span><span class="sxs-lookup"><span data-stu-id="16453-175">Property</span></span>   | <span data-ttu-id="16453-176">类型</span><span class="sxs-lookup"><span data-stu-id="16453-176">Type</span></span> |<span data-ttu-id="16453-177">说明</span><span class="sxs-lookup"><span data-stu-id="16453-177">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="16453-178">id</span><span class="sxs-lookup"><span data-stu-id="16453-178">id</span></span>| <span data-ttu-id="16453-179">String</span><span class="sxs-lookup"><span data-stu-id="16453-179">String</span></span>| <span data-ttu-id="16453-180">聊天的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="16453-180">The chat's unique identifier.</span></span> <span data-ttu-id="16453-181">只读。</span><span class="sxs-lookup"><span data-stu-id="16453-181">Read-only.</span></span>|
| <span data-ttu-id="16453-182">topic</span><span class="sxs-lookup"><span data-stu-id="16453-182">topic</span></span>| <span data-ttu-id="16453-183">String</span><span class="sxs-lookup"><span data-stu-id="16453-183">String</span></span>|  <span data-ttu-id="16453-184"> (聊天) 主题或主题。</span><span class="sxs-lookup"><span data-stu-id="16453-184">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="16453-185">仅适用于群聊。</span><span class="sxs-lookup"><span data-stu-id="16453-185">Only available for group chats.</span></span>|
| <span data-ttu-id="16453-186">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16453-186">createdDateTime</span></span>| <span data-ttu-id="16453-187">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16453-187">dateTimeOffset</span></span>|  <span data-ttu-id="16453-188">创建聊天的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="16453-188">Date and time at which the chat was created.</span></span> <span data-ttu-id="16453-189">只读。</span><span class="sxs-lookup"><span data-stu-id="16453-189">Read-only.</span></span>|
| <span data-ttu-id="16453-190">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="16453-190">lastUpdatedDateTime</span></span>| <span data-ttu-id="16453-191">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16453-191">dateTimeOffset</span></span>|  <span data-ttu-id="16453-192">上次更改聊天的日期和时间或成员列表。</span><span class="sxs-lookup"><span data-stu-id="16453-192">Date and time at which the chat was renamed or list of members were last changed.</span></span> <span data-ttu-id="16453-193">只读。</span><span class="sxs-lookup"><span data-stu-id="16453-193">Read-only.</span></span>|
| <span data-ttu-id="16453-194">chatType</span><span class="sxs-lookup"><span data-stu-id="16453-194">chatType</span></span>| [<span data-ttu-id="16453-195">chatType</span><span class="sxs-lookup"><span data-stu-id="16453-195">chatType</span></span>](../resources/chat.md#chattype-values) | <span data-ttu-id="16453-196">指定聊天类型。</span><span class="sxs-lookup"><span data-stu-id="16453-196">Specifies the type of chat.</span></span> <span data-ttu-id="16453-197">可能的值是： `group` 和 `oneOnOne` `meeting` 。</span><span class="sxs-lookup"><span data-stu-id="16453-197">Possible values are:`group`, `oneOnOne` and `meeting`.</span></span>|

### <a name="chattype-values"></a><span data-ttu-id="16453-198">chatType 值</span><span class="sxs-lookup"><span data-stu-id="16453-198">chatType values</span></span> 

| <span data-ttu-id="16453-199">成员</span><span class="sxs-lookup"><span data-stu-id="16453-199">Member</span></span>             | <span data-ttu-id="16453-200">值</span><span class="sxs-lookup"><span data-stu-id="16453-200">Value</span></span> | <span data-ttu-id="16453-201">说明</span><span class="sxs-lookup"><span data-stu-id="16453-201">Description</span></span>               |
| :----------------- | :---- | :------------------------ |
|<span data-ttu-id="16453-202">oneOnOne</span><span class="sxs-lookup"><span data-stu-id="16453-202">oneOnOne</span></span>            | <span data-ttu-id="16453-203">0</span><span class="sxs-lookup"><span data-stu-id="16453-203">0</span></span>     | <span data-ttu-id="16453-204">指示聊天为一对一聊天。</span><span class="sxs-lookup"><span data-stu-id="16453-204">Indicates that the chat is a 1:1 chat.</span></span> <span data-ttu-id="16453-205">对于此类聊天，名单大小是固定的;无法删除/添加成员。</span><span class="sxs-lookup"><span data-stu-id="16453-205">The roster size is fixed for this type of chat; members cannot be removed/added.</span></span>|
|<span data-ttu-id="16453-206">group</span><span class="sxs-lookup"><span data-stu-id="16453-206">group</span></span>               | <span data-ttu-id="16453-207">1</span><span class="sxs-lookup"><span data-stu-id="16453-207">1</span></span>     | <span data-ttu-id="16453-208">指示聊天是群聊。</span><span class="sxs-lookup"><span data-stu-id="16453-208">Indicates that the chat is a group chat.</span></span> <span data-ttu-id="16453-209">可以针对 (聊天类型更新至少两) 名单大小。</span><span class="sxs-lookup"><span data-stu-id="16453-209">The roster size (of at least two people) can be updated for this type of chat.</span></span> <span data-ttu-id="16453-210">稍后可以删除/添加成员。</span><span class="sxs-lookup"><span data-stu-id="16453-210">Members can be removed/added later.</span></span>|
|<span data-ttu-id="16453-211">meeting</span><span class="sxs-lookup"><span data-stu-id="16453-211">meeting</span></span>             | <span data-ttu-id="16453-212">2</span><span class="sxs-lookup"><span data-stu-id="16453-212">2</span></span>     | <span data-ttu-id="16453-213">指示聊天与联机会议相关联。</span><span class="sxs-lookup"><span data-stu-id="16453-213">Indicates that the chat is associated with an online meeting.</span></span> <span data-ttu-id="16453-214">此类聊天仅在创建联机会议时创建。</span><span class="sxs-lookup"><span data-stu-id="16453-214">This type of chat is only created as part of the creation of an online meeting.</span></span>|
|<span data-ttu-id="16453-215">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="16453-215">unknownFutureValue</span></span>  | <span data-ttu-id="16453-216">3</span><span class="sxs-lookup"><span data-stu-id="16453-216">3</span></span>     | <span data-ttu-id="16453-217">Sentinel 值，用于指示未来值。</span><span class="sxs-lookup"><span data-stu-id="16453-217">Sentinel value to indicate future values.</span></span> |

## <a name="relationships"></a><span data-ttu-id="16453-218">关系</span><span class="sxs-lookup"><span data-stu-id="16453-218">Relationships</span></span>

| <span data-ttu-id="16453-219">关系</span><span class="sxs-lookup"><span data-stu-id="16453-219">Relationship</span></span> | <span data-ttu-id="16453-220">类型</span><span class="sxs-lookup"><span data-stu-id="16453-220">Type</span></span> |<span data-ttu-id="16453-221">说明</span><span class="sxs-lookup"><span data-stu-id="16453-221">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="16453-222">installedApps</span><span class="sxs-lookup"><span data-stu-id="16453-222">installedApps</span></span> | <span data-ttu-id="16453-223">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16453-223">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="16453-224">聊天中所有应用的集合。</span><span class="sxs-lookup"><span data-stu-id="16453-224">A collection of all the apps in the chat.</span></span> <span data-ttu-id="16453-225">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="16453-225">Nullable.</span></span> |
| <span data-ttu-id="16453-226">members</span><span class="sxs-lookup"><span data-stu-id="16453-226">members</span></span> | <span data-ttu-id="16453-227">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16453-227">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="16453-228">聊天中所有成员的集合。</span><span class="sxs-lookup"><span data-stu-id="16453-228">A collection of all the members in the chat.</span></span> <span data-ttu-id="16453-229">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="16453-229">Nullable.</span></span> |
| <span data-ttu-id="16453-230">messages</span><span class="sxs-lookup"><span data-stu-id="16453-230">messages</span></span> | <span data-ttu-id="16453-231">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16453-231">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="16453-232">聊天中所有消息的集合。</span><span class="sxs-lookup"><span data-stu-id="16453-232">A collection of all the messages in the chat.</span></span> <span data-ttu-id="16453-233">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="16453-233">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="16453-234">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16453-234">JSON representation</span></span>

<span data-ttu-id="16453-235">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16453-235">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="16453-236">另请参阅</span><span class="sxs-lookup"><span data-stu-id="16453-236">See also</span></span>

- [<span data-ttu-id="16453-237">频道</span><span class="sxs-lookup"><span data-stu-id="16453-237">channel</span></span>](channel.md)
- [<span data-ttu-id="16453-238">chatMessage</span><span class="sxs-lookup"><span data-stu-id="16453-238">chatMessage</span></span>](chatmessage.md)

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


