---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 Chatmessages 集合的集合。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 88d08c8e6e0222c339c99db9cab9243f9c48c1f3
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597254"
---
# <a name="chat-resource-type"></a><span data-ttu-id="3cf17-103">聊天资源类型</span><span class="sxs-lookup"><span data-stu-id="3cf17-103">chat resource type</span></span>

<span data-ttu-id="3cf17-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cf17-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cf17-105">聊天是一个或多个参与者之间的 [chatmessages 集合](chatmessage.md) 的集合。</span><span class="sxs-lookup"><span data-stu-id="3cf17-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="3cf17-106">参与者可以是用户或应用程序。</span><span class="sxs-lookup"><span data-stu-id="3cf17-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="3cf17-107">方法</span><span class="sxs-lookup"><span data-stu-id="3cf17-107">Methods</span></span>

|  <span data-ttu-id="3cf17-108">方法</span><span class="sxs-lookup"><span data-stu-id="3cf17-108">Method</span></span>       |  <span data-ttu-id="3cf17-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="3cf17-109">Return Type</span></span>  | <span data-ttu-id="3cf17-110">Description</span><span class="sxs-lookup"><span data-stu-id="3cf17-110">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="3cf17-111">列出聊天</span><span class="sxs-lookup"><span data-stu-id="3cf17-111">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="3cf17-112">[聊天](chat.md) 收藏</span><span class="sxs-lookup"><span data-stu-id="3cf17-112">[chat](chat.md) collection</span></span> | <span data-ttu-id="3cf17-113">获取用户所属的聊天列表。</span><span class="sxs-lookup"><span data-stu-id="3cf17-113">Get the list of chats a user is part of.</span></span>| 
|[<span data-ttu-id="3cf17-114">获取聊天</span><span class="sxs-lookup"><span data-stu-id="3cf17-114">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="3cf17-115">聊天</span><span class="sxs-lookup"><span data-stu-id="3cf17-115">chat</span></span>](chat.md) | <span data-ttu-id="3cf17-116">读取聊天的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3cf17-116">Read properties and relationships of the chat.</span></span>| 
|[<span data-ttu-id="3cf17-117">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="3cf17-117">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="3cf17-118">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3cf17-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="3cf17-119">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="3cf17-119">Get the list of all users in the chat.</span></span>| 
|[<span data-ttu-id="3cf17-120">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="3cf17-120">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="3cf17-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="3cf17-121">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="3cf17-122">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="3cf17-122">Get a single user in the chat.</span></span>| 
|[<span data-ttu-id="3cf17-123">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="3cf17-123">List messages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="3cf17-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="3cf17-124">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="3cf17-125">获取一对一聊天或群组聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="3cf17-125">Get messages in a 1:1 or group chat.</span></span> | 
|[<span data-ttu-id="3cf17-126">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="3cf17-126">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="3cf17-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="3cf17-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="3cf17-128">获取聊天中的单个消息。</span><span class="sxs-lookup"><span data-stu-id="3cf17-128">Get a single message in a chat.</span></span> | 
|[<span data-ttu-id="3cf17-129">在用户和应用之间获取聊天</span><span class="sxs-lookup"><span data-stu-id="3cf17-129">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="3cf17-130">聊天</span><span class="sxs-lookup"><span data-stu-id="3cf17-130">chat</span></span>](chat.md)| <span data-ttu-id="3cf17-131">在用户和应用之间获取一对一聊天</span><span class="sxs-lookup"><span data-stu-id="3cf17-131">Get one-on-one chat between user and the app</span></span> |
|[<span data-ttu-id="3cf17-132">获取所有聊天消息</span><span class="sxs-lookup"><span data-stu-id="3cf17-132">Get all chat messages</span></span>](../api/chats-getallmessages.md)| <span data-ttu-id="3cf17-133">[聊天](chat.md) 收藏</span><span class="sxs-lookup"><span data-stu-id="3cf17-133">[chat](chat.md) collection</span></span>| <span data-ttu-id="3cf17-134">从用户参与的所有聊天中获取邮件，包括一对一聊天、群研讨和会议聊天。</span><span class="sxs-lookup"><span data-stu-id="3cf17-134">Get messages from all chats that a user is a participant in, including one-on-one chats, group chats, and meeting chats.</span></span> |

><span data-ttu-id="3cf17-135">**注意：** 使用应用程序权限时，请务必了解如何获取聊天 ID。</span><span class="sxs-lookup"><span data-stu-id="3cf17-135">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="3cf17-136">由于不支持列出具有应用程序权限的聊天，因此并非所有方案都可行。</span><span class="sxs-lookup"><span data-stu-id="3cf17-136">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="3cf17-137">可以获取具有委派权限的聊天 Id，也可以通过应用程序权限获取 [/chats/getAllMessages 的更改通知](../api/subscription-post-subscriptions.md) 。</span><span class="sxs-lookup"><span data-stu-id="3cf17-137">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="3cf17-138">属性</span><span class="sxs-lookup"><span data-stu-id="3cf17-138">Properties</span></span>

| <span data-ttu-id="3cf17-139">属性</span><span class="sxs-lookup"><span data-stu-id="3cf17-139">Property</span></span>   | <span data-ttu-id="3cf17-140">类型</span><span class="sxs-lookup"><span data-stu-id="3cf17-140">Type</span></span> |<span data-ttu-id="3cf17-141">说明</span><span class="sxs-lookup"><span data-stu-id="3cf17-141">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3cf17-142">id</span><span class="sxs-lookup"><span data-stu-id="3cf17-142">id</span></span>| <span data-ttu-id="3cf17-143">String</span><span class="sxs-lookup"><span data-stu-id="3cf17-143">String</span></span>| <span data-ttu-id="3cf17-144">聊天的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3cf17-144">The chat's unique identifier.</span></span> <span data-ttu-id="3cf17-145">只读。</span><span class="sxs-lookup"><span data-stu-id="3cf17-145">Read-only.</span></span>|
| <span data-ttu-id="3cf17-146">topic</span><span class="sxs-lookup"><span data-stu-id="3cf17-146">topic</span></span>| <span data-ttu-id="3cf17-147">String</span><span class="sxs-lookup"><span data-stu-id="3cf17-147">String</span></span>|  <span data-ttu-id="3cf17-148"> (聊天的可选) 主题或主题。</span><span class="sxs-lookup"><span data-stu-id="3cf17-148">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="3cf17-149">仅适用于组聊天。</span><span class="sxs-lookup"><span data-stu-id="3cf17-149">Only available for group chats.</span></span>|
| <span data-ttu-id="3cf17-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3cf17-150">createdDateTime</span></span>| <span data-ttu-id="3cf17-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cf17-151">dateTimeOffset</span></span>|  <span data-ttu-id="3cf17-152">聊天的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3cf17-152">Date and time at which the chat was created.</span></span> <span data-ttu-id="3cf17-153">只读。</span><span class="sxs-lookup"><span data-stu-id="3cf17-153">Read-only.</span></span>|
| <span data-ttu-id="3cf17-154">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3cf17-154">lastUpdatedDateTime</span></span>| <span data-ttu-id="3cf17-155">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cf17-155">dateTimeOffset</span></span>|  <span data-ttu-id="3cf17-156">重命名或更改成员身份时的聊天的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3cf17-156">Date and time at which the chat was renamed or membership changed.</span></span> <span data-ttu-id="3cf17-157">将邮件发送到聊天时，不会对 lastUpdatedDateTime 进行更新。</span><span class="sxs-lookup"><span data-stu-id="3cf17-157">lastUpdatedDateTime is not updated when a message is sent to the chat.</span></span> <span data-ttu-id="3cf17-158">只读。</span><span class="sxs-lookup"><span data-stu-id="3cf17-158">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3cf17-159">关系</span><span class="sxs-lookup"><span data-stu-id="3cf17-159">Relationships</span></span>

| <span data-ttu-id="3cf17-160">关系</span><span class="sxs-lookup"><span data-stu-id="3cf17-160">Relationship</span></span> | <span data-ttu-id="3cf17-161">类型</span><span class="sxs-lookup"><span data-stu-id="3cf17-161">Type</span></span> |<span data-ttu-id="3cf17-162">说明</span><span class="sxs-lookup"><span data-stu-id="3cf17-162">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3cf17-163">installedApps</span><span class="sxs-lookup"><span data-stu-id="3cf17-163">installedApps</span></span> | <span data-ttu-id="3cf17-164">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3cf17-164">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="3cf17-165">聊天中所有应用的集合。</span><span class="sxs-lookup"><span data-stu-id="3cf17-165">A collection of all the apps in the chat.</span></span> <span data-ttu-id="3cf17-166">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3cf17-166">Nullable.</span></span> |
| <span data-ttu-id="3cf17-167">members</span><span class="sxs-lookup"><span data-stu-id="3cf17-167">members</span></span> | <span data-ttu-id="3cf17-168">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3cf17-168">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="3cf17-169">聊天中所有人员的集合。</span><span class="sxs-lookup"><span data-stu-id="3cf17-169">A collection of all people in the chat.</span></span> <span data-ttu-id="3cf17-170">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3cf17-170">Nullable.</span></span> |
| <span data-ttu-id="3cf17-171">messages</span><span class="sxs-lookup"><span data-stu-id="3cf17-171">messages</span></span> | <span data-ttu-id="3cf17-172">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3cf17-172">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="3cf17-173">聊天中所有邮件的集合。</span><span class="sxs-lookup"><span data-stu-id="3cf17-173">A collection of all the messages in the chat.</span></span> <span data-ttu-id="3cf17-174">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3cf17-174">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3cf17-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3cf17-175">JSON representation</span></span>

<span data-ttu-id="3cf17-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3cf17-176">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="3cf17-177">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3cf17-177">See also</span></span>

- [<span data-ttu-id="3cf17-178">频道</span><span class="sxs-lookup"><span data-stu-id="3cf17-178">channel</span></span>](channel.md)
- [<span data-ttu-id="3cf17-179">chatMessage</span><span class="sxs-lookup"><span data-stu-id="3cf17-179">chatMessage</span></span>](chatmessage.md)

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


