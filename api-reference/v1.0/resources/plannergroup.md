---
title: plannerGroup 资源类型
description: '**PlannerGroup**资源为组提供计划工具资源的访问权限。 它不包含任何可用的属性。'
ms.openlocfilehash: 3a2bb9cfd90a36f6b0a2148e0d789ac97b2199fb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010073"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="7a312-104">plannerGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a312-104">plannerGroup resource type</span></span>

<span data-ttu-id="7a312-p102">**plannerGroup** 资源提供[组](group.md)的 Planner 资源的访问权限。它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="7a312-p102">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="7a312-107">方法</span><span class="sxs-lookup"><span data-stu-id="7a312-107">Methods</span></span>

| <span data-ttu-id="7a312-108">方法</span><span class="sxs-lookup"><span data-stu-id="7a312-108">Method</span></span>           | <span data-ttu-id="7a312-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="7a312-109">Return Type</span></span>    |<span data-ttu-id="7a312-110">说明</span><span class="sxs-lookup"><span data-stu-id="7a312-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7a312-111">List plans</span><span class="sxs-lookup"><span data-stu-id="7a312-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="7a312-112">[plannerPlan](plannerplan.md) collection</span><span class="sxs-lookup"><span data-stu-id="7a312-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="7a312-113">获取 **plannerPlan** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7a312-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="7a312-114">属性</span><span class="sxs-lookup"><span data-stu-id="7a312-114">Properties</span></span>
| <span data-ttu-id="7a312-115">属性</span><span class="sxs-lookup"><span data-stu-id="7a312-115">Property</span></span>     | <span data-ttu-id="7a312-116">类型</span><span class="sxs-lookup"><span data-stu-id="7a312-116">Type</span></span>   |<span data-ttu-id="7a312-117">说明</span><span class="sxs-lookup"><span data-stu-id="7a312-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a312-118">id</span><span class="sxs-lookup"><span data-stu-id="7a312-118">id</span></span>|<span data-ttu-id="7a312-119">String</span><span class="sxs-lookup"><span data-stu-id="7a312-119">String</span></span>| <span data-ttu-id="7a312-p103">只读。**plannerGroup** 的标识符</span><span class="sxs-lookup"><span data-stu-id="7a312-p103">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a312-122">关系</span><span class="sxs-lookup"><span data-stu-id="7a312-122">Relationships</span></span>
| <span data-ttu-id="7a312-123">关系</span><span class="sxs-lookup"><span data-stu-id="7a312-123">Relationship</span></span> | <span data-ttu-id="7a312-124">类型</span><span class="sxs-lookup"><span data-stu-id="7a312-124">Type</span></span>   |<span data-ttu-id="7a312-125">说明</span><span class="sxs-lookup"><span data-stu-id="7a312-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a312-126">plans</span><span class="sxs-lookup"><span data-stu-id="7a312-126">plans</span></span>|<span data-ttu-id="7a312-127">[plannerPlan](plannerplan.md) collection</span><span class="sxs-lookup"><span data-stu-id="7a312-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="7a312-p104">只读。可为 NULL。返回组拥有的 [plannerPlans](plannerplan.md)。</span><span class="sxs-lookup"><span data-stu-id="7a312-p104">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a312-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a312-131">JSON representation</span></span>
<span data-ttu-id="7a312-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a312-132">Here is a JSON representation of the resource.</span></span>

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