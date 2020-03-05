---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 Chatmessages 集合的集合。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3fa6952640a1986d0139007ba863275aef2bc6aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507738"
---
# <a name="chat-resource-type"></a><span data-ttu-id="0ad54-103">聊天资源类型</span><span class="sxs-lookup"><span data-stu-id="0ad54-103">chat resource type</span></span>

<span data-ttu-id="0ad54-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0ad54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ad54-105">聊天是一个或多个参与者之间的[chatmessages 集合](chatmessage.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="0ad54-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="0ad54-106">参与者可以是用户或应用程序。</span><span class="sxs-lookup"><span data-stu-id="0ad54-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="0ad54-107">方法</span><span class="sxs-lookup"><span data-stu-id="0ad54-107">Methods</span></span>

|  <span data-ttu-id="0ad54-108">方法</span><span class="sxs-lookup"><span data-stu-id="0ad54-108">Method</span></span>       |  <span data-ttu-id="0ad54-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="0ad54-109">Return Type</span></span>  | <span data-ttu-id="0ad54-110">说明</span><span class="sxs-lookup"><span data-stu-id="0ad54-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0ad54-111">列出聊天</span><span class="sxs-lookup"><span data-stu-id="0ad54-111">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="0ad54-112">[聊天](channel.md)收藏</span><span class="sxs-lookup"><span data-stu-id="0ad54-112">[chat](channel.md) collection</span></span> | <span data-ttu-id="0ad54-113">获取用户所属的聊天列表。</span><span class="sxs-lookup"><span data-stu-id="0ad54-113">Get the list of chats a user is part of.</span></span>|
|[<span data-ttu-id="0ad54-114">获取聊天</span><span class="sxs-lookup"><span data-stu-id="0ad54-114">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="0ad54-115">参与</span><span class="sxs-lookup"><span data-stu-id="0ad54-115">chat</span></span>](channel.md) | <span data-ttu-id="0ad54-116">读取聊天的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0ad54-116">Read properties and relationships of the chat.</span></span>|
|[<span data-ttu-id="0ad54-117">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="0ad54-117">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="0ad54-118">[conversationmember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0ad54-118">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="0ad54-119">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="0ad54-119">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="0ad54-120">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="0ad54-120">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="0ad54-121">conversationmember</span><span class="sxs-lookup"><span data-stu-id="0ad54-121">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="0ad54-122">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="0ad54-122">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="0ad54-123">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="0ad54-123">List messages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="0ad54-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0ad54-124">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="0ad54-125">获取一对一聊天或群组聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="0ad54-125">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="0ad54-126">获取聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="0ad54-126">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="0ad54-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0ad54-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="0ad54-128">获取聊天中的单个消息。</span><span class="sxs-lookup"><span data-stu-id="0ad54-128">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="0ad54-129">属性</span><span class="sxs-lookup"><span data-stu-id="0ad54-129">Properties</span></span>

| <span data-ttu-id="0ad54-130">属性</span><span class="sxs-lookup"><span data-stu-id="0ad54-130">Property</span></span>   | <span data-ttu-id="0ad54-131">类型</span><span class="sxs-lookup"><span data-stu-id="0ad54-131">Type</span></span> |<span data-ttu-id="0ad54-132">说明</span><span class="sxs-lookup"><span data-stu-id="0ad54-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0ad54-133">id</span><span class="sxs-lookup"><span data-stu-id="0ad54-133">id</span></span>| <span data-ttu-id="0ad54-134">String</span><span class="sxs-lookup"><span data-stu-id="0ad54-134">String</span></span>| <span data-ttu-id="0ad54-135">聊天的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0ad54-135">The chat's unique identifier.</span></span> <span data-ttu-id="0ad54-136">只读。</span><span class="sxs-lookup"><span data-stu-id="0ad54-136">Read-only.</span></span>|
| <span data-ttu-id="0ad54-137">topic</span><span class="sxs-lookup"><span data-stu-id="0ad54-137">topic</span></span>| <span data-ttu-id="0ad54-138">String</span><span class="sxs-lookup"><span data-stu-id="0ad54-138">String</span></span>|  <span data-ttu-id="0ad54-139">Optional聊天的主题或主题。</span><span class="sxs-lookup"><span data-stu-id="0ad54-139">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="0ad54-140">仅适用于组聊天。</span><span class="sxs-lookup"><span data-stu-id="0ad54-140">Only available for group chats.</span></span>|
| <span data-ttu-id="0ad54-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ad54-141">createdDateTime</span></span>| <span data-ttu-id="0ad54-142">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ad54-142">dateTimeOffset</span></span>|  <span data-ttu-id="0ad54-143">聊天的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0ad54-143">Date and time at which the chat was created.</span></span> <span data-ttu-id="0ad54-144">只读。</span><span class="sxs-lookup"><span data-stu-id="0ad54-144">Read-only.</span></span>|
| <span data-ttu-id="0ad54-145">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ad54-145">lastUpdatedDateTime</span></span>| <span data-ttu-id="0ad54-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ad54-146">dateTimeOffset</span></span>|  <span data-ttu-id="0ad54-147">更新聊天的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0ad54-147">Date and time at which the chat was updated.</span></span> <span data-ttu-id="0ad54-148">只读。</span><span class="sxs-lookup"><span data-stu-id="0ad54-148">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ad54-149">关系</span><span class="sxs-lookup"><span data-stu-id="0ad54-149">Relationships</span></span>

| <span data-ttu-id="0ad54-150">关系</span><span class="sxs-lookup"><span data-stu-id="0ad54-150">Relationship</span></span> | <span data-ttu-id="0ad54-151">类型</span><span class="sxs-lookup"><span data-stu-id="0ad54-151">Type</span></span> |<span data-ttu-id="0ad54-152">说明</span><span class="sxs-lookup"><span data-stu-id="0ad54-152">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0ad54-153">installedApps</span><span class="sxs-lookup"><span data-stu-id="0ad54-153">installedApps</span></span> | <span data-ttu-id="0ad54-154">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0ad54-154">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="0ad54-155">聊天中所有应用的集合。</span><span class="sxs-lookup"><span data-stu-id="0ad54-155">A collection of all the apps in the chat.</span></span> <span data-ttu-id="0ad54-156">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="0ad54-156">Nullable.</span></span> |
| <span data-ttu-id="0ad54-157">members</span><span class="sxs-lookup"><span data-stu-id="0ad54-157">members</span></span> | <span data-ttu-id="0ad54-158">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0ad54-158">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="0ad54-159">聊天中所有人员的集合。</span><span class="sxs-lookup"><span data-stu-id="0ad54-159">A collection of all people in the chat.</span></span> <span data-ttu-id="0ad54-160">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="0ad54-160">Nullable.</span></span> |
| <span data-ttu-id="0ad54-161">messages</span><span class="sxs-lookup"><span data-stu-id="0ad54-161">messages</span></span> | <span data-ttu-id="0ad54-162">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0ad54-162">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="0ad54-163">聊天中所有邮件的集合。</span><span class="sxs-lookup"><span data-stu-id="0ad54-163">A collection of all the messages in the chat.</span></span> <span data-ttu-id="0ad54-164">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="0ad54-164">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0ad54-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ad54-165">JSON representation</span></span>

<span data-ttu-id="0ad54-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ad54-166">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="0ad54-167">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0ad54-167">See also</span></span>

- [<span data-ttu-id="0ad54-168">频道</span><span class="sxs-lookup"><span data-stu-id="0ad54-168">channel</span></span>](channel.md)
- [<span data-ttu-id="0ad54-169">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0ad54-169">chatMessage</span></span>](chatmessage.md)

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
