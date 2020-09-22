---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 Chatmessages 集合的集合。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7c365fd343af3078663cbd184b67b49feb37945c
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193475"
---
# <a name="chat-resource-type"></a><span data-ttu-id="2f8f9-103">聊天资源类型</span><span class="sxs-lookup"><span data-stu-id="2f8f9-103">chat resource type</span></span>

<span data-ttu-id="2f8f9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f8f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f8f9-105">聊天是一个或多个参与者之间的 [chatmessages 集合](chatmessage.md) 的集合。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="2f8f9-106">参与者可以是用户或应用程序。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="2f8f9-107">方法</span><span class="sxs-lookup"><span data-stu-id="2f8f9-107">Methods</span></span>

|  <span data-ttu-id="2f8f9-108">方法</span><span class="sxs-lookup"><span data-stu-id="2f8f9-108">Method</span></span>       |  <span data-ttu-id="2f8f9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2f8f9-109">Return Type</span></span>  | <span data-ttu-id="2f8f9-110">说明</span><span class="sxs-lookup"><span data-stu-id="2f8f9-110">Description</span></span>| <span data-ttu-id="2f8f9-111">权限</span><span class="sxs-lookup"><span data-stu-id="2f8f9-111">Permissions</span></span> |
|:---------------|:--------|:----------|-----------|
|[<span data-ttu-id="2f8f9-112">列出聊天</span><span class="sxs-lookup"><span data-stu-id="2f8f9-112">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="2f8f9-113">[聊天](chat.md) 收藏</span><span class="sxs-lookup"><span data-stu-id="2f8f9-113">[chat](chat.md) collection</span></span> | <span data-ttu-id="2f8f9-114">获取用户所属的聊天列表。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-114">Get the list of chats a user is part of.</span></span>| <span data-ttu-id="2f8f9-115">**仅委派**</span><span class="sxs-lookup"><span data-stu-id="2f8f9-115">**Delegated only**</span></span> |
|[<span data-ttu-id="2f8f9-116">获取聊天</span><span class="sxs-lookup"><span data-stu-id="2f8f9-116">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="2f8f9-117">聊天</span><span class="sxs-lookup"><span data-stu-id="2f8f9-117">chat</span></span>](chat.md) | <span data-ttu-id="2f8f9-118">读取聊天的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-118">Read properties and relationships of the chat.</span></span>| <span data-ttu-id="2f8f9-119">**仅委派**</span><span class="sxs-lookup"><span data-stu-id="2f8f9-119">**Delegated only**</span></span> |
|[<span data-ttu-id="2f8f9-120">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="2f8f9-120">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="2f8f9-121">[conversationmember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f8f9-121">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="2f8f9-122">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-122">Get the list of all users in the chat.</span></span>| <span data-ttu-id="2f8f9-123">委派和应用程序 \*</span><span class="sxs-lookup"><span data-stu-id="2f8f9-123">Delegated and application\*</span></span> |
|[<span data-ttu-id="2f8f9-124">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="2f8f9-124">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="2f8f9-125">conversationmember</span><span class="sxs-lookup"><span data-stu-id="2f8f9-125">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="2f8f9-126">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-126">Get a single user in the chat.</span></span>| <span data-ttu-id="2f8f9-127">委派和应用程序 \*</span><span class="sxs-lookup"><span data-stu-id="2f8f9-127">Delegated and application\*</span></span> |
|[<span data-ttu-id="2f8f9-128">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="2f8f9-128">List messages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="2f8f9-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="2f8f9-129">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="2f8f9-130">获取一对一聊天或群组聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-130">Get messages in a 1:1 or group chat.</span></span> | <span data-ttu-id="2f8f9-131">委派和应用程序 \*</span><span class="sxs-lookup"><span data-stu-id="2f8f9-131">Delegated and application\*</span></span> |
|[<span data-ttu-id="2f8f9-132">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="2f8f9-132">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="2f8f9-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="2f8f9-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="2f8f9-134">获取聊天中的单个消息。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-134">Get a single message in a chat.</span></span> | <span data-ttu-id="2f8f9-135">委派和应用程序 \*</span><span class="sxs-lookup"><span data-stu-id="2f8f9-135">Delegated and application\*</span></span> |

<span data-ttu-id="2f8f9-136">\*> **注意：** 使用应用程序权限时，请务必了解如何获取聊天 ID。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-136">\*> **Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="2f8f9-137">由于不支持列出具有应用程序权限的聊天，因此并非所有方案都可行。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-137">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="2f8f9-138">可以获取具有委派权限的聊天 Id，也可以通过应用程序权限获取 [/chats/getAllMessages 的更改通知](../api/subscription-post-subscriptions.md) 。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-138">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="2f8f9-139">属性</span><span class="sxs-lookup"><span data-stu-id="2f8f9-139">Properties</span></span>

| <span data-ttu-id="2f8f9-140">属性</span><span class="sxs-lookup"><span data-stu-id="2f8f9-140">Property</span></span>   | <span data-ttu-id="2f8f9-141">类型</span><span class="sxs-lookup"><span data-stu-id="2f8f9-141">Type</span></span> |<span data-ttu-id="2f8f9-142">说明</span><span class="sxs-lookup"><span data-stu-id="2f8f9-142">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2f8f9-143">id</span><span class="sxs-lookup"><span data-stu-id="2f8f9-143">id</span></span>| <span data-ttu-id="2f8f9-144">字符串</span><span class="sxs-lookup"><span data-stu-id="2f8f9-144">String</span></span>| <span data-ttu-id="2f8f9-145">聊天的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-145">The chat's unique identifier.</span></span> <span data-ttu-id="2f8f9-146">只读。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-146">Read-only.</span></span>|
| <span data-ttu-id="2f8f9-147">topic</span><span class="sxs-lookup"><span data-stu-id="2f8f9-147">topic</span></span>| <span data-ttu-id="2f8f9-148">String</span><span class="sxs-lookup"><span data-stu-id="2f8f9-148">String</span></span>|  <span data-ttu-id="2f8f9-149"> (聊天的可选) 主题或主题。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-149">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="2f8f9-150">仅适用于组聊天。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-150">Only available for group chats.</span></span>|
| <span data-ttu-id="2f8f9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f8f9-151">createdDateTime</span></span>| <span data-ttu-id="2f8f9-152">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f8f9-152">dateTimeOffset</span></span>|  <span data-ttu-id="2f8f9-153">聊天的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-153">Date and time at which the chat was created.</span></span> <span data-ttu-id="2f8f9-154">只读。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-154">Read-only.</span></span>|
| <span data-ttu-id="2f8f9-155">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f8f9-155">lastUpdatedDateTime</span></span>| <span data-ttu-id="2f8f9-156">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f8f9-156">dateTimeOffset</span></span>|  <span data-ttu-id="2f8f9-157">重命名或更改成员身份时的聊天的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-157">Date and time at which the chat was renamed or membership changed.</span></span> <span data-ttu-id="2f8f9-158">将邮件发送到聊天时，不会对 lastUpdatedDateTime 进行更新。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-158">lastUpdatedDateTime is not updated when a message is sent to the chat.</span></span> <span data-ttu-id="2f8f9-159">只读。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-159">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f8f9-160">关系</span><span class="sxs-lookup"><span data-stu-id="2f8f9-160">Relationships</span></span>

| <span data-ttu-id="2f8f9-161">关系</span><span class="sxs-lookup"><span data-stu-id="2f8f9-161">Relationship</span></span> | <span data-ttu-id="2f8f9-162">类型</span><span class="sxs-lookup"><span data-stu-id="2f8f9-162">Type</span></span> |<span data-ttu-id="2f8f9-163">说明</span><span class="sxs-lookup"><span data-stu-id="2f8f9-163">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2f8f9-164">installedApps</span><span class="sxs-lookup"><span data-stu-id="2f8f9-164">installedApps</span></span> | <span data-ttu-id="2f8f9-165">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f8f9-165">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="2f8f9-166">聊天中所有应用的集合。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-166">A collection of all the apps in the chat.</span></span> <span data-ttu-id="2f8f9-167">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-167">Nullable.</span></span> |
| <span data-ttu-id="2f8f9-168">members</span><span class="sxs-lookup"><span data-stu-id="2f8f9-168">members</span></span> | <span data-ttu-id="2f8f9-169">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f8f9-169">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="2f8f9-170">聊天中所有人员的集合。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-170">A collection of all people in the chat.</span></span> <span data-ttu-id="2f8f9-171">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-171">Nullable.</span></span> |
| <span data-ttu-id="2f8f9-172">messages</span><span class="sxs-lookup"><span data-stu-id="2f8f9-172">messages</span></span> | <span data-ttu-id="2f8f9-173">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f8f9-173">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="2f8f9-174">聊天中所有邮件的集合。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-174">A collection of all the messages in the chat.</span></span> <span data-ttu-id="2f8f9-175">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-175">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2f8f9-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f8f9-176">JSON representation</span></span>

<span data-ttu-id="2f8f9-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f8f9-177">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="2f8f9-178">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2f8f9-178">See also</span></span>

- [<span data-ttu-id="2f8f9-179">频道</span><span class="sxs-lookup"><span data-stu-id="2f8f9-179">channel</span></span>](channel.md)
- [<span data-ttu-id="2f8f9-180">chatMessage</span><span class="sxs-lookup"><span data-stu-id="2f8f9-180">chatMessage</span></span>](chatmessage.md)

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


