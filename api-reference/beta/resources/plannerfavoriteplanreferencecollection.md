---
title: plannerFavoritePlanReferenceCollection 资源类型
description: " 值是 plannerFavoritePlanReference 对象。"
author: TarkanSevilmis
ms.openlocfilehash: 056cb7b9ba728aa9dfe44ae4b90e550876461d6b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344224"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a><span data-ttu-id="ff064-103">plannerFavoritePlanReferenceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff064-103">plannerFavoritePlanReferenceCollection resource type</span></span>

> <span data-ttu-id="ff064-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ff064-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff064-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ff064-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff064-106">**PlannerFavoritePlanReferenceCollection**资源代表由用户标记为收藏的计划对引用的集合。</span><span class="sxs-lookup"><span data-stu-id="ff064-106">The **plannerFavoritePlanReferenceCollection** resource represents the collection of references to plans that are marked as a favorite by a user.</span></span> <span data-ttu-id="ff064-107">此资源是开放的类型， [plannerUser](planneruser.md)对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="ff064-107">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="ff064-108">中的属性值对的属性名称是相应计划; 的 ID值是[plannerFavoritePlanReference](plannerfavoriteplanreference.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ff064-108">The property name in the property-value pair is the ID of the corresponding plan; the value is the [plannerFavoritePlanReference](plannerfavoriteplanreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="ff064-109">Properties</span><span class="sxs-lookup"><span data-stu-id="ff064-109">Properties</span></span>
<span data-ttu-id="ff064-110">您可以定义此打开类型的属性。</span><span class="sxs-lookup"><span data-stu-id="ff064-110">You can define the properties of this open type.</span></span> <span data-ttu-id="ff064-111">属性名称是`id` [plannerPlan](plannerplan.md)资源的值和它们的值必须是[plannerFavoritePlanReference](plannerfavoriteplanreference.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ff064-111">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerFavoritePlanReference](plannerfavoriteplanreference.md) objects.</span></span> <span data-ttu-id="ff064-112">在收藏夹列表中删除项目，设置对属性的值`null`。</span><span class="sxs-lookup"><span data-stu-id="ff064-112">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ff064-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff064-113">JSON representation</span></span>

<span data-ttu-id="ff064-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff064-114">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
