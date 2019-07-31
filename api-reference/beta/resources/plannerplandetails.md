---
title: plannerPlanDetails 资源类型
description: '**PlannerPlanDetails**资源表示有关计划的其他信息。 每个 plan 对象都有一个详细信息对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 61296138f1477219e85ae7fd372102b8c7fd3a47
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965885"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="8310d-104">plannerPlanDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="8310d-104">plannerPlanDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8310d-105">**PlannerPlanDetails**资源表示有关计划的其他信息。</span><span class="sxs-lookup"><span data-stu-id="8310d-105">The **plannerPlanDetails** resource represents the additional information about a plan.</span></span> <span data-ttu-id="8310d-106">每个[plan](plannerplan.md)对象都有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="8310d-106">Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="8310d-107">方法</span><span class="sxs-lookup"><span data-stu-id="8310d-107">Methods</span></span>

| <span data-ttu-id="8310d-108">方法</span><span class="sxs-lookup"><span data-stu-id="8310d-108">Method</span></span>           | <span data-ttu-id="8310d-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8310d-109">Return Type</span></span>    |<span data-ttu-id="8310d-110">说明</span><span class="sxs-lookup"><span data-stu-id="8310d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8310d-111">获取 plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="8310d-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="8310d-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="8310d-112">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="8310d-113">读取**plannerPlanDetails**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8310d-113">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="8310d-114">更新</span><span class="sxs-lookup"><span data-stu-id="8310d-114">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="8310d-115">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="8310d-115">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="8310d-116">更新**plannerPlanDetails**对象。</span><span class="sxs-lookup"><span data-stu-id="8310d-116">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8310d-117">属性</span><span class="sxs-lookup"><span data-stu-id="8310d-117">Properties</span></span>
| <span data-ttu-id="8310d-118">属性</span><span class="sxs-lookup"><span data-stu-id="8310d-118">Property</span></span>     | <span data-ttu-id="8310d-119">类型</span><span class="sxs-lookup"><span data-stu-id="8310d-119">Type</span></span>   |<span data-ttu-id="8310d-120">说明</span><span class="sxs-lookup"><span data-stu-id="8310d-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8310d-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="8310d-121">categoryDescriptions</span></span>|[<span data-ttu-id="8310d-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="8310d-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="8310d-123">指定可与计划中的任务相关联的六个类别的描述的对象</span><span class="sxs-lookup"><span data-stu-id="8310d-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="8310d-124">id</span><span class="sxs-lookup"><span data-stu-id="8310d-124">id</span></span>|<span data-ttu-id="8310d-125">String</span><span class="sxs-lookup"><span data-stu-id="8310d-125">String</span></span>| <span data-ttu-id="8310d-126">只读。</span><span class="sxs-lookup"><span data-stu-id="8310d-126">Read-only.</span></span> <span data-ttu-id="8310d-127">计划详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="8310d-127">The ID of the plan details.</span></span> <span data-ttu-id="8310d-128">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="8310d-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="8310d-129">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="8310d-129">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="8310d-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="8310d-130">sharedWith</span></span>|[<span data-ttu-id="8310d-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="8310d-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="8310d-132">与之共享此计划的用户 Id 集。</span><span class="sxs-lookup"><span data-stu-id="8310d-132">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="8310d-133">如果使用的是 Office 365 组, 请使用组 API 来管理组成员身份, 以共享[组的](group.md)计划。</span><span class="sxs-lookup"><span data-stu-id="8310d-133">If you are using Office 365 Groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="8310d-134">您还可以将组的现有成员添加到此集合中, 但不需要使其访问组拥有的计划。</span><span class="sxs-lookup"><span data-stu-id="8310d-134">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="8310d-135">contextDetails</span><span class="sxs-lookup"><span data-stu-id="8310d-135">contextDetails</span></span>|[<span data-ttu-id="8310d-136">plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="8310d-136">plannerPlanContextDetailsCollection</span></span>](plannerplancontextdetailscollection.md)|<span data-ttu-id="8310d-137">只读。</span><span class="sxs-lookup"><span data-stu-id="8310d-137">Read-only.</span></span> <span data-ttu-id="8310d-138">与为[plannerPlan](plannerplan.md)容器定义的[plannerPlanContext](plannerplancontext.md)条目相关联的附加信息的集合。</span><span class="sxs-lookup"><span data-stu-id="8310d-138">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8310d-139">关系</span><span class="sxs-lookup"><span data-stu-id="8310d-139">Relationships</span></span>
<span data-ttu-id="8310d-140">无。</span><span class="sxs-lookup"><span data-stu-id="8310d-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="8310d-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8310d-141">JSON representation</span></span>
<span data-ttu-id="8310d-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8310d-142">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
