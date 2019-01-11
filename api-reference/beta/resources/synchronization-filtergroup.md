---
title: filterGroup 资源类型
description: 定义一对象视为范围内必须满足的子句。 对象属于组的范围内 (组计算为`true`) 才组的所有子句都计算为`true`。
localization_priority: Normal
ms.openlocfilehash: 174c02518069e949c49887d9e21e778e8455509a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836111"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="06b9d-104">filterGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="06b9d-104">filterGroup resource type</span></span>

> <span data-ttu-id="06b9d-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="06b9d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06b9d-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="06b9d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="06b9d-107">定义一对象视为范围内必须满足的子句。</span><span class="sxs-lookup"><span data-stu-id="06b9d-107">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="06b9d-108">对象属于组的范围内 (组计算为`true`) 才组的所有子句都计算为`true`。</span><span class="sxs-lookup"><span data-stu-id="06b9d-108">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="06b9d-109">属性</span><span class="sxs-lookup"><span data-stu-id="06b9d-109">Properties</span></span>
| <span data-ttu-id="06b9d-110">属性</span><span class="sxs-lookup"><span data-stu-id="06b9d-110">Property</span></span>     | <span data-ttu-id="06b9d-111">类型</span><span class="sxs-lookup"><span data-stu-id="06b9d-111">Type</span></span>   |<span data-ttu-id="06b9d-112">Description</span><span class="sxs-lookup"><span data-stu-id="06b9d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06b9d-113">子句</span><span class="sxs-lookup"><span data-stu-id="06b9d-113">clauses</span></span>|<span data-ttu-id="06b9d-114">[filterClause](synchronization-filterclause.md)集合</span><span class="sxs-lookup"><span data-stu-id="06b9d-114">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="06b9d-115">筛选此组的子句 （条件）。</span><span class="sxs-lookup"><span data-stu-id="06b9d-115">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="06b9d-116">组中的所有子句都必须满足顺序筛选器组计算结果为`true`。</span><span class="sxs-lookup"><span data-stu-id="06b9d-116">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="06b9d-117">name</span><span class="sxs-lookup"><span data-stu-id="06b9d-117">name</span></span>|<span data-ttu-id="06b9d-118">字符串</span><span class="sxs-lookup"><span data-stu-id="06b9d-118">String</span></span>|<span data-ttu-id="06b9d-119">可读的筛选器组的名称。</span><span class="sxs-lookup"><span data-stu-id="06b9d-119">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06b9d-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06b9d-120">JSON representation</span></span>

<span data-ttu-id="06b9d-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06b9d-121">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "filterGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
