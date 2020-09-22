---
title: conditionalAccessUsers 资源类型
description: 代表策略作用域中包含和排除的用户、组和角色。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d1294551fd568b9f41072d3707d64a88d4b04edc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994237"
---
# <a name="conditionalaccessusers-resource-type"></a><span data-ttu-id="ef522-103">conditionalAccessUsers 资源类型</span><span class="sxs-lookup"><span data-stu-id="ef522-103">conditionalAccessUsers resource type</span></span>

<span data-ttu-id="ef522-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef522-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef522-105">代表策略作用域中包含和排除的用户、组和角色。</span><span class="sxs-lookup"><span data-stu-id="ef522-105">Represents users, groups, and roles included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="ef522-106">属性</span><span class="sxs-lookup"><span data-stu-id="ef522-106">Properties</span></span>

| <span data-ttu-id="ef522-107">属性</span><span class="sxs-lookup"><span data-stu-id="ef522-107">Property</span></span>     | <span data-ttu-id="ef522-108">类型</span><span class="sxs-lookup"><span data-stu-id="ef522-108">Type</span></span>        | <span data-ttu-id="ef522-109">说明</span><span class="sxs-lookup"><span data-stu-id="ef522-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ef522-110">includeUsers</span><span class="sxs-lookup"><span data-stu-id="ef522-110">includeUsers</span></span> | <span data-ttu-id="ef522-111">String collection</span><span class="sxs-lookup"><span data-stu-id="ef522-111">String collection</span></span> | <span data-ttu-id="ef522-112">策略作用域中的用户 Id，除非明确排除或 `None` 或或 `All` `GuestsOrExternalUsers` 。</span><span class="sxs-lookup"><span data-stu-id="ef522-112">User IDs in scope of policy unless explicitly excluded, or `None` or `All` or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="ef522-113">excludeUsers</span><span class="sxs-lookup"><span data-stu-id="ef522-113">excludeUsers</span></span> | <span data-ttu-id="ef522-114">String collection</span><span class="sxs-lookup"><span data-stu-id="ef522-114">String collection</span></span> | <span data-ttu-id="ef522-115">从策略作用域和/或中排除的用户 Id `GuestsOrExternalUsers` 。</span><span class="sxs-lookup"><span data-stu-id="ef522-115">User IDs excluded from scope of policy and/or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="ef522-116">includeGroups</span><span class="sxs-lookup"><span data-stu-id="ef522-116">includeGroups</span></span> | <span data-ttu-id="ef522-117">String collection</span><span class="sxs-lookup"><span data-stu-id="ef522-117">String collection</span></span> | <span data-ttu-id="ef522-118">除非明确排除或，否则策略作用域中的组 Id `All` 。</span><span class="sxs-lookup"><span data-stu-id="ef522-118">Group IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="ef522-119">excludeGroups</span><span class="sxs-lookup"><span data-stu-id="ef522-119">excludeGroups</span></span> | <span data-ttu-id="ef522-120">String collection</span><span class="sxs-lookup"><span data-stu-id="ef522-120">String collection</span></span> | <span data-ttu-id="ef522-121">从策略作用域中排除的组 Id。</span><span class="sxs-lookup"><span data-stu-id="ef522-121">Group IDs excluded from scope of policy.</span></span> |
| <span data-ttu-id="ef522-122">includeRoles</span><span class="sxs-lookup"><span data-stu-id="ef522-122">includeRoles</span></span> | <span data-ttu-id="ef522-123">String collection</span><span class="sxs-lookup"><span data-stu-id="ef522-123">String collection</span></span> | <span data-ttu-id="ef522-124">策略作用域中的角色 Id，除非明确排除或 `All` 。</span><span class="sxs-lookup"><span data-stu-id="ef522-124">Role IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="ef522-125">excludeRoles</span><span class="sxs-lookup"><span data-stu-id="ef522-125">excludeRoles</span></span> | <span data-ttu-id="ef522-126">String collection</span><span class="sxs-lookup"><span data-stu-id="ef522-126">String collection</span></span> | <span data-ttu-id="ef522-127">从策略范围中排除的角色 Id。</span><span class="sxs-lookup"><span data-stu-id="ef522-127">Role IDs excluded from scope of policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ef522-128">关系</span><span class="sxs-lookup"><span data-stu-id="ef522-128">Relationships</span></span>

<span data-ttu-id="ef522-129">无。</span><span class="sxs-lookup"><span data-stu-id="ef522-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef522-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ef522-130">JSON representation</span></span>

<span data-ttu-id="ef522-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef522-131">The following is a JSON representation of the resource.</span></span>

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

