---
title: plannerPlanContextDetailsCollection 资源类型
description: " 值是 plannerPlanContextDetails 对象。"
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 2731827a5d9cdb5297e619ecef164339a1b909c0
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571231"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a><span data-ttu-id="827b2-103">plannerPlanContextDetailsCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="827b2-103">plannerPlanContextDetailsCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="827b2-104">**PlannerPlanContextDetailsCollection**资源表示的外部上下文计划链接到的集合。</span><span class="sxs-lookup"><span data-stu-id="827b2-104">The **plannerPlanContextDetailsCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="827b2-105">此资源是开放的类型， [plannerPlanDetails](plannerplandetails.md)对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="827b2-105">This resource is an open type and is part of the [plannerPlanDetails](plannerplandetails.md) object.</span></span> <span data-ttu-id="827b2-106">中的属性值对的属性名称是上下文; 特定于应用程序的标识符值是[plannerPlanContextDetails](plannerplancontextdetails.md)对象。</span><span class="sxs-lookup"><span data-stu-id="827b2-106">The property name in the property-value pair is an app-specific identifier of the context; the value is the [plannerPlanContextDetails](plannerplancontextdetails.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="827b2-107">属性</span><span class="sxs-lookup"><span data-stu-id="827b2-107">Properties</span></span>
<span data-ttu-id="827b2-108">打开类型的属性可定义由客户端。</span><span class="sxs-lookup"><span data-stu-id="827b2-108">Properties of an open type can be defined by the client.</span></span> <span data-ttu-id="827b2-109">在这种情况下，客户应使用的独特的标识符值，该值代表外部上下文与属性名称。</span><span class="sxs-lookup"><span data-stu-id="827b2-109">In this case, the client should use a distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="827b2-110">属性值必须是[plannerPlanContextDetails](plannerplancontextdetails.md)对象。</span><span class="sxs-lookup"><span data-stu-id="827b2-110">The property values must be [plannerPlanContextDetails](plannerplancontextdetails.md) objects.</span></span> <span data-ttu-id="827b2-111">基于 OData，在打开的类型的属性名称不能包含下列字符： `.`， `:`， `@`， `%`。</span><span class="sxs-lookup"><span data-stu-id="827b2-111">Based on OData, property names in open types cannot contain the following characters: `.`, `:`, `@`, `%`.</span></span> <span data-ttu-id="827b2-112">需要 URL 编码格式编码这些字符。</span><span class="sxs-lookup"><span data-stu-id="827b2-112">These characters need to be encoded with URL encoding format.</span></span> <span data-ttu-id="827b2-113">在收藏夹列表中删除项目，需要的值从集合中删除[plannerPlanContextCollection](plannerplancontextcollection.md)相反，其自动将此对象中删除的项。</span><span class="sxs-lookup"><span data-stu-id="827b2-113">To remove an item in the favorites list, the value needs to be removed from the [plannerPlanContextCollection](plannerplancontextcollection.md) collection instead, which will automatically remove the entry in this object.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"
}-->
```json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontextdetailscollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
