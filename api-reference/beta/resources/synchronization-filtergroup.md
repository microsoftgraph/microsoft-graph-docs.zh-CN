---
title: filterGroup 资源类型
description: 定义要在范围中考虑对象必须满足的一组子句。 仅当组的所有子句都计算为`true` `true`时，才会在组的作用域中考虑对象（组的计算结果为）。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 433528d9d663a3dc19cecaa5c2dad68e362dc882
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520182"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="7a461-104">filterGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a461-104">filterGroup resource type</span></span>

<span data-ttu-id="7a461-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7a461-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a461-106">定义要在范围中考虑对象必须满足的一组子句。</span><span class="sxs-lookup"><span data-stu-id="7a461-106">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="7a461-107">仅当组的所有子句都计算为`true` `true`时，才会在组的作用域中考虑对象（组的计算结果为）。</span><span class="sxs-lookup"><span data-stu-id="7a461-107">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="7a461-108">属性</span><span class="sxs-lookup"><span data-stu-id="7a461-108">Properties</span></span>
| <span data-ttu-id="7a461-109">属性</span><span class="sxs-lookup"><span data-stu-id="7a461-109">Property</span></span>     | <span data-ttu-id="7a461-110">类型</span><span class="sxs-lookup"><span data-stu-id="7a461-110">Type</span></span>   |<span data-ttu-id="7a461-111">说明</span><span class="sxs-lookup"><span data-stu-id="7a461-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a461-112">and</span><span class="sxs-lookup"><span data-stu-id="7a461-112">clauses</span></span>|<span data-ttu-id="7a461-113">[filterClause](synchronization-filterclause.md)集合</span><span class="sxs-lookup"><span data-stu-id="7a461-113">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="7a461-114">此组的筛选子句（条件）。</span><span class="sxs-lookup"><span data-stu-id="7a461-114">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="7a461-115">必须满足组中的所有子句，筛选器组才能进行计算`true`。</span><span class="sxs-lookup"><span data-stu-id="7a461-115">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="7a461-116">name</span><span class="sxs-lookup"><span data-stu-id="7a461-116">name</span></span>|<span data-ttu-id="7a461-117">String</span><span class="sxs-lookup"><span data-stu-id="7a461-117">String</span></span>|<span data-ttu-id="7a461-118">易于阅读的筛选器组名称。</span><span class="sxs-lookup"><span data-stu-id="7a461-118">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a461-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a461-119">JSON representation</span></span>

<span data-ttu-id="7a461-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a461-120">The following is a JSON representation of the resource.</span></span>

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
