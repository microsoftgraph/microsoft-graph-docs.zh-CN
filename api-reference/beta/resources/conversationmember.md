---
title: conversationMember 资源类型
description: 表示对话中的用户。
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: f6908106390e527ab4e33e777dd232b58ead727a
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2019
ms.locfileid: "34379274"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="aafb8-103">conversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="aafb8-103">conversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aafb8-104">表示[聊天](chat.md)中的用户。</span><span class="sxs-lookup"><span data-stu-id="aafb8-104">Represents a user in a [chat](chat.md).</span></span>

## <a name="methods"></a><span data-ttu-id="aafb8-105">方法</span><span class="sxs-lookup"><span data-stu-id="aafb8-105">Methods</span></span>

| <span data-ttu-id="aafb8-106">方法</span><span class="sxs-lookup"><span data-stu-id="aafb8-106">Method</span></span>       | <span data-ttu-id="aafb8-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="aafb8-107">Return Type</span></span>  |<span data-ttu-id="aafb8-108">说明</span><span class="sxs-lookup"><span data-stu-id="aafb8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aafb8-109">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="aafb8-109">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="aafb8-110">[conversationmember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aafb8-110">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="aafb8-111">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="aafb8-111">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="aafb8-112">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="aafb8-112">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="aafb8-113">conversationmember</span><span class="sxs-lookup"><span data-stu-id="aafb8-113">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="aafb8-114">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="aafb8-114">Get a single user in the chat.</span></span>|

## <a name="properties"></a><span data-ttu-id="aafb8-115">属性</span><span class="sxs-lookup"><span data-stu-id="aafb8-115">Properties</span></span>
| <span data-ttu-id="aafb8-116">属性</span><span class="sxs-lookup"><span data-stu-id="aafb8-116">Property</span></span>     | <span data-ttu-id="aafb8-117">类型</span><span class="sxs-lookup"><span data-stu-id="aafb8-117">Type</span></span>   |<span data-ttu-id="aafb8-118">说明</span><span class="sxs-lookup"><span data-stu-id="aafb8-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aafb8-119">id</span><span class="sxs-lookup"><span data-stu-id="aafb8-119">id</span></span>|<span data-ttu-id="aafb8-120">String</span><span class="sxs-lookup"><span data-stu-id="aafb8-120">String</span></span>| <span data-ttu-id="aafb8-121">只读。</span><span class="sxs-lookup"><span data-stu-id="aafb8-121">Read-only.</span></span> <span data-ttu-id="aafb8-122">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="aafb8-122">Unique ID of the message.</span></span>|
|<span data-ttu-id="aafb8-123">displayName</span><span class="sxs-lookup"><span data-stu-id="aafb8-123">displayName</span></span>| <span data-ttu-id="aafb8-124">string</span><span class="sxs-lookup"><span data-stu-id="aafb8-124">string</span></span> | <span data-ttu-id="aafb8-125">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="aafb8-125">The display name of the user.</span></span> |
|<span data-ttu-id="aafb8-126">角色</span><span class="sxs-lookup"><span data-stu-id="aafb8-126">roles</span></span>| <span data-ttu-id="aafb8-127">string 集合</span><span class="sxs-lookup"><span data-stu-id="aafb8-127">string collection</span></span> | <span data-ttu-id="aafb8-128">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="aafb8-128">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aafb8-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aafb8-129">JSON representation</span></span>

<span data-ttu-id="aafb8-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aafb8-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversationMember"
}-->

```json
{
  "id": "string (identifier)",
  "displayName" : "string",
  "roles" : ["string"]
}

```

## <a name="see-also"></a><span data-ttu-id="aafb8-131">另请参阅</span><span class="sxs-lookup"><span data-stu-id="aafb8-131">See Also</span></span>

[<span data-ttu-id="aafb8-132">aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="aafb8-132">aadUserConversationMember</span></span>](aaduserconversationmember.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversationMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
