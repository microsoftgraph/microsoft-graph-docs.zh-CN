---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemAnalytics
localization_priority: Normal
ms.openlocfilehash: 862b0b14f1efeb3a83dd4b842c0eb995abeabb80
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620260"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="2e225-102">itemAnalytics 资源类型</span><span class="sxs-lookup"><span data-stu-id="2e225-102">itemAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e225-103">**ItemAnalytics**资源提供有关项目上发生的活动的分析。</span><span class="sxs-lookup"><span data-stu-id="2e225-103">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="2e225-104">此资源目前仅适用于 SharePoint 和 OneDrive for business。</span><span class="sxs-lookup"><span data-stu-id="2e225-104">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="2e225-105">您还可以使用[getActivitiesByInterval][] API 检索自定义时间范围或时间间隔内的分析。</span><span class="sxs-lookup"><span data-stu-id="2e225-105">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="2e225-106">**注意:\*\*\*\*ItemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。</span><span class="sxs-lookup"><span data-stu-id="2e225-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e225-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2e225-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2e225-108">属性</span><span class="sxs-lookup"><span data-stu-id="2e225-108">Properties</span></span>

| <span data-ttu-id="2e225-109">属性</span><span class="sxs-lookup"><span data-stu-id="2e225-109">Property</span></span>      | <span data-ttu-id="2e225-110">类型</span><span class="sxs-lookup"><span data-stu-id="2e225-110">Type</span></span>                 | <span data-ttu-id="2e225-111">说明</span><span class="sxs-lookup"><span data-stu-id="2e225-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="2e225-112">allTime</span><span class="sxs-lookup"><span data-stu-id="2e225-112">allTime</span></span>       | <span data-ttu-id="2e225-113">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="2e225-113">[itemActivityStat][]</span></span> | <span data-ttu-id="2e225-114">对项目生命周期的分析。</span><span class="sxs-lookup"><span data-stu-id="2e225-114">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="2e225-115">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="2e225-115">lastSevenDays</span></span> | <span data-ttu-id="2e225-116">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="2e225-116">[itemActivityStat][]</span></span> | <span data-ttu-id="2e225-117">最近七天的分析。</span><span class="sxs-lookup"><span data-stu-id="2e225-117">Analytics for the last seven days.</span></span>

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
