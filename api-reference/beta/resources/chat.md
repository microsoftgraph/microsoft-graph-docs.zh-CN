---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 Chatmessages 集合的集合。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e95adb1c00b88fcc2649acb669ee693caef6cccf
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778656"
---
# <a name="chat-resource-type"></a><span data-ttu-id="070f9-103">聊天资源类型</span><span class="sxs-lookup"><span data-stu-id="070f9-103">chat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="070f9-104">聊天是一个或多个参与者之间的[chatmessages 集合](chatmessage.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="070f9-104">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="070f9-105">参与者可以是用户或应用程序。</span><span class="sxs-lookup"><span data-stu-id="070f9-105">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="070f9-106">方法</span><span class="sxs-lookup"><span data-stu-id="070f9-106">Methods</span></span>

|  <span data-ttu-id="070f9-107">方法</span><span class="sxs-lookup"><span data-stu-id="070f9-107">Method</span></span>       |  <span data-ttu-id="070f9-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="070f9-108">Return Type</span></span>  | <span data-ttu-id="070f9-109">说明</span><span class="sxs-lookup"><span data-stu-id="070f9-109">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="070f9-110">列出聊天</span><span class="sxs-lookup"><span data-stu-id="070f9-110">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="070f9-111">[聊天](channel.md)收藏</span><span class="sxs-lookup"><span data-stu-id="070f9-111">[chat](channel.md) collection</span></span> | <span data-ttu-id="070f9-112">获取用户所属的聊天列表。</span><span class="sxs-lookup"><span data-stu-id="070f9-112">Get the list of chats a user is part of.</span></span>|
|[<span data-ttu-id="070f9-113">获取聊天</span><span class="sxs-lookup"><span data-stu-id="070f9-113">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="070f9-114">参与</span><span class="sxs-lookup"><span data-stu-id="070f9-114">chat</span></span>](channel.md) | <span data-ttu-id="070f9-115">读取聊天的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="070f9-115">Read properties and relationships of the chat.</span></span>|
|[<span data-ttu-id="070f9-116">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="070f9-116">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="070f9-117">[conversationmember](conversationmember.md)集合</span><span class="sxs-lookup"><span data-stu-id="070f9-117">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="070f9-118">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="070f9-118">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="070f9-119">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="070f9-119">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="070f9-120">conversationmember</span><span class="sxs-lookup"><span data-stu-id="070f9-120">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="070f9-121">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="070f9-121">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="070f9-122">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="070f9-122">List messages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="070f9-123">chatMessage</span><span class="sxs-lookup"><span data-stu-id="070f9-123">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="070f9-124">获取一对一聊天或群组聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="070f9-124">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="070f9-125">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="070f9-125">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="070f9-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="070f9-126">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="070f9-127">获取聊天中的单个消息。</span><span class="sxs-lookup"><span data-stu-id="070f9-127">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="070f9-128">属性</span><span class="sxs-lookup"><span data-stu-id="070f9-128">Properties</span></span>

| <span data-ttu-id="070f9-129">属性</span><span class="sxs-lookup"><span data-stu-id="070f9-129">Property</span></span>     | <span data-ttu-id="070f9-130">类型</span><span class="sxs-lookup"><span data-stu-id="070f9-130">Type</span></span>   |<span data-ttu-id="070f9-131">说明</span><span class="sxs-lookup"><span data-stu-id="070f9-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="070f9-132">id</span><span class="sxs-lookup"><span data-stu-id="070f9-132">id</span></span>| <span data-ttu-id="070f9-133">String</span><span class="sxs-lookup"><span data-stu-id="070f9-133">String</span></span>| <span data-ttu-id="070f9-134">聊天的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="070f9-134">The chat's unique identifier.</span></span> <span data-ttu-id="070f9-135">只读。</span><span class="sxs-lookup"><span data-stu-id="070f9-135">Read-only.</span></span>|
| <span data-ttu-id="070f9-136">topic</span><span class="sxs-lookup"><span data-stu-id="070f9-136">topic</span></span>| <span data-ttu-id="070f9-137">String</span><span class="sxs-lookup"><span data-stu-id="070f9-137">String</span></span>|  <span data-ttu-id="070f9-138">Optional聊天的主题或主题。</span><span class="sxs-lookup"><span data-stu-id="070f9-138">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="070f9-139">仅适用于组聊天。</span><span class="sxs-lookup"><span data-stu-id="070f9-139">Only available for group chats.</span></span>|
| <span data-ttu-id="070f9-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="070f9-140">createdDateTime</span></span>| <span data-ttu-id="070f9-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="070f9-141">dateTimeOffset</span></span>|  <span data-ttu-id="070f9-142">聊天的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="070f9-142">Date and time at which the chat was created.</span></span> <span data-ttu-id="070f9-143">只读。</span><span class="sxs-lookup"><span data-stu-id="070f9-143">Read-only.</span></span>|
| <span data-ttu-id="070f9-144">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="070f9-144">lastUpdatedDateTime</span></span>| <span data-ttu-id="070f9-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="070f9-145">dateTimeOffset</span></span>|  <span data-ttu-id="070f9-146">更新聊天的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="070f9-146">Date and time at which the chat was updated.</span></span> <span data-ttu-id="070f9-147">只读。</span><span class="sxs-lookup"><span data-stu-id="070f9-147">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="070f9-148">关系</span><span class="sxs-lookup"><span data-stu-id="070f9-148">Relationships</span></span>
| <span data-ttu-id="070f9-149">关系</span><span class="sxs-lookup"><span data-stu-id="070f9-149">Relationship</span></span> | <span data-ttu-id="070f9-150">类型</span><span class="sxs-lookup"><span data-stu-id="070f9-150">Type</span></span>   |<span data-ttu-id="070f9-151">说明</span><span class="sxs-lookup"><span data-stu-id="070f9-151">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="070f9-152">成员</span><span class="sxs-lookup"><span data-stu-id="070f9-152">members</span></span> | <span data-ttu-id="070f9-153">[conversationMember](conversationmember.md)集合</span><span class="sxs-lookup"><span data-stu-id="070f9-153">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="070f9-154">聊天中所有人员的集合。</span><span class="sxs-lookup"><span data-stu-id="070f9-154">A collection of all people in the chat.</span></span> <span data-ttu-id="070f9-155">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="070f9-155">Nullable.</span></span> |
| <span data-ttu-id="070f9-156">messages</span><span class="sxs-lookup"><span data-stu-id="070f9-156">messages</span></span> | <span data-ttu-id="070f9-157">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="070f9-157">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="070f9-158">聊天中所有邮件的集合。</span><span class="sxs-lookup"><span data-stu-id="070f9-158">A collection of all the messages in the chat.</span></span> <span data-ttu-id="070f9-159">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="070f9-159">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="070f9-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="070f9-160">JSON representation</span></span>

<span data-ttu-id="070f9-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="070f9-161">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="070f9-162">另请参阅</span><span class="sxs-lookup"><span data-stu-id="070f9-162">See also</span></span>

- [<span data-ttu-id="070f9-163">频道</span><span class="sxs-lookup"><span data-stu-id="070f9-163">channel</span></span>](channel.md)
- [<span data-ttu-id="070f9-164">chatMessage</span><span class="sxs-lookup"><span data-stu-id="070f9-164">chatMessage</span></span>](chatmessage.md)

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
