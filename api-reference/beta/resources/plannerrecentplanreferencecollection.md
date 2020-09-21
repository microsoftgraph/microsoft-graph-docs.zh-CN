---
title: plannerRecentPlanReferenceCollection 资源类型
description: '**PlannerRecentPlanReferenceCollection**资源表示对用户最近查看的计划的引用集合。 此资源是打开的类型，并且是 plannerUser 对象的一部分。 属性名称是对应计划的 ID。 属性-值对中的值是 plannerRecentPlanReference 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 529552be4497729824ddfb9fa9e84ea82e8ccd0d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064003"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a><span data-ttu-id="4502c-106">plannerRecentPlanReferenceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="4502c-106">plannerRecentPlanReferenceCollection resource type</span></span>

<span data-ttu-id="4502c-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4502c-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4502c-108">**PlannerRecentPlanReferenceCollection**资源表示对用户最近查看的计划的引用集合。</span><span class="sxs-lookup"><span data-stu-id="4502c-108">The **plannerRecentPlanReferenceCollection** resource represents the collection of references to plans that were recently viewed by a user.</span></span> <span data-ttu-id="4502c-109">此资源是打开的类型，并且是 [plannerUser](planneruser.md) 对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="4502c-109">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="4502c-110">属性名称是对应计划的 ID。</span><span class="sxs-lookup"><span data-stu-id="4502c-110">The property name is the ID of the corresponding plan.</span></span> <span data-ttu-id="4502c-111">属性-值对中的值是 [plannerRecentPlanReference](plannerrecentplanreference.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4502c-111">The value in the property-value pair is the [plannerRecentPlanReference](plannerrecentplanreference.md) object.</span></span>
<span data-ttu-id="4502c-112">如果将新的引用添加到此集合中，则当集合的大小超过预先确定的最大值时，将自动删除最旧的项。</span><span class="sxs-lookup"><span data-stu-id="4502c-112">Adding new references to this collection will automatically remove the oldest entries when the size of the collection exceeds a predetermined maximum value.</span></span>


## <a name="properties"></a><span data-ttu-id="4502c-113">属性</span><span class="sxs-lookup"><span data-stu-id="4502c-113">Properties</span></span>
<span data-ttu-id="4502c-114">您可以定义此开放类型的属性。</span><span class="sxs-lookup"><span data-stu-id="4502c-114">You can define the properties of this open type.</span></span> <span data-ttu-id="4502c-115">属性名称是 `id` [plannerPlan](plannerplan.md) 资源的值，它们的值必须是 [plannerRecentPlanReference](plannerrecentplanreference.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4502c-115">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerRecentPlanReference](plannerrecentplanreference.md) objects.</span></span> <span data-ttu-id="4502c-116">若要删除收藏夹列表中的项，请将该属性的值设置为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="4502c-116">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="4502c-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4502c-117">JSON representation</span></span>

<span data-ttu-id="4502c-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4502c-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"
}-->

```json
{
  "7oTB5aMIAE2rVo-1N-L7RmQAGX2q": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReference",
    "lastAccessedDateTime": "2017-12-02T22:49:46.155Z",
    "planTitle": "Purchase Workflow"
  },
  "iKNMHkk3vEWpSF7F7iZWIGQAAMMw": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReference",
    "lastAccessedDateTime": "2017-12-03T21:59:28.975Z",
    "planTitle": "New Year's Office Party"
  }
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerRecentPlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


