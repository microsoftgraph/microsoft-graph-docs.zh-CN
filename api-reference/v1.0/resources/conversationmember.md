---
title: conversationMember 资源类型
description: 代表对话中的用户。
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 970e64ff358654aafee5b47a229a8425fdc69c9e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725832"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="ba94b-103">conversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba94b-103">conversationMember resource type</span></span>

<span data-ttu-id="ba94b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba94b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba94b-105">代表 [团队](team.md)中的用户。</span><span class="sxs-lookup"><span data-stu-id="ba94b-105">Represents a user in a [team](team.md).</span></span>
<span data-ttu-id="ba94b-106">另请参阅 [aadUserConversationMember](aaduserconversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="ba94b-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ba94b-107">Methods</span><span class="sxs-lookup"><span data-stu-id="ba94b-107">Methods</span></span>

| <span data-ttu-id="ba94b-108">方法</span><span class="sxs-lookup"><span data-stu-id="ba94b-108">Method</span></span>       | <span data-ttu-id="ba94b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ba94b-109">Return Type</span></span>  |<span data-ttu-id="ba94b-110">说明</span><span class="sxs-lookup"><span data-stu-id="ba94b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ba94b-111">列出成员</span><span class="sxs-lookup"><span data-stu-id="ba94b-111">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="ba94b-112">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ba94b-112">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="ba94b-113">获取包含聊天或频道中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="ba94b-113">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="ba94b-114">获取成员</span><span class="sxs-lookup"><span data-stu-id="ba94b-114">Get member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="ba94b-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ba94b-115">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="ba94b-116">获取聊天或频道中的一位用户。</span><span class="sxs-lookup"><span data-stu-id="ba94b-116">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="ba94b-117">添加成员</span><span class="sxs-lookup"><span data-stu-id="ba94b-117">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="ba94b-118">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ba94b-118">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="ba94b-119">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="ba94b-119">Add a member to a channel.</span></span>|
|[<span data-ttu-id="ba94b-120">更新成员</span><span class="sxs-lookup"><span data-stu-id="ba94b-120">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="ba94b-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ba94b-121">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="ba94b-122">更新频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="ba94b-122">Update a member in the channel.</span></span>|
|[<span data-ttu-id="ba94b-123">删除成员</span><span class="sxs-lookup"><span data-stu-id="ba94b-123">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="ba94b-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ba94b-124">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="ba94b-125">删除频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="ba94b-125">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="ba94b-126">属性</span><span class="sxs-lookup"><span data-stu-id="ba94b-126">Properties</span></span>

| <span data-ttu-id="ba94b-127">属性</span><span class="sxs-lookup"><span data-stu-id="ba94b-127">Property</span></span>   | <span data-ttu-id="ba94b-128">类型</span><span class="sxs-lookup"><span data-stu-id="ba94b-128">Type</span></span> |<span data-ttu-id="ba94b-129">说明</span><span class="sxs-lookup"><span data-stu-id="ba94b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba94b-130">id</span><span class="sxs-lookup"><span data-stu-id="ba94b-130">id</span></span>|<span data-ttu-id="ba94b-131">String</span><span class="sxs-lookup"><span data-stu-id="ba94b-131">String</span></span>| <span data-ttu-id="ba94b-132">只读。</span><span class="sxs-lookup"><span data-stu-id="ba94b-132">Read-only.</span></span> <span data-ttu-id="ba94b-133">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="ba94b-133">Unique ID of the user.</span></span>|
|<span data-ttu-id="ba94b-134">displayName</span><span class="sxs-lookup"><span data-stu-id="ba94b-134">displayName</span></span>| <span data-ttu-id="ba94b-135">string</span><span class="sxs-lookup"><span data-stu-id="ba94b-135">string</span></span> | <span data-ttu-id="ba94b-136">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ba94b-136">The display name of the user.</span></span> |
|<span data-ttu-id="ba94b-137">角色</span><span class="sxs-lookup"><span data-stu-id="ba94b-137">roles</span></span>| <span data-ttu-id="ba94b-138">string 集合</span><span class="sxs-lookup"><span data-stu-id="ba94b-138">string collection</span></span> | <span data-ttu-id="ba94b-139">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="ba94b-139">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ba94b-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba94b-140">JSON representation</span></span>

<span data-ttu-id="ba94b-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba94b-141">The following is a JSON representation of the resource.</span></span>

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

