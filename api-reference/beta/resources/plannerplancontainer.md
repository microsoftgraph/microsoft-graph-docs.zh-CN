---
title: plannerPlanContainer 资源类型
description: 表示 plannerPlan 的容器。 容器是指定授权规则和计划的生存期的资源。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8b3abb10892077159e6f02c33a31d501a75dba2a
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883231"
---
# <a name="plannerplancontainer-resource-type"></a><span data-ttu-id="4918e-104">plannerPlanContainer 资源类型</span><span class="sxs-lookup"><span data-stu-id="4918e-104">plannerPlanContainer resource type</span></span>

<span data-ttu-id="4918e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4918e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4918e-106">表示 [plannerPlan 的容器](plannerPlan.md)。</span><span class="sxs-lookup"><span data-stu-id="4918e-106">Represents a container for a [plannerPlan](plannerPlan.md).</span></span> <span data-ttu-id="4918e-107">容器是指定授权规则和计划的生存期的资源。</span><span class="sxs-lookup"><span data-stu-id="4918e-107">The container is a resource that specifies authorization rules and the lifetime of the plan.</span></span> <span data-ttu-id="4918e-108">这意味着只有有权使用包含计划的资源的人员才能使用计划及其中的任务。</span><span class="sxs-lookup"><span data-stu-id="4918e-108">This means that only the people who are authorized to work with the resource containing the plan will be able to work with the plan and the tasks within it.</span></span> <span data-ttu-id="4918e-109">删除包含的资源时，也会删除包含的计划。</span><span class="sxs-lookup"><span data-stu-id="4918e-109">When the containing resource is deleted, the contained plans are also deleted.</span></span> <span data-ttu-id="4918e-110">**plannerPlanContainer** 的属性在计划创建后无法更改。</span><span class="sxs-lookup"><span data-stu-id="4918e-110">Properties of **plannerPlanContainer** cannot be changed after the plan is created.</span></span>

<span data-ttu-id="4918e-111">Planner 当前支持下表中列出的容器类型。</span><span class="sxs-lookup"><span data-stu-id="4918e-111">Planner currently supports the container types listed in the following table.</span></span> <span data-ttu-id="4918e-112">创建计划时，必须使用表中标识的资源的路径指定 **containerUrl** 属性。</span><span class="sxs-lookup"><span data-stu-id="4918e-112">When creating a plan, the **containerUrl** property must be specified with the path of the resource identified in the table.</span></span>

|<span data-ttu-id="4918e-113">类型</span><span class="sxs-lookup"><span data-stu-id="4918e-113">Type</span></span>|<span data-ttu-id="4918e-114">Description</span><span class="sxs-lookup"><span data-stu-id="4918e-114">Description</span></span>|<span data-ttu-id="4918e-115">资源的路径</span><span class="sxs-lookup"><span data-stu-id="4918e-115">Path to the resource</span></span>|
|----|-----------|--------------------|
|<span data-ttu-id="4918e-116">group</span><span class="sxs-lookup"><span data-stu-id="4918e-116">group</span></span>| <span data-ttu-id="4918e-117">计划包含在组内。</span><span class="sxs-lookup"><span data-stu-id="4918e-117">Plan is contained by a group.</span></span>| <span data-ttu-id="4918e-118"> https://graph.microsoft.com/v1.0/groups/&lt;id&gt;</span><span class="sxs-lookup"><span data-stu-id="4918e-118">https://graph.microsoft.com/v1.0/groups/&lt;id&gt;</span></span>|

## <a name="properties"></a><span data-ttu-id="4918e-119">属性</span><span class="sxs-lookup"><span data-stu-id="4918e-119">Properties</span></span>
|<span data-ttu-id="4918e-120">属性</span><span class="sxs-lookup"><span data-stu-id="4918e-120">Property</span></span>|<span data-ttu-id="4918e-121">类型</span><span class="sxs-lookup"><span data-stu-id="4918e-121">Type</span></span>|<span data-ttu-id="4918e-122">Description</span><span class="sxs-lookup"><span data-stu-id="4918e-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4918e-123">containerId</span><span class="sxs-lookup"><span data-stu-id="4918e-123">containerId</span></span>|<span data-ttu-id="4918e-124">String</span><span class="sxs-lookup"><span data-stu-id="4918e-124">String</span></span>|<span data-ttu-id="4918e-125">包含计划的资源的标识符。</span><span class="sxs-lookup"><span data-stu-id="4918e-125">The identifier of the resource that contains the plan.</span></span>|
|<span data-ttu-id="4918e-126">type</span><span class="sxs-lookup"><span data-stu-id="4918e-126">type</span></span>|<span data-ttu-id="4918e-127">plannerContainerType</span><span class="sxs-lookup"><span data-stu-id="4918e-127">plannerContainerType</span></span>| <span data-ttu-id="4918e-128">包含计划的资源的类型。</span><span class="sxs-lookup"><span data-stu-id="4918e-128">The type of the resource that contains the plan.</span></span> <span data-ttu-id="4918e-129">有关支持的类型，请参阅上表。</span><span class="sxs-lookup"><span data-stu-id="4918e-129">See the previous table for supported types.</span></span> <span data-ttu-id="4918e-130">可取值为：`group`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="4918e-130">Possible values are: `group`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4918e-131">url</span><span class="sxs-lookup"><span data-stu-id="4918e-131">url</span></span>|<span data-ttu-id="4918e-132">String</span><span class="sxs-lookup"><span data-stu-id="4918e-132">String</span></span>|<span data-ttu-id="4918e-133">容器的完整规范 URL。</span><span class="sxs-lookup"><span data-stu-id="4918e-133">The full canonical URL of the container.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4918e-134">关系</span><span class="sxs-lookup"><span data-stu-id="4918e-134">Relationships</span></span>
<span data-ttu-id="4918e-135">无。</span><span class="sxs-lookup"><span data-stu-id="4918e-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4918e-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4918e-136">JSON representation</span></span>
<span data-ttu-id="4918e-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4918e-137">The following is a JSON representation of the resource.</span></span>
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

