---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 Chatmessages 集合的集合。
author: clearab
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 83ab8428fb09a7a2dc0546dcebdf2f409d90d25a
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908488"
---
# <a name="chat-resource-type"></a><span data-ttu-id="3737f-103">聊天资源类型</span><span class="sxs-lookup"><span data-stu-id="3737f-103">chat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3737f-104">聊天是一个或多个参与者之间的[chatmessages 集合](chatmessage.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="3737f-104">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="3737f-105">参与者可以是用户或应用程序。</span><span class="sxs-lookup"><span data-stu-id="3737f-105">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="3737f-106">方法</span><span class="sxs-lookup"><span data-stu-id="3737f-106">Methods</span></span>

|  <span data-ttu-id="3737f-107">方法</span><span class="sxs-lookup"><span data-stu-id="3737f-107">Method</span></span>       |  <span data-ttu-id="3737f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3737f-108">Return Type</span></span>  | <span data-ttu-id="3737f-109">说明</span><span class="sxs-lookup"><span data-stu-id="3737f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3737f-110">列出聊天</span><span class="sxs-lookup"><span data-stu-id="3737f-110">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="3737f-111">[聊天](channel.md)收藏</span><span class="sxs-lookup"><span data-stu-id="3737f-111">[chat](channel.md) collection</span></span> | <span data-ttu-id="3737f-112">获取用户所属的聊天列表。</span><span class="sxs-lookup"><span data-stu-id="3737f-112">Get the list of chats a user is part of.</span></span>|
|[<span data-ttu-id="3737f-113">获取聊天</span><span class="sxs-lookup"><span data-stu-id="3737f-113">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="3737f-114">参与</span><span class="sxs-lookup"><span data-stu-id="3737f-114">chat</span></span>](channel.md) | <span data-ttu-id="3737f-115">读取聊天的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3737f-115">Read properties and relationships of the chat.</span></span>|
|[<span data-ttu-id="3737f-116">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="3737f-116">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="3737f-117">[conversationmember](conversationmember.md)集合</span><span class="sxs-lookup"><span data-stu-id="3737f-117">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="3737f-118">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="3737f-118">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="3737f-119">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="3737f-119">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="3737f-120">conversationmember</span><span class="sxs-lookup"><span data-stu-id="3737f-120">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="3737f-121">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="3737f-121">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="3737f-122">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="3737f-122">List messages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="3737f-123">chatMessage</span><span class="sxs-lookup"><span data-stu-id="3737f-123">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="3737f-124">获取一对一聊天或群组聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="3737f-124">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="3737f-125">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="3737f-125">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="3737f-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="3737f-126">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="3737f-127">获取聊天中的单个消息。</span><span class="sxs-lookup"><span data-stu-id="3737f-127">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="3737f-128">属性</span><span class="sxs-lookup"><span data-stu-id="3737f-128">Properties</span></span>

| <span data-ttu-id="3737f-129">属性</span><span class="sxs-lookup"><span data-stu-id="3737f-129">Property</span></span>   | <span data-ttu-id="3737f-130">类型</span><span class="sxs-lookup"><span data-stu-id="3737f-130">Type</span></span> |<span data-ttu-id="3737f-131">说明</span><span class="sxs-lookup"><span data-stu-id="3737f-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3737f-132">id</span><span class="sxs-lookup"><span data-stu-id="3737f-132">id</span></span>| <span data-ttu-id="3737f-133">String</span><span class="sxs-lookup"><span data-stu-id="3737f-133">String</span></span>| <span data-ttu-id="3737f-134">聊天的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3737f-134">The chat's unique identifier.</span></span> <span data-ttu-id="3737f-135">只读。</span><span class="sxs-lookup"><span data-stu-id="3737f-135">Read-only.</span></span>|
| <span data-ttu-id="3737f-136">topic</span><span class="sxs-lookup"><span data-stu-id="3737f-136">topic</span></span>| <span data-ttu-id="3737f-137">String</span><span class="sxs-lookup"><span data-stu-id="3737f-137">String</span></span>|  <span data-ttu-id="3737f-138">Optional聊天的主题或主题。</span><span class="sxs-lookup"><span data-stu-id="3737f-138">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="3737f-139">仅适用于组聊天。</span><span class="sxs-lookup"><span data-stu-id="3737f-139">Only available for group chats.</span></span>|
| <span data-ttu-id="3737f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3737f-140">createdDateTime</span></span>| <span data-ttu-id="3737f-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3737f-141">dateTimeOffset</span></span>|  <span data-ttu-id="3737f-142">聊天的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3737f-142">Date and time at which the chat was created.</span></span> <span data-ttu-id="3737f-143">只读。</span><span class="sxs-lookup"><span data-stu-id="3737f-143">Read-only.</span></span>|
| <span data-ttu-id="3737f-144">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3737f-144">lastUpdatedDateTime</span></span>| <span data-ttu-id="3737f-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3737f-145">dateTimeOffset</span></span>|  <span data-ttu-id="3737f-146">更新聊天的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3737f-146">Date and time at which the chat was updated.</span></span> <span data-ttu-id="3737f-147">只读。</span><span class="sxs-lookup"><span data-stu-id="3737f-147">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3737f-148">关系</span><span class="sxs-lookup"><span data-stu-id="3737f-148">Relationships</span></span>

| <span data-ttu-id="3737f-149">关系</span><span class="sxs-lookup"><span data-stu-id="3737f-149">Relationship</span></span> | <span data-ttu-id="3737f-150">类型</span><span class="sxs-lookup"><span data-stu-id="3737f-150">Type</span></span> |<span data-ttu-id="3737f-151">说明</span><span class="sxs-lookup"><span data-stu-id="3737f-151">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3737f-152">installedApps</span><span class="sxs-lookup"><span data-stu-id="3737f-152">installedApps</span></span> | <span data-ttu-id="3737f-153">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3737f-153">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="3737f-154">聊天中所有应用的集合。</span><span class="sxs-lookup"><span data-stu-id="3737f-154">A collection of all the apps in the chat.</span></span> <span data-ttu-id="3737f-155">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3737f-155">Nullable.</span></span> |
| <span data-ttu-id="3737f-156">members</span><span class="sxs-lookup"><span data-stu-id="3737f-156">members</span></span> | <span data-ttu-id="3737f-157">[conversationMember](conversationmember.md)集合</span><span class="sxs-lookup"><span data-stu-id="3737f-157">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="3737f-158">聊天中所有人员的集合。</span><span class="sxs-lookup"><span data-stu-id="3737f-158">A collection of all people in the chat.</span></span> <span data-ttu-id="3737f-159">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3737f-159">Nullable.</span></span> |
| <span data-ttu-id="3737f-160">messages</span><span class="sxs-lookup"><span data-stu-id="3737f-160">messages</span></span> | <span data-ttu-id="3737f-161">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3737f-161">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="3737f-162">聊天中所有邮件的集合。</span><span class="sxs-lookup"><span data-stu-id="3737f-162">A collection of all the messages in the chat.</span></span> <span data-ttu-id="3737f-163">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3737f-163">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3737f-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3737f-164">JSON representation</span></span>

<span data-ttu-id="3737f-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3737f-165">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="3737f-166">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3737f-166">See also</span></span>

- [<span data-ttu-id="3737f-167">频道</span><span class="sxs-lookup"><span data-stu-id="3737f-167">channel</span></span>](channel.md)
- [<span data-ttu-id="3737f-168">chatMessage</span><span class="sxs-lookup"><span data-stu-id="3737f-168">chatMessage</span></span>](chatmessage.md)

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
