---
title: filterGroup 资源类型
description: 定义一对象视为范围内必须满足的子句。 对象属于组的范围内 (组计算为`true`) 才组的所有子句都计算为`true`。
localization_priority: Normal
ms.openlocfilehash: b71bdf16d6639b5ecc8512565ccf56d592a0da58
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514185"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="b50b7-104">filterGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="b50b7-104">filterGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b50b7-105">定义一对象视为范围内必须满足的子句。</span><span class="sxs-lookup"><span data-stu-id="b50b7-105">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="b50b7-106">对象属于组的范围内 (组计算为`true`) 才组的所有子句都计算为`true`。</span><span class="sxs-lookup"><span data-stu-id="b50b7-106">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="b50b7-107">属性</span><span class="sxs-lookup"><span data-stu-id="b50b7-107">Properties</span></span>
| <span data-ttu-id="b50b7-108">属性</span><span class="sxs-lookup"><span data-stu-id="b50b7-108">Property</span></span>     | <span data-ttu-id="b50b7-109">类型</span><span class="sxs-lookup"><span data-stu-id="b50b7-109">Type</span></span>   |<span data-ttu-id="b50b7-110">说明</span><span class="sxs-lookup"><span data-stu-id="b50b7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b50b7-111">子句</span><span class="sxs-lookup"><span data-stu-id="b50b7-111">clauses</span></span>|<span data-ttu-id="b50b7-112">[filterClause](synchronization-filterclause.md)集合</span><span class="sxs-lookup"><span data-stu-id="b50b7-112">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="b50b7-113">筛选此组的子句 （条件）。</span><span class="sxs-lookup"><span data-stu-id="b50b7-113">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="b50b7-114">组中的所有子句都必须满足顺序筛选器组计算结果为`true`。</span><span class="sxs-lookup"><span data-stu-id="b50b7-114">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="b50b7-115">name</span><span class="sxs-lookup"><span data-stu-id="b50b7-115">name</span></span>|<span data-ttu-id="b50b7-116">String</span><span class="sxs-lookup"><span data-stu-id="b50b7-116">String</span></span>|<span data-ttu-id="b50b7-117">可读的筛选器组的名称。</span><span class="sxs-lookup"><span data-stu-id="b50b7-117">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b50b7-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b50b7-118">JSON representation</span></span>

<span data-ttu-id="b50b7-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b50b7-119">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filtergroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
