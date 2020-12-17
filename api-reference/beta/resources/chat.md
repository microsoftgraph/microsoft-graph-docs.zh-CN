---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 chatMessages 集合。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9f378eeb9191993e348c20d523b36160bd854717
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706050"
---
# <a name="chat-resource-type"></a><span data-ttu-id="ade0f-103">聊天资源类型</span><span class="sxs-lookup"><span data-stu-id="ade0f-103">chat resource type</span></span>

<span data-ttu-id="ade0f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ade0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ade0f-105">聊天是一个或多个参与者之间的 [chatMessages](chatmessage.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="ade0f-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="ade0f-106">参与者可以是用户或应用。</span><span class="sxs-lookup"><span data-stu-id="ade0f-106">Participants can be users or apps.</span></span>

> <span data-ttu-id="ade0f-107">**注意**：如果聊天与 [onlineMeeting](../resources/onlinemeeting.md) 实例关联，则列出的一些方法将可传递地影响会议。</span><span class="sxs-lookup"><span data-stu-id="ade0f-107">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then some of the listed methods will transitively impact the meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="ade0f-108">方法</span><span class="sxs-lookup"><span data-stu-id="ade0f-108">Methods</span></span>

|  <span data-ttu-id="ade0f-109">方法</span><span class="sxs-lookup"><span data-stu-id="ade0f-109">Method</span></span>       |  <span data-ttu-id="ade0f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ade0f-110">Return Type</span></span>  | <span data-ttu-id="ade0f-111">说明</span><span class="sxs-lookup"><span data-stu-id="ade0f-111">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="ade0f-112">列出聊天</span><span class="sxs-lookup"><span data-stu-id="ade0f-112">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="ade0f-113">[chat](chat.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ade0f-113">[chat](chat.md) collection</span></span> | <span data-ttu-id="ade0f-114">获取用户参与的聊天列表。</span><span class="sxs-lookup"><span data-stu-id="ade0f-114">Get the list of chats a user is part of.</span></span>| 
|[<span data-ttu-id="ade0f-115">创建聊天</span><span class="sxs-lookup"><span data-stu-id="ade0f-115">Create chat</span></span>](../api/chat-post.md) | [<span data-ttu-id="ade0f-116">聊天</span><span class="sxs-lookup"><span data-stu-id="ade0f-116">chat</span></span>](chat.md) | <span data-ttu-id="ade0f-117">创建新聊天。</span><span class="sxs-lookup"><span data-stu-id="ade0f-117">Create a new chat.</span></span>| 
|[<span data-ttu-id="ade0f-118">获取聊天</span><span class="sxs-lookup"><span data-stu-id="ade0f-118">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="ade0f-119">聊天</span><span class="sxs-lookup"><span data-stu-id="ade0f-119">chat</span></span>](chat.md) | <span data-ttu-id="ade0f-120">读取聊天的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ade0f-120">Read properties and relationships of the chat.</span></span>| 
|[<span data-ttu-id="ade0f-121">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="ade0f-121">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="ade0f-122">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ade0f-122">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="ade0f-123">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="ade0f-123">Get the list of all users in the chat.</span></span>| 
|[<span data-ttu-id="ade0f-124">添加聊天成员</span><span class="sxs-lookup"><span data-stu-id="ade0f-124">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="ade0f-125">位置标头</span><span class="sxs-lookup"><span data-stu-id="ade0f-125">Location header</span></span> | <span data-ttu-id="ade0f-126">向聊天中添加用户。</span><span class="sxs-lookup"><span data-stu-id="ade0f-126">Add a user to the chat.</span></span>| 
|[<span data-ttu-id="ade0f-127">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="ade0f-127">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="ade0f-128">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ade0f-128">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="ade0f-129">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="ade0f-129">Get a single user in the chat.</span></span>| 
|[<span data-ttu-id="ade0f-130">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="ade0f-130">List messages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="ade0f-131">chatMessage</span><span class="sxs-lookup"><span data-stu-id="ade0f-131">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="ade0f-132">获取一对一聊天或群组聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="ade0f-132">Get messages in a 1:1 or group chat.</span></span> | 
|[<span data-ttu-id="ade0f-133">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="ade0f-133">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="ade0f-134">chatMessage</span><span class="sxs-lookup"><span data-stu-id="ade0f-134">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="ade0f-135">获取聊天中的单个消息。</span><span class="sxs-lookup"><span data-stu-id="ade0f-135">Get a single message in a chat.</span></span> | 
|[<span data-ttu-id="ade0f-136">获取用户和应用之间的聊天</span><span class="sxs-lookup"><span data-stu-id="ade0f-136">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="ade0f-137">聊天</span><span class="sxs-lookup"><span data-stu-id="ade0f-137">chat</span></span>](chat.md)| <span data-ttu-id="ade0f-138">获取用户与应用之间的一对一聊天</span><span class="sxs-lookup"><span data-stu-id="ade0f-138">Get one-on-one chat between user and the app</span></span> |
|[<span data-ttu-id="ade0f-139">获取所有聊天消息</span><span class="sxs-lookup"><span data-stu-id="ade0f-139">Get all chat messages</span></span>](../api/chats-getallmessages.md)| <span data-ttu-id="ade0f-140">[chat](chat.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ade0f-140">[chat](chat.md) collection</span></span>| <span data-ttu-id="ade0f-141">从用户参与的所有聊天（包括一对一聊天、群聊和会议聊天）获取消息。</span><span class="sxs-lookup"><span data-stu-id="ade0f-141">Get messages from all chats that a user is a participant in, including one-on-one chats, group chats, and meeting chats.</span></span> |
|[<span data-ttu-id="ade0f-142">列出聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="ade0f-142">List apps in chat</span></span>](../api/chat-list-installedapps.md) |<span data-ttu-id="ade0f-143">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ade0f-143">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="ade0f-144">列出安装在聊天聊天 (关联的会议) 。</span><span class="sxs-lookup"><span data-stu-id="ade0f-144">List apps installed in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="ade0f-145">获取聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="ade0f-145">Get app in chat</span></span>](../api/chat-get-installedapps.md) | [<span data-ttu-id="ade0f-146">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ade0f-146">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="ade0f-147">获取在聊天聊天和关联会议 (安装的特定) 。</span><span class="sxs-lookup"><span data-stu-id="ade0f-147">Get a specific app installed in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="ade0f-148">在聊天中添加应用</span><span class="sxs-lookup"><span data-stu-id="ade0f-148">Add app in chat</span></span>](../api/chat-post-installedapps.md) | | <span data-ttu-id="ade0f-149">添加 (在) 和关联的会议 (中安装) 。</span><span class="sxs-lookup"><span data-stu-id="ade0f-149">Add (install) an app in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="ade0f-150">升级聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="ade0f-150">Upgrade app in chat</span></span>](../api/chat-teamsappinstallation-upgrade.md) | <span data-ttu-id="ade0f-151">无</span><span class="sxs-lookup"><span data-stu-id="ade0f-151">None</span></span> | <span data-ttu-id="ade0f-152">更新到安装在聊天会话和相关会议 (应用的) 。</span><span class="sxs-lookup"><span data-stu-id="ade0f-152">Update to the latest version of the app installed in chat (and associated meeting).</span></span>|
|[<span data-ttu-id="ade0f-153">从聊天中卸载应用</span><span class="sxs-lookup"><span data-stu-id="ade0f-153">Uninstall app from chat</span></span>](../api/chat-delete-installedapps.md) | <span data-ttu-id="ade0f-154">无</span><span class="sxs-lookup"><span data-stu-id="ade0f-154">None</span></span> | <span data-ttu-id="ade0f-155">从 (会议) 中删除 (应用程序) 。</span><span class="sxs-lookup"><span data-stu-id="ade0f-155">Remove (uninstall) app from a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="ade0f-156">列出聊天中的选项卡</span><span class="sxs-lookup"><span data-stu-id="ade0f-156">List tabs in chat</span></span>](../api/chat-list-tabs.md) | [<span data-ttu-id="ade0f-157">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ade0f-157">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ade0f-158">列出固定到聊天聊天 (关联的会议) 。</span><span class="sxs-lookup"><span data-stu-id="ade0f-158">List tabs pinned to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="ade0f-159">获取聊天中的选项卡</span><span class="sxs-lookup"><span data-stu-id="ade0f-159">Get tab in chat</span></span>](../api/chat-get-tabs.md) | [<span data-ttu-id="ade0f-160">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ade0f-160">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ade0f-161">获取固定到聊天会话和关联 (的特定选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="ade0f-161">Get a specific tab pinned to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="ade0f-162">向聊天添加选项卡</span><span class="sxs-lookup"><span data-stu-id="ade0f-162">Add tab to chat</span></span>](../api/chat-post-tabs.md) | [<span data-ttu-id="ade0f-163">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ade0f-163">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ade0f-164">将 (固定) 选项卡添加到聊天 (关联的会议) 。</span><span class="sxs-lookup"><span data-stu-id="ade0f-164">Add (pin) a tab to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="ade0f-165">聊天中的"更新"选项卡</span><span class="sxs-lookup"><span data-stu-id="ade0f-165">Update tab in chat</span></span>](../api/chat-patch-tabs.md) | [<span data-ttu-id="ade0f-166">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ade0f-166">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ade0f-167">更新聊天会话和关联会议 (选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="ade0f-167">Update the properties of a tab in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="ade0f-168">从聊天中删除选项卡</span><span class="sxs-lookup"><span data-stu-id="ade0f-168">Remove tab from chat</span></span>](../api/chat-delete-tabs.md) | <span data-ttu-id="ade0f-169">无</span><span class="sxs-lookup"><span data-stu-id="ade0f-169">None</span></span> | <span data-ttu-id="ade0f-170">从 (活动) 关联的会议选项卡 (取消固定) 。</span><span class="sxs-lookup"><span data-stu-id="ade0f-170">Remove (unpin) a tab from a chat (and associated meeting).</span></span>|

><span data-ttu-id="ade0f-171">**注意：** 使用应用程序权限时，请确保你了解如何获取聊天 ID。</span><span class="sxs-lookup"><span data-stu-id="ade0f-171">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="ade0f-172">由于不支持列出具有应用程序权限的聊天，因此并非所有方案都可行。</span><span class="sxs-lookup"><span data-stu-id="ade0f-172">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="ade0f-173">可以获取具有委派权限的聊天 ID，以及从具有应用程序权限 [的 /chats/getAllMessages](../api/subscription-post-subscriptions.md) 更改通知获取。</span><span class="sxs-lookup"><span data-stu-id="ade0f-173">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="ade0f-174">属性</span><span class="sxs-lookup"><span data-stu-id="ade0f-174">Properties</span></span>

| <span data-ttu-id="ade0f-175">属性</span><span class="sxs-lookup"><span data-stu-id="ade0f-175">Property</span></span>   | <span data-ttu-id="ade0f-176">类型</span><span class="sxs-lookup"><span data-stu-id="ade0f-176">Type</span></span> |<span data-ttu-id="ade0f-177">说明</span><span class="sxs-lookup"><span data-stu-id="ade0f-177">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ade0f-178">id</span><span class="sxs-lookup"><span data-stu-id="ade0f-178">id</span></span>| <span data-ttu-id="ade0f-179">字符串</span><span class="sxs-lookup"><span data-stu-id="ade0f-179">String</span></span>| <span data-ttu-id="ade0f-180">聊天的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ade0f-180">The chat's unique identifier.</span></span> <span data-ttu-id="ade0f-181">只读。</span><span class="sxs-lookup"><span data-stu-id="ade0f-181">Read-only.</span></span>|
| <span data-ttu-id="ade0f-182">topic</span><span class="sxs-lookup"><span data-stu-id="ade0f-182">topic</span></span>| <span data-ttu-id="ade0f-183">String</span><span class="sxs-lookup"><span data-stu-id="ade0f-183">String</span></span>|  <span data-ttu-id="ade0f-184"> (聊天) 主题或主题的可选选项。</span><span class="sxs-lookup"><span data-stu-id="ade0f-184">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="ade0f-185">仅适用于群聊。</span><span class="sxs-lookup"><span data-stu-id="ade0f-185">Only available for group chats.</span></span>|
| <span data-ttu-id="ade0f-186">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ade0f-186">createdDateTime</span></span>| <span data-ttu-id="ade0f-187">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ade0f-187">dateTimeOffset</span></span>|  <span data-ttu-id="ade0f-188">创建聊天的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ade0f-188">Date and time at which the chat was created.</span></span> <span data-ttu-id="ade0f-189">只读。</span><span class="sxs-lookup"><span data-stu-id="ade0f-189">Read-only.</span></span>|
| <span data-ttu-id="ade0f-190">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ade0f-190">lastUpdatedDateTime</span></span>| <span data-ttu-id="ade0f-191">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ade0f-191">dateTimeOffset</span></span>|  <span data-ttu-id="ade0f-192">上次更改聊天或成员列表的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ade0f-192">Date and time at which the chat was renamed or list of members were last changed.</span></span> <span data-ttu-id="ade0f-193">只读。</span><span class="sxs-lookup"><span data-stu-id="ade0f-193">Read-only.</span></span>|
| <span data-ttu-id="ade0f-194">chatType</span><span class="sxs-lookup"><span data-stu-id="ade0f-194">chatType</span></span>| [<span data-ttu-id="ade0f-195">chatType</span><span class="sxs-lookup"><span data-stu-id="ade0f-195">chatType</span></span>](../resources/chat.md#chattype-values) | <span data-ttu-id="ade0f-196">指定聊天类型。</span><span class="sxs-lookup"><span data-stu-id="ade0f-196">Specifies the type of chat.</span></span> <span data-ttu-id="ade0f-197">可能的值是： `group` 和 `oneOnOne` `meeting` 。</span><span class="sxs-lookup"><span data-stu-id="ade0f-197">Possible values are:`group`, `oneOnOne` and `meeting`.</span></span>|

### <a name="chattype-values"></a><span data-ttu-id="ade0f-198">chatType 值</span><span class="sxs-lookup"><span data-stu-id="ade0f-198">chatType values</span></span> 

| <span data-ttu-id="ade0f-199">成员</span><span class="sxs-lookup"><span data-stu-id="ade0f-199">Member</span></span>             | <span data-ttu-id="ade0f-200">值</span><span class="sxs-lookup"><span data-stu-id="ade0f-200">Value</span></span> | <span data-ttu-id="ade0f-201">说明</span><span class="sxs-lookup"><span data-stu-id="ade0f-201">Description</span></span>               |
| :----------------- | :---- | :------------------------ |
|<span data-ttu-id="ade0f-202">oneOnOne</span><span class="sxs-lookup"><span data-stu-id="ade0f-202">oneOnOne</span></span>            | <span data-ttu-id="ade0f-203">0</span><span class="sxs-lookup"><span data-stu-id="ade0f-203">0</span></span>     | <span data-ttu-id="ade0f-204">指示聊天为一对一聊天。</span><span class="sxs-lookup"><span data-stu-id="ade0f-204">Indicates that the chat is a 1:1 chat.</span></span> <span data-ttu-id="ade0f-205">对于此类聊天，名单大小是固定的;无法删除/添加成员。</span><span class="sxs-lookup"><span data-stu-id="ade0f-205">The roster size is fixed for this type of chat; members cannot be removed/added.</span></span>|
|<span data-ttu-id="ade0f-206">group</span><span class="sxs-lookup"><span data-stu-id="ade0f-206">group</span></span>               | <span data-ttu-id="ade0f-207">1</span><span class="sxs-lookup"><span data-stu-id="ade0f-207">1</span></span>     | <span data-ttu-id="ade0f-208">指示聊天是群聊。</span><span class="sxs-lookup"><span data-stu-id="ade0f-208">Indicates that the chat is a group chat.</span></span> <span data-ttu-id="ade0f-209">可以针对 (更新至少两) 用户名单大小。</span><span class="sxs-lookup"><span data-stu-id="ade0f-209">The roster size (of at least two people) can be updated for this type of chat.</span></span> <span data-ttu-id="ade0f-210">稍后可以删除/添加成员。</span><span class="sxs-lookup"><span data-stu-id="ade0f-210">Members can be removed/added later.</span></span>|
|<span data-ttu-id="ade0f-211">meeting</span><span class="sxs-lookup"><span data-stu-id="ade0f-211">meeting</span></span>             | <span data-ttu-id="ade0f-212">2</span><span class="sxs-lookup"><span data-stu-id="ade0f-212">2</span></span>     | <span data-ttu-id="ade0f-213">指示聊天与联机会议关联。</span><span class="sxs-lookup"><span data-stu-id="ade0f-213">Indicates that the chat is associated with an online meeting.</span></span> <span data-ttu-id="ade0f-214">此类聊天仅作为联机会议创建的一部分创建。</span><span class="sxs-lookup"><span data-stu-id="ade0f-214">This type of chat is only created as part of the creation of an online meeting.</span></span>|
|<span data-ttu-id="ade0f-215">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="ade0f-215">unknownFutureValue</span></span>  | <span data-ttu-id="ade0f-216">3</span><span class="sxs-lookup"><span data-stu-id="ade0f-216">3</span></span>     | <span data-ttu-id="ade0f-217">指示未来值的 Sentinel 值。</span><span class="sxs-lookup"><span data-stu-id="ade0f-217">Sentinel value to indicate future values.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ade0f-218">关系</span><span class="sxs-lookup"><span data-stu-id="ade0f-218">Relationships</span></span>

| <span data-ttu-id="ade0f-219">关系</span><span class="sxs-lookup"><span data-stu-id="ade0f-219">Relationship</span></span> | <span data-ttu-id="ade0f-220">类型</span><span class="sxs-lookup"><span data-stu-id="ade0f-220">Type</span></span> |<span data-ttu-id="ade0f-221">说明</span><span class="sxs-lookup"><span data-stu-id="ade0f-221">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ade0f-222">installedApps</span><span class="sxs-lookup"><span data-stu-id="ade0f-222">installedApps</span></span> | <span data-ttu-id="ade0f-223">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ade0f-223">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="ade0f-224">聊天中所有应用的集合。</span><span class="sxs-lookup"><span data-stu-id="ade0f-224">A collection of all the apps in the chat.</span></span> <span data-ttu-id="ade0f-225">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="ade0f-225">Nullable.</span></span> |
| <span data-ttu-id="ade0f-226">members</span><span class="sxs-lookup"><span data-stu-id="ade0f-226">members</span></span> | <span data-ttu-id="ade0f-227">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ade0f-227">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="ade0f-228">聊天中所有成员的集合。</span><span class="sxs-lookup"><span data-stu-id="ade0f-228">A collection of all the members in the chat.</span></span> <span data-ttu-id="ade0f-229">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="ade0f-229">Nullable.</span></span> |
| <span data-ttu-id="ade0f-230">messages</span><span class="sxs-lookup"><span data-stu-id="ade0f-230">messages</span></span> | <span data-ttu-id="ade0f-231">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ade0f-231">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="ade0f-232">聊天中所有消息的集合。</span><span class="sxs-lookup"><span data-stu-id="ade0f-232">A collection of all the messages in the chat.</span></span> <span data-ttu-id="ade0f-233">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="ade0f-233">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ade0f-234">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ade0f-234">JSON representation</span></span>

<span data-ttu-id="ade0f-235">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ade0f-235">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="ade0f-236">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ade0f-236">See also</span></span>

- [<span data-ttu-id="ade0f-237">频道</span><span class="sxs-lookup"><span data-stu-id="ade0f-237">channel</span></span>](channel.md)
- [<span data-ttu-id="ade0f-238">chatMessage</span><span class="sxs-lookup"><span data-stu-id="ade0f-238">chatMessage</span></span>](chatmessage.md)

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


