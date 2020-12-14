---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 chatMessages 集合。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dcfa853f8ba246443f0f5073a4a62fd84f92adc6
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659406"
---
# <a name="chat-resource-type"></a><span data-ttu-id="fdff1-103">聊天资源类型</span><span class="sxs-lookup"><span data-stu-id="fdff1-103">chat resource type</span></span>

<span data-ttu-id="fdff1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdff1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdff1-105">聊天是一个或多个参与者之间的 [chatMessages](chatmessage.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="fdff1-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="fdff1-106">参与者可以是用户或应用。</span><span class="sxs-lookup"><span data-stu-id="fdff1-106">Participants can be users or apps.</span></span>

> <span data-ttu-id="fdff1-107">**注意**：如果聊天与 [onlineMeeting](../resources/onlinemeeting.md) 实例关联，则列出的一些方法将可传递地影响会议。</span><span class="sxs-lookup"><span data-stu-id="fdff1-107">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then some of the listed methods will transitively impact the meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="fdff1-108">方法</span><span class="sxs-lookup"><span data-stu-id="fdff1-108">Methods</span></span>

|  <span data-ttu-id="fdff1-109">方法</span><span class="sxs-lookup"><span data-stu-id="fdff1-109">Method</span></span>       |  <span data-ttu-id="fdff1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="fdff1-110">Return Type</span></span>  | <span data-ttu-id="fdff1-111">说明</span><span class="sxs-lookup"><span data-stu-id="fdff1-111">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="fdff1-112">列出聊天</span><span class="sxs-lookup"><span data-stu-id="fdff1-112">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="fdff1-113">[chat](chat.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fdff1-113">[chat](chat.md) collection</span></span> | <span data-ttu-id="fdff1-114">获取用户参与的聊天列表。</span><span class="sxs-lookup"><span data-stu-id="fdff1-114">Get the list of chats a user is part of.</span></span>| 
|[<span data-ttu-id="fdff1-115">获取聊天</span><span class="sxs-lookup"><span data-stu-id="fdff1-115">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="fdff1-116">聊天</span><span class="sxs-lookup"><span data-stu-id="fdff1-116">chat</span></span>](chat.md) | <span data-ttu-id="fdff1-117">读取聊天的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fdff1-117">Read properties and relationships of the chat.</span></span>| 
|[<span data-ttu-id="fdff1-118">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="fdff1-118">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="fdff1-119">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fdff1-119">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="fdff1-120">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="fdff1-120">Get the list of all users in the chat.</span></span>| 
|[<span data-ttu-id="fdff1-121">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="fdff1-121">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="fdff1-122">conversationMember</span><span class="sxs-lookup"><span data-stu-id="fdff1-122">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="fdff1-123">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="fdff1-123">Get a single user in the chat.</span></span>| 
|[<span data-ttu-id="fdff1-124">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="fdff1-124">List messages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="fdff1-125">chatMessage</span><span class="sxs-lookup"><span data-stu-id="fdff1-125">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="fdff1-126">获取一对一聊天或群组聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="fdff1-126">Get messages in a 1:1 or group chat.</span></span> | 
|[<span data-ttu-id="fdff1-127">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="fdff1-127">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="fdff1-128">chatMessage</span><span class="sxs-lookup"><span data-stu-id="fdff1-128">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="fdff1-129">获取聊天中的单个消息。</span><span class="sxs-lookup"><span data-stu-id="fdff1-129">Get a single message in a chat.</span></span> | 
|[<span data-ttu-id="fdff1-130">获取用户和应用之间的聊天</span><span class="sxs-lookup"><span data-stu-id="fdff1-130">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="fdff1-131">聊天</span><span class="sxs-lookup"><span data-stu-id="fdff1-131">chat</span></span>](chat.md)| <span data-ttu-id="fdff1-132">获取用户与应用之间的一对一聊天</span><span class="sxs-lookup"><span data-stu-id="fdff1-132">Get one-on-one chat between user and the app</span></span> |
|[<span data-ttu-id="fdff1-133">获取所有聊天消息</span><span class="sxs-lookup"><span data-stu-id="fdff1-133">Get all chat messages</span></span>](../api/chats-getallmessages.md)| <span data-ttu-id="fdff1-134">[chat](chat.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fdff1-134">[chat](chat.md) collection</span></span>| <span data-ttu-id="fdff1-135">从用户参与的所有聊天（包括一对一聊天、群聊和会议聊天）获取消息。</span><span class="sxs-lookup"><span data-stu-id="fdff1-135">Get messages from all chats that a user is a participant in, including one-on-one chats, group chats, and meeting chats.</span></span> |
|[<span data-ttu-id="fdff1-136">列出聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="fdff1-136">List apps in chat</span></span>](../api/chat-list-installedapps.md) |<span data-ttu-id="fdff1-137">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fdff1-137">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="fdff1-138">列出安装在聊天聊天 (关联的会议) 。</span><span class="sxs-lookup"><span data-stu-id="fdff1-138">List apps installed in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="fdff1-139">获取聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="fdff1-139">Get app in chat</span></span>](../api/chat-get-installedapps.md) | [<span data-ttu-id="fdff1-140">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="fdff1-140">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="fdff1-141">获取在聊天聊天和关联会议 (安装的特定) 。</span><span class="sxs-lookup"><span data-stu-id="fdff1-141">Get a specific app installed in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="fdff1-142">在聊天中添加应用</span><span class="sxs-lookup"><span data-stu-id="fdff1-142">Add app in chat</span></span>](../api/chat-post-installedapps.md) | | <span data-ttu-id="fdff1-143">添加 (在) 和关联的会议 (中安装) 。</span><span class="sxs-lookup"><span data-stu-id="fdff1-143">Add (install) an app in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="fdff1-144">升级聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="fdff1-144">Upgrade app in chat</span></span>](../api/chat-teamsappinstallation-upgrade.md) | <span data-ttu-id="fdff1-145">无</span><span class="sxs-lookup"><span data-stu-id="fdff1-145">None</span></span> | <span data-ttu-id="fdff1-146">更新到安装在聊天会话和相关会议 (应用的) 。</span><span class="sxs-lookup"><span data-stu-id="fdff1-146">Update to the latest version of the app installed in chat (and associated meeting).</span></span>|
|[<span data-ttu-id="fdff1-147">从聊天中卸载应用</span><span class="sxs-lookup"><span data-stu-id="fdff1-147">Uninstall app from chat</span></span>](../api/chat-delete-installedapps.md) | <span data-ttu-id="fdff1-148">无</span><span class="sxs-lookup"><span data-stu-id="fdff1-148">None</span></span> | <span data-ttu-id="fdff1-149">从 (会议) 中删除 (应用程序) 。</span><span class="sxs-lookup"><span data-stu-id="fdff1-149">Remove (uninstall) app from a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="fdff1-150">列出聊天中的选项卡</span><span class="sxs-lookup"><span data-stu-id="fdff1-150">List tabs in chat</span></span>](../api/chat-list-tabs.md) | [<span data-ttu-id="fdff1-151">teamsTab</span><span class="sxs-lookup"><span data-stu-id="fdff1-151">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="fdff1-152">列出固定到聊天聊天 (关联的会议) 。</span><span class="sxs-lookup"><span data-stu-id="fdff1-152">List tabs pinned to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="fdff1-153">获取聊天中的选项卡</span><span class="sxs-lookup"><span data-stu-id="fdff1-153">Get tab in chat</span></span>](../api/chat-get-tabs.md) | [<span data-ttu-id="fdff1-154">teamsTab</span><span class="sxs-lookup"><span data-stu-id="fdff1-154">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="fdff1-155">获取固定到聊天会话和相关 (的特定选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="fdff1-155">Get a specific tab pinned to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="fdff1-156">向聊天添加选项卡</span><span class="sxs-lookup"><span data-stu-id="fdff1-156">Add tab to chat</span></span>](../api/chat-post-tabs.md) | [<span data-ttu-id="fdff1-157">teamsTab</span><span class="sxs-lookup"><span data-stu-id="fdff1-157">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="fdff1-158">将 (固定) 选项卡添加到聊天 (关联的会议) 。</span><span class="sxs-lookup"><span data-stu-id="fdff1-158">Add (pin) a tab to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="fdff1-159">聊天中的"更新"选项卡</span><span class="sxs-lookup"><span data-stu-id="fdff1-159">Update tab in chat</span></span>](../api/chat-patch-tabs.md) | [<span data-ttu-id="fdff1-160">teamsTab</span><span class="sxs-lookup"><span data-stu-id="fdff1-160">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="fdff1-161">更新聊天会话和关联会议 (选项卡) 。</span><span class="sxs-lookup"><span data-stu-id="fdff1-161">Update the properties of a tab in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="fdff1-162">从聊天中删除选项卡</span><span class="sxs-lookup"><span data-stu-id="fdff1-162">Remove tab from chat</span></span>](../api/chat-delete-tabs.md) | <span data-ttu-id="fdff1-163">无</span><span class="sxs-lookup"><span data-stu-id="fdff1-163">None</span></span> | <span data-ttu-id="fdff1-164">从 (活动) 关联的会议选项卡 (取消固定) 。</span><span class="sxs-lookup"><span data-stu-id="fdff1-164">Remove (unpin) a tab from a chat (and associated meeting).</span></span>|

><span data-ttu-id="fdff1-165">**注意：** 使用应用程序权限时，请确保你了解如何获取聊天 ID。</span><span class="sxs-lookup"><span data-stu-id="fdff1-165">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="fdff1-166">由于不支持列出具有应用程序权限的聊天，因此并非所有方案都可行。</span><span class="sxs-lookup"><span data-stu-id="fdff1-166">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="fdff1-167">可以获取具有委派权限的聊天 ID，以及从具有应用程序权限 [的 /chats/getAllMessages](../api/subscription-post-subscriptions.md) 更改通知获取。</span><span class="sxs-lookup"><span data-stu-id="fdff1-167">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="fdff1-168">属性</span><span class="sxs-lookup"><span data-stu-id="fdff1-168">Properties</span></span>

| <span data-ttu-id="fdff1-169">属性</span><span class="sxs-lookup"><span data-stu-id="fdff1-169">Property</span></span>   | <span data-ttu-id="fdff1-170">类型</span><span class="sxs-lookup"><span data-stu-id="fdff1-170">Type</span></span> |<span data-ttu-id="fdff1-171">说明</span><span class="sxs-lookup"><span data-stu-id="fdff1-171">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fdff1-172">id</span><span class="sxs-lookup"><span data-stu-id="fdff1-172">id</span></span>| <span data-ttu-id="fdff1-173">String</span><span class="sxs-lookup"><span data-stu-id="fdff1-173">String</span></span>| <span data-ttu-id="fdff1-174">聊天的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fdff1-174">The chat's unique identifier.</span></span> <span data-ttu-id="fdff1-175">只读。</span><span class="sxs-lookup"><span data-stu-id="fdff1-175">Read-only.</span></span>|
| <span data-ttu-id="fdff1-176">topic</span><span class="sxs-lookup"><span data-stu-id="fdff1-176">topic</span></span>| <span data-ttu-id="fdff1-177">String</span><span class="sxs-lookup"><span data-stu-id="fdff1-177">String</span></span>|  <span data-ttu-id="fdff1-178"> (聊天) 主题或主题的可选选项。</span><span class="sxs-lookup"><span data-stu-id="fdff1-178">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="fdff1-179">仅适用于群聊。</span><span class="sxs-lookup"><span data-stu-id="fdff1-179">Only available for group chats.</span></span>|
| <span data-ttu-id="fdff1-180">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fdff1-180">createdDateTime</span></span>| <span data-ttu-id="fdff1-181">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdff1-181">dateTimeOffset</span></span>|  <span data-ttu-id="fdff1-182">创建聊天的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fdff1-182">Date and time at which the chat was created.</span></span> <span data-ttu-id="fdff1-183">只读。</span><span class="sxs-lookup"><span data-stu-id="fdff1-183">Read-only.</span></span>|
| <span data-ttu-id="fdff1-184">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="fdff1-184">lastUpdatedDateTime</span></span>| <span data-ttu-id="fdff1-185">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdff1-185">dateTimeOffset</span></span>|  <span data-ttu-id="fdff1-186">重命名聊天或更改成员身份的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fdff1-186">Date and time at which the chat was renamed or membership changed.</span></span> <span data-ttu-id="fdff1-187">lastUpdatedDateTime 在消息发送到聊天时不会更新。</span><span class="sxs-lookup"><span data-stu-id="fdff1-187">lastUpdatedDateTime is not updated when a message is sent to the chat.</span></span> <span data-ttu-id="fdff1-188">只读。</span><span class="sxs-lookup"><span data-stu-id="fdff1-188">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdff1-189">关系</span><span class="sxs-lookup"><span data-stu-id="fdff1-189">Relationships</span></span>

| <span data-ttu-id="fdff1-190">关系</span><span class="sxs-lookup"><span data-stu-id="fdff1-190">Relationship</span></span> | <span data-ttu-id="fdff1-191">类型</span><span class="sxs-lookup"><span data-stu-id="fdff1-191">Type</span></span> |<span data-ttu-id="fdff1-192">说明</span><span class="sxs-lookup"><span data-stu-id="fdff1-192">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fdff1-193">installedApps</span><span class="sxs-lookup"><span data-stu-id="fdff1-193">installedApps</span></span> | <span data-ttu-id="fdff1-194">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fdff1-194">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="fdff1-195">聊天中所有应用的集合。</span><span class="sxs-lookup"><span data-stu-id="fdff1-195">A collection of all the apps in the chat.</span></span> <span data-ttu-id="fdff1-196">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="fdff1-196">Nullable.</span></span> |
| <span data-ttu-id="fdff1-197">members</span><span class="sxs-lookup"><span data-stu-id="fdff1-197">members</span></span> | <span data-ttu-id="fdff1-198">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fdff1-198">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="fdff1-199">聊天中所有人员的集合。</span><span class="sxs-lookup"><span data-stu-id="fdff1-199">A collection of all people in the chat.</span></span> <span data-ttu-id="fdff1-200">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="fdff1-200">Nullable.</span></span> |
| <span data-ttu-id="fdff1-201">messages</span><span class="sxs-lookup"><span data-stu-id="fdff1-201">messages</span></span> | <span data-ttu-id="fdff1-202">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fdff1-202">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="fdff1-203">聊天中所有消息的集合。</span><span class="sxs-lookup"><span data-stu-id="fdff1-203">A collection of all the messages in the chat.</span></span> <span data-ttu-id="fdff1-204">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="fdff1-204">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fdff1-205">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fdff1-205">JSON representation</span></span>

<span data-ttu-id="fdff1-206">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fdff1-206">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="fdff1-207">另请参阅</span><span class="sxs-lookup"><span data-stu-id="fdff1-207">See also</span></span>

- [<span data-ttu-id="fdff1-208">频道</span><span class="sxs-lookup"><span data-stu-id="fdff1-208">channel</span></span>](channel.md)
- [<span data-ttu-id="fdff1-209">chatMessage</span><span class="sxs-lookup"><span data-stu-id="fdff1-209">chatMessage</span></span>](chatmessage.md)

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


