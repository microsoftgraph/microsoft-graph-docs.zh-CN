---
title: plannerFavoritePlanReferenceCollection 资源类型
description: " 值是 plannerFavoritePlanReference 对象。"
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: c473d4101a1247420e641b532ea04dfbc1a26d2c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519484"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a><span data-ttu-id="da890-103">plannerFavoritePlanReferenceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="da890-103">plannerFavoritePlanReferenceCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da890-104">**PlannerFavoritePlanReferenceCollection**资源代表由用户标记为收藏的计划对引用的集合。</span><span class="sxs-lookup"><span data-stu-id="da890-104">The **plannerFavoritePlanReferenceCollection** resource represents the collection of references to plans that are marked as a favorite by a user.</span></span> <span data-ttu-id="da890-105">此资源是开放的类型， [plannerUser](planneruser.md)对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="da890-105">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="da890-106">中的属性值对的属性名称是相应计划; 的 ID值是[plannerFavoritePlanReference](plannerfavoriteplanreference.md)对象。</span><span class="sxs-lookup"><span data-stu-id="da890-106">The property name in the property-value pair is the ID of the corresponding plan; the value is the [plannerFavoritePlanReference](plannerfavoriteplanreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="da890-107">属性</span><span class="sxs-lookup"><span data-stu-id="da890-107">Properties</span></span>
<span data-ttu-id="da890-108">您可以定义此打开类型的属性。</span><span class="sxs-lookup"><span data-stu-id="da890-108">You can define the properties of this open type.</span></span> <span data-ttu-id="da890-109">属性名称是`id` [plannerPlan](plannerplan.md)资源的值和它们的值必须是[plannerFavoritePlanReference](plannerfavoriteplanreference.md)对象。</span><span class="sxs-lookup"><span data-stu-id="da890-109">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerFavoritePlanReference](plannerfavoriteplanreference.md) objects.</span></span> <span data-ttu-id="da890-110">在收藏夹列表中删除项目，设置对属性的值`null`。</span><span class="sxs-lookup"><span data-stu-id="da890-110">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="da890-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da890-111">JSON representation</span></span>

<span data-ttu-id="da890-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da890-112">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerfavoriteplanreferencecollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
