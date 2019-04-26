---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemAnalytics
localization_priority: Normal
ms.openlocfilehash: 2869655b3b645fc8d30ceec3867c28ca81ac9d51
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345448"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="9f390-102">itemAnalytics 资源类型</span><span class="sxs-lookup"><span data-stu-id="9f390-102">itemAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f390-103">**itemAnalytics**资源提供有关项目上发生的活动的分析。</span><span class="sxs-lookup"><span data-stu-id="9f390-103">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="9f390-104">此资源目前仅适用于 SharePoint 和 OneDrive for business。</span><span class="sxs-lookup"><span data-stu-id="9f390-104">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="9f390-105">您还可以使用[getActivitiesByInterval][] API 检索自定义时间范围或时间间隔内的分析。</span><span class="sxs-lookup"><span data-stu-id="9f390-105">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="9f390-106">**注意:\*\*\*\*itemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。</span><span class="sxs-lookup"><span data-stu-id="9f390-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f390-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9f390-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemAnalytics",
  "@type.aka": "oneDrive.analytics"
}-->

```json
{
  "allTime": {"@odata.type": "microsoft.graph.itemActivityStat"},
  "lastSevenDays": {"@odata.type": "microsoft.graph.itemActivityStat"}
}
```

## <a name="properties"></a><span data-ttu-id="9f390-108">属性</span><span class="sxs-lookup"><span data-stu-id="9f390-108">Properties</span></span>

| <span data-ttu-id="9f390-109">属性</span><span class="sxs-lookup"><span data-stu-id="9f390-109">Property</span></span>      | <span data-ttu-id="9f390-110">类型</span><span class="sxs-lookup"><span data-stu-id="9f390-110">Type</span></span>                 | <span data-ttu-id="9f390-111">说明</span><span class="sxs-lookup"><span data-stu-id="9f390-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="9f390-112">allTime</span><span class="sxs-lookup"><span data-stu-id="9f390-112">allTime</span></span>       | <span data-ttu-id="9f390-113">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="9f390-113">[itemActivityStat][]</span></span> | <span data-ttu-id="9f390-114">项目的生命周期中的分析。</span><span class="sxs-lookup"><span data-stu-id="9f390-114">Analytics over the the item's lifespan.</span></span>
| <span data-ttu-id="9f390-115">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="9f390-115">lastSevenDays</span></span> | <span data-ttu-id="9f390-116">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="9f390-116">[itemActivityStat][]</span></span> | <span data-ttu-id="9f390-117">最近七天的分析。</span><span class="sxs-lookup"><span data-stu-id="9f390-117">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md


[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

<!--
{
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics",
  "suppressions": []
}
-->
