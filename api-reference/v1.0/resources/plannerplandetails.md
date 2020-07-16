---
title: plannerPlanDetails 资源类型
description: '**PlannerPlanDetails**资源表示有关计划的其他信息。 每个 plan 对象都有一个详细信息对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: ec6f22b9a14fc25f6c63b3e6e7c93ec66e4741d2
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896999"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="85e18-104">plannerPlanDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="85e18-104">plannerPlanDetails resource type</span></span>

<span data-ttu-id="85e18-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85e18-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="85e18-106">**PlannerPlanDetails**资源表示有关计划的其他信息。</span><span class="sxs-lookup"><span data-stu-id="85e18-106">The **plannerPlanDetails** resource represents the additional information about a plan.</span></span> <span data-ttu-id="85e18-107">每个[plan](plannerplan.md)对象都有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="85e18-107">Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="85e18-108">方法</span><span class="sxs-lookup"><span data-stu-id="85e18-108">Methods</span></span>

| <span data-ttu-id="85e18-109">方法</span><span class="sxs-lookup"><span data-stu-id="85e18-109">Method</span></span>           | <span data-ttu-id="85e18-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="85e18-110">Return Type</span></span>    |<span data-ttu-id="85e18-111">说明</span><span class="sxs-lookup"><span data-stu-id="85e18-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="85e18-112">获取 plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="85e18-112">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="85e18-113">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="85e18-113">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="85e18-114">读取**plannerPlanDetails**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="85e18-114">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="85e18-115">更新</span><span class="sxs-lookup"><span data-stu-id="85e18-115">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="85e18-116">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="85e18-116">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="85e18-117">更新**plannerPlanDetails**对象。</span><span class="sxs-lookup"><span data-stu-id="85e18-117">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="85e18-118">属性</span><span class="sxs-lookup"><span data-stu-id="85e18-118">Properties</span></span>
| <span data-ttu-id="85e18-119">属性</span><span class="sxs-lookup"><span data-stu-id="85e18-119">Property</span></span>     | <span data-ttu-id="85e18-120">类型</span><span class="sxs-lookup"><span data-stu-id="85e18-120">Type</span></span>   |<span data-ttu-id="85e18-121">说明</span><span class="sxs-lookup"><span data-stu-id="85e18-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85e18-122">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="85e18-122">categoryDescriptions</span></span>|[<span data-ttu-id="85e18-123">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="85e18-123">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="85e18-124">指定可与计划中的任务相关联的六个类别的描述的对象</span><span class="sxs-lookup"><span data-stu-id="85e18-124">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="85e18-125">id</span><span class="sxs-lookup"><span data-stu-id="85e18-125">id</span></span>|<span data-ttu-id="85e18-126">String</span><span class="sxs-lookup"><span data-stu-id="85e18-126">String</span></span>| <span data-ttu-id="85e18-127">只读。</span><span class="sxs-lookup"><span data-stu-id="85e18-127">Read-only.</span></span> <span data-ttu-id="85e18-128">计划详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="85e18-128">ID of the plan details.</span></span> <span data-ttu-id="85e18-129">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="85e18-129">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="85e18-130">[格式验证](planner-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="85e18-130">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="85e18-131">sharedWith</span><span class="sxs-lookup"><span data-stu-id="85e18-131">sharedWith</span></span>|[<span data-ttu-id="85e18-132">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="85e18-132">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="85e18-133">与之共享此计划的用户 id 集。</span><span class="sxs-lookup"><span data-stu-id="85e18-133">Set of user ids that this plan is shared with.</span></span> <span data-ttu-id="85e18-134">如果您利用的是 Microsoft 365 组，请使用组 API 来管理组成员身份，以共享[组的](group.md)计划。</span><span class="sxs-lookup"><span data-stu-id="85e18-134">If you are leveraging Microsoft 365 groups, use the Groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="85e18-135">您还可以将组的现有成员添加到此集合中，但它们不需要他们访问该组拥有的计划。</span><span class="sxs-lookup"><span data-stu-id="85e18-135">You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="85e18-136">关系</span><span class="sxs-lookup"><span data-stu-id="85e18-136">Relationships</span></span>
<span data-ttu-id="85e18-137">无</span><span class="sxs-lookup"><span data-stu-id="85e18-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="85e18-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85e18-138">JSON representation</span></span>
<span data-ttu-id="85e18-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85e18-139">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
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
