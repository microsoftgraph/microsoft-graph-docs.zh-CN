---
title: plannerGroup 资源类型
description: '**PlannerGroup**资源提供对组的 Planner 资源的访问。 它不包含任何可用属性。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 4d20a6d5c4918f729189e95a27bad18d9f872c8a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521725"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="02616-104">plannerGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="02616-104">plannerGroup resource type</span></span>

<span data-ttu-id="02616-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02616-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02616-106">**PlannerGroup**资源提供对[组](group.md)的 Planner 资源的访问。</span><span class="sxs-lookup"><span data-stu-id="02616-106">The **plannerGroup** resource provides access to Planner resources for a [group](group.md).</span></span> <span data-ttu-id="02616-107">它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="02616-107">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="02616-108">方法</span><span class="sxs-lookup"><span data-stu-id="02616-108">Methods</span></span>

| <span data-ttu-id="02616-109">方法</span><span class="sxs-lookup"><span data-stu-id="02616-109">Method</span></span>           | <span data-ttu-id="02616-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="02616-110">Return Type</span></span>    |<span data-ttu-id="02616-111">说明</span><span class="sxs-lookup"><span data-stu-id="02616-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="02616-112">列出计划</span><span class="sxs-lookup"><span data-stu-id="02616-112">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="02616-113">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="02616-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="02616-114">获取**plannerPlan**对象集合。</span><span class="sxs-lookup"><span data-stu-id="02616-114">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="02616-115">属性</span><span class="sxs-lookup"><span data-stu-id="02616-115">Properties</span></span>
| <span data-ttu-id="02616-116">属性</span><span class="sxs-lookup"><span data-stu-id="02616-116">Property</span></span>     | <span data-ttu-id="02616-117">类型</span><span class="sxs-lookup"><span data-stu-id="02616-117">Type</span></span>   |<span data-ttu-id="02616-118">说明</span><span class="sxs-lookup"><span data-stu-id="02616-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02616-119">id</span><span class="sxs-lookup"><span data-stu-id="02616-119">id</span></span>|<span data-ttu-id="02616-120">String</span><span class="sxs-lookup"><span data-stu-id="02616-120">String</span></span>| <span data-ttu-id="02616-121">只读。</span><span class="sxs-lookup"><span data-stu-id="02616-121">Read-only.</span></span> <span data-ttu-id="02616-122">**PlannerGroup**的标识符</span><span class="sxs-lookup"><span data-stu-id="02616-122">Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="02616-123">关系</span><span class="sxs-lookup"><span data-stu-id="02616-123">Relationships</span></span>
| <span data-ttu-id="02616-124">关系</span><span class="sxs-lookup"><span data-stu-id="02616-124">Relationship</span></span> | <span data-ttu-id="02616-125">类型</span><span class="sxs-lookup"><span data-stu-id="02616-125">Type</span></span>   |<span data-ttu-id="02616-126">说明</span><span class="sxs-lookup"><span data-stu-id="02616-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02616-127">计划</span><span class="sxs-lookup"><span data-stu-id="02616-127">plans</span></span>|<span data-ttu-id="02616-128">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="02616-128">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="02616-129">只读。</span><span class="sxs-lookup"><span data-stu-id="02616-129">Read-only.</span></span> <span data-ttu-id="02616-130">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="02616-130">Nullable.</span></span> <span data-ttu-id="02616-131">返回组所拥有的[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="02616-131">Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02616-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02616-132">JSON representation</span></span>
<span data-ttu-id="02616-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02616-133">Here is a JSON representation of the resource.</span></span>

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
