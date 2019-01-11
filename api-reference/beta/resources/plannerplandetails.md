---
title: plannerPlanDetails 资源类型
description: '**plannerPlanDetails** 资源表示计划的其他相关信息。每个计划对象均有一个详细信息对象。'
localization_priority: Normal
ms.openlocfilehash: 117a2f69324180a7ef45dcf96c773f510bdbcb9d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860155"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="7d90a-104">plannerPlanDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d90a-104">plannerPlanDetails resource type</span></span>

> <span data-ttu-id="7d90a-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7d90a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d90a-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7d90a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d90a-p103">**plannerPlanDetails** 资源表示计划的其他相关信息。每个[计划](plannerplan.md)对象均有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="7d90a-p103">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="7d90a-109">方法</span><span class="sxs-lookup"><span data-stu-id="7d90a-109">Methods</span></span>

| <span data-ttu-id="7d90a-110">方法</span><span class="sxs-lookup"><span data-stu-id="7d90a-110">Method</span></span>           | <span data-ttu-id="7d90a-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="7d90a-111">Return Type</span></span>    |<span data-ttu-id="7d90a-112">说明</span><span class="sxs-lookup"><span data-stu-id="7d90a-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7d90a-113">Get plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="7d90a-113">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="7d90a-114">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="7d90a-114">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="7d90a-115">读取的属性和**plannerPlanDetails**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="7d90a-115">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="7d90a-116">Update</span><span class="sxs-lookup"><span data-stu-id="7d90a-116">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="7d90a-117">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="7d90a-117">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="7d90a-118">更新**plannerPlanDetails**对象。</span><span class="sxs-lookup"><span data-stu-id="7d90a-118">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7d90a-119">属性</span><span class="sxs-lookup"><span data-stu-id="7d90a-119">Properties</span></span>
| <span data-ttu-id="7d90a-120">属性</span><span class="sxs-lookup"><span data-stu-id="7d90a-120">Property</span></span>     | <span data-ttu-id="7d90a-121">类型</span><span class="sxs-lookup"><span data-stu-id="7d90a-121">Type</span></span>   |<span data-ttu-id="7d90a-122">说明</span><span class="sxs-lookup"><span data-stu-id="7d90a-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d90a-123">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="7d90a-123">categoryDescriptions</span></span>|[<span data-ttu-id="7d90a-124">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="7d90a-124">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="7d90a-125">指定可与计划中的任务相关联的六个类别的描述的对象</span><span class="sxs-lookup"><span data-stu-id="7d90a-125">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="7d90a-126">id</span><span class="sxs-lookup"><span data-stu-id="7d90a-126">id</span></span>|<span data-ttu-id="7d90a-127">String</span><span class="sxs-lookup"><span data-stu-id="7d90a-127">String</span></span>| <span data-ttu-id="7d90a-128">只读。</span><span class="sxs-lookup"><span data-stu-id="7d90a-128">Read-only.</span></span> <span data-ttu-id="7d90a-129">计划详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="7d90a-129">The ID of the plan details.</span></span> <span data-ttu-id="7d90a-130">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="7d90a-130">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="7d90a-131">服务上执行[格式验证](tasks-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="7d90a-131">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="7d90a-132">sharedWith</span><span class="sxs-lookup"><span data-stu-id="7d90a-132">sharedWith</span></span>|[<span data-ttu-id="7d90a-133">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="7d90a-133">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="7d90a-134">用户与共享此计划的 Id 集。</span><span class="sxs-lookup"><span data-stu-id="7d90a-134">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="7d90a-135">如果您使用的 Office 365 组，可以使用组 API 管理组成员身份共享的[组的](group.md)计划。</span><span class="sxs-lookup"><span data-stu-id="7d90a-135">If you are using Office 365 Groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="7d90a-136">尽管不作要求以便访问计划组拥有的顺序，还可以向此集合中，添加现有组的成员。</span><span class="sxs-lookup"><span data-stu-id="7d90a-136">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="7d90a-137">contextDetails</span><span class="sxs-lookup"><span data-stu-id="7d90a-137">contextDetails</span></span>|[<span data-ttu-id="7d90a-138">plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="7d90a-138">plannerPlanContextDetailsCollection</span></span>](plannerplancontextdetailscollection.md)|<span data-ttu-id="7d90a-139">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="7d90a-139">Read-only.</span></span> <span data-ttu-id="7d90a-140">定义对[plannerPlan](plannerplan.md)容器的[plannerPlanContext](plannerplancontext.md)条目关联的其他信息的集合。</span><span class="sxs-lookup"><span data-stu-id="7d90a-140">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7d90a-141">Relationships</span><span class="sxs-lookup"><span data-stu-id="7d90a-141">Relationships</span></span>
<span data-ttu-id="7d90a-142">无。</span><span class="sxs-lookup"><span data-stu-id="7d90a-142">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="7d90a-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d90a-143">JSON representation</span></span>
<span data-ttu-id="7d90a-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d90a-144">The following is a JSON representation of the resource.</span></span>

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
