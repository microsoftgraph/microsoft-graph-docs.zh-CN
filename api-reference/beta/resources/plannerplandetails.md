---
title: plannerPlanDetails 资源类型
description: '**PlannerPlanDetails**资源表示有关计划的其他信息。 每个 plan 对象都有一个详细信息对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 4ec087de509d66f48c8921252cb1b058e6581741
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521676"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="13cbf-104">plannerPlanDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="13cbf-104">plannerPlanDetails resource type</span></span>

<span data-ttu-id="13cbf-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="13cbf-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13cbf-106">**PlannerPlanDetails**资源表示有关计划的其他信息。</span><span class="sxs-lookup"><span data-stu-id="13cbf-106">The **plannerPlanDetails** resource represents the additional information about a plan.</span></span> <span data-ttu-id="13cbf-107">每个[plan](plannerplan.md)对象都有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="13cbf-107">Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="13cbf-108">方法</span><span class="sxs-lookup"><span data-stu-id="13cbf-108">Methods</span></span>

| <span data-ttu-id="13cbf-109">方法</span><span class="sxs-lookup"><span data-stu-id="13cbf-109">Method</span></span>           | <span data-ttu-id="13cbf-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="13cbf-110">Return Type</span></span>    |<span data-ttu-id="13cbf-111">说明</span><span class="sxs-lookup"><span data-stu-id="13cbf-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="13cbf-112">获取 plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="13cbf-112">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="13cbf-113">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="13cbf-113">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="13cbf-114">读取**plannerPlanDetails**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="13cbf-114">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="13cbf-115">更新</span><span class="sxs-lookup"><span data-stu-id="13cbf-115">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="13cbf-116">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="13cbf-116">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="13cbf-117">更新**plannerPlanDetails**对象。</span><span class="sxs-lookup"><span data-stu-id="13cbf-117">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="13cbf-118">属性</span><span class="sxs-lookup"><span data-stu-id="13cbf-118">Properties</span></span>
| <span data-ttu-id="13cbf-119">属性</span><span class="sxs-lookup"><span data-stu-id="13cbf-119">Property</span></span>     | <span data-ttu-id="13cbf-120">类型</span><span class="sxs-lookup"><span data-stu-id="13cbf-120">Type</span></span>   |<span data-ttu-id="13cbf-121">说明</span><span class="sxs-lookup"><span data-stu-id="13cbf-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13cbf-122">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="13cbf-122">categoryDescriptions</span></span>|[<span data-ttu-id="13cbf-123">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="13cbf-123">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="13cbf-124">指定可与计划中的任务相关联的六个类别的描述的对象</span><span class="sxs-lookup"><span data-stu-id="13cbf-124">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="13cbf-125">id</span><span class="sxs-lookup"><span data-stu-id="13cbf-125">id</span></span>|<span data-ttu-id="13cbf-126">String</span><span class="sxs-lookup"><span data-stu-id="13cbf-126">String</span></span>| <span data-ttu-id="13cbf-127">只读。</span><span class="sxs-lookup"><span data-stu-id="13cbf-127">Read-only.</span></span> <span data-ttu-id="13cbf-128">计划详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="13cbf-128">The ID of the plan details.</span></span> <span data-ttu-id="13cbf-129">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="13cbf-129">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="13cbf-130">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="13cbf-130">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="13cbf-131">sharedWith</span><span class="sxs-lookup"><span data-stu-id="13cbf-131">sharedWith</span></span>|[<span data-ttu-id="13cbf-132">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="13cbf-132">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="13cbf-133">与之共享此计划的用户 Id 集。</span><span class="sxs-lookup"><span data-stu-id="13cbf-133">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="13cbf-134">如果使用的是 Office 365 组，请使用组 API 来管理组成员身份，以共享[组的](group.md)计划。</span><span class="sxs-lookup"><span data-stu-id="13cbf-134">If you are using Office 365 Groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="13cbf-135">您还可以将组的现有成员添加到此集合中，但不需要使其访问组拥有的计划。</span><span class="sxs-lookup"><span data-stu-id="13cbf-135">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="13cbf-136">contextDetails</span><span class="sxs-lookup"><span data-stu-id="13cbf-136">contextDetails</span></span>|[<span data-ttu-id="13cbf-137">plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="13cbf-137">plannerPlanContextDetailsCollection</span></span>](plannerplancontextdetailscollection.md)|<span data-ttu-id="13cbf-138">只读。</span><span class="sxs-lookup"><span data-stu-id="13cbf-138">Read-only.</span></span> <span data-ttu-id="13cbf-139">与为[plannerPlan](plannerplan.md)容器定义的[plannerPlanContext](plannerplancontext.md)条目相关联的附加信息的集合。</span><span class="sxs-lookup"><span data-stu-id="13cbf-139">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="13cbf-140">关系</span><span class="sxs-lookup"><span data-stu-id="13cbf-140">Relationships</span></span>
<span data-ttu-id="13cbf-141">无。</span><span class="sxs-lookup"><span data-stu-id="13cbf-141">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="13cbf-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13cbf-142">JSON representation</span></span>
<span data-ttu-id="13cbf-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13cbf-143">The following is a JSON representation of the resource.</span></span>

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
