---
title: conversationMember 资源类型
description: 代表对话中的用户。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 17fee8985e2383f0ede652cc1e1a6d8e9dc3304c
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873418"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="2c2d1-103">conversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c2d1-103">conversationMember resource type</span></span>

<span data-ttu-id="2c2d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c2d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c2d1-105">代表 [团队](team.md)中的用户。</span><span class="sxs-lookup"><span data-stu-id="2c2d1-105">Represents a user in a [team](team.md).</span></span>
<span data-ttu-id="2c2d1-106">另请参阅 [aadUserConversationMember](aaduserconversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="2c2d1-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2c2d1-107">属性</span><span class="sxs-lookup"><span data-stu-id="2c2d1-107">Properties</span></span>

| <span data-ttu-id="2c2d1-108">属性</span><span class="sxs-lookup"><span data-stu-id="2c2d1-108">Property</span></span>   | <span data-ttu-id="2c2d1-109">类型</span><span class="sxs-lookup"><span data-stu-id="2c2d1-109">Type</span></span> |<span data-ttu-id="2c2d1-110">说明</span><span class="sxs-lookup"><span data-stu-id="2c2d1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c2d1-111">id</span><span class="sxs-lookup"><span data-stu-id="2c2d1-111">id</span></span>|<span data-ttu-id="2c2d1-112">String</span><span class="sxs-lookup"><span data-stu-id="2c2d1-112">String</span></span>| <span data-ttu-id="2c2d1-113">只读。</span><span class="sxs-lookup"><span data-stu-id="2c2d1-113">Read-only.</span></span> <span data-ttu-id="2c2d1-114">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="2c2d1-114">Unique ID of the user.</span></span>|
|<span data-ttu-id="2c2d1-115">displayName</span><span class="sxs-lookup"><span data-stu-id="2c2d1-115">displayName</span></span>| <span data-ttu-id="2c2d1-116">string</span><span class="sxs-lookup"><span data-stu-id="2c2d1-116">string</span></span> | <span data-ttu-id="2c2d1-117">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2c2d1-117">The display name of the user.</span></span> |
|<span data-ttu-id="2c2d1-118">角色</span><span class="sxs-lookup"><span data-stu-id="2c2d1-118">roles</span></span>| <span data-ttu-id="2c2d1-119">string 集合</span><span class="sxs-lookup"><span data-stu-id="2c2d1-119">string collection</span></span> | <span data-ttu-id="2c2d1-120">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="2c2d1-120">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2c2d1-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c2d1-121">JSON representation</span></span>

<span data-ttu-id="2c2d1-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c2d1-122">The following is a JSON representation of the resource.</span></span>

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
