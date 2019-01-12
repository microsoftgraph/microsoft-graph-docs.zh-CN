---
title: plannerGroup 资源类型
description: '**PlannerGroup**资源为组提供计划工具资源的访问权限。 它不包含任何可用的属性。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 54b6b1d61a98aae3918fd3fcb888f470179ece15
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961706"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="22948-104">plannerGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="22948-104">plannerGroup resource type</span></span>

> <span data-ttu-id="22948-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="22948-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22948-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="22948-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22948-p103">**plannerGroup** 资源提供[组](group.md)的 Planner 资源的访问权限。它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="22948-p103">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="22948-109">方法</span><span class="sxs-lookup"><span data-stu-id="22948-109">Methods</span></span>

| <span data-ttu-id="22948-110">方法</span><span class="sxs-lookup"><span data-stu-id="22948-110">Method</span></span>           | <span data-ttu-id="22948-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="22948-111">Return Type</span></span>    |<span data-ttu-id="22948-112">说明</span><span class="sxs-lookup"><span data-stu-id="22948-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="22948-113">List plans</span><span class="sxs-lookup"><span data-stu-id="22948-113">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="22948-114">[plannerPlan](plannerplan.md) collection</span><span class="sxs-lookup"><span data-stu-id="22948-114">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="22948-115">获取 **plannerPlan** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="22948-115">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="22948-116">属性</span><span class="sxs-lookup"><span data-stu-id="22948-116">Properties</span></span>
| <span data-ttu-id="22948-117">属性</span><span class="sxs-lookup"><span data-stu-id="22948-117">Property</span></span>     | <span data-ttu-id="22948-118">类型</span><span class="sxs-lookup"><span data-stu-id="22948-118">Type</span></span>   |<span data-ttu-id="22948-119">说明</span><span class="sxs-lookup"><span data-stu-id="22948-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22948-120">id</span><span class="sxs-lookup"><span data-stu-id="22948-120">id</span></span>|<span data-ttu-id="22948-121">String</span><span class="sxs-lookup"><span data-stu-id="22948-121">String</span></span>| <span data-ttu-id="22948-p104">只读。**plannerGroup** 的标识符</span><span class="sxs-lookup"><span data-stu-id="22948-p104">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="22948-124">关系</span><span class="sxs-lookup"><span data-stu-id="22948-124">Relationships</span></span>
| <span data-ttu-id="22948-125">关系</span><span class="sxs-lookup"><span data-stu-id="22948-125">Relationship</span></span> | <span data-ttu-id="22948-126">类型</span><span class="sxs-lookup"><span data-stu-id="22948-126">Type</span></span>   |<span data-ttu-id="22948-127">说明</span><span class="sxs-lookup"><span data-stu-id="22948-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22948-128">plans</span><span class="sxs-lookup"><span data-stu-id="22948-128">plans</span></span>|<span data-ttu-id="22948-129">[plannerPlan](plannerplan.md) collection</span><span class="sxs-lookup"><span data-stu-id="22948-129">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="22948-p105">只读。可为 NULL。返回组拥有的 [plannerPlans](plannerplan.md)。</span><span class="sxs-lookup"><span data-stu-id="22948-p105">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22948-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22948-133">JSON representation</span></span>
<span data-ttu-id="22948-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22948-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
