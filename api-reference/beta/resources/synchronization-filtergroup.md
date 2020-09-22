---
title: filterGroup 资源类型
description: 定义要在范围中考虑对象必须满足的一组子句。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4dd174442cedf8f194bb9faf87d8e844b8c73163
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079759"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="85c50-103">filterGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="85c50-103">filterGroup resource type</span></span>

<span data-ttu-id="85c50-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85c50-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85c50-105">定义要在范围中考虑对象必须满足的一组子句。</span><span class="sxs-lookup"><span data-stu-id="85c50-105">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="85c50-106">在组的作用域中考虑对象，只有在将 `true` 组的所有子句计算为时，才会将组评估为)  (`true` 。</span><span class="sxs-lookup"><span data-stu-id="85c50-106">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="85c50-107">属性</span><span class="sxs-lookup"><span data-stu-id="85c50-107">Properties</span></span>
| <span data-ttu-id="85c50-108">属性</span><span class="sxs-lookup"><span data-stu-id="85c50-108">Property</span></span>     | <span data-ttu-id="85c50-109">类型</span><span class="sxs-lookup"><span data-stu-id="85c50-109">Type</span></span>   |<span data-ttu-id="85c50-110">说明</span><span class="sxs-lookup"><span data-stu-id="85c50-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85c50-111">and</span><span class="sxs-lookup"><span data-stu-id="85c50-111">clauses</span></span>|<span data-ttu-id="85c50-112">[filterClause](synchronization-filterclause.md) 集合</span><span class="sxs-lookup"><span data-stu-id="85c50-112">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="85c50-113">此组的 (条件) 的筛选子句。</span><span class="sxs-lookup"><span data-stu-id="85c50-113">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="85c50-114">必须满足组中的所有子句，筛选器组才能进行计算 `true` 。</span><span class="sxs-lookup"><span data-stu-id="85c50-114">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="85c50-115">名称</span><span class="sxs-lookup"><span data-stu-id="85c50-115">name</span></span>|<span data-ttu-id="85c50-116">String</span><span class="sxs-lookup"><span data-stu-id="85c50-116">String</span></span>|<span data-ttu-id="85c50-117">易于阅读的筛选器组名称。</span><span class="sxs-lookup"><span data-stu-id="85c50-117">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="85c50-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85c50-118">JSON representation</span></span>

<span data-ttu-id="85c50-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85c50-119">The following is a JSON representation of the resource.</span></span>

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


