---
title: plannerFavoritePlanReferenceCollection 资源类型
description: " 值是 plannerFavoritePlanReference 对象。"
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 67149f0ccf8ec04fe702a0d77b1fb2f5f6020365
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965945"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a><span data-ttu-id="6ef7f-103">plannerFavoritePlanReferenceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ef7f-103">plannerFavoritePlanReferenceCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ef7f-104">**PlannerFavoritePlanReferenceCollection**资源表示对计划的引用的集合, 这些计划被用户标记为收藏。</span><span class="sxs-lookup"><span data-stu-id="6ef7f-104">The **plannerFavoritePlanReferenceCollection** resource represents the collection of references to plans that are marked as a favorite by a user.</span></span> <span data-ttu-id="6ef7f-105">此资源是打开的类型, 并且是[plannerUser](planneruser.md)对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="6ef7f-105">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="6ef7f-106">属性值对中的属性名称是对应计划的 ID;值是[plannerFavoritePlanReference](plannerfavoriteplanreference.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6ef7f-106">The property name in the property-value pair is the ID of the corresponding plan; the value is the [plannerFavoritePlanReference](plannerfavoriteplanreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="6ef7f-107">属性</span><span class="sxs-lookup"><span data-stu-id="6ef7f-107">Properties</span></span>
<span data-ttu-id="6ef7f-108">您可以定义此开放类型的属性。</span><span class="sxs-lookup"><span data-stu-id="6ef7f-108">You can define the properties of this open type.</span></span> <span data-ttu-id="6ef7f-109">属性名称是`id` [plannerPlan](plannerplan.md)资源的值, 它们的值必须是[plannerFavoritePlanReference](plannerfavoriteplanreference.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6ef7f-109">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerFavoritePlanReference](plannerfavoriteplanreference.md) objects.</span></span> <span data-ttu-id="6ef7f-110">若要删除收藏夹列表中的项, 请将该属性的值设置`null`为。</span><span class="sxs-lookup"><span data-stu-id="6ef7f-110">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="6ef7f-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ef7f-111">JSON representation</span></span>

<span data-ttu-id="6ef7f-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ef7f-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"
}-->

```json
{
  "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReference",
    "orderHint": "8586866870001551087",
    "planTitle": "Customer reviews"
  },
  "uZWtCtli30CGoWLIWSat1mQAC0ai": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReference",
    "orderHint": "8586848705198093378",
    "planTitle": "Order Management (December 2017)"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
