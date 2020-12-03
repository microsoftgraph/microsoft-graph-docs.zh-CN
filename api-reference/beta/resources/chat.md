---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 Chatmessages 集合的集合。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e6316f7c3aad0fc90e258d145b57942395265ce7
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563448"
---
# <a name="chat-resource-type"></a><span data-ttu-id="14bb2-103">聊天资源类型</span><span class="sxs-lookup"><span data-stu-id="14bb2-103">chat resource type</span></span>

<span data-ttu-id="14bb2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14bb2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14bb2-105">聊天是一个或多个参与者之间的 [chatmessages 集合](chatmessage.md) 的集合。</span><span class="sxs-lookup"><span data-stu-id="14bb2-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="14bb2-106">参与者可以是用户或应用程序。</span><span class="sxs-lookup"><span data-stu-id="14bb2-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="14bb2-107">方法</span><span class="sxs-lookup"><span data-stu-id="14bb2-107">Methods</span></span>

|  <span data-ttu-id="14bb2-108">方法</span><span class="sxs-lookup"><span data-stu-id="14bb2-108">Method</span></span>       |  <span data-ttu-id="14bb2-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="14bb2-109">Return Type</span></span>  | <span data-ttu-id="14bb2-110">说明</span><span class="sxs-lookup"><span data-stu-id="14bb2-110">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="14bb2-111">列出聊天</span><span class="sxs-lookup"><span data-stu-id="14bb2-111">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="14bb2-112">[聊天](chat.md) 收藏</span><span class="sxs-lookup"><span data-stu-id="14bb2-112">[chat](chat.md) collection</span></span> | <span data-ttu-id="14bb2-113">获取用户所属的聊天列表。</span><span class="sxs-lookup"><span data-stu-id="14bb2-113">Get the list of chats a user is part of.</span></span>| 
|[<span data-ttu-id="14bb2-114">获取聊天</span><span class="sxs-lookup"><span data-stu-id="14bb2-114">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="14bb2-115">聊天</span><span class="sxs-lookup"><span data-stu-id="14bb2-115">chat</span></span>](chat.md) | <span data-ttu-id="14bb2-116">读取聊天的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="14bb2-116">Read properties and relationships of the chat.</span></span>| 
|[<span data-ttu-id="14bb2-117">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="14bb2-117">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="14bb2-118">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14bb2-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="14bb2-119">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="14bb2-119">Get the list of all users in the chat.</span></span>| 
|[<span data-ttu-id="14bb2-120">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="14bb2-120">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="14bb2-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="14bb2-121">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="14bb2-122">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="14bb2-122">Get a single user in the chat.</span></span>| 
|[<span data-ttu-id="14bb2-123">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="14bb2-123">List messages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="14bb2-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="14bb2-124">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="14bb2-125">获取一对一聊天或群组聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="14bb2-125">Get messages in a 1:1 or group chat.</span></span> | 
|[<span data-ttu-id="14bb2-126">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="14bb2-126">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="14bb2-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="14bb2-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="14bb2-128">获取聊天中的单个消息。</span><span class="sxs-lookup"><span data-stu-id="14bb2-128">Get a single message in a chat.</span></span> | 
|[<span data-ttu-id="14bb2-129">在用户和应用之间获取聊天</span><span class="sxs-lookup"><span data-stu-id="14bb2-129">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="14bb2-130">聊天</span><span class="sxs-lookup"><span data-stu-id="14bb2-130">chat</span></span>](chat.md)| <span data-ttu-id="14bb2-131">在用户和应用之间获取一对一聊天</span><span class="sxs-lookup"><span data-stu-id="14bb2-131">Get one-on-one chat between user and the app</span></span> |

><span data-ttu-id="14bb2-132">**注意：** 使用应用程序权限时，请务必了解如何获取聊天 ID。</span><span class="sxs-lookup"><span data-stu-id="14bb2-132">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="14bb2-133">由于不支持列出具有应用程序权限的聊天，因此并非所有方案都可行。</span><span class="sxs-lookup"><span data-stu-id="14bb2-133">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="14bb2-134">可以获取具有委派权限的聊天 Id，也可以通过应用程序权限获取 [/chats/getAllMessages 的更改通知](../api/subscription-post-subscriptions.md) 。</span><span class="sxs-lookup"><span data-stu-id="14bb2-134">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="14bb2-135">属性</span><span class="sxs-lookup"><span data-stu-id="14bb2-135">Properties</span></span>

| <span data-ttu-id="14bb2-136">属性</span><span class="sxs-lookup"><span data-stu-id="14bb2-136">Property</span></span>   | <span data-ttu-id="14bb2-137">类型</span><span class="sxs-lookup"><span data-stu-id="14bb2-137">Type</span></span> |<span data-ttu-id="14bb2-138">说明</span><span class="sxs-lookup"><span data-stu-id="14bb2-138">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="14bb2-139">id</span><span class="sxs-lookup"><span data-stu-id="14bb2-139">id</span></span>| <span data-ttu-id="14bb2-140">String</span><span class="sxs-lookup"><span data-stu-id="14bb2-140">String</span></span>| <span data-ttu-id="14bb2-141">聊天的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="14bb2-141">The chat's unique identifier.</span></span> <span data-ttu-id="14bb2-142">只读。</span><span class="sxs-lookup"><span data-stu-id="14bb2-142">Read-only.</span></span>|
| <span data-ttu-id="14bb2-143">topic</span><span class="sxs-lookup"><span data-stu-id="14bb2-143">topic</span></span>| <span data-ttu-id="14bb2-144">String</span><span class="sxs-lookup"><span data-stu-id="14bb2-144">String</span></span>|  <span data-ttu-id="14bb2-145"> (聊天的可选) 主题或主题。</span><span class="sxs-lookup"><span data-stu-id="14bb2-145">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="14bb2-146">仅适用于组聊天。</span><span class="sxs-lookup"><span data-stu-id="14bb2-146">Only available for group chats.</span></span>|
| <span data-ttu-id="14bb2-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14bb2-147">createdDateTime</span></span>| <span data-ttu-id="14bb2-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14bb2-148">dateTimeOffset</span></span>|  <span data-ttu-id="14bb2-149">聊天的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="14bb2-149">Date and time at which the chat was created.</span></span> <span data-ttu-id="14bb2-150">只读。</span><span class="sxs-lookup"><span data-stu-id="14bb2-150">Read-only.</span></span>|
| <span data-ttu-id="14bb2-151">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="14bb2-151">lastUpdatedDateTime</span></span>| <span data-ttu-id="14bb2-152">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14bb2-152">dateTimeOffset</span></span>|  <span data-ttu-id="14bb2-153">重命名或更改成员身份时的聊天的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="14bb2-153">Date and time at which the chat was renamed or membership changed.</span></span> <span data-ttu-id="14bb2-154">将邮件发送到聊天时，不会对 lastUpdatedDateTime 进行更新。</span><span class="sxs-lookup"><span data-stu-id="14bb2-154">lastUpdatedDateTime is not updated when a message is sent to the chat.</span></span> <span data-ttu-id="14bb2-155">只读。</span><span class="sxs-lookup"><span data-stu-id="14bb2-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14bb2-156">关系</span><span class="sxs-lookup"><span data-stu-id="14bb2-156">Relationships</span></span>

| <span data-ttu-id="14bb2-157">关系</span><span class="sxs-lookup"><span data-stu-id="14bb2-157">Relationship</span></span> | <span data-ttu-id="14bb2-158">类型</span><span class="sxs-lookup"><span data-stu-id="14bb2-158">Type</span></span> |<span data-ttu-id="14bb2-159">说明</span><span class="sxs-lookup"><span data-stu-id="14bb2-159">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="14bb2-160">installedApps</span><span class="sxs-lookup"><span data-stu-id="14bb2-160">installedApps</span></span> | <span data-ttu-id="14bb2-161">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14bb2-161">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="14bb2-162">聊天中所有应用的集合。</span><span class="sxs-lookup"><span data-stu-id="14bb2-162">A collection of all the apps in the chat.</span></span> <span data-ttu-id="14bb2-163">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="14bb2-163">Nullable.</span></span> |
| <span data-ttu-id="14bb2-164">members</span><span class="sxs-lookup"><span data-stu-id="14bb2-164">members</span></span> | <span data-ttu-id="14bb2-165">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14bb2-165">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="14bb2-166">聊天中所有人员的集合。</span><span class="sxs-lookup"><span data-stu-id="14bb2-166">A collection of all people in the chat.</span></span> <span data-ttu-id="14bb2-167">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="14bb2-167">Nullable.</span></span> |
| <span data-ttu-id="14bb2-168">messages</span><span class="sxs-lookup"><span data-stu-id="14bb2-168">messages</span></span> | <span data-ttu-id="14bb2-169">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14bb2-169">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="14bb2-170">聊天中所有邮件的集合。</span><span class="sxs-lookup"><span data-stu-id="14bb2-170">A collection of all the messages in the chat.</span></span> <span data-ttu-id="14bb2-171">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="14bb2-171">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="14bb2-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14bb2-172">JSON representation</span></span>

<span data-ttu-id="14bb2-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14bb2-173">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="14bb2-174">另请参阅</span><span class="sxs-lookup"><span data-stu-id="14bb2-174">See also</span></span>

- [<span data-ttu-id="14bb2-175">频道</span><span class="sxs-lookup"><span data-stu-id="14bb2-175">channel</span></span>](channel.md)
- [<span data-ttu-id="14bb2-176">chatMessage</span><span class="sxs-lookup"><span data-stu-id="14bb2-176">chatMessage</span></span>](chatmessage.md)

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


