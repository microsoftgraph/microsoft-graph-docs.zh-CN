---
title: conditionalAccessUsers 资源类型
description: 表示策略作用域中包括和排除的用户、组和角色。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 8f75eb86ab9627b2cb9d507de9321743524203b3
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129770"
---
# <a name="conditionalaccessusers-resource-type"></a><span data-ttu-id="6f247-103">conditionalAccessUsers 资源类型</span><span class="sxs-lookup"><span data-stu-id="6f247-103">conditionalAccessUsers resource type</span></span>

<span data-ttu-id="6f247-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f247-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6f247-105">表示策略作用域中包括和排除的用户、组和角色。</span><span class="sxs-lookup"><span data-stu-id="6f247-105">Represents users, groups, and roles included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="6f247-106">属性</span><span class="sxs-lookup"><span data-stu-id="6f247-106">Properties</span></span>

| <span data-ttu-id="6f247-107">属性</span><span class="sxs-lookup"><span data-stu-id="6f247-107">Property</span></span>     | <span data-ttu-id="6f247-108">类型</span><span class="sxs-lookup"><span data-stu-id="6f247-108">Type</span></span>        | <span data-ttu-id="6f247-109">说明</span><span class="sxs-lookup"><span data-stu-id="6f247-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6f247-110">includeUsers</span><span class="sxs-lookup"><span data-stu-id="6f247-110">includeUsers</span></span> | <span data-ttu-id="6f247-111">String collection</span><span class="sxs-lookup"><span data-stu-id="6f247-111">String collection</span></span> | <span data-ttu-id="6f247-112">策略范围内的用户 ID（除非明确排除）或 `None` 或 `All` `GuestsOrExternalUsers` 。</span><span class="sxs-lookup"><span data-stu-id="6f247-112">User IDs in scope of policy unless explicitly excluded, or `None` or `All` or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="6f247-113">excludeUsers</span><span class="sxs-lookup"><span data-stu-id="6f247-113">excludeUsers</span></span> | <span data-ttu-id="6f247-114">String collection</span><span class="sxs-lookup"><span data-stu-id="6f247-114">String collection</span></span> | <span data-ttu-id="6f247-115">策略作用域中排除的用户 ID 和/或 `GuestsOrExternalUsers` 。</span><span class="sxs-lookup"><span data-stu-id="6f247-115">User IDs excluded from scope of policy and/or `GuestsOrExternalUsers`.</span></span> |
| <span data-ttu-id="6f247-116">includeGroups</span><span class="sxs-lookup"><span data-stu-id="6f247-116">includeGroups</span></span> | <span data-ttu-id="6f247-117">String collection</span><span class="sxs-lookup"><span data-stu-id="6f247-117">String collection</span></span> | <span data-ttu-id="6f247-118">策略作用域中的组 ID（除非明确排除）或 `All` 。</span><span class="sxs-lookup"><span data-stu-id="6f247-118">Group IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="6f247-119">excludeGroups</span><span class="sxs-lookup"><span data-stu-id="6f247-119">excludeGroups</span></span> | <span data-ttu-id="6f247-120">String collection</span><span class="sxs-lookup"><span data-stu-id="6f247-120">String collection</span></span> | <span data-ttu-id="6f247-121">从策略作用域中排除的组 ID。</span><span class="sxs-lookup"><span data-stu-id="6f247-121">Group IDs excluded from scope of policy.</span></span> |
| <span data-ttu-id="6f247-122">includeRoles</span><span class="sxs-lookup"><span data-stu-id="6f247-122">includeRoles</span></span> | <span data-ttu-id="6f247-123">String collection</span><span class="sxs-lookup"><span data-stu-id="6f247-123">String collection</span></span> | <span data-ttu-id="6f247-124">策略作用域中的角色 ID（除非明确排除）或 `All` 。</span><span class="sxs-lookup"><span data-stu-id="6f247-124">Role IDs in scope of policy unless explicitly excluded, or `All`.</span></span> |
| <span data-ttu-id="6f247-125">excludeRoles</span><span class="sxs-lookup"><span data-stu-id="6f247-125">excludeRoles</span></span> | <span data-ttu-id="6f247-126">String collection</span><span class="sxs-lookup"><span data-stu-id="6f247-126">String collection</span></span> | <span data-ttu-id="6f247-127">从策略作用域排除的角色 ID。</span><span class="sxs-lookup"><span data-stu-id="6f247-127">Role IDs excluded from scope of policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6f247-128">关系</span><span class="sxs-lookup"><span data-stu-id="6f247-128">Relationships</span></span>

<span data-ttu-id="6f247-129">无。</span><span class="sxs-lookup"><span data-stu-id="6f247-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f247-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f247-130">JSON representation</span></span>

<span data-ttu-id="6f247-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f247-131">The following is a JSON representation of the resource.</span></span>

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

