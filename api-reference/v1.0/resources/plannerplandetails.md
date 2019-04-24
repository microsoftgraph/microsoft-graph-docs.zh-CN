---
title: plannerPlanDetails 资源类型
description: '**plannerPlanDetails**资源表示有关计划的其他信息。 每个 plan 对象都有一个详细信息对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5661477ff59036e633eb82c23e9c50d7c2c8b4a9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462329"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="2d206-104">plannerPlanDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="2d206-104">plannerPlanDetails resource type</span></span>


<span data-ttu-id="2d206-105">**plannerPlanDetails**资源表示有关计划的其他信息。</span><span class="sxs-lookup"><span data-stu-id="2d206-105">The **plannerPlanDetails** resource represents the additional information about a plan.</span></span> <span data-ttu-id="2d206-106">每个[plan](plannerplan.md)对象都有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="2d206-106">Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="2d206-107">方法</span><span class="sxs-lookup"><span data-stu-id="2d206-107">Methods</span></span>

| <span data-ttu-id="2d206-108">方法</span><span class="sxs-lookup"><span data-stu-id="2d206-108">Method</span></span>           | <span data-ttu-id="2d206-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2d206-109">Return Type</span></span>    |<span data-ttu-id="2d206-110">说明</span><span class="sxs-lookup"><span data-stu-id="2d206-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2d206-111">获取 plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="2d206-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="2d206-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="2d206-112">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="2d206-113">读取**plannerPlanDetails**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2d206-113">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="2d206-114">更新</span><span class="sxs-lookup"><span data-stu-id="2d206-114">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="2d206-115">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="2d206-115">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="2d206-116">更新**plannerPlanDetails**对象。</span><span class="sxs-lookup"><span data-stu-id="2d206-116">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2d206-117">属性</span><span class="sxs-lookup"><span data-stu-id="2d206-117">Properties</span></span>
| <span data-ttu-id="2d206-118">属性</span><span class="sxs-lookup"><span data-stu-id="2d206-118">Property</span></span>     | <span data-ttu-id="2d206-119">类型</span><span class="sxs-lookup"><span data-stu-id="2d206-119">Type</span></span>   |<span data-ttu-id="2d206-120">说明</span><span class="sxs-lookup"><span data-stu-id="2d206-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d206-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="2d206-121">categoryDescriptions</span></span>|[<span data-ttu-id="2d206-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="2d206-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="2d206-123">指定可与计划中的任务相关联的六个类别的描述的对象</span><span class="sxs-lookup"><span data-stu-id="2d206-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="2d206-124">id</span><span class="sxs-lookup"><span data-stu-id="2d206-124">id</span></span>|<span data-ttu-id="2d206-125">String</span><span class="sxs-lookup"><span data-stu-id="2d206-125">String</span></span>| <span data-ttu-id="2d206-126">只读。</span><span class="sxs-lookup"><span data-stu-id="2d206-126">Read-only.</span></span> <span data-ttu-id="2d206-127">计划详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="2d206-127">ID of the plan details.</span></span> <span data-ttu-id="2d206-128">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="2d206-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="2d206-129">[格式验证](planner-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="2d206-129">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="2d206-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="2d206-130">sharedWith</span></span>|[<span data-ttu-id="2d206-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="2d206-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="2d206-p104">此计划共享的用户 id 集合。如果你正在利用 Office 365 组，使用组 API 管理组成员身份以共享[组的](group.md)计划。你还可以将现有的组成员添加到此集合，尽管他们无需访问组拥有的计划。</span><span class="sxs-lookup"><span data-stu-id="2d206-p104">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2d206-135">关系</span><span class="sxs-lookup"><span data-stu-id="2d206-135">Relationships</span></span>
<span data-ttu-id="2d206-136">无</span><span class="sxs-lookup"><span data-stu-id="2d206-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2d206-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d206-137">JSON representation</span></span>
<span data-ttu-id="2d206-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d206-138">Here is a JSON representation of the resource.</span></span>

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
