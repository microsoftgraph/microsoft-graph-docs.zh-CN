---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 Chatmessages 集合的集合。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8d0977593d46f3bfc063053791fa498c14fbf7a6
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124474"
---
# <a name="chat-resource-type"></a><span data-ttu-id="33d8f-103">聊天资源类型</span><span class="sxs-lookup"><span data-stu-id="33d8f-103">chat resource type</span></span>

<span data-ttu-id="33d8f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33d8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33d8f-105">聊天是一个或多个参与者之间的[chatmessages 集合](chatmessage.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="33d8f-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="33d8f-106">参与者可以是用户或应用程序。</span><span class="sxs-lookup"><span data-stu-id="33d8f-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="33d8f-107">方法</span><span class="sxs-lookup"><span data-stu-id="33d8f-107">Methods</span></span>

|  <span data-ttu-id="33d8f-108">方法</span><span class="sxs-lookup"><span data-stu-id="33d8f-108">Method</span></span>       |  <span data-ttu-id="33d8f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="33d8f-109">Return Type</span></span>  | <span data-ttu-id="33d8f-110">说明</span><span class="sxs-lookup"><span data-stu-id="33d8f-110">Description</span></span>| <span data-ttu-id="33d8f-111">权限</span><span class="sxs-lookup"><span data-stu-id="33d8f-111">Permissions</span></span> |
|:---------------|:--------|:----------|-----------|
|[<span data-ttu-id="33d8f-112">列出聊天</span><span class="sxs-lookup"><span data-stu-id="33d8f-112">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="33d8f-113">[聊天](channel.md)收藏</span><span class="sxs-lookup"><span data-stu-id="33d8f-113">[chat](channel.md) collection</span></span> | <span data-ttu-id="33d8f-114">获取用户所属的聊天列表。</span><span class="sxs-lookup"><span data-stu-id="33d8f-114">Get the list of chats a user is part of.</span></span>| <span data-ttu-id="33d8f-115">**仅委派**</span><span class="sxs-lookup"><span data-stu-id="33d8f-115">**Delegated only**</span></span> |
|[<span data-ttu-id="33d8f-116">获取聊天</span><span class="sxs-lookup"><span data-stu-id="33d8f-116">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="33d8f-117">参与</span><span class="sxs-lookup"><span data-stu-id="33d8f-117">chat</span></span>](channel.md) | <span data-ttu-id="33d8f-118">读取聊天的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="33d8f-118">Read properties and relationships of the chat.</span></span>| <span data-ttu-id="33d8f-119">委派和应用程序</span><span class="sxs-lookup"><span data-stu-id="33d8f-119">Delegated and application</span></span> |
|[<span data-ttu-id="33d8f-120">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="33d8f-120">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="33d8f-121">[conversationmember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="33d8f-121">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="33d8f-122">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="33d8f-122">Get the list of all users in the chat.</span></span>| <span data-ttu-id="33d8f-123">委派和应用程序（如下所示）</span><span class="sxs-lookup"><span data-stu-id="33d8f-123">Delegated and application (see below)</span></span> |
|[<span data-ttu-id="33d8f-124">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="33d8f-124">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="33d8f-125">conversationmember</span><span class="sxs-lookup"><span data-stu-id="33d8f-125">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="33d8f-126">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="33d8f-126">Get a single user in the chat.</span></span>| <span data-ttu-id="33d8f-127">委派和应用程序（请参阅注释）</span><span class="sxs-lookup"><span data-stu-id="33d8f-127">Delegated and application (see note)</span></span> |
|[<span data-ttu-id="33d8f-128">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="33d8f-128">List messages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="33d8f-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="33d8f-129">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="33d8f-130">获取一对一聊天或群组聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="33d8f-130">Get messages in a 1:1 or group chat.</span></span> | <span data-ttu-id="33d8f-131">委派和应用程序（请参阅注释）</span><span class="sxs-lookup"><span data-stu-id="33d8f-131">Delegated and application (see note)</span></span> |
|[<span data-ttu-id="33d8f-132">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="33d8f-132">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="33d8f-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="33d8f-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="33d8f-134">获取聊天中的单个消息。</span><span class="sxs-lookup"><span data-stu-id="33d8f-134">Get a single message in a chat.</span></span> | <span data-ttu-id="33d8f-135">委派和应用程序（请参阅注释）</span><span class="sxs-lookup"><span data-stu-id="33d8f-135">Delegated and application (see note)</span></span> |

> <span data-ttu-id="33d8f-136">**注意：** 使用应用程序权限时，请务必了解如何获取聊天 ID。</span><span class="sxs-lookup"><span data-stu-id="33d8f-136">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="33d8f-137">由于不支持列出具有应用程序权限的聊天，因此并非所有方案都可行。</span><span class="sxs-lookup"><span data-stu-id="33d8f-137">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="33d8f-138">可以获取具有委派权限的聊天 Id，也可以通过应用程序权限获取[/chats/allMessages 的更改通知](../api/subscription-post-subscriptions.md)。</span><span class="sxs-lookup"><span data-stu-id="33d8f-138">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/allMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="33d8f-139">属性</span><span class="sxs-lookup"><span data-stu-id="33d8f-139">Properties</span></span>

| <span data-ttu-id="33d8f-140">属性</span><span class="sxs-lookup"><span data-stu-id="33d8f-140">Property</span></span>   | <span data-ttu-id="33d8f-141">类型</span><span class="sxs-lookup"><span data-stu-id="33d8f-141">Type</span></span> |<span data-ttu-id="33d8f-142">说明</span><span class="sxs-lookup"><span data-stu-id="33d8f-142">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="33d8f-143">id</span><span class="sxs-lookup"><span data-stu-id="33d8f-143">id</span></span>| <span data-ttu-id="33d8f-144">String</span><span class="sxs-lookup"><span data-stu-id="33d8f-144">String</span></span>| <span data-ttu-id="33d8f-145">聊天的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="33d8f-145">The chat's unique identifier.</span></span> <span data-ttu-id="33d8f-146">只读。</span><span class="sxs-lookup"><span data-stu-id="33d8f-146">Read-only.</span></span>|
| <span data-ttu-id="33d8f-147">topic</span><span class="sxs-lookup"><span data-stu-id="33d8f-147">topic</span></span>| <span data-ttu-id="33d8f-148">String</span><span class="sxs-lookup"><span data-stu-id="33d8f-148">String</span></span>|  <span data-ttu-id="33d8f-149">Optional聊天的主题或主题。</span><span class="sxs-lookup"><span data-stu-id="33d8f-149">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="33d8f-150">仅适用于组聊天。</span><span class="sxs-lookup"><span data-stu-id="33d8f-150">Only available for group chats.</span></span>|
| <span data-ttu-id="33d8f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33d8f-151">createdDateTime</span></span>| <span data-ttu-id="33d8f-152">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33d8f-152">dateTimeOffset</span></span>|  <span data-ttu-id="33d8f-153">聊天的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="33d8f-153">Date and time at which the chat was created.</span></span> <span data-ttu-id="33d8f-154">只读。</span><span class="sxs-lookup"><span data-stu-id="33d8f-154">Read-only.</span></span>|
| <span data-ttu-id="33d8f-155">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="33d8f-155">lastUpdatedDateTime</span></span>| <span data-ttu-id="33d8f-156">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33d8f-156">dateTimeOffset</span></span>|  <span data-ttu-id="33d8f-157">更新聊天的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="33d8f-157">Date and time at which the chat was updated.</span></span> <span data-ttu-id="33d8f-158">只读。</span><span class="sxs-lookup"><span data-stu-id="33d8f-158">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33d8f-159">关系</span><span class="sxs-lookup"><span data-stu-id="33d8f-159">Relationships</span></span>

| <span data-ttu-id="33d8f-160">关系</span><span class="sxs-lookup"><span data-stu-id="33d8f-160">Relationship</span></span> | <span data-ttu-id="33d8f-161">类型</span><span class="sxs-lookup"><span data-stu-id="33d8f-161">Type</span></span> |<span data-ttu-id="33d8f-162">说明</span><span class="sxs-lookup"><span data-stu-id="33d8f-162">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="33d8f-163">installedApps</span><span class="sxs-lookup"><span data-stu-id="33d8f-163">installedApps</span></span> | <span data-ttu-id="33d8f-164">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="33d8f-164">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="33d8f-165">聊天中所有应用的集合。</span><span class="sxs-lookup"><span data-stu-id="33d8f-165">A collection of all the apps in the chat.</span></span> <span data-ttu-id="33d8f-166">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="33d8f-166">Nullable.</span></span> |
| <span data-ttu-id="33d8f-167">members</span><span class="sxs-lookup"><span data-stu-id="33d8f-167">members</span></span> | <span data-ttu-id="33d8f-168">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="33d8f-168">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="33d8f-169">聊天中所有人员的集合。</span><span class="sxs-lookup"><span data-stu-id="33d8f-169">A collection of all people in the chat.</span></span> <span data-ttu-id="33d8f-170">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="33d8f-170">Nullable.</span></span> |
| <span data-ttu-id="33d8f-171">messages</span><span class="sxs-lookup"><span data-stu-id="33d8f-171">messages</span></span> | <span data-ttu-id="33d8f-172">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="33d8f-172">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="33d8f-173">聊天中所有邮件的集合。</span><span class="sxs-lookup"><span data-stu-id="33d8f-173">A collection of all the messages in the chat.</span></span> <span data-ttu-id="33d8f-174">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="33d8f-174">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="33d8f-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="33d8f-175">JSON representation</span></span>

<span data-ttu-id="33d8f-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33d8f-176">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="33d8f-177">另请参阅</span><span class="sxs-lookup"><span data-stu-id="33d8f-177">See also</span></span>

- [<span data-ttu-id="33d8f-178">频道</span><span class="sxs-lookup"><span data-stu-id="33d8f-178">channel</span></span>](channel.md)
- [<span data-ttu-id="33d8f-179">chatMessage</span><span class="sxs-lookup"><span data-stu-id="33d8f-179">chatMessage</span></span>](chatmessage.md)

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
