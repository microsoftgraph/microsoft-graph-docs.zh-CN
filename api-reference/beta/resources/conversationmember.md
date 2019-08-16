---
title: conversationMember 资源类型
description: 表示对话中的用户。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca5115922dfb40239b8ca290a39f3c5953d4e4ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973973"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="5e617-103">conversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e617-103">conversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e617-104">表示[聊天](chat.md)中的用户。</span><span class="sxs-lookup"><span data-stu-id="5e617-104">Represents a user in a [chat](chat.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5e617-105">方法</span><span class="sxs-lookup"><span data-stu-id="5e617-105">Methods</span></span>

| <span data-ttu-id="5e617-106">方法</span><span class="sxs-lookup"><span data-stu-id="5e617-106">Method</span></span>       | <span data-ttu-id="5e617-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="5e617-107">Return Type</span></span>  |<span data-ttu-id="5e617-108">说明</span><span class="sxs-lookup"><span data-stu-id="5e617-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5e617-109">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="5e617-109">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="5e617-110">[conversationmember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5e617-110">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="5e617-111">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="5e617-111">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="5e617-112">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="5e617-112">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="5e617-113">conversationmember</span><span class="sxs-lookup"><span data-stu-id="5e617-113">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="5e617-114">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="5e617-114">Get a single user in the chat.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e617-115">属性</span><span class="sxs-lookup"><span data-stu-id="5e617-115">Properties</span></span>

| <span data-ttu-id="5e617-116">属性</span><span class="sxs-lookup"><span data-stu-id="5e617-116">Property</span></span>     | <span data-ttu-id="5e617-117">类型</span><span class="sxs-lookup"><span data-stu-id="5e617-117">Type</span></span>   |<span data-ttu-id="5e617-118">说明</span><span class="sxs-lookup"><span data-stu-id="5e617-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e617-119">id</span><span class="sxs-lookup"><span data-stu-id="5e617-119">id</span></span>|<span data-ttu-id="5e617-120">String</span><span class="sxs-lookup"><span data-stu-id="5e617-120">String</span></span>| <span data-ttu-id="5e617-121">只读。</span><span class="sxs-lookup"><span data-stu-id="5e617-121">Read-only.</span></span> <span data-ttu-id="5e617-122">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="5e617-122">Unique ID of the message.</span></span>|
|<span data-ttu-id="5e617-123">displayName</span><span class="sxs-lookup"><span data-stu-id="5e617-123">displayName</span></span>| <span data-ttu-id="5e617-124">string</span><span class="sxs-lookup"><span data-stu-id="5e617-124">string</span></span> | <span data-ttu-id="5e617-125">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5e617-125">The display name of the user.</span></span> |
|<span data-ttu-id="5e617-126">角色</span><span class="sxs-lookup"><span data-stu-id="5e617-126">roles</span></span>| <span data-ttu-id="5e617-127">string 集合</span><span class="sxs-lookup"><span data-stu-id="5e617-127">string collection</span></span> | <span data-ttu-id="5e617-128">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="5e617-128">The roles for that user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5e617-129">关系</span><span class="sxs-lookup"><span data-stu-id="5e617-129">Relationships</span></span>

<span data-ttu-id="5e617-130">无</span><span class="sxs-lookup"><span data-stu-id="5e617-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e617-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e617-131">JSON representation</span></span>

<span data-ttu-id="5e617-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e617-132">The following is a JSON representation of the resource.</span></span>

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