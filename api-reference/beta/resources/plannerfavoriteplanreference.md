---
title: plannerFavoritePlanReference 资源类型
description: '**PlannerFavoritePlanReference**资源类型代表对由用户标记为收藏 plannerPlan 的引用。 '
ms.openlocfilehash: bd399572dfce54ee7e46da6af60eb661484519de
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043342"
---
# <a name="plannerfavoriteplanreference-resource-type"></a><span data-ttu-id="b5719-103">plannerFavoritePlanReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5719-103">plannerFavoritePlanReference resource type</span></span>

> <span data-ttu-id="b5719-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b5719-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5719-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b5719-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b5719-106">**PlannerFavoritePlanReference**资源类型代表对由用户标记为收藏[plannerPlan](plannerplan.md)的引用。</span><span class="sxs-lookup"><span data-stu-id="b5719-106">The **plannerFavoritePlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has been marked as a favorite by the user.</span></span> <span data-ttu-id="b5719-107">客户端应注意**plannerFavoritePlanReference**条目可以引用**plannerPlans**的被删除，用户不再可以访问，或已更新具有不同的标题。</span><span class="sxs-lookup"><span data-stu-id="b5719-107">Clients should note that **plannerFavoritePlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>

<span data-ttu-id="b5719-108">我们建议客户端差异时通知用户，并保持最新条目。</span><span class="sxs-lookup"><span data-stu-id="b5719-108">We recommend that clients notify users when there are discrepancies and keep the entries up to date.</span></span>


## <a name="properties"></a><span data-ttu-id="b5719-109">属性</span><span class="sxs-lookup"><span data-stu-id="b5719-109">Properties</span></span>
| <span data-ttu-id="b5719-110">属性</span><span class="sxs-lookup"><span data-stu-id="b5719-110">Property</span></span>     | <span data-ttu-id="b5719-111">类型</span><span class="sxs-lookup"><span data-stu-id="b5719-111">Type</span></span>   |<span data-ttu-id="b5719-112">说明</span><span class="sxs-lookup"><span data-stu-id="b5719-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5719-113">orderHint</span><span class="sxs-lookup"><span data-stu-id="b5719-113">orderHint</span></span>|<span data-ttu-id="b5719-114">字符串</span><span class="sxs-lookup"><span data-stu-id="b5719-114">String</span></span>|<span data-ttu-id="b5719-p103">用于为列表视图中的此类型项目排序的提示。此格式在[使用规划器中的排序提示](planner-order-hint-format.md)定义中。</span><span class="sxs-lookup"><span data-stu-id="b5719-p103">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="b5719-117">planTitle</span><span class="sxs-lookup"><span data-stu-id="b5719-117">planTitle</span></span>|<span data-ttu-id="b5719-118">字符串</span><span class="sxs-lookup"><span data-stu-id="b5719-118">String</span></span>|<span data-ttu-id="b5719-119">用户将其标记为收藏时计划的标题。</span><span class="sxs-lookup"><span data-stu-id="b5719-119">Title of the plan at the time the user marked it as a favorite.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b5719-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5719-120">JSON representation</span></span>

<span data-ttu-id="b5719-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5719-121">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
