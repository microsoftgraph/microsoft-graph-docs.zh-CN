---
title: plannerPlanDetails 资源类型
description: '**plannerPlanDetails** 资源表示计划的其他相关信息。每个计划对象均有一个详细信息对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9d10f5b04bc3b98a5e32eac7b577cbf4c582bab4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529878"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="bd787-104">plannerPlanDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="bd787-104">plannerPlanDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd787-p102">**plannerPlanDetails** 资源表示计划的其他相关信息。每个[计划](plannerplan.md)对象均有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="bd787-p102">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="bd787-107">方法</span><span class="sxs-lookup"><span data-stu-id="bd787-107">Methods</span></span>

| <span data-ttu-id="bd787-108">方法</span><span class="sxs-lookup"><span data-stu-id="bd787-108">Method</span></span>           | <span data-ttu-id="bd787-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="bd787-109">Return Type</span></span>    |<span data-ttu-id="bd787-110">说明</span><span class="sxs-lookup"><span data-stu-id="bd787-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bd787-111">Get plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="bd787-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="bd787-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="bd787-112">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="bd787-113">读取的属性和**plannerPlanDetails**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="bd787-113">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="bd787-114">Update</span><span class="sxs-lookup"><span data-stu-id="bd787-114">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="bd787-115">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="bd787-115">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="bd787-116">更新**plannerPlanDetails**对象。</span><span class="sxs-lookup"><span data-stu-id="bd787-116">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bd787-117">属性</span><span class="sxs-lookup"><span data-stu-id="bd787-117">Properties</span></span>
| <span data-ttu-id="bd787-118">属性</span><span class="sxs-lookup"><span data-stu-id="bd787-118">Property</span></span>     | <span data-ttu-id="bd787-119">类型</span><span class="sxs-lookup"><span data-stu-id="bd787-119">Type</span></span>   |<span data-ttu-id="bd787-120">说明</span><span class="sxs-lookup"><span data-stu-id="bd787-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd787-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="bd787-121">categoryDescriptions</span></span>|[<span data-ttu-id="bd787-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="bd787-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="bd787-123">指定可与计划中的任务相关联的六个类别的描述的对象</span><span class="sxs-lookup"><span data-stu-id="bd787-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="bd787-124">id</span><span class="sxs-lookup"><span data-stu-id="bd787-124">id</span></span>|<span data-ttu-id="bd787-125">String</span><span class="sxs-lookup"><span data-stu-id="bd787-125">String</span></span>| <span data-ttu-id="bd787-126">只读。</span><span class="sxs-lookup"><span data-stu-id="bd787-126">Read-only.</span></span> <span data-ttu-id="bd787-127">计划详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="bd787-127">The ID of the plan details.</span></span> <span data-ttu-id="bd787-128">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="bd787-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="bd787-129">服务上执行[格式验证](tasks-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="bd787-129">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="bd787-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="bd787-130">sharedWith</span></span>|[<span data-ttu-id="bd787-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="bd787-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="bd787-132">用户与共享此计划的 Id 集。</span><span class="sxs-lookup"><span data-stu-id="bd787-132">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="bd787-133">如果您使用的 Office 365 组，可以使用组 API 管理组成员身份共享的[组的](group.md)计划。</span><span class="sxs-lookup"><span data-stu-id="bd787-133">If you are using Office 365 Groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="bd787-134">尽管不作要求以便访问计划组拥有的顺序，还可以向此集合中，添加现有组的成员。</span><span class="sxs-lookup"><span data-stu-id="bd787-134">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="bd787-135">contextDetails</span><span class="sxs-lookup"><span data-stu-id="bd787-135">contextDetails</span></span>|[<span data-ttu-id="bd787-136">plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="bd787-136">plannerPlanContextDetailsCollection</span></span>](plannerplancontextdetailscollection.md)|<span data-ttu-id="bd787-137">只读。</span><span class="sxs-lookup"><span data-stu-id="bd787-137">Read-only.</span></span> <span data-ttu-id="bd787-138">定义对[plannerPlan](plannerplan.md)容器的[plannerPlanContext](plannerplancontext.md)条目关联的其他信息的集合。</span><span class="sxs-lookup"><span data-stu-id="bd787-138">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bd787-139">关系</span><span class="sxs-lookup"><span data-stu-id="bd787-139">Relationships</span></span>
<span data-ttu-id="bd787-140">无。</span><span class="sxs-lookup"><span data-stu-id="bd787-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="bd787-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bd787-141">JSON representation</span></span>
<span data-ttu-id="bd787-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd787-142">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplandetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
