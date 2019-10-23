---
title: conditionalAccessUsers 资源类型
description: 代表策略作用域中包含和排除的用户、组和角色。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7e54c5b018331952776b36a0ab3c07be88c2be7c
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638475"
---
# <a name="conditionalaccessusers-resource-type"></a><span data-ttu-id="ad4a3-103">conditionalAccessUsers 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad4a3-103">conditionalAccessUsers resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad4a3-104">代表策略作用域中包含和排除的用户、组和角色。</span><span class="sxs-lookup"><span data-stu-id="ad4a3-104">Represents users, groups, and roles included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="ad4a3-105">属性</span><span class="sxs-lookup"><span data-stu-id="ad4a3-105">Properties</span></span>

| <span data-ttu-id="ad4a3-106">属性</span><span class="sxs-lookup"><span data-stu-id="ad4a3-106">Property</span></span>     | <span data-ttu-id="ad4a3-107">类型</span><span class="sxs-lookup"><span data-stu-id="ad4a3-107">Type</span></span>        | <span data-ttu-id="ad4a3-108">说明</span><span class="sxs-lookup"><span data-stu-id="ad4a3-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ad4a3-109">includeUsers</span><span class="sxs-lookup"><span data-stu-id="ad4a3-109">includeUsers</span></span> | <span data-ttu-id="ad4a3-110">String collection</span><span class="sxs-lookup"><span data-stu-id="ad4a3-110">String collection</span></span> | <span data-ttu-id="ad4a3-111">策略作用域中的用户 Id，除非明确排除`None`或`All`或`GuestsOrExternalUsers`或。</span><span class="sxs-lookup"><span data-stu-id="ad4a3-111">User IDs in scope of policy unless explicitly excluded, or `None` or `All` or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="ad4a3-112">excludeUsers</span><span class="sxs-lookup"><span data-stu-id="ad4a3-112">excludeUsers</span></span> | <span data-ttu-id="ad4a3-113">String collection</span><span class="sxs-lookup"><span data-stu-id="ad4a3-113">String collection</span></span> | <span data-ttu-id="ad4a3-114">从策略作用域和/或`GuestsOrExternalUsers`中排除的用户 id。</span><span class="sxs-lookup"><span data-stu-id="ad4a3-114">User IDs excluded from scope of policy and/or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="ad4a3-115">includeGroups</span><span class="sxs-lookup"><span data-stu-id="ad4a3-115">includeGroups</span></span> | <span data-ttu-id="ad4a3-116">String collection</span><span class="sxs-lookup"><span data-stu-id="ad4a3-116">String collection</span></span> | <span data-ttu-id="ad4a3-117">除非明确排除或`All`，否则策略作用域中的组 id。</span><span class="sxs-lookup"><span data-stu-id="ad4a3-117">Group IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="ad4a3-118">excludeGroups</span><span class="sxs-lookup"><span data-stu-id="ad4a3-118">excludeGroups</span></span> | <span data-ttu-id="ad4a3-119">String collection</span><span class="sxs-lookup"><span data-stu-id="ad4a3-119">String collection</span></span> | <span data-ttu-id="ad4a3-120">从策略作用域中排除的组 Id。</span><span class="sxs-lookup"><span data-stu-id="ad4a3-120">Group IDs excluded from scope of policy.</span></span> |
| <span data-ttu-id="ad4a3-121">includeRoles</span><span class="sxs-lookup"><span data-stu-id="ad4a3-121">includeRoles</span></span> | <span data-ttu-id="ad4a3-122">String collection</span><span class="sxs-lookup"><span data-stu-id="ad4a3-122">String collection</span></span> | <span data-ttu-id="ad4a3-123">策略作用域中的角色 Id，除非明确排除`All`或。</span><span class="sxs-lookup"><span data-stu-id="ad4a3-123">Role IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="ad4a3-124">excludeRoles</span><span class="sxs-lookup"><span data-stu-id="ad4a3-124">excludeRoles</span></span> | <span data-ttu-id="ad4a3-125">String collection</span><span class="sxs-lookup"><span data-stu-id="ad4a3-125">String collection</span></span> | <span data-ttu-id="ad4a3-126">从策略范围中排除的角色 Id。</span><span class="sxs-lookup"><span data-stu-id="ad4a3-126">Role IDs excluded from scope of policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ad4a3-127">关系</span><span class="sxs-lookup"><span data-stu-id="ad4a3-127">Relationships</span></span>

<span data-ttu-id="ad4a3-128">无。</span><span class="sxs-lookup"><span data-stu-id="ad4a3-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad4a3-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad4a3-129">JSON representation</span></span>

<span data-ttu-id="ad4a3-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad4a3-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeUsers",
    "excludeUsers",
    "includeGroups",
    "excludeGroups",
    "includeRoles",
    "excludeRoles"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessUsers",
  "baseType": null
}-->

```json
{
  "excludeGroups": ["String"],
  "excludeRoles": ["String"],
  "excludeUsers": ["String"],
  "includeGroups": ["String"],
  "includeRoles": ["String"],
  "includeUsers": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessUsers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->