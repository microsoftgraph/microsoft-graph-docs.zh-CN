---
title: plannerRecentPlanReferenceCollection 资源类型
description: '**plannerRecentPlanReferenceCollection**资源表示对用户最近查看的计划的引用集合。 此资源是打开的类型, 并且是 plannerUser 对象的一部分。 属性名称是对应计划的 ID。 属性-值对中的值是 plannerRecentPlanReference 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: e27375e3f2395b3528873d8b83f0b5aa6f48d52e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583177"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a><span data-ttu-id="2bb9c-106">plannerRecentPlanReferenceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="2bb9c-106">plannerRecentPlanReferenceCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bb9c-107">**plannerRecentPlanReferenceCollection**资源表示对用户最近查看的计划的引用集合。</span><span class="sxs-lookup"><span data-stu-id="2bb9c-107">The **plannerRecentPlanReferenceCollection** resource represents the collection of references to plans that were recently viewed by a user.</span></span> <span data-ttu-id="2bb9c-108">此资源是打开的类型, 并且是[plannerUser](planneruser.md)对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="2bb9c-108">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="2bb9c-109">属性名称是对应计划的 ID。</span><span class="sxs-lookup"><span data-stu-id="2bb9c-109">The property name is the ID of the corresponding plan.</span></span> <span data-ttu-id="2bb9c-110">属性-值对中的值是[plannerRecentPlanReference](plannerrecentplanreference.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2bb9c-110">The value in the property-value pair is the [plannerRecentPlanReference](plannerrecentplanreference.md) object.</span></span>
<span data-ttu-id="2bb9c-111">如果将新的引用添加到此集合中, 则当集合的大小超过预先确定的最大值时, 将自动删除最旧的项。</span><span class="sxs-lookup"><span data-stu-id="2bb9c-111">Adding new references to this collection will automatically remove the oldest entries when the size of the collection exceeds a predetermined maximum value.</span></span>


## <a name="properties"></a><span data-ttu-id="2bb9c-112">属性</span><span class="sxs-lookup"><span data-stu-id="2bb9c-112">Properties</span></span>
<span data-ttu-id="2bb9c-113">您可以定义此开放类型的属性。</span><span class="sxs-lookup"><span data-stu-id="2bb9c-113">You can define the properties of this open type.</span></span> <span data-ttu-id="2bb9c-114">属性名称是`id` [plannerPlan](plannerplan.md)资源的值, 它们的值必须是[plannerRecentPlanReference](plannerrecentplanreference.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2bb9c-114">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerRecentPlanReference](plannerrecentplanreference.md) objects.</span></span> <span data-ttu-id="2bb9c-115">若要删除收藏夹列表中的项, 请将该属性的值设置`null`为。</span><span class="sxs-lookup"><span data-stu-id="2bb9c-115">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="2bb9c-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2bb9c-116">JSON representation</span></span>

<span data-ttu-id="2bb9c-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2bb9c-117">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerrecentplanreferencecollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
