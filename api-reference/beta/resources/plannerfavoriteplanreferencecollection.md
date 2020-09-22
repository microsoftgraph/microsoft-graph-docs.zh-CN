---
title: plannerFavoritePlanReferenceCollection 资源类型
description: " 值是 plannerFavoritePlanReference 对象。"
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 079b841e32058fd5989944528c524a437405f3f6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993160"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a><span data-ttu-id="d0c16-103">plannerFavoritePlanReferenceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0c16-103">plannerFavoritePlanReferenceCollection resource type</span></span>

<span data-ttu-id="d0c16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0c16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0c16-105">**PlannerFavoritePlanReferenceCollection**资源表示对计划的引用的集合，这些计划被用户标记为收藏。</span><span class="sxs-lookup"><span data-stu-id="d0c16-105">The **plannerFavoritePlanReferenceCollection** resource represents the collection of references to plans that are marked as a favorite by a user.</span></span> <span data-ttu-id="d0c16-106">此资源是打开的类型，并且是 [plannerUser](planneruser.md) 对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="d0c16-106">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="d0c16-107">属性值对中的属性名称是对应计划的 ID;值是 [plannerFavoritePlanReference](plannerfavoriteplanreference.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0c16-107">The property name in the property-value pair is the ID of the corresponding plan; the value is the [plannerFavoritePlanReference](plannerfavoriteplanreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="d0c16-108">属性</span><span class="sxs-lookup"><span data-stu-id="d0c16-108">Properties</span></span>
<span data-ttu-id="d0c16-109">您可以定义此开放类型的属性。</span><span class="sxs-lookup"><span data-stu-id="d0c16-109">You can define the properties of this open type.</span></span> <span data-ttu-id="d0c16-110">属性名称是 `id` [plannerPlan](plannerplan.md) 资源的值，它们的值必须是 [plannerFavoritePlanReference](plannerfavoriteplanreference.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0c16-110">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerFavoritePlanReference](plannerfavoriteplanreference.md) objects.</span></span> <span data-ttu-id="d0c16-111">若要删除收藏夹列表中的项，请将该属性的值设置为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="d0c16-111">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="d0c16-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0c16-112">JSON representation</span></span>

<span data-ttu-id="d0c16-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0c16-113">The following is a JSON representation of the resource.</span></span>

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


