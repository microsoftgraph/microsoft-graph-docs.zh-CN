---
title: plannerFavoritePlanReference 资源类型
description: '**PlannerFavoritePlanReference**资源类型代表对已标记为用户收藏的 plannerPlan 的引用。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 07803375ca31162f0f7e392d81edb83ab2bd6da3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009067"
---
# <a name="plannerfavoriteplanreference-resource-type"></a><span data-ttu-id="56e43-103">plannerFavoritePlanReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="56e43-103">plannerFavoritePlanReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56e43-104">**PlannerFavoritePlanReference**资源类型代表对已标记为用户收藏的[plannerPlan](plannerplan.md)的引用。</span><span class="sxs-lookup"><span data-stu-id="56e43-104">The **plannerFavoritePlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has been marked as a favorite by the user.</span></span> <span data-ttu-id="56e43-105">客户端应注意, **plannerFavoritePlanReference**条目可以引用已删除的**plannerPlans** 、用户无法再访问或已使用其他标题进行更新。</span><span class="sxs-lookup"><span data-stu-id="56e43-105">Clients should note that **plannerFavoritePlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>

<span data-ttu-id="56e43-106">我们建议客户端在存在差异时通知用户, 并将这些条目保持为最新。</span><span class="sxs-lookup"><span data-stu-id="56e43-106">We recommend that clients notify users when there are discrepancies and keep the entries up to date.</span></span>


## <a name="properties"></a><span data-ttu-id="56e43-107">属性</span><span class="sxs-lookup"><span data-stu-id="56e43-107">Properties</span></span>
| <span data-ttu-id="56e43-108">属性</span><span class="sxs-lookup"><span data-stu-id="56e43-108">Property</span></span>     | <span data-ttu-id="56e43-109">类型</span><span class="sxs-lookup"><span data-stu-id="56e43-109">Type</span></span>   |<span data-ttu-id="56e43-110">说明</span><span class="sxs-lookup"><span data-stu-id="56e43-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56e43-111">orderHint</span><span class="sxs-lookup"><span data-stu-id="56e43-111">orderHint</span></span>|<span data-ttu-id="56e43-112">String</span><span class="sxs-lookup"><span data-stu-id="56e43-112">String</span></span>|<span data-ttu-id="56e43-p102">用于为列表视图中的此类型项目排序的提示。此格式在[使用规划器中的排序提示](planner-order-hint-format.md)定义中。</span><span class="sxs-lookup"><span data-stu-id="56e43-p102">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="56e43-115">planTitle</span><span class="sxs-lookup"><span data-stu-id="56e43-115">planTitle</span></span>|<span data-ttu-id="56e43-116">String</span><span class="sxs-lookup"><span data-stu-id="56e43-116">String</span></span>|<span data-ttu-id="56e43-117">用户将其标记为收藏时计划的标题。</span><span class="sxs-lookup"><span data-stu-id="56e43-117">Title of the plan at the time the user marked it as a favorite.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="56e43-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56e43-118">JSON representation</span></span>

<span data-ttu-id="56e43-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56e43-119">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
