---
title: filterGroup 资源类型
description: 定义要在范围中考虑对象必须满足的一组子句。 仅当组的所有子句都计算为`true` `true`时, 才会在组的作用域中考虑对象 (组的计算结果为)。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c411b85f2661829fe8739b8f8dc1cdd09639723c
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621443"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="2e070-104">filterGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="2e070-104">filterGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e070-105">定义要在范围中考虑对象必须满足的一组子句。</span><span class="sxs-lookup"><span data-stu-id="2e070-105">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="2e070-106">仅当组的所有子句都计算为`true` `true`时, 才会在组的作用域中考虑对象 (组的计算结果为)。</span><span class="sxs-lookup"><span data-stu-id="2e070-106">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="2e070-107">属性</span><span class="sxs-lookup"><span data-stu-id="2e070-107">Properties</span></span>
| <span data-ttu-id="2e070-108">属性</span><span class="sxs-lookup"><span data-stu-id="2e070-108">Property</span></span>     | <span data-ttu-id="2e070-109">类型</span><span class="sxs-lookup"><span data-stu-id="2e070-109">Type</span></span>   |<span data-ttu-id="2e070-110">说明</span><span class="sxs-lookup"><span data-stu-id="2e070-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e070-111">and</span><span class="sxs-lookup"><span data-stu-id="2e070-111">clauses</span></span>|<span data-ttu-id="2e070-112">[filterClause](synchronization-filterclause.md)集合</span><span class="sxs-lookup"><span data-stu-id="2e070-112">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="2e070-113">此组的筛选子句 (条件)。</span><span class="sxs-lookup"><span data-stu-id="2e070-113">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="2e070-114">必须满足组中的所有子句, 筛选器组才能进行计算`true`。</span><span class="sxs-lookup"><span data-stu-id="2e070-114">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="2e070-115">name</span><span class="sxs-lookup"><span data-stu-id="2e070-115">name</span></span>|<span data-ttu-id="2e070-116">String</span><span class="sxs-lookup"><span data-stu-id="2e070-116">String</span></span>|<span data-ttu-id="2e070-117">易于阅读的筛选器组名称。</span><span class="sxs-lookup"><span data-stu-id="2e070-117">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e070-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2e070-118">JSON representation</span></span>

<span data-ttu-id="2e070-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e070-119">The following is a JSON representation of the resource.</span></span>

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
