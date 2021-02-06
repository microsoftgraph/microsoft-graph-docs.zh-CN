---
title: filterGroup 资源类型
description: 定义对象必须满足的一组子句才能在范围中考虑。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 6338ae4b02b79d1512d5e9f695a69155197e2f4a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131913"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="bda3c-103">filterGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="bda3c-103">filterGroup resource type</span></span>

<span data-ttu-id="bda3c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bda3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bda3c-105">定义对象必须满足的一组子句才能在范围中考虑。</span><span class="sxs-lookup"><span data-stu-id="bda3c-105">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="bda3c-106">在组范围内考虑对象 (只有在组的所有子句都计算为) 计算组时，才计算为一 `true` 个对象 `true` 。</span><span class="sxs-lookup"><span data-stu-id="bda3c-106">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="bda3c-107">属性</span><span class="sxs-lookup"><span data-stu-id="bda3c-107">Properties</span></span>
| <span data-ttu-id="bda3c-108">属性</span><span class="sxs-lookup"><span data-stu-id="bda3c-108">Property</span></span>     | <span data-ttu-id="bda3c-109">类型</span><span class="sxs-lookup"><span data-stu-id="bda3c-109">Type</span></span>   |<span data-ttu-id="bda3c-110">说明</span><span class="sxs-lookup"><span data-stu-id="bda3c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bda3c-111">clauses</span><span class="sxs-lookup"><span data-stu-id="bda3c-111">clauses</span></span>|<span data-ttu-id="bda3c-112">[filterClause](synchronization-filterclause.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bda3c-112">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="bda3c-113">Filter 子句 (此) 条件。</span><span class="sxs-lookup"><span data-stu-id="bda3c-113">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="bda3c-114">必须满足组内的所有子句，筛选器组才能计算结果 `true` 。</span><span class="sxs-lookup"><span data-stu-id="bda3c-114">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="bda3c-115">name</span><span class="sxs-lookup"><span data-stu-id="bda3c-115">name</span></span>|<span data-ttu-id="bda3c-116">字符串</span><span class="sxs-lookup"><span data-stu-id="bda3c-116">String</span></span>|<span data-ttu-id="bda3c-117">筛选器组的可读名称。</span><span class="sxs-lookup"><span data-stu-id="bda3c-117">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bda3c-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bda3c-118">JSON representation</span></span>

<span data-ttu-id="bda3c-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bda3c-119">The following is a JSON representation of the resource.</span></span>

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


