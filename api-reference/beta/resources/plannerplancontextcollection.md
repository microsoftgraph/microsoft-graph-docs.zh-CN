---
title: plannerPlanContextCollection 资源类型
description: '**PlannerPlanContextCollection**资源表示规划所链接到的外部上下文的集合。 此资源是打开的类型, 并且是 plannerPlan 对象的一部分。 属性-值对中的值是 plannerPlanContext 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 34fecf604b68fe092e1feeac2c0e99cc0d59cd77
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965927"
---
# <a name="plannerplancontextcollection-resource-type"></a><span data-ttu-id="8df13-105">plannerPlanContextCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="8df13-105">plannerPlanContextCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="8df13-106">**PlannerPlanContextCollection**资源表示规划所链接到的外部上下文的集合。</span><span class="sxs-lookup"><span data-stu-id="8df13-106">The **plannerPlanContextCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="8df13-107">此资源是打开的类型, 并且是[plannerPlan](plannerplan.md)对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="8df13-107">This resource is an open type and is part of the [plannerPlan](plannerplan.md) object.</span></span> <span data-ttu-id="8df13-108">属性-值对中的值是[plannerPlanContext](plannerplancontext.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8df13-108">The value in the property-value pair is the [plannerPlanContext](plannerplancontext.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="8df13-109">属性</span><span class="sxs-lookup"><span data-stu-id="8df13-109">Properties</span></span>
<span data-ttu-id="8df13-110">您可以定义此开放类型的属性。</span><span class="sxs-lookup"><span data-stu-id="8df13-110">You can define the properties of this open type.</span></span> <span data-ttu-id="8df13-111">属性值应是表示外部上下文作为属性名称的独特标识符。</span><span class="sxs-lookup"><span data-stu-id="8df13-111">The property values should be distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="8df13-112">属性值必须是[plannerPlanContext](plannerplancontext.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8df13-112">The property values must be [plannerPlanContext](plannerplancontext.md) objects.</span></span> <span data-ttu-id="8df13-113">根据 OData 要求, 开放式类型中的属性名称不能包含以下字符: `.`、 `:`、 `%`、 `@`。</span><span class="sxs-lookup"><span data-stu-id="8df13-113">Based on OData requirements, property names in open types cannot contain the following characters: `.`, `:`, `%`, `@`.</span></span> <span data-ttu-id="8df13-114">需要使用 URL 编码对这些字符进行编码。</span><span class="sxs-lookup"><span data-stu-id="8df13-114">These characters need to be encoded using URL encoding.</span></span> <span data-ttu-id="8df13-115">若要删除收藏夹列表中的项, 请将该属性的值设置`null`为。</span><span class="sxs-lookup"><span data-stu-id="8df13-115">To remove an item in the favorites list, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8df13-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8df13-116">JSON representation</span></span>

<span data-ttu-id="8df13-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8df13-117">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
