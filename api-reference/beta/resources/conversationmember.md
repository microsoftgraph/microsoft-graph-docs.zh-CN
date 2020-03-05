---
title: conversationMember 资源类型
description: 表示对话中的用户。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 796bbe9f64342f97a9ae18363fdc01dc1712d015
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507399"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="eb685-103">conversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb685-103">conversationMember resource type</span></span>

<span data-ttu-id="eb685-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="eb685-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb685-105">表示[聊天](chat.md)或[频道](channel.md)中的用户。</span><span class="sxs-lookup"><span data-stu-id="eb685-105">Represents a user in a [chat](chat.md) or a [channel](channel.md).</span></span>

## <a name="methods"></a><span data-ttu-id="eb685-106">方法</span><span class="sxs-lookup"><span data-stu-id="eb685-106">Methods</span></span>

| <span data-ttu-id="eb685-107">方法</span><span class="sxs-lookup"><span data-stu-id="eb685-107">Method</span></span>       | <span data-ttu-id="eb685-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="eb685-108">Return Type</span></span>  |<span data-ttu-id="eb685-109">说明</span><span class="sxs-lookup"><span data-stu-id="eb685-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eb685-110">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="eb685-110">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="eb685-111">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb685-111">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="eb685-112">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="eb685-112">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="eb685-113">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="eb685-113">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="eb685-114">conversationMember</span><span class="sxs-lookup"><span data-stu-id="eb685-114">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="eb685-115">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="eb685-115">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="eb685-116">列出成员</span><span class="sxs-lookup"><span data-stu-id="eb685-116">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="eb685-117">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb685-117">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="eb685-118">获取包含聊天或频道中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="eb685-118">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="eb685-119">获取成员</span><span class="sxs-lookup"><span data-stu-id="eb685-119">Get member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="eb685-120">conversationMember</span><span class="sxs-lookup"><span data-stu-id="eb685-120">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="eb685-121">获取聊天或频道中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="eb685-121">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="eb685-122">添加成员</span><span class="sxs-lookup"><span data-stu-id="eb685-122">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="eb685-123">conversationMember</span><span class="sxs-lookup"><span data-stu-id="eb685-123">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="eb685-124">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="eb685-124">Add a member to a channel.</span></span>|
|[<span data-ttu-id="eb685-125">更新成员</span><span class="sxs-lookup"><span data-stu-id="eb685-125">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="eb685-126">conversationMember</span><span class="sxs-lookup"><span data-stu-id="eb685-126">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="eb685-127">更新频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="eb685-127">Update a member in the channel.</span></span>|
|[<span data-ttu-id="eb685-128">删除成员</span><span class="sxs-lookup"><span data-stu-id="eb685-128">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="eb685-129">conversationMember</span><span class="sxs-lookup"><span data-stu-id="eb685-129">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="eb685-130">删除频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="eb685-130">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="eb685-131">属性</span><span class="sxs-lookup"><span data-stu-id="eb685-131">Properties</span></span>

| <span data-ttu-id="eb685-132">属性</span><span class="sxs-lookup"><span data-stu-id="eb685-132">Property</span></span>   | <span data-ttu-id="eb685-133">类型</span><span class="sxs-lookup"><span data-stu-id="eb685-133">Type</span></span> |<span data-ttu-id="eb685-134">说明</span><span class="sxs-lookup"><span data-stu-id="eb685-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb685-135">id</span><span class="sxs-lookup"><span data-stu-id="eb685-135">id</span></span>|<span data-ttu-id="eb685-136">String</span><span class="sxs-lookup"><span data-stu-id="eb685-136">String</span></span>| <span data-ttu-id="eb685-137">只读。</span><span class="sxs-lookup"><span data-stu-id="eb685-137">Read-only.</span></span> <span data-ttu-id="eb685-138">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="eb685-138">Unique ID of the user.</span></span>|
|<span data-ttu-id="eb685-139">displayName</span><span class="sxs-lookup"><span data-stu-id="eb685-139">displayName</span></span>| <span data-ttu-id="eb685-140">string</span><span class="sxs-lookup"><span data-stu-id="eb685-140">string</span></span> | <span data-ttu-id="eb685-141">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="eb685-141">The display name of the user.</span></span> |
|<span data-ttu-id="eb685-142">角色</span><span class="sxs-lookup"><span data-stu-id="eb685-142">roles</span></span>| <span data-ttu-id="eb685-143">string 集合</span><span class="sxs-lookup"><span data-stu-id="eb685-143">string collection</span></span> | <span data-ttu-id="eb685-144">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="eb685-144">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eb685-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb685-145">JSON representation</span></span>

<span data-ttu-id="eb685-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb685-146">The following is a JSON representation of the resource.</span></span>

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
