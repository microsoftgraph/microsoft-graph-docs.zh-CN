---
title: plannerPlanDetails 资源类型
description: '**plannerPlanDetails** 资源表示计划的其他相关信息。每个计划对象均有一个详细信息对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: dfb142c8fbd6b2354a3a2d03d29480d119284146
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942379"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="817cf-104">plannerPlanDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="817cf-104">plannerPlanDetails resource type</span></span>

> <span data-ttu-id="817cf-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="817cf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="817cf-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="817cf-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="817cf-p103">**plannerPlanDetails** 资源表示计划的其他相关信息。每个[计划](plannerplan.md)对象均有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="817cf-p103">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="817cf-109">方法</span><span class="sxs-lookup"><span data-stu-id="817cf-109">Methods</span></span>

| <span data-ttu-id="817cf-110">方法</span><span class="sxs-lookup"><span data-stu-id="817cf-110">Method</span></span>           | <span data-ttu-id="817cf-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="817cf-111">Return Type</span></span>    |<span data-ttu-id="817cf-112">说明</span><span class="sxs-lookup"><span data-stu-id="817cf-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="817cf-113">Get plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="817cf-113">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="817cf-114">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="817cf-114">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="817cf-115">读取的属性和**plannerPlanDetails**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="817cf-115">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="817cf-116">Update</span><span class="sxs-lookup"><span data-stu-id="817cf-116">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="817cf-117">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="817cf-117">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="817cf-118">更新**plannerPlanDetails**对象。</span><span class="sxs-lookup"><span data-stu-id="817cf-118">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="817cf-119">属性</span><span class="sxs-lookup"><span data-stu-id="817cf-119">Properties</span></span>
| <span data-ttu-id="817cf-120">属性</span><span class="sxs-lookup"><span data-stu-id="817cf-120">Property</span></span>     | <span data-ttu-id="817cf-121">类型</span><span class="sxs-lookup"><span data-stu-id="817cf-121">Type</span></span>   |<span data-ttu-id="817cf-122">说明</span><span class="sxs-lookup"><span data-stu-id="817cf-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="817cf-123">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="817cf-123">categoryDescriptions</span></span>|[<span data-ttu-id="817cf-124">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="817cf-124">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="817cf-125">指定可与计划中的任务相关联的六个类别的描述的对象</span><span class="sxs-lookup"><span data-stu-id="817cf-125">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="817cf-126">id</span><span class="sxs-lookup"><span data-stu-id="817cf-126">id</span></span>|<span data-ttu-id="817cf-127">String</span><span class="sxs-lookup"><span data-stu-id="817cf-127">String</span></span>| <span data-ttu-id="817cf-128">只读。</span><span class="sxs-lookup"><span data-stu-id="817cf-128">Read-only.</span></span> <span data-ttu-id="817cf-129">计划详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="817cf-129">The ID of the plan details.</span></span> <span data-ttu-id="817cf-130">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="817cf-130">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="817cf-131">服务上执行[格式验证](tasks-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="817cf-131">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="817cf-132">sharedWith</span><span class="sxs-lookup"><span data-stu-id="817cf-132">sharedWith</span></span>|[<span data-ttu-id="817cf-133">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="817cf-133">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="817cf-134">用户与共享此计划的 Id 集。</span><span class="sxs-lookup"><span data-stu-id="817cf-134">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="817cf-135">如果您使用的 Office 365 组，可以使用组 API 管理组成员身份共享的[组的](group.md)计划。</span><span class="sxs-lookup"><span data-stu-id="817cf-135">If you are using Office 365 Groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="817cf-136">尽管不作要求以便访问计划组拥有的顺序，还可以向此集合中，添加现有组的成员。</span><span class="sxs-lookup"><span data-stu-id="817cf-136">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="817cf-137">contextDetails</span><span class="sxs-lookup"><span data-stu-id="817cf-137">contextDetails</span></span>|[<span data-ttu-id="817cf-138">plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="817cf-138">plannerPlanContextDetailsCollection</span></span>](plannerplancontextdetailscollection.md)|<span data-ttu-id="817cf-139">只读。</span><span class="sxs-lookup"><span data-stu-id="817cf-139">Read-only.</span></span> <span data-ttu-id="817cf-140">定义对[plannerPlan](plannerplan.md)容器的[plannerPlanContext](plannerplancontext.md)条目关联的其他信息的集合。</span><span class="sxs-lookup"><span data-stu-id="817cf-140">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="817cf-141">Relationships</span><span class="sxs-lookup"><span data-stu-id="817cf-141">Relationships</span></span>
<span data-ttu-id="817cf-142">无。</span><span class="sxs-lookup"><span data-stu-id="817cf-142">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="817cf-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="817cf-143">JSON representation</span></span>
<span data-ttu-id="817cf-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="817cf-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "contextDetails": {"@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
