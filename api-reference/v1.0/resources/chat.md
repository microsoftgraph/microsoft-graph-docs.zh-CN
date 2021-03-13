---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 chatMessages 集合。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f9162e39e1326d89818f959e846ccde5f04350e9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776814"
---
# <a name="chat-resource-type"></a><span data-ttu-id="d09d5-103">聊天资源类型</span><span class="sxs-lookup"><span data-stu-id="d09d5-103">chat resource type</span></span>

<span data-ttu-id="d09d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d09d5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d09d5-105">聊天是一个或多个 [参与者之间的 chatMessages](chatmessage.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="d09d5-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="d09d5-106">参与者可以是用户或应用。</span><span class="sxs-lookup"><span data-stu-id="d09d5-106">Participants can be users or apps.</span></span>

> <span data-ttu-id="d09d5-107">**注意**：如果聊天与 [onlineMeeting](../resources/onlinemeeting.md) 实例关联，则列出的一些方法将可传递影响会议。</span><span class="sxs-lookup"><span data-stu-id="d09d5-107">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then some of the listed methods will transitively impact the meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="d09d5-108">方法</span><span class="sxs-lookup"><span data-stu-id="d09d5-108">Methods</span></span>

|  <span data-ttu-id="d09d5-109">方法</span><span class="sxs-lookup"><span data-stu-id="d09d5-109">Method</span></span>       |  <span data-ttu-id="d09d5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d09d5-110">Return Type</span></span>  | <span data-ttu-id="d09d5-111">说明</span><span class="sxs-lookup"><span data-stu-id="d09d5-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d09d5-112">创建聊天</span><span class="sxs-lookup"><span data-stu-id="d09d5-112">Create chat</span></span>](../api/chat-post.md) | [<span data-ttu-id="d09d5-113">聊天</span><span class="sxs-lookup"><span data-stu-id="d09d5-113">chat</span></span>](chat.md) | <span data-ttu-id="d09d5-114">创建新聊天。</span><span class="sxs-lookup"><span data-stu-id="d09d5-114">Create a new chat.</span></span>| 
|[<span data-ttu-id="d09d5-115">获取聊天</span><span class="sxs-lookup"><span data-stu-id="d09d5-115">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="d09d5-116">聊天</span><span class="sxs-lookup"><span data-stu-id="d09d5-116">chat</span></span>](chat.md) | <span data-ttu-id="d09d5-117">读取聊天的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d09d5-117">Read properties and relationships of the chat.</span></span>| 
|[<span data-ttu-id="d09d5-118">更新聊天</span><span class="sxs-lookup"><span data-stu-id="d09d5-118">Update chat</span></span>](../api/chat-patch.md) | [<span data-ttu-id="d09d5-119">聊天</span><span class="sxs-lookup"><span data-stu-id="d09d5-119">chat</span></span>](chat.md) | <span data-ttu-id="d09d5-120">更新聊天的属性。</span><span class="sxs-lookup"><span data-stu-id="d09d5-120">Update properties of the chat.</span></span>|
|[<span data-ttu-id="d09d5-121">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="d09d5-121">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="d09d5-122">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d09d5-122">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="d09d5-123">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="d09d5-123">Get the list of all users in the chat.</span></span>| 
|[<span data-ttu-id="d09d5-124">添加聊天成员</span><span class="sxs-lookup"><span data-stu-id="d09d5-124">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="d09d5-125">位置标头</span><span class="sxs-lookup"><span data-stu-id="d09d5-125">Location header</span></span> | <span data-ttu-id="d09d5-126">向聊天中添加用户。</span><span class="sxs-lookup"><span data-stu-id="d09d5-126">Add a user to the chat.</span></span>| 
|[<span data-ttu-id="d09d5-127">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="d09d5-127">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="d09d5-128">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d09d5-128">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="d09d5-129">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="d09d5-129">Get a single user in the chat.</span></span>| 
|[<span data-ttu-id="d09d5-130">删除聊天成员</span><span class="sxs-lookup"><span data-stu-id="d09d5-130">Remove chat member</span></span>](../api/chat-delete-members.md)|<span data-ttu-id="d09d5-131">无</span><span class="sxs-lookup"><span data-stu-id="d09d5-131">None</span></span>|<span data-ttu-id="d09d5-132">从聊天中删除用户。</span><span class="sxs-lookup"><span data-stu-id="d09d5-132">Remove a user from the chat.</span></span>|
|[<span data-ttu-id="d09d5-133">获取用户和应用之间的聊天</span><span class="sxs-lookup"><span data-stu-id="d09d5-133">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="d09d5-134">聊天</span><span class="sxs-lookup"><span data-stu-id="d09d5-134">chat</span></span>](chat.md)| <span data-ttu-id="d09d5-135">获取用户与应用之间的一对一聊天</span><span class="sxs-lookup"><span data-stu-id="d09d5-135">Get one-on-one chat between user and the app</span></span> |
|[<span data-ttu-id="d09d5-136">列出聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="d09d5-136">List apps in chat</span></span>](../api/chat-list-installedapps.md) |<span data-ttu-id="d09d5-137">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d09d5-137">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="d09d5-138">列出聊天网站中安装 (关联的会议) 。</span><span class="sxs-lookup"><span data-stu-id="d09d5-138">List apps installed in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="d09d5-139">在聊天中获取应用</span><span class="sxs-lookup"><span data-stu-id="d09d5-139">Get app in chat</span></span>](../api/chat-get-installedapps.md) | [<span data-ttu-id="d09d5-140">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d09d5-140">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="d09d5-141">获取安装在聊天会话和关联会议 (中的特定) 。</span><span class="sxs-lookup"><span data-stu-id="d09d5-141">Get a specific app installed in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="d09d5-142">在聊天中添加应用</span><span class="sxs-lookup"><span data-stu-id="d09d5-142">Add app in chat</span></span>](../api/chat-post-installedapps.md) | | <span data-ttu-id="d09d5-143">添加 (在) 会议及其关联会议 (中安装) 。</span><span class="sxs-lookup"><span data-stu-id="d09d5-143">Add (install) an app in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="d09d5-144">升级聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="d09d5-144">Upgrade app in chat</span></span>](../api/chat-teamsappinstallation-upgrade.md) | <span data-ttu-id="d09d5-145">无</span><span class="sxs-lookup"><span data-stu-id="d09d5-145">None</span></span> | <span data-ttu-id="d09d5-146">更新到聊天会话和相关会议 (安装的应用的) 。</span><span class="sxs-lookup"><span data-stu-id="d09d5-146">Update to the latest version of the app installed in chat (and associated meeting).</span></span>|
|[<span data-ttu-id="d09d5-147">从聊天中卸载应用</span><span class="sxs-lookup"><span data-stu-id="d09d5-147">Uninstall app from chat</span></span>](../api/chat-delete-installedapps.md) | <span data-ttu-id="d09d5-148">无</span><span class="sxs-lookup"><span data-stu-id="d09d5-148">None</span></span> | <span data-ttu-id="d09d5-149">从 (和) 会议记录中删除 (卸载) 。</span><span class="sxs-lookup"><span data-stu-id="d09d5-149">Remove (uninstall) app from a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="d09d5-150">列出聊天中的选项卡</span><span class="sxs-lookup"><span data-stu-id="d09d5-150">List tabs in chat</span></span>](../api/chat-list-tabs.md) | [<span data-ttu-id="d09d5-151">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d09d5-151">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="d09d5-152">列出固定到聊天 (关联的会议选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="d09d5-152">List tabs pinned to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="d09d5-153">在聊天中获取选项卡</span><span class="sxs-lookup"><span data-stu-id="d09d5-153">Get tab in chat</span></span>](../api/chat-get-tabs.md) | [<span data-ttu-id="d09d5-154">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d09d5-154">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="d09d5-155">获取固定到聊天组和关联 (的特定选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="d09d5-155">Get a specific tab pinned to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="d09d5-156">向聊天添加选项卡</span><span class="sxs-lookup"><span data-stu-id="d09d5-156">Add tab to chat</span></span>](../api/chat-post-tabs.md) | [<span data-ttu-id="d09d5-157">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d09d5-157">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="d09d5-158">将 (固定) 选项卡添加到聊天 (关联的会议) 。</span><span class="sxs-lookup"><span data-stu-id="d09d5-158">Add (pin) a tab to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="d09d5-159">聊天中的"更新"选项卡</span><span class="sxs-lookup"><span data-stu-id="d09d5-159">Update tab in chat</span></span>](../api/chat-patch-tabs.md) | [<span data-ttu-id="d09d5-160">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d09d5-160">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="d09d5-161">更新聊天记录和相关会议 (选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="d09d5-161">Update the properties of a tab in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="d09d5-162">从聊天中删除选项卡</span><span class="sxs-lookup"><span data-stu-id="d09d5-162">Remove tab from chat</span></span>](../api/chat-delete-tabs.md) | <span data-ttu-id="d09d5-163">无</span><span class="sxs-lookup"><span data-stu-id="d09d5-163">None</span></span> | <span data-ttu-id="d09d5-164">从 (和) 会议记录中删除 (取消固定选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="d09d5-164">Remove (unpin) a tab from a chat (and associated meeting).</span></span>|

><span data-ttu-id="d09d5-165">**注意：** 使用应用程序权限时，请务必了解如何获取聊天 ID。</span><span class="sxs-lookup"><span data-stu-id="d09d5-165">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="d09d5-166">由于不支持列出具有应用程序权限的聊天，因此并非所有方案都可行。</span><span class="sxs-lookup"><span data-stu-id="d09d5-166">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="d09d5-167">可以获取具有委派权限的聊天 ID，以及从具有应用程序权限的 [/chats/getAllMessages](../api/subscription-post-subscriptions.md) 更改通知获取。</span><span class="sxs-lookup"><span data-stu-id="d09d5-167">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="d09d5-168">属性</span><span class="sxs-lookup"><span data-stu-id="d09d5-168">Properties</span></span>

| <span data-ttu-id="d09d5-169">属性</span><span class="sxs-lookup"><span data-stu-id="d09d5-169">Property</span></span>   | <span data-ttu-id="d09d5-170">类型</span><span class="sxs-lookup"><span data-stu-id="d09d5-170">Type</span></span> |<span data-ttu-id="d09d5-171">说明</span><span class="sxs-lookup"><span data-stu-id="d09d5-171">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d09d5-172">id</span><span class="sxs-lookup"><span data-stu-id="d09d5-172">id</span></span>| <span data-ttu-id="d09d5-173">字符串</span><span class="sxs-lookup"><span data-stu-id="d09d5-173">String</span></span>| <span data-ttu-id="d09d5-174">聊天的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d09d5-174">The chat's unique identifier.</span></span> <span data-ttu-id="d09d5-175">只读。</span><span class="sxs-lookup"><span data-stu-id="d09d5-175">Read-only.</span></span>|
| <span data-ttu-id="d09d5-176">topic</span><span class="sxs-lookup"><span data-stu-id="d09d5-176">topic</span></span>| <span data-ttu-id="d09d5-177">String</span><span class="sxs-lookup"><span data-stu-id="d09d5-177">String</span></span>|  <span data-ttu-id="d09d5-178"> (聊天) 主题或主题。</span><span class="sxs-lookup"><span data-stu-id="d09d5-178">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="d09d5-179">仅适用于群聊。</span><span class="sxs-lookup"><span data-stu-id="d09d5-179">Only available for group chats.</span></span>|
| <span data-ttu-id="d09d5-180">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d09d5-180">createdDateTime</span></span>| <span data-ttu-id="d09d5-181">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d09d5-181">dateTimeOffset</span></span>|  <span data-ttu-id="d09d5-182">创建聊天的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d09d5-182">Date and time at which the chat was created.</span></span> <span data-ttu-id="d09d5-183">只读。</span><span class="sxs-lookup"><span data-stu-id="d09d5-183">Read-only.</span></span>|
| <span data-ttu-id="d09d5-184">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d09d5-184">lastUpdatedDateTime</span></span>| <span data-ttu-id="d09d5-185">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d09d5-185">dateTimeOffset</span></span>|  <span data-ttu-id="d09d5-186">上次更改聊天的日期和时间或成员列表。</span><span class="sxs-lookup"><span data-stu-id="d09d5-186">Date and time at which the chat was renamed or list of members were last changed.</span></span> <span data-ttu-id="d09d5-187">只读。</span><span class="sxs-lookup"><span data-stu-id="d09d5-187">Read-only.</span></span>|
| <span data-ttu-id="d09d5-188">chatType</span><span class="sxs-lookup"><span data-stu-id="d09d5-188">chatType</span></span>| [<span data-ttu-id="d09d5-189">chatType</span><span class="sxs-lookup"><span data-stu-id="d09d5-189">chatType</span></span>](../resources/chat.md#chattype-values) | <span data-ttu-id="d09d5-190">指定聊天类型。</span><span class="sxs-lookup"><span data-stu-id="d09d5-190">Specifies the type of chat.</span></span> <span data-ttu-id="d09d5-191">可能的值是： `group` 和 `oneOnOne` `meeting` 。</span><span class="sxs-lookup"><span data-stu-id="d09d5-191">Possible values are:`group`, `oneOnOne` and `meeting`.</span></span>|

### <a name="chattype-values"></a><span data-ttu-id="d09d5-192">chatType 值</span><span class="sxs-lookup"><span data-stu-id="d09d5-192">chatType values</span></span> 

| <span data-ttu-id="d09d5-193">成员</span><span class="sxs-lookup"><span data-stu-id="d09d5-193">Member</span></span>             | <span data-ttu-id="d09d5-194">值</span><span class="sxs-lookup"><span data-stu-id="d09d5-194">Value</span></span> | <span data-ttu-id="d09d5-195">说明</span><span class="sxs-lookup"><span data-stu-id="d09d5-195">Description</span></span>               |
| :----------------- | :---- | :------------------------ |
|<span data-ttu-id="d09d5-196">oneOnOne</span><span class="sxs-lookup"><span data-stu-id="d09d5-196">oneOnOne</span></span>            | <span data-ttu-id="d09d5-197">0</span><span class="sxs-lookup"><span data-stu-id="d09d5-197">0</span></span>     | <span data-ttu-id="d09d5-198">指示聊天为一对一聊天。</span><span class="sxs-lookup"><span data-stu-id="d09d5-198">Indicates that the chat is a 1:1 chat.</span></span> <span data-ttu-id="d09d5-199">对于此类聊天，名单大小是固定的;无法删除/添加成员。</span><span class="sxs-lookup"><span data-stu-id="d09d5-199">The roster size is fixed for this type of chat; members cannot be removed/added.</span></span>|
|<span data-ttu-id="d09d5-200">group</span><span class="sxs-lookup"><span data-stu-id="d09d5-200">group</span></span>               | <span data-ttu-id="d09d5-201">1</span><span class="sxs-lookup"><span data-stu-id="d09d5-201">1</span></span>     | <span data-ttu-id="d09d5-202">指示聊天是群聊。</span><span class="sxs-lookup"><span data-stu-id="d09d5-202">Indicates that the chat is a group chat.</span></span> <span data-ttu-id="d09d5-203">可以针对 (聊天类型更新至少两) 名单大小。</span><span class="sxs-lookup"><span data-stu-id="d09d5-203">The roster size (of at least two people) can be updated for this type of chat.</span></span> <span data-ttu-id="d09d5-204">稍后可以删除/添加成员。</span><span class="sxs-lookup"><span data-stu-id="d09d5-204">Members can be removed/added later.</span></span>|
|<span data-ttu-id="d09d5-205">meeting</span><span class="sxs-lookup"><span data-stu-id="d09d5-205">meeting</span></span>             | <span data-ttu-id="d09d5-206">2</span><span class="sxs-lookup"><span data-stu-id="d09d5-206">2</span></span>     | <span data-ttu-id="d09d5-207">指示聊天与联机会议相关联。</span><span class="sxs-lookup"><span data-stu-id="d09d5-207">Indicates that the chat is associated with an online meeting.</span></span> <span data-ttu-id="d09d5-208">此类聊天仅在创建联机会议时创建。</span><span class="sxs-lookup"><span data-stu-id="d09d5-208">This type of chat is only created as part of the creation of an online meeting.</span></span>|
|<span data-ttu-id="d09d5-209">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="d09d5-209">unknownFutureValue</span></span>  | <span data-ttu-id="d09d5-210">3</span><span class="sxs-lookup"><span data-stu-id="d09d5-210">3</span></span>     | <span data-ttu-id="d09d5-211">Sentinel 值，用于指示未来值。</span><span class="sxs-lookup"><span data-stu-id="d09d5-211">Sentinel value to indicate future values.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d09d5-212">关系</span><span class="sxs-lookup"><span data-stu-id="d09d5-212">Relationships</span></span>

| <span data-ttu-id="d09d5-213">关系</span><span class="sxs-lookup"><span data-stu-id="d09d5-213">Relationship</span></span> | <span data-ttu-id="d09d5-214">类型</span><span class="sxs-lookup"><span data-stu-id="d09d5-214">Type</span></span> |<span data-ttu-id="d09d5-215">说明</span><span class="sxs-lookup"><span data-stu-id="d09d5-215">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d09d5-216">installedApps</span><span class="sxs-lookup"><span data-stu-id="d09d5-216">installedApps</span></span> | <span data-ttu-id="d09d5-217">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d09d5-217">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="d09d5-218">聊天中所有应用的集合。</span><span class="sxs-lookup"><span data-stu-id="d09d5-218">A collection of all the apps in the chat.</span></span> <span data-ttu-id="d09d5-219">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d09d5-219">Nullable.</span></span> |
| <span data-ttu-id="d09d5-220">members</span><span class="sxs-lookup"><span data-stu-id="d09d5-220">members</span></span> | <span data-ttu-id="d09d5-221">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d09d5-221">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="d09d5-222">聊天中所有成员的集合。</span><span class="sxs-lookup"><span data-stu-id="d09d5-222">A collection of all the members in the chat.</span></span> <span data-ttu-id="d09d5-223">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d09d5-223">Nullable.</span></span> |
| <span data-ttu-id="d09d5-224">messages</span><span class="sxs-lookup"><span data-stu-id="d09d5-224">messages</span></span> | <span data-ttu-id="d09d5-225">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d09d5-225">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="d09d5-226">聊天中所有消息的集合。</span><span class="sxs-lookup"><span data-stu-id="d09d5-226">A collection of all the messages in the chat.</span></span> <span data-ttu-id="d09d5-227">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d09d5-227">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d09d5-228">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d09d5-228">JSON representation</span></span>

<span data-ttu-id="d09d5-229">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d09d5-229">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="d09d5-230">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d09d5-230">See also</span></span>

- [<span data-ttu-id="d09d5-231">频道</span><span class="sxs-lookup"><span data-stu-id="d09d5-231">channel</span></span>](channel.md)
- [<span data-ttu-id="d09d5-232">chatMessage</span><span class="sxs-lookup"><span data-stu-id="d09d5-232">chatMessage</span></span>](chatmessage.md)

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


