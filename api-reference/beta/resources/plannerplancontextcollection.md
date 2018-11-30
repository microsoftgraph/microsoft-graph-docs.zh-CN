---
title: plannerPlanContextCollection 资源类型
description: '**PlannerPlanContextCollection**资源表示的外部上下文计划链接到的集合。 此资源是开放的类型，plannerPlan 对象的一部分。 属性值对中的值是 plannerPlanContext 对象。'
ms.openlocfilehash: ae17e604bf3d59b7b825fe36a8f93f05d5cc835f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045152"
---
# <a name="plannerplancontextcollection-resource-type"></a><span data-ttu-id="dceb6-105">plannerPlanContextCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="dceb6-105">plannerPlanContextCollection resource type</span></span>

> <span data-ttu-id="dceb6-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dceb6-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dceb6-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dceb6-107">Use of these APIs in production applications is not supported.</span></span>


<span data-ttu-id="dceb6-108">**PlannerPlanContextCollection**资源表示的外部上下文计划链接到的集合。</span><span class="sxs-lookup"><span data-stu-id="dceb6-108">The **plannerPlanContextCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="dceb6-109">此资源是开放的类型， [plannerPlan](plannerplan.md)对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="dceb6-109">This resource is an open type and is part of the [plannerPlan](plannerplan.md) object.</span></span> <span data-ttu-id="dceb6-110">属性值对中的值是[plannerPlanContext](plannerplancontext.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dceb6-110">The value in the property-value pair is the [plannerPlanContext](plannerplancontext.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="dceb6-111">属性</span><span class="sxs-lookup"><span data-stu-id="dceb6-111">Properties</span></span>
<span data-ttu-id="dceb6-112">您可以定义此打开类型的属性。</span><span class="sxs-lookup"><span data-stu-id="dceb6-112">You can define the properties of this open type.</span></span> <span data-ttu-id="dceb6-113">属性值应为独特标识符值，该值代表外部上下文与属性名称。</span><span class="sxs-lookup"><span data-stu-id="dceb6-113">The property values should be distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="dceb6-114">属性值必须是[plannerPlanContext](plannerplancontext.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dceb6-114">The property values must be [plannerPlanContext](plannerplancontext.md) objects.</span></span> <span data-ttu-id="dceb6-115">基于 OData 要求，在打开的类型的属性名称不能包含下列字符： `.`， `:`， `%`， `@`。</span><span class="sxs-lookup"><span data-stu-id="dceb6-115">Based on OData requirements, property names in open types cannot contain the following characters: `.`, `:`, `%`, `@`.</span></span> <span data-ttu-id="dceb6-116">需要使用 URL 编码进行编码这些字符。</span><span class="sxs-lookup"><span data-stu-id="dceb6-116">These characters need to be encoded using URL encoding.</span></span> <span data-ttu-id="dceb6-117">在收藏夹列表中删除项目，设置对属性的值`null`。</span><span class="sxs-lookup"><span data-stu-id="dceb6-117">To remove an item in the favorites list, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dceb6-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dceb6-118">JSON representation</span></span>

<span data-ttu-id="dceb6-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dceb6-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
