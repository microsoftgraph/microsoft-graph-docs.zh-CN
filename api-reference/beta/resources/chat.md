---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 chatmessages 集合的集合。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1091021235a50d3dfa237467e319da9b131b7a72
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339711"
---
# <a name="chat-resource-type"></a><span data-ttu-id="89d14-103">聊天资源类型</span><span class="sxs-lookup"><span data-stu-id="89d14-103">chat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89d14-104">聊天是一个或多个参与者之间的[chatmessages 集合](chatmessage.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="89d14-104">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="89d14-105">参与者可以是用户或应用程序。</span><span class="sxs-lookup"><span data-stu-id="89d14-105">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="89d14-106">方法</span><span class="sxs-lookup"><span data-stu-id="89d14-106">Methods</span></span>

|  <span data-ttu-id="89d14-107">方法</span><span class="sxs-lookup"><span data-stu-id="89d14-107">Method</span></span>       |  <span data-ttu-id="89d14-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="89d14-108">Return Type</span></span>  | <span data-ttu-id="89d14-109">说明</span><span class="sxs-lookup"><span data-stu-id="89d14-109">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="89d14-110">列出聊天</span><span class="sxs-lookup"><span data-stu-id="89d14-110">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="89d14-111">[聊天](channel.md)收藏</span><span class="sxs-lookup"><span data-stu-id="89d14-111">[chat](channel.md) collection</span></span> | <span data-ttu-id="89d14-112">获取用户所属的聊天列表。</span><span class="sxs-lookup"><span data-stu-id="89d14-112">Get the list of chats a user is part of.</span></span>|
|[<span data-ttu-id="89d14-113">获取聊天</span><span class="sxs-lookup"><span data-stu-id="89d14-113">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="89d14-114">参与</span><span class="sxs-lookup"><span data-stu-id="89d14-114">chat</span></span>](channel.md) | <span data-ttu-id="89d14-115">读取聊天的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="89d14-115">Read properties and relationships of the chat.</span></span>|
|[<span data-ttu-id="89d14-116">列出聊天中的邮件</span><span class="sxs-lookup"><span data-stu-id="89d14-116">List messages in a chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="89d14-117">chatMessage</span><span class="sxs-lookup"><span data-stu-id="89d14-117">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="89d14-118">获取1:1 或组聊天中的邮件。</span><span class="sxs-lookup"><span data-stu-id="89d14-118">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="89d14-119">在聊天中获取邮件</span><span class="sxs-lookup"><span data-stu-id="89d14-119">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="89d14-120">chatMessage</span><span class="sxs-lookup"><span data-stu-id="89d14-120">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="89d14-121">在聊天中获取一封邮件。</span><span class="sxs-lookup"><span data-stu-id="89d14-121">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="89d14-122">属性</span><span class="sxs-lookup"><span data-stu-id="89d14-122">Properties</span></span>

| <span data-ttu-id="89d14-123">属性</span><span class="sxs-lookup"><span data-stu-id="89d14-123">Property</span></span>     | <span data-ttu-id="89d14-124">类型</span><span class="sxs-lookup"><span data-stu-id="89d14-124">Type</span></span>   |<span data-ttu-id="89d14-125">说明</span><span class="sxs-lookup"><span data-stu-id="89d14-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="89d14-126">id</span><span class="sxs-lookup"><span data-stu-id="89d14-126">id</span></span>| <span data-ttu-id="89d14-127">String</span><span class="sxs-lookup"><span data-stu-id="89d14-127">String</span></span>| <span data-ttu-id="89d14-128">聊天的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="89d14-128">The chat's unique identifier.</span></span> <span data-ttu-id="89d14-129">只读。</span><span class="sxs-lookup"><span data-stu-id="89d14-129">Read-only.</span></span>|
| <span data-ttu-id="89d14-130">topic</span><span class="sxs-lookup"><span data-stu-id="89d14-130">topic</span></span>| <span data-ttu-id="89d14-131">String</span><span class="sxs-lookup"><span data-stu-id="89d14-131">String</span></span>|  <span data-ttu-id="89d14-132">Optional聊天的主题或主题。</span><span class="sxs-lookup"><span data-stu-id="89d14-132">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="89d14-133">仅适用于组聊天。</span><span class="sxs-lookup"><span data-stu-id="89d14-133">Only available for group chats.</span></span>|
| <span data-ttu-id="89d14-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89d14-134">createdDateTime</span></span>| <span data-ttu-id="89d14-135">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89d14-135">dateTimeOffset</span></span>|  <span data-ttu-id="89d14-136">聊天的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="89d14-136">Date and time at which the chat was created.</span></span> <span data-ttu-id="89d14-137">只读。</span><span class="sxs-lookup"><span data-stu-id="89d14-137">Read-only.</span></span>|
| <span data-ttu-id="89d14-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="89d14-138">lastUpdatedDateTime</span></span>| <span data-ttu-id="89d14-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89d14-139">dateTimeOffset</span></span>|  <span data-ttu-id="89d14-140">更新聊天的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="89d14-140">Date and time at which the chat was updated.</span></span> <span data-ttu-id="89d14-141">只读。</span><span class="sxs-lookup"><span data-stu-id="89d14-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89d14-142">关系</span><span class="sxs-lookup"><span data-stu-id="89d14-142">Relationships</span></span>
| <span data-ttu-id="89d14-143">关系</span><span class="sxs-lookup"><span data-stu-id="89d14-143">Relationship</span></span> | <span data-ttu-id="89d14-144">类型</span><span class="sxs-lookup"><span data-stu-id="89d14-144">Type</span></span>   |<span data-ttu-id="89d14-145">说明</span><span class="sxs-lookup"><span data-stu-id="89d14-145">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="89d14-146">messages</span><span class="sxs-lookup"><span data-stu-id="89d14-146">messages</span></span> | <span data-ttu-id="89d14-147">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89d14-147">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="89d14-148">聊天中所有邮件的集合。</span><span class="sxs-lookup"><span data-stu-id="89d14-148">A collection of all the messages in the chat.</span></span> <span data-ttu-id="89d14-149">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="89d14-149">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="89d14-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89d14-150">JSON representation</span></span>

<span data-ttu-id="89d14-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89d14-151">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="89d14-152">另请参阅</span><span class="sxs-lookup"><span data-stu-id="89d14-152">See also</span></span>

- [<span data-ttu-id="89d14-153">频道</span><span class="sxs-lookup"><span data-stu-id="89d14-153">channel</span></span>](channel.md)
- [<span data-ttu-id="89d14-154">chatMessage</span><span class="sxs-lookup"><span data-stu-id="89d14-154">chatMessage</span></span>](chatmessage.md)

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
