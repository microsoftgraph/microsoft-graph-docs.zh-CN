---
title: plannerUser 资源类型
description: 为用户提供**plannerUser**资源计划工具资源的访问权限。 它不包含任何可用的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b73e422e232a96068f4545def0f0fdbd9f74ff07
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953553"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="d7fd8-104">plannerUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7fd8-104">plannerUser resource type</span></span>

<span data-ttu-id="d7fd8-p102">**plannerUser** 资源提供[用户](user.md)的 Planner 资源的访问权限。它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="d7fd8-p102">The **plannerUser** resource provide access to Planner resources for a [user](user.md). It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="d7fd8-107">方法</span><span class="sxs-lookup"><span data-stu-id="d7fd8-107">Methods</span></span>

| <span data-ttu-id="d7fd8-108">方法</span><span class="sxs-lookup"><span data-stu-id="d7fd8-108">Method</span></span>           | <span data-ttu-id="d7fd8-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d7fd8-109">Return Type</span></span>    |<span data-ttu-id="d7fd8-110">说明</span><span class="sxs-lookup"><span data-stu-id="d7fd8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d7fd8-111">List plans</span><span class="sxs-lookup"><span data-stu-id="d7fd8-111">List plans</span></span>](../api/planneruser-list-plans.md) |<span data-ttu-id="d7fd8-112">[plannerPlan](plannerplan.md) collection</span><span class="sxs-lookup"><span data-stu-id="d7fd8-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="d7fd8-113">获取 **plannerPlan** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d7fd8-113">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="d7fd8-114">List tasks</span><span class="sxs-lookup"><span data-stu-id="d7fd8-114">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="d7fd8-115">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="d7fd8-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d7fd8-116">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d7fd8-116">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="d7fd8-117">属性</span><span class="sxs-lookup"><span data-stu-id="d7fd8-117">Properties</span></span>
| <span data-ttu-id="d7fd8-118">属性</span><span class="sxs-lookup"><span data-stu-id="d7fd8-118">Property</span></span>     | <span data-ttu-id="d7fd8-119">类型</span><span class="sxs-lookup"><span data-stu-id="d7fd8-119">Type</span></span>   |<span data-ttu-id="d7fd8-120">说明</span><span class="sxs-lookup"><span data-stu-id="d7fd8-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7fd8-121">id</span><span class="sxs-lookup"><span data-stu-id="d7fd8-121">id</span></span>|<span data-ttu-id="d7fd8-122">字符串</span><span class="sxs-lookup"><span data-stu-id="d7fd8-122">String</span></span>| <span data-ttu-id="d7fd8-p103">只读。planenrUser 的标识符</span><span class="sxs-lookup"><span data-stu-id="d7fd8-p103">Read-only. Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7fd8-125">关系</span><span class="sxs-lookup"><span data-stu-id="d7fd8-125">Relationships</span></span>
| <span data-ttu-id="d7fd8-126">关系</span><span class="sxs-lookup"><span data-stu-id="d7fd8-126">Relationship</span></span> | <span data-ttu-id="d7fd8-127">类型</span><span class="sxs-lookup"><span data-stu-id="d7fd8-127">Type</span></span>   |<span data-ttu-id="d7fd8-128">说明</span><span class="sxs-lookup"><span data-stu-id="d7fd8-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7fd8-129">plans</span><span class="sxs-lookup"><span data-stu-id="d7fd8-129">plans</span></span>|<span data-ttu-id="d7fd8-130">[plannerPlan](plannerplan.md) collection</span><span class="sxs-lookup"><span data-stu-id="d7fd8-130">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="d7fd8-p104">只读。可为 NULL。返回分配给用户的 [plannerTasks](plannertask.md)。</span><span class="sxs-lookup"><span data-stu-id="d7fd8-p104">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="d7fd8-134">tasks</span><span class="sxs-lookup"><span data-stu-id="d7fd8-134">tasks</span></span>|<span data-ttu-id="d7fd8-135">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="d7fd8-135">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d7fd8-p105">只读。可为 NULL。返回与用户共享的 [plannerPlans](plannerplan.md)。</span><span class="sxs-lookup"><span data-stu-id="d7fd8-p105">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7fd8-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7fd8-139">JSON representation</span></span>
<span data-ttu-id="d7fd8-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7fd8-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
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
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
