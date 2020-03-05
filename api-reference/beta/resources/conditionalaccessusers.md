---
title: conditionalAccessUsers 资源类型
description: 代表策略作用域中包含和排除的用户、组和角色。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 269fe0552c69773fa62b97cf9803b3e0127f655b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507504"
---
# <a name="conditionalaccessusers-resource-type"></a><span data-ttu-id="dd43d-103">conditionalAccessUsers 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd43d-103">conditionalAccessUsers resource type</span></span>

<span data-ttu-id="dd43d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="dd43d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd43d-105">代表策略作用域中包含和排除的用户、组和角色。</span><span class="sxs-lookup"><span data-stu-id="dd43d-105">Represents users, groups, and roles included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="dd43d-106">属性</span><span class="sxs-lookup"><span data-stu-id="dd43d-106">Properties</span></span>

| <span data-ttu-id="dd43d-107">属性</span><span class="sxs-lookup"><span data-stu-id="dd43d-107">Property</span></span>     | <span data-ttu-id="dd43d-108">类型</span><span class="sxs-lookup"><span data-stu-id="dd43d-108">Type</span></span>        | <span data-ttu-id="dd43d-109">说明</span><span class="sxs-lookup"><span data-stu-id="dd43d-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="dd43d-110">includeUsers</span><span class="sxs-lookup"><span data-stu-id="dd43d-110">includeUsers</span></span> | <span data-ttu-id="dd43d-111">String 集合</span><span class="sxs-lookup"><span data-stu-id="dd43d-111">String collection</span></span> | <span data-ttu-id="dd43d-112">策略作用域中的用户 Id，除非明确排除`None`或`All`或`GuestsOrExternalUsers`或。</span><span class="sxs-lookup"><span data-stu-id="dd43d-112">User IDs in scope of policy unless explicitly excluded, or `None` or `All` or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="dd43d-113">excludeUsers</span><span class="sxs-lookup"><span data-stu-id="dd43d-113">excludeUsers</span></span> | <span data-ttu-id="dd43d-114">String 集合</span><span class="sxs-lookup"><span data-stu-id="dd43d-114">String collection</span></span> | <span data-ttu-id="dd43d-115">从策略作用域和/或`GuestsOrExternalUsers`中排除的用户 id。</span><span class="sxs-lookup"><span data-stu-id="dd43d-115">User IDs excluded from scope of policy and/or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="dd43d-116">includeGroups</span><span class="sxs-lookup"><span data-stu-id="dd43d-116">includeGroups</span></span> | <span data-ttu-id="dd43d-117">String 集合</span><span class="sxs-lookup"><span data-stu-id="dd43d-117">String collection</span></span> | <span data-ttu-id="dd43d-118">除非明确排除或`All`，否则策略作用域中的组 id。</span><span class="sxs-lookup"><span data-stu-id="dd43d-118">Group IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="dd43d-119">excludeGroups</span><span class="sxs-lookup"><span data-stu-id="dd43d-119">excludeGroups</span></span> | <span data-ttu-id="dd43d-120">String 集合</span><span class="sxs-lookup"><span data-stu-id="dd43d-120">String collection</span></span> | <span data-ttu-id="dd43d-121">从策略作用域中排除的组 Id。</span><span class="sxs-lookup"><span data-stu-id="dd43d-121">Group IDs excluded from scope of policy.</span></span> |
| <span data-ttu-id="dd43d-122">includeRoles</span><span class="sxs-lookup"><span data-stu-id="dd43d-122">includeRoles</span></span> | <span data-ttu-id="dd43d-123">String 集合</span><span class="sxs-lookup"><span data-stu-id="dd43d-123">String collection</span></span> | <span data-ttu-id="dd43d-124">策略作用域中的角色 Id，除非明确排除`All`或。</span><span class="sxs-lookup"><span data-stu-id="dd43d-124">Role IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="dd43d-125">excludeRoles</span><span class="sxs-lookup"><span data-stu-id="dd43d-125">excludeRoles</span></span> | <span data-ttu-id="dd43d-126">String 集合</span><span class="sxs-lookup"><span data-stu-id="dd43d-126">String collection</span></span> | <span data-ttu-id="dd43d-127">从策略范围中排除的角色 Id。</span><span class="sxs-lookup"><span data-stu-id="dd43d-127">Role IDs excluded from scope of policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="dd43d-128">关系</span><span class="sxs-lookup"><span data-stu-id="dd43d-128">Relationships</span></span>

<span data-ttu-id="dd43d-129">无。</span><span class="sxs-lookup"><span data-stu-id="dd43d-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd43d-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd43d-130">JSON representation</span></span>

<span data-ttu-id="dd43d-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd43d-131">The following is a JSON representation of the resource.</span></span>

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