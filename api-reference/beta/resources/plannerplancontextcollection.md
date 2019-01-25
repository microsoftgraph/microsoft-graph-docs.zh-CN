---
title: plannerPlanContextCollection 资源类型
description: '**PlannerPlanContextCollection**资源表示的外部上下文计划链接到的集合。 此资源是开放的类型，plannerPlan 对象的一部分。 属性值对中的值是 plannerPlanContext 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 6ec515a164c5b0fca6334930b55a4b5d4e73b7d9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516495"
---
# <a name="plannerplancontextcollection-resource-type"></a><span data-ttu-id="839cc-105">plannerPlanContextCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="839cc-105">plannerPlanContextCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="839cc-106">**PlannerPlanContextCollection**资源表示的外部上下文计划链接到的集合。</span><span class="sxs-lookup"><span data-stu-id="839cc-106">The **plannerPlanContextCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="839cc-107">此资源是开放的类型， [plannerPlan](plannerplan.md)对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="839cc-107">This resource is an open type and is part of the [plannerPlan](plannerplan.md) object.</span></span> <span data-ttu-id="839cc-108">属性值对中的值是[plannerPlanContext](plannerplancontext.md)对象。</span><span class="sxs-lookup"><span data-stu-id="839cc-108">The value in the property-value pair is the [plannerPlanContext](plannerplancontext.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="839cc-109">属性</span><span class="sxs-lookup"><span data-stu-id="839cc-109">Properties</span></span>
<span data-ttu-id="839cc-110">您可以定义此打开类型的属性。</span><span class="sxs-lookup"><span data-stu-id="839cc-110">You can define the properties of this open type.</span></span> <span data-ttu-id="839cc-111">属性值应为独特标识符值，该值代表外部上下文与属性名称。</span><span class="sxs-lookup"><span data-stu-id="839cc-111">The property values should be distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="839cc-112">属性值必须是[plannerPlanContext](plannerplancontext.md)对象。</span><span class="sxs-lookup"><span data-stu-id="839cc-112">The property values must be [plannerPlanContext](plannerplancontext.md) objects.</span></span> <span data-ttu-id="839cc-113">基于 OData 要求，在打开的类型的属性名称不能包含下列字符： `.`， `:`， `%`， `@`。</span><span class="sxs-lookup"><span data-stu-id="839cc-113">Based on OData requirements, property names in open types cannot contain the following characters: `.`, `:`, `%`, `@`.</span></span> <span data-ttu-id="839cc-114">需要使用 URL 编码进行编码这些字符。</span><span class="sxs-lookup"><span data-stu-id="839cc-114">These characters need to be encoded using URL encoding.</span></span> <span data-ttu-id="839cc-115">在收藏夹列表中删除项目，设置对属性的值`null`。</span><span class="sxs-lookup"><span data-stu-id="839cc-115">To remove an item in the favorites list, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="839cc-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="839cc-116">JSON representation</span></span>

<span data-ttu-id="839cc-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="839cc-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextCollection"
}-->

```json
{
  "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
    "@odata.type": "#microsoft.graph.plannerPlanContext",
    "associationType": "Board",
    "createdDateTime": "2015-10-14T00:57:28.4698344Z",
    "displayNameSegments": [
        "Finance Team",
        "Budget Plans"
    ],
    "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontextcollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
