---
title: filterGroup 资源类型
description: 定义要在范围中考虑对象必须满足的一组子句。 仅当组的所有子句都计算为`true` `true`时, 才会在组的作用域中考虑对象 (组的计算结果为)。
localization_priority: Normal
ms.openlocfilehash: ac71d5aa8c278c4c65edd96f0adcb8278bfd3246
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342878"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="ad025-104">filterGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad025-104">filterGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad025-105">定义要在范围中考虑对象必须满足的一组子句。</span><span class="sxs-lookup"><span data-stu-id="ad025-105">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="ad025-106">仅当组的所有子句都计算为`true` `true`时, 才会在组的作用域中考虑对象 (组的计算结果为)。</span><span class="sxs-lookup"><span data-stu-id="ad025-106">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="ad025-107">属性</span><span class="sxs-lookup"><span data-stu-id="ad025-107">Properties</span></span>
| <span data-ttu-id="ad025-108">属性</span><span class="sxs-lookup"><span data-stu-id="ad025-108">Property</span></span>     | <span data-ttu-id="ad025-109">类型</span><span class="sxs-lookup"><span data-stu-id="ad025-109">Type</span></span>   |<span data-ttu-id="ad025-110">说明</span><span class="sxs-lookup"><span data-stu-id="ad025-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad025-111">and</span><span class="sxs-lookup"><span data-stu-id="ad025-111">clauses</span></span>|<span data-ttu-id="ad025-112">[filterClause](synchronization-filterclause.md)集合</span><span class="sxs-lookup"><span data-stu-id="ad025-112">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="ad025-113">此组的筛选子句 (条件)。</span><span class="sxs-lookup"><span data-stu-id="ad025-113">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="ad025-114">必须满足组中的所有子句, 筛选器组才能进行计算`true`。</span><span class="sxs-lookup"><span data-stu-id="ad025-114">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="ad025-115">name</span><span class="sxs-lookup"><span data-stu-id="ad025-115">name</span></span>|<span data-ttu-id="ad025-116">String</span><span class="sxs-lookup"><span data-stu-id="ad025-116">String</span></span>|<span data-ttu-id="ad025-117">易于阅读的筛选器组名称。</span><span class="sxs-lookup"><span data-stu-id="ad025-117">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad025-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad025-118">JSON representation</span></span>

<span data-ttu-id="ad025-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad025-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterGroup"
}-->

```json
{
  "clauses": [{"@odata.type": "microsoft.graph.filterClause"}],
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
