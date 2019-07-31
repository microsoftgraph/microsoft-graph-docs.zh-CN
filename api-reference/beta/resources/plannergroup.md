---
title: plannerGroup 资源类型
description: '**PlannerGroup**资源提供对组的 Planner 资源的访问。 它不包含任何可用属性。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 308c64e7eb086f48859581cf2d66aae07269fe6e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965955"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="ef97f-104">plannerGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="ef97f-104">plannerGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef97f-105">**PlannerGroup**资源提供对[组](group.md)的 Planner 资源的访问。</span><span class="sxs-lookup"><span data-stu-id="ef97f-105">The **plannerGroup** resource provides access to Planner resources for a [group](group.md).</span></span> <span data-ttu-id="ef97f-106">它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="ef97f-106">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="ef97f-107">方法</span><span class="sxs-lookup"><span data-stu-id="ef97f-107">Methods</span></span>

| <span data-ttu-id="ef97f-108">方法</span><span class="sxs-lookup"><span data-stu-id="ef97f-108">Method</span></span>           | <span data-ttu-id="ef97f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ef97f-109">Return Type</span></span>    |<span data-ttu-id="ef97f-110">说明</span><span class="sxs-lookup"><span data-stu-id="ef97f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ef97f-111">列出计划</span><span class="sxs-lookup"><span data-stu-id="ef97f-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="ef97f-112">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ef97f-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="ef97f-113">获取**plannerPlan**对象集合。</span><span class="sxs-lookup"><span data-stu-id="ef97f-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="ef97f-114">属性</span><span class="sxs-lookup"><span data-stu-id="ef97f-114">Properties</span></span>
| <span data-ttu-id="ef97f-115">属性</span><span class="sxs-lookup"><span data-stu-id="ef97f-115">Property</span></span>     | <span data-ttu-id="ef97f-116">类型</span><span class="sxs-lookup"><span data-stu-id="ef97f-116">Type</span></span>   |<span data-ttu-id="ef97f-117">说明</span><span class="sxs-lookup"><span data-stu-id="ef97f-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef97f-118">id</span><span class="sxs-lookup"><span data-stu-id="ef97f-118">id</span></span>|<span data-ttu-id="ef97f-119">String</span><span class="sxs-lookup"><span data-stu-id="ef97f-119">String</span></span>| <span data-ttu-id="ef97f-120">只读。</span><span class="sxs-lookup"><span data-stu-id="ef97f-120">Read-only.</span></span> <span data-ttu-id="ef97f-121">**PlannerGroup**的标识符</span><span class="sxs-lookup"><span data-stu-id="ef97f-121">Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef97f-122">关系</span><span class="sxs-lookup"><span data-stu-id="ef97f-122">Relationships</span></span>
| <span data-ttu-id="ef97f-123">关系</span><span class="sxs-lookup"><span data-stu-id="ef97f-123">Relationship</span></span> | <span data-ttu-id="ef97f-124">类型</span><span class="sxs-lookup"><span data-stu-id="ef97f-124">Type</span></span>   |<span data-ttu-id="ef97f-125">说明</span><span class="sxs-lookup"><span data-stu-id="ef97f-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef97f-126">计划</span><span class="sxs-lookup"><span data-stu-id="ef97f-126">plans</span></span>|<span data-ttu-id="ef97f-127">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ef97f-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="ef97f-128">只读。</span><span class="sxs-lookup"><span data-stu-id="ef97f-128">Read-only.</span></span> <span data-ttu-id="ef97f-129">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="ef97f-129">Nullable.</span></span> <span data-ttu-id="ef97f-130">返回组所拥有的[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="ef97f-130">Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ef97f-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ef97f-131">JSON representation</span></span>
<span data-ttu-id="ef97f-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef97f-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.plannerGroup"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
