---
title: conversationMember 资源类型
description: 表示对话中的用户。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d9e50c0ca27843461b41b4d86f29ce3604788866
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016763"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="8c1b3-103">conversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c1b3-103">conversationMember resource type</span></span>

<span data-ttu-id="8c1b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c1b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c1b3-105">表示[聊天](chat.md)或[频道](channel.md)中的用户。</span><span class="sxs-lookup"><span data-stu-id="8c1b3-105">Represents a user in a [chat](chat.md) or a [channel](channel.md).</span></span>
<span data-ttu-id="8c1b3-106">另请参阅 [aadUserConversationMember](aaduserconversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="8c1b3-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8c1b3-107">方法</span><span class="sxs-lookup"><span data-stu-id="8c1b3-107">Methods</span></span>

| <span data-ttu-id="8c1b3-108">方法</span><span class="sxs-lookup"><span data-stu-id="8c1b3-108">Method</span></span>       | <span data-ttu-id="8c1b3-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8c1b3-109">Return Type</span></span>  |<span data-ttu-id="8c1b3-110">说明</span><span class="sxs-lookup"><span data-stu-id="8c1b3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8c1b3-111">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="8c1b3-111">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="8c1b3-112">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8c1b3-112">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="8c1b3-113">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="8c1b3-113">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="8c1b3-114">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="8c1b3-114">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="8c1b3-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="8c1b3-115">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="8c1b3-116">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="8c1b3-116">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="8c1b3-117">列出成员</span><span class="sxs-lookup"><span data-stu-id="8c1b3-117">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="8c1b3-118">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8c1b3-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="8c1b3-119">获取包含聊天或频道中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="8c1b3-119">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="8c1b3-120">获取成员</span><span class="sxs-lookup"><span data-stu-id="8c1b3-120">Get member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="8c1b3-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="8c1b3-121">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="8c1b3-122">获取聊天或频道中的一位用户。</span><span class="sxs-lookup"><span data-stu-id="8c1b3-122">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="8c1b3-123">添加成员</span><span class="sxs-lookup"><span data-stu-id="8c1b3-123">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="8c1b3-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="8c1b3-124">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="8c1b3-125">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="8c1b3-125">Add a member to a channel.</span></span>|
|[<span data-ttu-id="8c1b3-126">更新成员</span><span class="sxs-lookup"><span data-stu-id="8c1b3-126">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="8c1b3-127">conversationMember</span><span class="sxs-lookup"><span data-stu-id="8c1b3-127">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="8c1b3-128">更新频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="8c1b3-128">Update a member in the channel.</span></span>|
|[<span data-ttu-id="8c1b3-129">删除成员</span><span class="sxs-lookup"><span data-stu-id="8c1b3-129">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="8c1b3-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="8c1b3-130">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="8c1b3-131">删除频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="8c1b3-131">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="8c1b3-132">属性</span><span class="sxs-lookup"><span data-stu-id="8c1b3-132">Properties</span></span>

| <span data-ttu-id="8c1b3-133">属性</span><span class="sxs-lookup"><span data-stu-id="8c1b3-133">Property</span></span>   | <span data-ttu-id="8c1b3-134">类型</span><span class="sxs-lookup"><span data-stu-id="8c1b3-134">Type</span></span> |<span data-ttu-id="8c1b3-135">说明</span><span class="sxs-lookup"><span data-stu-id="8c1b3-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c1b3-136">id</span><span class="sxs-lookup"><span data-stu-id="8c1b3-136">id</span></span>|<span data-ttu-id="8c1b3-137">String</span><span class="sxs-lookup"><span data-stu-id="8c1b3-137">String</span></span>| <span data-ttu-id="8c1b3-138">只读。</span><span class="sxs-lookup"><span data-stu-id="8c1b3-138">Read-only.</span></span> <span data-ttu-id="8c1b3-139">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="8c1b3-139">Unique ID of the user.</span></span>|
|<span data-ttu-id="8c1b3-140">displayName</span><span class="sxs-lookup"><span data-stu-id="8c1b3-140">displayName</span></span>| <span data-ttu-id="8c1b3-141">string</span><span class="sxs-lookup"><span data-stu-id="8c1b3-141">string</span></span> | <span data-ttu-id="8c1b3-142">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="8c1b3-142">The display name of the user.</span></span> |
|<span data-ttu-id="8c1b3-143">角色</span><span class="sxs-lookup"><span data-stu-id="8c1b3-143">roles</span></span>| <span data-ttu-id="8c1b3-144">string 集合</span><span class="sxs-lookup"><span data-stu-id="8c1b3-144">string collection</span></span> | <span data-ttu-id="8c1b3-145">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="8c1b3-145">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8c1b3-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c1b3-146">JSON representation</span></span>

<span data-ttu-id="8c1b3-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c1b3-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conversationMember",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "roles": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


