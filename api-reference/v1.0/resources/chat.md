---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 Chatmessages 集合的集合。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7f9cc43442e077dfe245fa8422b954859bf1c569
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564068"
---
# <a name="chat-resource-type"></a><span data-ttu-id="75f1e-103">聊天资源类型</span><span class="sxs-lookup"><span data-stu-id="75f1e-103">chat resource type</span></span>

<span data-ttu-id="75f1e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75f1e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75f1e-105">聊天是一个或多个参与者之间的 [chatmessages 集合](chatmessage.md) 的集合。</span><span class="sxs-lookup"><span data-stu-id="75f1e-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="75f1e-106">参与者可以是用户或应用程序。</span><span class="sxs-lookup"><span data-stu-id="75f1e-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="75f1e-107">方法</span><span class="sxs-lookup"><span data-stu-id="75f1e-107">Methods</span></span>

|  <span data-ttu-id="75f1e-108">方法</span><span class="sxs-lookup"><span data-stu-id="75f1e-108">Method</span></span>       |  <span data-ttu-id="75f1e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="75f1e-109">Return Type</span></span>  | <span data-ttu-id="75f1e-110">说明</span><span class="sxs-lookup"><span data-stu-id="75f1e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="75f1e-111">在用户和应用之间获取聊天</span><span class="sxs-lookup"><span data-stu-id="75f1e-111">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="75f1e-112">聊天</span><span class="sxs-lookup"><span data-stu-id="75f1e-112">chat</span></span>](chat.md)| <span data-ttu-id="75f1e-113">在用户和应用之间获取一对一聊天</span><span class="sxs-lookup"><span data-stu-id="75f1e-113">Get one-on-one chat between user and the app</span></span> | 

><span data-ttu-id="75f1e-114">**注意：** 使用应用程序权限时，请务必了解如何获取聊天 ID。</span><span class="sxs-lookup"><span data-stu-id="75f1e-114">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="75f1e-115">由于不支持列出具有应用程序权限的聊天，因此并非所有方案都可行。</span><span class="sxs-lookup"><span data-stu-id="75f1e-115">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="75f1e-116">可以获取具有委派权限的聊天 Id，也可以通过应用程序权限获取 [/chats/getAllMessages 的更改通知](../api/subscription-post-subscriptions.md) 。</span><span class="sxs-lookup"><span data-stu-id="75f1e-116">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="75f1e-117">属性</span><span class="sxs-lookup"><span data-stu-id="75f1e-117">Properties</span></span>

| <span data-ttu-id="75f1e-118">属性</span><span class="sxs-lookup"><span data-stu-id="75f1e-118">Property</span></span>   | <span data-ttu-id="75f1e-119">类型</span><span class="sxs-lookup"><span data-stu-id="75f1e-119">Type</span></span> |<span data-ttu-id="75f1e-120">说明</span><span class="sxs-lookup"><span data-stu-id="75f1e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="75f1e-121">id</span><span class="sxs-lookup"><span data-stu-id="75f1e-121">id</span></span>| <span data-ttu-id="75f1e-122">String</span><span class="sxs-lookup"><span data-stu-id="75f1e-122">String</span></span>| <span data-ttu-id="75f1e-123">聊天的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="75f1e-123">The chat's unique identifier.</span></span> <span data-ttu-id="75f1e-124">只读。</span><span class="sxs-lookup"><span data-stu-id="75f1e-124">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="75f1e-125">关系</span><span class="sxs-lookup"><span data-stu-id="75f1e-125">Relationships</span></span>

| <span data-ttu-id="75f1e-126">关系</span><span class="sxs-lookup"><span data-stu-id="75f1e-126">Relationship</span></span> | <span data-ttu-id="75f1e-127">类型</span><span class="sxs-lookup"><span data-stu-id="75f1e-127">Type</span></span> |<span data-ttu-id="75f1e-128">说明</span><span class="sxs-lookup"><span data-stu-id="75f1e-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="75f1e-129">messages</span><span class="sxs-lookup"><span data-stu-id="75f1e-129">messages</span></span> | <span data-ttu-id="75f1e-130">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75f1e-130">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="75f1e-131">聊天中所有邮件的集合。</span><span class="sxs-lookup"><span data-stu-id="75f1e-131">A collection of all the messages in the chat.</span></span> <span data-ttu-id="75f1e-132">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="75f1e-132">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="75f1e-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="75f1e-133">JSON representation</span></span>

<span data-ttu-id="75f1e-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75f1e-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chat"
}-->

```json
{
  "id": "string (identifier)",
}
```

## <a name="see-also"></a><span data-ttu-id="75f1e-135">另请参阅</span><span class="sxs-lookup"><span data-stu-id="75f1e-135">See also</span></span>

- [<span data-ttu-id="75f1e-136">频道</span><span class="sxs-lookup"><span data-stu-id="75f1e-136">channel</span></span>](channel.md)
- [<span data-ttu-id="75f1e-137">chatMessage</span><span class="sxs-lookup"><span data-stu-id="75f1e-137">chatMessage</span></span>](chatmessage.md)

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


