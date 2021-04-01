---
title: plannerPlanContainer 资源类型
description: 表示 plannerPlan 的容器。 容器是指定授权规则和计划的生命周期的资源。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: acb7a85683bc94795953e524ee9630d6cfc01f24
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473883"
---
# <a name="plannerplancontainer-resource-type"></a><span data-ttu-id="c3b71-104">plannerPlanContainer 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3b71-104">plannerPlanContainer resource type</span></span>

<span data-ttu-id="c3b71-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3b71-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3b71-106">表示 [plannerPlan 的容器](plannerPlan.md)。</span><span class="sxs-lookup"><span data-stu-id="c3b71-106">Represents a container for a [plannerPlan](plannerPlan.md).</span></span> <span data-ttu-id="c3b71-107">容器是指定授权规则和计划的生命周期的资源。</span><span class="sxs-lookup"><span data-stu-id="c3b71-107">The container is a resource that specifies authorization rules and the lifetime of the plan.</span></span> <span data-ttu-id="c3b71-108">这意味着只有有权使用包含计划的资源的人员才能使用计划及其中的任务。</span><span class="sxs-lookup"><span data-stu-id="c3b71-108">This means that only the people who are authorized to work with the resource containing the plan will be able to work with the plan and the tasks within it.</span></span> <span data-ttu-id="c3b71-109">删除包含的资源时，还将删除包含的计划。</span><span class="sxs-lookup"><span data-stu-id="c3b71-109">When the containing resource is deleted, the contained plans are also deleted.</span></span> <span data-ttu-id="c3b71-110">**plannerPlanContainer** 的属性无法在计划创建后更改。</span><span class="sxs-lookup"><span data-stu-id="c3b71-110">Properties of **plannerPlanContainer** cannot be changed after the plan is created.</span></span>

<span data-ttu-id="c3b71-111">Planner 当前支持下表中列出的容器类型。</span><span class="sxs-lookup"><span data-stu-id="c3b71-111">Planner currently supports the container types listed in the following table.</span></span> <span data-ttu-id="c3b71-112">创建计划时，必须使用表中标识的资源的路径指定 **containerUrl** 属性。</span><span class="sxs-lookup"><span data-stu-id="c3b71-112">When creating a plan, the **containerUrl** property must be specified with the path of the resource identified in the table.</span></span>

|<span data-ttu-id="c3b71-113">类型</span><span class="sxs-lookup"><span data-stu-id="c3b71-113">Type</span></span>|<span data-ttu-id="c3b71-114">说明</span><span class="sxs-lookup"><span data-stu-id="c3b71-114">Description</span></span>|<span data-ttu-id="c3b71-115">资源的路径</span><span class="sxs-lookup"><span data-stu-id="c3b71-115">Path to the resource</span></span>|
|----|-----------|--------------------|
|<span data-ttu-id="c3b71-116">group</span><span class="sxs-lookup"><span data-stu-id="c3b71-116">group</span></span>| <span data-ttu-id="c3b71-117">计划包含在组 [中](group.md)。</span><span class="sxs-lookup"><span data-stu-id="c3b71-117">Plan is contained by a [group](group.md).</span></span>| <span data-ttu-id="c3b71-118"> https://graph.microsoft.com/beta/groups/&lt;id&gt;</span><span class="sxs-lookup"><span data-stu-id="c3b71-118">https://graph.microsoft.com/beta/groups/&lt;id&gt;</span></span>|
|<span data-ttu-id="c3b71-119">roster</span><span class="sxs-lookup"><span data-stu-id="c3b71-119">roster</span></span>| <span data-ttu-id="c3b71-120">计划包含在 [plannerRoster 中](plannerroster.md)</span><span class="sxs-lookup"><span data-stu-id="c3b71-120">Plan is contained by a [plannerRoster](plannerroster.md)</span></span> | <span data-ttu-id="c3b71-121"> https://graph.microsoft.com/beta/planner/rosters/&lt;id&gt;</span><span class="sxs-lookup"><span data-stu-id="c3b71-121">https://graph.microsoft.com/beta/planner/rosters/&lt;id&gt;</span></span>|

## <a name="properties"></a><span data-ttu-id="c3b71-122">属性</span><span class="sxs-lookup"><span data-stu-id="c3b71-122">Properties</span></span>
|<span data-ttu-id="c3b71-123">属性</span><span class="sxs-lookup"><span data-stu-id="c3b71-123">Property</span></span>|<span data-ttu-id="c3b71-124">类型</span><span class="sxs-lookup"><span data-stu-id="c3b71-124">Type</span></span>|<span data-ttu-id="c3b71-125">说明</span><span class="sxs-lookup"><span data-stu-id="c3b71-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3b71-126">containerId</span><span class="sxs-lookup"><span data-stu-id="c3b71-126">containerId</span></span>|<span data-ttu-id="c3b71-127">String</span><span class="sxs-lookup"><span data-stu-id="c3b71-127">String</span></span>|<span data-ttu-id="c3b71-128">包含计划的资源的标识符。</span><span class="sxs-lookup"><span data-stu-id="c3b71-128">The identifier of the resource that contains the plan.</span></span>|
|<span data-ttu-id="c3b71-129">type</span><span class="sxs-lookup"><span data-stu-id="c3b71-129">type</span></span>|<span data-ttu-id="c3b71-130">plannerContainerType</span><span class="sxs-lookup"><span data-stu-id="c3b71-130">plannerContainerType</span></span>| <span data-ttu-id="c3b71-131">包含计划的资源的类型。</span><span class="sxs-lookup"><span data-stu-id="c3b71-131">The type of the resource that contains the plan.</span></span> <span data-ttu-id="c3b71-132">有关支持的类型，请参阅上表。</span><span class="sxs-lookup"><span data-stu-id="c3b71-132">See the previous table for supported types.</span></span> <span data-ttu-id="c3b71-133">可取值为：`group`、`roster`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c3b71-133">Possible values are: `group`, `roster`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c3b71-134">url</span><span class="sxs-lookup"><span data-stu-id="c3b71-134">url</span></span>|<span data-ttu-id="c3b71-135">String</span><span class="sxs-lookup"><span data-stu-id="c3b71-135">String</span></span>|<span data-ttu-id="c3b71-136">容器的完整规范 URL。</span><span class="sxs-lookup"><span data-stu-id="c3b71-136">The full canonical URL of the container.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3b71-137">关系</span><span class="sxs-lookup"><span data-stu-id="c3b71-137">Relationships</span></span>
<span data-ttu-id="c3b71-138">无。</span><span class="sxs-lookup"><span data-stu-id="c3b71-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3b71-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3b71-139">JSON representation</span></span>
<span data-ttu-id="c3b71-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3b71-140">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerPlanContainer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerPlanContainer",
  "url": "String",
  "containerId": "String",
  "type": "String"
}
```

