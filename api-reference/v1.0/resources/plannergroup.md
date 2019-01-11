---
title: plannerGroup 资源类型
description: '**PlannerGroup**资源为组提供计划工具资源的访问权限。 它不包含任何可用的属性。'
localization_priority: Normal
ms.openlocfilehash: ac55c0acd3561205654383cbb1b3d264c219d1a3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871965"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="b01c0-104">plannerGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="b01c0-104">plannerGroup resource type</span></span>

<span data-ttu-id="b01c0-p102">**plannerGroup** 资源提供[组](group.md)的 Planner 资源的访问权限。它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="b01c0-p102">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="b01c0-107">方法</span><span class="sxs-lookup"><span data-stu-id="b01c0-107">Methods</span></span>

| <span data-ttu-id="b01c0-108">方法</span><span class="sxs-lookup"><span data-stu-id="b01c0-108">Method</span></span>           | <span data-ttu-id="b01c0-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b01c0-109">Return Type</span></span>    |<span data-ttu-id="b01c0-110">说明</span><span class="sxs-lookup"><span data-stu-id="b01c0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b01c0-111">List plans</span><span class="sxs-lookup"><span data-stu-id="b01c0-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="b01c0-112">[plannerPlan](plannerplan.md) collection</span><span class="sxs-lookup"><span data-stu-id="b01c0-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="b01c0-113">获取 **plannerPlan** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b01c0-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="b01c0-114">属性</span><span class="sxs-lookup"><span data-stu-id="b01c0-114">Properties</span></span>
| <span data-ttu-id="b01c0-115">属性</span><span class="sxs-lookup"><span data-stu-id="b01c0-115">Property</span></span>     | <span data-ttu-id="b01c0-116">类型</span><span class="sxs-lookup"><span data-stu-id="b01c0-116">Type</span></span>   |<span data-ttu-id="b01c0-117">说明</span><span class="sxs-lookup"><span data-stu-id="b01c0-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b01c0-118">id</span><span class="sxs-lookup"><span data-stu-id="b01c0-118">id</span></span>|<span data-ttu-id="b01c0-119">String</span><span class="sxs-lookup"><span data-stu-id="b01c0-119">String</span></span>| <span data-ttu-id="b01c0-p103">只读。**plannerGroup** 的标识符</span><span class="sxs-lookup"><span data-stu-id="b01c0-p103">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="b01c0-122">关系</span><span class="sxs-lookup"><span data-stu-id="b01c0-122">Relationships</span></span>
| <span data-ttu-id="b01c0-123">关系</span><span class="sxs-lookup"><span data-stu-id="b01c0-123">Relationship</span></span> | <span data-ttu-id="b01c0-124">类型</span><span class="sxs-lookup"><span data-stu-id="b01c0-124">Type</span></span>   |<span data-ttu-id="b01c0-125">说明</span><span class="sxs-lookup"><span data-stu-id="b01c0-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b01c0-126">plans</span><span class="sxs-lookup"><span data-stu-id="b01c0-126">plans</span></span>|<span data-ttu-id="b01c0-127">[plannerPlan](plannerplan.md) collection</span><span class="sxs-lookup"><span data-stu-id="b01c0-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="b01c0-p104">只读。可为 NULL。返回组拥有的 [plannerPlans](plannerplan.md)。</span><span class="sxs-lookup"><span data-stu-id="b01c0-p104">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b01c0-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b01c0-131">JSON representation</span></span>
<span data-ttu-id="b01c0-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b01c0-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
