---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 Chatmessages 集合的集合。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f1745f987577d94f14f81d79a9f8afb89c1ab793
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606935"
---
# <a name="chat-resource-type"></a><span data-ttu-id="25fad-103">聊天资源类型</span><span class="sxs-lookup"><span data-stu-id="25fad-103">chat resource type</span></span>

<span data-ttu-id="25fad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25fad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25fad-105">聊天是一个或多个参与者之间的 [chatmessages 集合](chatmessage.md) 的集合。</span><span class="sxs-lookup"><span data-stu-id="25fad-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="25fad-106">参与者可以是用户或应用程序。</span><span class="sxs-lookup"><span data-stu-id="25fad-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="25fad-107">方法</span><span class="sxs-lookup"><span data-stu-id="25fad-107">Methods</span></span>

|  <span data-ttu-id="25fad-108">方法</span><span class="sxs-lookup"><span data-stu-id="25fad-108">Method</span></span>       |  <span data-ttu-id="25fad-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="25fad-109">Return Type</span></span>  | <span data-ttu-id="25fad-110">Description</span><span class="sxs-lookup"><span data-stu-id="25fad-110">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="25fad-111">列出聊天</span><span class="sxs-lookup"><span data-stu-id="25fad-111">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="25fad-112">[聊天](chat.md) 收藏</span><span class="sxs-lookup"><span data-stu-id="25fad-112">[chat](chat.md) collection</span></span> | <span data-ttu-id="25fad-113">获取用户所属的聊天列表。</span><span class="sxs-lookup"><span data-stu-id="25fad-113">Get the list of chats a user is part of.</span></span>| 
|[<span data-ttu-id="25fad-114">获取聊天</span><span class="sxs-lookup"><span data-stu-id="25fad-114">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="25fad-115">聊天</span><span class="sxs-lookup"><span data-stu-id="25fad-115">chat</span></span>](chat.md) | <span data-ttu-id="25fad-116">读取聊天的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="25fad-116">Read properties and relationships of the chat.</span></span>| 
|[<span data-ttu-id="25fad-117">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="25fad-117">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="25fad-118">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25fad-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="25fad-119">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="25fad-119">Get the list of all users in the chat.</span></span>| 
|[<span data-ttu-id="25fad-120">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="25fad-120">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="25fad-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="25fad-121">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="25fad-122">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="25fad-122">Get a single user in the chat.</span></span>| 
|[<span data-ttu-id="25fad-123">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="25fad-123">List messages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="25fad-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="25fad-124">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="25fad-125">获取一对一聊天或群组聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="25fad-125">Get messages in a 1:1 or group chat.</span></span> | 
|[<span data-ttu-id="25fad-126">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="25fad-126">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="25fad-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="25fad-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="25fad-128">获取聊天中的单个消息。</span><span class="sxs-lookup"><span data-stu-id="25fad-128">Get a single message in a chat.</span></span> | 
|[<span data-ttu-id="25fad-129">在用户和应用之间获取聊天</span><span class="sxs-lookup"><span data-stu-id="25fad-129">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="25fad-130">聊天</span><span class="sxs-lookup"><span data-stu-id="25fad-130">chat</span></span>](chat.md)| <span data-ttu-id="25fad-131">在用户和应用之间获取一对一聊天</span><span class="sxs-lookup"><span data-stu-id="25fad-131">Get one-on-one chat between user and the app</span></span> |
|[<span data-ttu-id="25fad-132">获取所有聊天消息</span><span class="sxs-lookup"><span data-stu-id="25fad-132">Get all chat messages</span></span>](../api/chats-getallmessages.md)| <span data-ttu-id="25fad-133">[聊天](chat.md) 收藏</span><span class="sxs-lookup"><span data-stu-id="25fad-133">[chat](chat.md) collection</span></span>| <span data-ttu-id="25fad-134">从用户参与的所有聊天中获取邮件，包括一对一聊天、群研讨和会议聊天。</span><span class="sxs-lookup"><span data-stu-id="25fad-134">Get messages from all chats that a user is a participant in, including one-on-one chats, group chats, and meeting chats.</span></span> |
|[<span data-ttu-id="25fad-135">列出聊天中的应用程序</span><span class="sxs-lookup"><span data-stu-id="25fad-135">List apps in chat</span></span>](../api/chat-list-installedapps.md) |<span data-ttu-id="25fad-136">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25fad-136">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="25fad-137">列出聊天中安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="25fad-137">List apps installed in a chat.</span></span>|
|[<span data-ttu-id="25fad-138">获取聊天中的应用程序</span><span class="sxs-lookup"><span data-stu-id="25fad-138">Get app in chat</span></span>](../api/chat-get-installedapps.md) | [<span data-ttu-id="25fad-139">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="25fad-139">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="25fad-140">获取聊天中安装的特定应用程序。</span><span class="sxs-lookup"><span data-stu-id="25fad-140">Get a specific app installed in a chat.</span></span>|
|[<span data-ttu-id="25fad-141">在聊天中添加应用程序</span><span class="sxs-lookup"><span data-stu-id="25fad-141">Add app in chat</span></span>](../api/chat-post-installedapps.md) | | <span data-ttu-id="25fad-142">添加 (在聊天中的应用程序) 安装。</span><span class="sxs-lookup"><span data-stu-id="25fad-142">Adds (installs) an app in a chat.</span></span>|
|[<span data-ttu-id="25fad-143">升级聊天中的应用程序</span><span class="sxs-lookup"><span data-stu-id="25fad-143">Upgrade app in chat</span></span>](../api/chat-teamsappinstallation-upgrade.md) | <span data-ttu-id="25fad-144">无</span><span class="sxs-lookup"><span data-stu-id="25fad-144">None</span></span> | <span data-ttu-id="25fad-145">更新到聊天中安装的最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="25fad-145">Update to the latest version of the app installed in chat.</span></span>|
|[<span data-ttu-id="25fad-146">从聊天中卸载应用程序</span><span class="sxs-lookup"><span data-stu-id="25fad-146">Uninstall app from chat</span></span>](../api/chat-delete-installedapps.md) | <span data-ttu-id="25fad-147">无</span><span class="sxs-lookup"><span data-stu-id="25fad-147">None</span></span> | <span data-ttu-id="25fad-148">从聊天中删除 (卸载) 应用程序。</span><span class="sxs-lookup"><span data-stu-id="25fad-148">Remove (uninstall) app from a chat.</span></span>|
|[<span data-ttu-id="25fad-149">聊天中的列表选项卡</span><span class="sxs-lookup"><span data-stu-id="25fad-149">List tabs in chat</span></span>](../api/chat-list-tabs.md) | [<span data-ttu-id="25fad-150">teamsTab</span><span class="sxs-lookup"><span data-stu-id="25fad-150">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="25fad-151">固定到聊天的列表选项卡。</span><span class="sxs-lookup"><span data-stu-id="25fad-151">List tabs pinned to a chat.</span></span>|
|[<span data-ttu-id="25fad-152">聊天中的 "获取" 选项卡</span><span class="sxs-lookup"><span data-stu-id="25fad-152">Get tab in chat</span></span>](../api/chat-get-tabs.md) | [<span data-ttu-id="25fad-153">teamsTab</span><span class="sxs-lookup"><span data-stu-id="25fad-153">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="25fad-154">获取固定到聊天的特定选项卡。</span><span class="sxs-lookup"><span data-stu-id="25fad-154">Get a specific tab pinned to a chat.</span></span>|
|[<span data-ttu-id="25fad-155">将选项卡添加到聊天</span><span class="sxs-lookup"><span data-stu-id="25fad-155">Add tab to chat</span></span>](../api/chat-post-tabs.md) | [<span data-ttu-id="25fad-156">teamsTab</span><span class="sxs-lookup"><span data-stu-id="25fad-156">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="25fad-157">向聊天添加 (pin) 选项卡。</span><span class="sxs-lookup"><span data-stu-id="25fad-157">Add (pin) a tab to a chat.</span></span>|
|[<span data-ttu-id="25fad-158">聊天中的更新选项卡</span><span class="sxs-lookup"><span data-stu-id="25fad-158">Update tab in chat</span></span>](../api/chat-patch-tabs.md) | [<span data-ttu-id="25fad-159">teamsTab</span><span class="sxs-lookup"><span data-stu-id="25fad-159">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="25fad-160">更新聊天中的选项卡的属性。</span><span class="sxs-lookup"><span data-stu-id="25fad-160">Updates the properties of a tab in a chat.</span></span>|
|[<span data-ttu-id="25fad-161">从聊天中删除选项卡</span><span class="sxs-lookup"><span data-stu-id="25fad-161">Remove tab from chat</span></span>](../api/chat-delete-tabs.md) | <span data-ttu-id="25fad-162">无</span><span class="sxs-lookup"><span data-stu-id="25fad-162">None</span></span> | <span data-ttu-id="25fad-163">) 聊天中的选项卡删除 (的 "取消固定"。</span><span class="sxs-lookup"><span data-stu-id="25fad-163">Remove (unpin) a tab from a chat.</span></span>|

><span data-ttu-id="25fad-164">**注意：** 使用应用程序权限时，请务必了解如何获取聊天 ID。</span><span class="sxs-lookup"><span data-stu-id="25fad-164">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="25fad-165">由于不支持列出具有应用程序权限的聊天，因此并非所有方案都可行。</span><span class="sxs-lookup"><span data-stu-id="25fad-165">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="25fad-166">可以获取具有委派权限的聊天 Id，也可以通过应用程序权限获取 [/chats/getAllMessages 的更改通知](../api/subscription-post-subscriptions.md) 。</span><span class="sxs-lookup"><span data-stu-id="25fad-166">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="25fad-167">属性</span><span class="sxs-lookup"><span data-stu-id="25fad-167">Properties</span></span>

| <span data-ttu-id="25fad-168">属性</span><span class="sxs-lookup"><span data-stu-id="25fad-168">Property</span></span>   | <span data-ttu-id="25fad-169">类型</span><span class="sxs-lookup"><span data-stu-id="25fad-169">Type</span></span> |<span data-ttu-id="25fad-170">说明</span><span class="sxs-lookup"><span data-stu-id="25fad-170">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="25fad-171">id</span><span class="sxs-lookup"><span data-stu-id="25fad-171">id</span></span>| <span data-ttu-id="25fad-172">String</span><span class="sxs-lookup"><span data-stu-id="25fad-172">String</span></span>| <span data-ttu-id="25fad-173">聊天的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="25fad-173">The chat's unique identifier.</span></span> <span data-ttu-id="25fad-174">只读。</span><span class="sxs-lookup"><span data-stu-id="25fad-174">Read-only.</span></span>|
| <span data-ttu-id="25fad-175">topic</span><span class="sxs-lookup"><span data-stu-id="25fad-175">topic</span></span>| <span data-ttu-id="25fad-176">String</span><span class="sxs-lookup"><span data-stu-id="25fad-176">String</span></span>|  <span data-ttu-id="25fad-177"> (聊天的可选) 主题或主题。</span><span class="sxs-lookup"><span data-stu-id="25fad-177">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="25fad-178">仅适用于组聊天。</span><span class="sxs-lookup"><span data-stu-id="25fad-178">Only available for group chats.</span></span>|
| <span data-ttu-id="25fad-179">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25fad-179">createdDateTime</span></span>| <span data-ttu-id="25fad-180">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25fad-180">dateTimeOffset</span></span>|  <span data-ttu-id="25fad-181">聊天的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="25fad-181">Date and time at which the chat was created.</span></span> <span data-ttu-id="25fad-182">只读。</span><span class="sxs-lookup"><span data-stu-id="25fad-182">Read-only.</span></span>|
| <span data-ttu-id="25fad-183">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="25fad-183">lastUpdatedDateTime</span></span>| <span data-ttu-id="25fad-184">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25fad-184">dateTimeOffset</span></span>|  <span data-ttu-id="25fad-185">重命名或更改成员身份时的聊天的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="25fad-185">Date and time at which the chat was renamed or membership changed.</span></span> <span data-ttu-id="25fad-186">将邮件发送到聊天时，不会对 lastUpdatedDateTime 进行更新。</span><span class="sxs-lookup"><span data-stu-id="25fad-186">lastUpdatedDateTime is not updated when a message is sent to the chat.</span></span> <span data-ttu-id="25fad-187">只读。</span><span class="sxs-lookup"><span data-stu-id="25fad-187">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25fad-188">关系</span><span class="sxs-lookup"><span data-stu-id="25fad-188">Relationships</span></span>

| <span data-ttu-id="25fad-189">关系</span><span class="sxs-lookup"><span data-stu-id="25fad-189">Relationship</span></span> | <span data-ttu-id="25fad-190">类型</span><span class="sxs-lookup"><span data-stu-id="25fad-190">Type</span></span> |<span data-ttu-id="25fad-191">说明</span><span class="sxs-lookup"><span data-stu-id="25fad-191">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="25fad-192">installedApps</span><span class="sxs-lookup"><span data-stu-id="25fad-192">installedApps</span></span> | <span data-ttu-id="25fad-193">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25fad-193">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="25fad-194">聊天中所有应用的集合。</span><span class="sxs-lookup"><span data-stu-id="25fad-194">A collection of all the apps in the chat.</span></span> <span data-ttu-id="25fad-195">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="25fad-195">Nullable.</span></span> |
| <span data-ttu-id="25fad-196">members</span><span class="sxs-lookup"><span data-stu-id="25fad-196">members</span></span> | <span data-ttu-id="25fad-197">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25fad-197">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="25fad-198">聊天中所有人员的集合。</span><span class="sxs-lookup"><span data-stu-id="25fad-198">A collection of all people in the chat.</span></span> <span data-ttu-id="25fad-199">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="25fad-199">Nullable.</span></span> |
| <span data-ttu-id="25fad-200">messages</span><span class="sxs-lookup"><span data-stu-id="25fad-200">messages</span></span> | <span data-ttu-id="25fad-201">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25fad-201">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="25fad-202">聊天中所有邮件的集合。</span><span class="sxs-lookup"><span data-stu-id="25fad-202">A collection of all the messages in the chat.</span></span> <span data-ttu-id="25fad-203">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="25fad-203">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="25fad-204">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="25fad-204">JSON representation</span></span>

<span data-ttu-id="25fad-205">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25fad-205">Here is a JSON representation of the resource.</span></span>

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
  "lastUpdatedDateTime": "dateTimeOffset"
}
```

## <a name="see-also"></a><span data-ttu-id="25fad-206">另请参阅</span><span class="sxs-lookup"><span data-stu-id="25fad-206">See also</span></span>

- [<span data-ttu-id="25fad-207">频道</span><span class="sxs-lookup"><span data-stu-id="25fad-207">channel</span></span>](channel.md)
- [<span data-ttu-id="25fad-208">chatMessage</span><span class="sxs-lookup"><span data-stu-id="25fad-208">chatMessage</span></span>](chatmessage.md)

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


