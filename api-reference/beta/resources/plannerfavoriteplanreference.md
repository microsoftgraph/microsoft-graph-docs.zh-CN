---
title: plannerFavoritePlanReference 资源类型
description: '**PlannerFavoritePlanReference**资源类型代表对由用户标记为收藏 plannerPlan 的引用。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 77a931a882cc4b01725bd8ceb0ae6bcc721a9013
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518385"
---
# <a name="plannerfavoriteplanreference-resource-type"></a><span data-ttu-id="e0a63-103">plannerFavoritePlanReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0a63-103">plannerFavoritePlanReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0a63-104">**PlannerFavoritePlanReference**资源类型代表对由用户标记为收藏[plannerPlan](plannerplan.md)的引用。</span><span class="sxs-lookup"><span data-stu-id="e0a63-104">The **plannerFavoritePlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has been marked as a favorite by the user.</span></span> <span data-ttu-id="e0a63-105">客户端应注意**plannerFavoritePlanReference**条目可以引用**plannerPlans**的被删除，用户不再可以访问，或已更新具有不同的标题。</span><span class="sxs-lookup"><span data-stu-id="e0a63-105">Clients should note that **plannerFavoritePlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>

<span data-ttu-id="e0a63-106">我们建议客户端差异时通知用户，并保持最新条目。</span><span class="sxs-lookup"><span data-stu-id="e0a63-106">We recommend that clients notify users when there are discrepancies and keep the entries up to date.</span></span>


## <a name="properties"></a><span data-ttu-id="e0a63-107">属性</span><span class="sxs-lookup"><span data-stu-id="e0a63-107">Properties</span></span>
| <span data-ttu-id="e0a63-108">属性</span><span class="sxs-lookup"><span data-stu-id="e0a63-108">Property</span></span>     | <span data-ttu-id="e0a63-109">类型</span><span class="sxs-lookup"><span data-stu-id="e0a63-109">Type</span></span>   |<span data-ttu-id="e0a63-110">说明</span><span class="sxs-lookup"><span data-stu-id="e0a63-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0a63-111">orderHint</span><span class="sxs-lookup"><span data-stu-id="e0a63-111">orderHint</span></span>|<span data-ttu-id="e0a63-112">String</span><span class="sxs-lookup"><span data-stu-id="e0a63-112">String</span></span>|<span data-ttu-id="e0a63-p102">用于为列表视图中的此类型项目排序的提示。此格式在[使用规划器中的排序提示](planner-order-hint-format.md)定义中。</span><span class="sxs-lookup"><span data-stu-id="e0a63-p102">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="e0a63-115">planTitle</span><span class="sxs-lookup"><span data-stu-id="e0a63-115">planTitle</span></span>|<span data-ttu-id="e0a63-116">String</span><span class="sxs-lookup"><span data-stu-id="e0a63-116">String</span></span>|<span data-ttu-id="e0a63-117">用户将其标记为收藏时计划的标题。</span><span class="sxs-lookup"><span data-stu-id="e0a63-117">Title of the plan at the time the user marked it as a favorite.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e0a63-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0a63-118">JSON representation</span></span>

<span data-ttu-id="e0a63-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0a63-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerFavoritePlanReference"
}-->

```json
{
  "orderHint": "String",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerfavoriteplanreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
