---
title: plannerGroup 资源类型
description: '**plannerGroup**资源提供对组的 Planner 资源的访问。 它不包含任何可用属性。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 84bb20d0b13f9a99db2f8c59b20e0c9c7c87f93f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457030"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="1ff69-104">plannerGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="1ff69-104">plannerGroup resource type</span></span>

<span data-ttu-id="1ff69-105">**plannerGroup**资源提供对[组](group.md)的 Planner 资源的访问。</span><span class="sxs-lookup"><span data-stu-id="1ff69-105">The **plannerGroup** resource provides access to Planner resources for a [group](group.md).</span></span> <span data-ttu-id="1ff69-106">它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="1ff69-106">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="1ff69-107">方法</span><span class="sxs-lookup"><span data-stu-id="1ff69-107">Methods</span></span>

| <span data-ttu-id="1ff69-108">方法</span><span class="sxs-lookup"><span data-stu-id="1ff69-108">Method</span></span>           | <span data-ttu-id="1ff69-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1ff69-109">Return Type</span></span>    |<span data-ttu-id="1ff69-110">说明</span><span class="sxs-lookup"><span data-stu-id="1ff69-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1ff69-111">列出计划</span><span class="sxs-lookup"><span data-stu-id="1ff69-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="1ff69-112">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ff69-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="1ff69-113">获取**plannerPlan**对象集合。</span><span class="sxs-lookup"><span data-stu-id="1ff69-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="1ff69-114">属性</span><span class="sxs-lookup"><span data-stu-id="1ff69-114">Properties</span></span>
| <span data-ttu-id="1ff69-115">属性</span><span class="sxs-lookup"><span data-stu-id="1ff69-115">Property</span></span>     | <span data-ttu-id="1ff69-116">类型</span><span class="sxs-lookup"><span data-stu-id="1ff69-116">Type</span></span>   |<span data-ttu-id="1ff69-117">说明</span><span class="sxs-lookup"><span data-stu-id="1ff69-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ff69-118">id</span><span class="sxs-lookup"><span data-stu-id="1ff69-118">id</span></span>|<span data-ttu-id="1ff69-119">String</span><span class="sxs-lookup"><span data-stu-id="1ff69-119">String</span></span>| <span data-ttu-id="1ff69-120">只读。</span><span class="sxs-lookup"><span data-stu-id="1ff69-120">Read-only.</span></span> <span data-ttu-id="1ff69-121">**plannerGroup**的标识符</span><span class="sxs-lookup"><span data-stu-id="1ff69-121">Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ff69-122">关系</span><span class="sxs-lookup"><span data-stu-id="1ff69-122">Relationships</span></span>
| <span data-ttu-id="1ff69-123">关系</span><span class="sxs-lookup"><span data-stu-id="1ff69-123">Relationship</span></span> | <span data-ttu-id="1ff69-124">类型</span><span class="sxs-lookup"><span data-stu-id="1ff69-124">Type</span></span>   |<span data-ttu-id="1ff69-125">描述</span><span class="sxs-lookup"><span data-stu-id="1ff69-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ff69-126">计划</span><span class="sxs-lookup"><span data-stu-id="1ff69-126">plans</span></span>|<span data-ttu-id="1ff69-127">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ff69-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="1ff69-128">只读。</span><span class="sxs-lookup"><span data-stu-id="1ff69-128">Read-only.</span></span> <span data-ttu-id="1ff69-129">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="1ff69-129">Nullable.</span></span> <span data-ttu-id="1ff69-130">返回组所拥有的[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="1ff69-130">Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1ff69-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1ff69-131">JSON representation</span></span>
<span data-ttu-id="1ff69-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ff69-132">Here is a JSON representation of the resource.</span></span>

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
