---
title: filterGroup 资源类型
description: 定义要在范围中考虑对象必须满足的一组子句。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6e7933bf2fef6240dd0dc53d7da975074225aa30
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217888"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="876ae-103">filterGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="876ae-103">filterGroup resource type</span></span>

<span data-ttu-id="876ae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="876ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="876ae-105">定义要在范围中考虑对象必须满足的一组子句。</span><span class="sxs-lookup"><span data-stu-id="876ae-105">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="876ae-106">仅当组的所有子句都计算为`true` `true`时，才会在组的作用域中考虑对象（组的计算结果为）。</span><span class="sxs-lookup"><span data-stu-id="876ae-106">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="876ae-107">属性</span><span class="sxs-lookup"><span data-stu-id="876ae-107">Properties</span></span>
| <span data-ttu-id="876ae-108">属性</span><span class="sxs-lookup"><span data-stu-id="876ae-108">Property</span></span>     | <span data-ttu-id="876ae-109">类型</span><span class="sxs-lookup"><span data-stu-id="876ae-109">Type</span></span>   |<span data-ttu-id="876ae-110">说明</span><span class="sxs-lookup"><span data-stu-id="876ae-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="876ae-111">and</span><span class="sxs-lookup"><span data-stu-id="876ae-111">clauses</span></span>|<span data-ttu-id="876ae-112">[filterClause](synchronization-filterclause.md)集合</span><span class="sxs-lookup"><span data-stu-id="876ae-112">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="876ae-113">此组的筛选子句（条件）。</span><span class="sxs-lookup"><span data-stu-id="876ae-113">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="876ae-114">必须满足组中的所有子句，筛选器组才能进行计算`true`。</span><span class="sxs-lookup"><span data-stu-id="876ae-114">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="876ae-115">name</span><span class="sxs-lookup"><span data-stu-id="876ae-115">name</span></span>|<span data-ttu-id="876ae-116">字符串</span><span class="sxs-lookup"><span data-stu-id="876ae-116">String</span></span>|<span data-ttu-id="876ae-117">易于阅读的筛选器组名称。</span><span class="sxs-lookup"><span data-stu-id="876ae-117">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="876ae-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="876ae-118">JSON representation</span></span>

<span data-ttu-id="876ae-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="876ae-119">The following is a JSON representation of the resource.</span></span>

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
