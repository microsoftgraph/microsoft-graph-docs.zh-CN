---
title: plannerRecentPlanReferenceCollection 资源类型
description: '**PlannerRecentPlanReferenceCollection**资源代表最近已由用户查看的计划对引用的集合。 此资源是开放的类型，plannerUser 对象的一部分。 属性名称是相应计划的 ID。 属性值对中的值是 plannerRecentPlanReference 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 84eaedb2f37aefae32b5efac1e5a4a5dfb38e0d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980760"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a><span data-ttu-id="04dac-106">plannerRecentPlanReferenceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="04dac-106">plannerRecentPlanReferenceCollection resource type</span></span>

> <span data-ttu-id="04dac-107">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="04dac-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04dac-108">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="04dac-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="04dac-109">**PlannerRecentPlanReferenceCollection**资源代表最近已由用户查看的计划对引用的集合。</span><span class="sxs-lookup"><span data-stu-id="04dac-109">The **plannerRecentPlanReferenceCollection** resource represents the collection of references to plans that were recently viewed by a user.</span></span> <span data-ttu-id="04dac-110">此资源是开放的类型， [plannerUser](planneruser.md)对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="04dac-110">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="04dac-111">属性名称是相应计划的 ID。</span><span class="sxs-lookup"><span data-stu-id="04dac-111">The property name is the ID of the corresponding plan.</span></span> <span data-ttu-id="04dac-112">属性值对中的值是[plannerRecentPlanReference](plannerrecentplanreference.md)对象。</span><span class="sxs-lookup"><span data-stu-id="04dac-112">The value in the property-value pair is the [plannerRecentPlanReference](plannerrecentplanreference.md) object.</span></span>
<span data-ttu-id="04dac-113">集合的大小超过预先确定的最大值时，添加对新引用此集合将自动删除最早的项。</span><span class="sxs-lookup"><span data-stu-id="04dac-113">Adding new references to this collection will automatically remove the oldest entries when the size of the collection exceeds a predetermined maximum value.</span></span>


## <a name="properties"></a><span data-ttu-id="04dac-114">属性</span><span class="sxs-lookup"><span data-stu-id="04dac-114">Properties</span></span>
<span data-ttu-id="04dac-115">您可以定义此打开类型的属性。</span><span class="sxs-lookup"><span data-stu-id="04dac-115">You can define the properties of this open type.</span></span> <span data-ttu-id="04dac-116">属性名称是`id` [plannerPlan](plannerplan.md)资源的值和它们的值必须是[plannerRecentPlanReference](plannerrecentplanreference.md)对象。</span><span class="sxs-lookup"><span data-stu-id="04dac-116">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerRecentPlanReference](plannerrecentplanreference.md) objects.</span></span> <span data-ttu-id="04dac-117">在收藏夹列表中删除项目，设置对属性的值`null`。</span><span class="sxs-lookup"><span data-stu-id="04dac-117">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="04dac-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04dac-118">JSON representation</span></span>

<span data-ttu-id="04dac-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04dac-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerRecentPlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
