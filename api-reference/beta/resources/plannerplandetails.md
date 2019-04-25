---
title: plannerPlanDetails 资源类型
description: '**plannerPlanDetails**资源表示有关计划的其他信息。 每个 plan 对象都有一个详细信息对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9d10f5b04bc3b98a5e32eac7b577cbf4c582bab4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522130"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="75d37-104">plannerPlanDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="75d37-104">plannerPlanDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75d37-105">**plannerPlanDetails**资源表示有关计划的其他信息。</span><span class="sxs-lookup"><span data-stu-id="75d37-105">The **plannerPlanDetails** resource represents the additional information about a plan.</span></span> <span data-ttu-id="75d37-106">每个[plan](plannerplan.md)对象都有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="75d37-106">Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="75d37-107">方法</span><span class="sxs-lookup"><span data-stu-id="75d37-107">Methods</span></span>

| <span data-ttu-id="75d37-108">方法</span><span class="sxs-lookup"><span data-stu-id="75d37-108">Method</span></span>           | <span data-ttu-id="75d37-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="75d37-109">Return Type</span></span>    |<span data-ttu-id="75d37-110">说明</span><span class="sxs-lookup"><span data-stu-id="75d37-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="75d37-111">获取 plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="75d37-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="75d37-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="75d37-112">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="75d37-113">读取**plannerPlanDetails**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="75d37-113">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="75d37-114">更新</span><span class="sxs-lookup"><span data-stu-id="75d37-114">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="75d37-115">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="75d37-115">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="75d37-116">更新**plannerPlanDetails**对象。</span><span class="sxs-lookup"><span data-stu-id="75d37-116">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="75d37-117">属性</span><span class="sxs-lookup"><span data-stu-id="75d37-117">Properties</span></span>
| <span data-ttu-id="75d37-118">属性</span><span class="sxs-lookup"><span data-stu-id="75d37-118">Property</span></span>     | <span data-ttu-id="75d37-119">类型</span><span class="sxs-lookup"><span data-stu-id="75d37-119">Type</span></span>   |<span data-ttu-id="75d37-120">说明</span><span class="sxs-lookup"><span data-stu-id="75d37-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75d37-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="75d37-121">categoryDescriptions</span></span>|[<span data-ttu-id="75d37-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="75d37-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="75d37-123">指定可与计划中的任务相关联的六个类别的描述的对象</span><span class="sxs-lookup"><span data-stu-id="75d37-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="75d37-124">id</span><span class="sxs-lookup"><span data-stu-id="75d37-124">id</span></span>|<span data-ttu-id="75d37-125">String</span><span class="sxs-lookup"><span data-stu-id="75d37-125">String</span></span>| <span data-ttu-id="75d37-126">只读。</span><span class="sxs-lookup"><span data-stu-id="75d37-126">Read-only.</span></span> <span data-ttu-id="75d37-127">计划详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="75d37-127">The ID of the plan details.</span></span> <span data-ttu-id="75d37-128">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="75d37-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="75d37-129">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="75d37-129">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="75d37-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="75d37-130">sharedWith</span></span>|[<span data-ttu-id="75d37-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="75d37-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="75d37-132">与之共享此计划的用户 id 集。</span><span class="sxs-lookup"><span data-stu-id="75d37-132">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="75d37-133">如果使用的是 Office 365 组, 请使用组 API 来管理组成员身份, 以共享[组的](group.md)计划。</span><span class="sxs-lookup"><span data-stu-id="75d37-133">If you are using Office 365 Groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="75d37-134">您还可以将组的现有成员添加到此集合中, 但不需要使其访问组拥有的计划。</span><span class="sxs-lookup"><span data-stu-id="75d37-134">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="75d37-135">contextDetails</span><span class="sxs-lookup"><span data-stu-id="75d37-135">contextDetails</span></span>|[<span data-ttu-id="75d37-136">plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="75d37-136">plannerPlanContextDetailsCollection</span></span>](plannerplancontextdetailscollection.md)|<span data-ttu-id="75d37-137">只读。</span><span class="sxs-lookup"><span data-stu-id="75d37-137">Read-only.</span></span> <span data-ttu-id="75d37-138">与为[plannerPlan](plannerplan.md)容器定义的[plannerPlanContext](plannerplancontext.md)条目相关联的附加信息的集合。</span><span class="sxs-lookup"><span data-stu-id="75d37-138">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="75d37-139">关系</span><span class="sxs-lookup"><span data-stu-id="75d37-139">Relationships</span></span>
<span data-ttu-id="75d37-140">无。</span><span class="sxs-lookup"><span data-stu-id="75d37-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="75d37-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="75d37-141">JSON representation</span></span>
<span data-ttu-id="75d37-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75d37-142">The following is a JSON representation of the resource.</span></span>

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
