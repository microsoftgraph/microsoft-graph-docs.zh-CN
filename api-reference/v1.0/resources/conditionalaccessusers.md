---
title: conditionalAccessUsers 资源类型
description: 代表策略作用域中包含和排除的用户、组和角色。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 460b14d88fcf153935948784c08a6d0a03d33553
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384495"
---
# <a name="conditionalaccessusers-resource-type"></a><span data-ttu-id="2d13d-103">conditionalAccessUsers 资源类型</span><span class="sxs-lookup"><span data-stu-id="2d13d-103">conditionalAccessUsers resource type</span></span>

<span data-ttu-id="2d13d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d13d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d13d-105">代表策略作用域中包含和排除的用户、组和角色。</span><span class="sxs-lookup"><span data-stu-id="2d13d-105">Represents users, groups, and roles included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="2d13d-106">属性</span><span class="sxs-lookup"><span data-stu-id="2d13d-106">Properties</span></span>

| <span data-ttu-id="2d13d-107">属性</span><span class="sxs-lookup"><span data-stu-id="2d13d-107">Property</span></span>     | <span data-ttu-id="2d13d-108">类型</span><span class="sxs-lookup"><span data-stu-id="2d13d-108">Type</span></span>        | <span data-ttu-id="2d13d-109">说明</span><span class="sxs-lookup"><span data-stu-id="2d13d-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2d13d-110">includeUsers</span><span class="sxs-lookup"><span data-stu-id="2d13d-110">includeUsers</span></span> | <span data-ttu-id="2d13d-111">String collection</span><span class="sxs-lookup"><span data-stu-id="2d13d-111">String collection</span></span> | <span data-ttu-id="2d13d-112">策略作用域中的用户 Id，除非明确排除或 `None` 或或 `All` `GuestsOrExternalUsers` 。</span><span class="sxs-lookup"><span data-stu-id="2d13d-112">User IDs in scope of policy unless explicitly excluded, or `None` or `All` or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="2d13d-113">excludeUsers</span><span class="sxs-lookup"><span data-stu-id="2d13d-113">excludeUsers</span></span> | <span data-ttu-id="2d13d-114">String collection</span><span class="sxs-lookup"><span data-stu-id="2d13d-114">String collection</span></span> | <span data-ttu-id="2d13d-115">从策略作用域和/或中排除的用户 Id `GuestsOrExternalUsers` 。</span><span class="sxs-lookup"><span data-stu-id="2d13d-115">User IDs excluded from scope of policy and/or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="2d13d-116">includeGroups</span><span class="sxs-lookup"><span data-stu-id="2d13d-116">includeGroups</span></span> | <span data-ttu-id="2d13d-117">String collection</span><span class="sxs-lookup"><span data-stu-id="2d13d-117">String collection</span></span> | <span data-ttu-id="2d13d-118">除非明确排除或，否则策略作用域中的组 Id `All` 。</span><span class="sxs-lookup"><span data-stu-id="2d13d-118">Group IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="2d13d-119">excludeGroups</span><span class="sxs-lookup"><span data-stu-id="2d13d-119">excludeGroups</span></span> | <span data-ttu-id="2d13d-120">String collection</span><span class="sxs-lookup"><span data-stu-id="2d13d-120">String collection</span></span> | <span data-ttu-id="2d13d-121">从策略作用域中排除的组 Id。</span><span class="sxs-lookup"><span data-stu-id="2d13d-121">Group IDs excluded from scope of policy.</span></span> |
| <span data-ttu-id="2d13d-122">includeRoles</span><span class="sxs-lookup"><span data-stu-id="2d13d-122">includeRoles</span></span> | <span data-ttu-id="2d13d-123">String collection</span><span class="sxs-lookup"><span data-stu-id="2d13d-123">String collection</span></span> | <span data-ttu-id="2d13d-124">策略作用域中的角色 Id，除非明确排除或 `All` 。</span><span class="sxs-lookup"><span data-stu-id="2d13d-124">Role IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="2d13d-125">excludeRoles</span><span class="sxs-lookup"><span data-stu-id="2d13d-125">excludeRoles</span></span> | <span data-ttu-id="2d13d-126">String collection</span><span class="sxs-lookup"><span data-stu-id="2d13d-126">String collection</span></span> | <span data-ttu-id="2d13d-127">从策略范围中排除的角色 Id。</span><span class="sxs-lookup"><span data-stu-id="2d13d-127">Role IDs excluded from scope of policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2d13d-128">关系</span><span class="sxs-lookup"><span data-stu-id="2d13d-128">Relationships</span></span>

<span data-ttu-id="2d13d-129">无。</span><span class="sxs-lookup"><span data-stu-id="2d13d-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d13d-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d13d-130">JSON representation</span></span>

<span data-ttu-id="2d13d-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d13d-131">The following is a JSON representation of the resource.</span></span>

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
