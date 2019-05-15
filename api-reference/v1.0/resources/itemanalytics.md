---
author: daspek
ms.author: dspektor
title: itemAnalytics 资源类型
description: ItemAnalytics 对象提供有关项目上发生的活动的分析。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5c716f8faaafffe6afd75987843e6b614f5d6552
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970635"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="2baca-103">itemAnalytics 资源类型</span><span class="sxs-lookup"><span data-stu-id="2baca-103">itemAnalytics resource type</span></span>

<span data-ttu-id="2baca-104">**ItemAnalytics**资源提供有关项目上发生的活动的分析。</span><span class="sxs-lookup"><span data-stu-id="2baca-104">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="2baca-105">此资源目前仅适用于 SharePoint 和 OneDrive for business。</span><span class="sxs-lookup"><span data-stu-id="2baca-105">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="2baca-106">您还可以使用[getActivitiesByInterval][] API 检索自定义时间范围或时间间隔内的分析。</span><span class="sxs-lookup"><span data-stu-id="2baca-106">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="2baca-107">**注意:\*\*\*\*ItemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。</span><span class="sxs-lookup"><span data-stu-id="2baca-107">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="properties"></a><span data-ttu-id="2baca-108">属性</span><span class="sxs-lookup"><span data-stu-id="2baca-108">Properties</span></span>

| <span data-ttu-id="2baca-109">属性</span><span class="sxs-lookup"><span data-stu-id="2baca-109">Property</span></span>      | <span data-ttu-id="2baca-110">类型</span><span class="sxs-lookup"><span data-stu-id="2baca-110">Type</span></span>                 | <span data-ttu-id="2baca-111">说明</span><span class="sxs-lookup"><span data-stu-id="2baca-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="2baca-112">allTime</span><span class="sxs-lookup"><span data-stu-id="2baca-112">allTime</span></span>       | <span data-ttu-id="2baca-113">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="2baca-113">[itemActivityStat][]</span></span> | <span data-ttu-id="2baca-114">项目的生命周期中的分析。</span><span class="sxs-lookup"><span data-stu-id="2baca-114">Analytics over the the item's lifespan.</span></span>
| <span data-ttu-id="2baca-115">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="2baca-115">lastSevenDays</span></span> | <span data-ttu-id="2baca-116">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="2baca-116">[itemActivityStat][]</span></span> | <span data-ttu-id="2baca-117">最近七天的分析。</span><span class="sxs-lookup"><span data-stu-id="2baca-117">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="json-representation"></a><span data-ttu-id="2baca-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2baca-120">JSON representation</span></span>

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
