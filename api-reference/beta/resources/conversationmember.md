---
title: conversationMember 资源类型
description: 表示对话中的用户。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9e20a1aa0ef42f41a3fc300f804bb5477b5fe1cb
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633697"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="c1332-103">conversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="c1332-103">conversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1332-104">表示[聊天](chat.md)或[频道](channel.md)中的用户。</span><span class="sxs-lookup"><span data-stu-id="c1332-104">Represents a user in a [chat](chat.md) or a [channel](channel.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c1332-105">方法</span><span class="sxs-lookup"><span data-stu-id="c1332-105">Methods</span></span>

| <span data-ttu-id="c1332-106">方法</span><span class="sxs-lookup"><span data-stu-id="c1332-106">Method</span></span>       | <span data-ttu-id="c1332-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="c1332-107">Return Type</span></span>  |<span data-ttu-id="c1332-108">说明</span><span class="sxs-lookup"><span data-stu-id="c1332-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c1332-109">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="c1332-109">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="c1332-110">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c1332-110">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="c1332-111">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="c1332-111">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="c1332-112">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="c1332-112">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="c1332-113">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c1332-113">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="c1332-114">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="c1332-114">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="c1332-115">列出成员</span><span class="sxs-lookup"><span data-stu-id="c1332-115">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="c1332-116">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c1332-116">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="c1332-117">获取包含聊天或频道中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="c1332-117">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="c1332-118">获取成员</span><span class="sxs-lookup"><span data-stu-id="c1332-118">Get member groups</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="c1332-119">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c1332-119">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="c1332-120">获取聊天或频道中的一位用户。</span><span class="sxs-lookup"><span data-stu-id="c1332-120">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="c1332-121">添加成员</span><span class="sxs-lookup"><span data-stu-id="c1332-121">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="c1332-122">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c1332-122">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="c1332-123">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="c1332-123">Add a member to a class.</span></span>|
|[<span data-ttu-id="c1332-124">更新成员</span><span class="sxs-lookup"><span data-stu-id="c1332-124">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="c1332-125">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c1332-125">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="c1332-126">更新频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="c1332-126">Update a member in the channel.</span></span>|
|[<span data-ttu-id="c1332-127">删除成员</span><span class="sxs-lookup"><span data-stu-id="c1332-127">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="c1332-128">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c1332-128">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="c1332-129">删除频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="c1332-129">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="c1332-130">属性</span><span class="sxs-lookup"><span data-stu-id="c1332-130">Properties</span></span>

| <span data-ttu-id="c1332-131">属性</span><span class="sxs-lookup"><span data-stu-id="c1332-131">Property</span></span>   | <span data-ttu-id="c1332-132">类型</span><span class="sxs-lookup"><span data-stu-id="c1332-132">Type</span></span> |<span data-ttu-id="c1332-133">说明</span><span class="sxs-lookup"><span data-stu-id="c1332-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1332-134">id</span><span class="sxs-lookup"><span data-stu-id="c1332-134">id</span></span>|<span data-ttu-id="c1332-135">String</span><span class="sxs-lookup"><span data-stu-id="c1332-135">String</span></span>| <span data-ttu-id="c1332-136">只读。</span><span class="sxs-lookup"><span data-stu-id="c1332-136">Read-only.</span></span> <span data-ttu-id="c1332-137">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="c1332-137">Unique ID of the message.</span></span>|
|<span data-ttu-id="c1332-138">displayName</span><span class="sxs-lookup"><span data-stu-id="c1332-138">displayName</span></span>| <span data-ttu-id="c1332-139">string</span><span class="sxs-lookup"><span data-stu-id="c1332-139">string</span></span> | <span data-ttu-id="c1332-140">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c1332-140">The display name of the user.</span></span> |
|<span data-ttu-id="c1332-141">角色</span><span class="sxs-lookup"><span data-stu-id="c1332-141">roles</span></span>| <span data-ttu-id="c1332-142">string 集合</span><span class="sxs-lookup"><span data-stu-id="c1332-142">string collection</span></span> | <span data-ttu-id="c1332-143">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="c1332-143">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c1332-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1332-144">JSON representation</span></span>

<span data-ttu-id="c1332-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1332-145">The following is a JSON representation of the resource.</span></span>

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
