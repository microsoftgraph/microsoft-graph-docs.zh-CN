---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: itemAnalytics
localization_priority: Normal
ms.openlocfilehash: 72e7f4de752ec04fbc5ebd98655254e2597fa499
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514962"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="101ae-102">itemAnalytics 资源类型</span><span class="sxs-lookup"><span data-stu-id="101ae-102">itemAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="101ae-103">**ItemAnalytics**资源提供有关活动项上发生的分析。</span><span class="sxs-lookup"><span data-stu-id="101ae-103">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="101ae-104">此资源是当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="101ae-104">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="101ae-105">[GetActivitiesByInterval][] API 还可用于检索分析通过自定义的时间范围或时间间隔。</span><span class="sxs-lookup"><span data-stu-id="101ae-105">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="101ae-106">**注意：\*\*\*\*ItemAnalytics**资源尚不可用所有[国家/地区的部署](/graph/deployments)中。</span><span class="sxs-lookup"><span data-stu-id="101ae-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="101ae-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="101ae-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="101ae-108">属性</span><span class="sxs-lookup"><span data-stu-id="101ae-108">Properties</span></span>

| <span data-ttu-id="101ae-109">属性</span><span class="sxs-lookup"><span data-stu-id="101ae-109">Property</span></span>      | <span data-ttu-id="101ae-110">类型</span><span class="sxs-lookup"><span data-stu-id="101ae-110">Type</span></span>                 | <span data-ttu-id="101ae-111">说明</span><span class="sxs-lookup"><span data-stu-id="101ae-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="101ae-112">allTime</span><span class="sxs-lookup"><span data-stu-id="101ae-112">allTime</span></span>       | <span data-ttu-id="101ae-113">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="101ae-113">[itemActivityStat][]</span></span> | <span data-ttu-id="101ae-114">通过分析的项目生命周期。</span><span class="sxs-lookup"><span data-stu-id="101ae-114">Analytics over the the item's lifespan.</span></span>
| <span data-ttu-id="101ae-115">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="101ae-115">lastSevenDays</span></span> | <span data-ttu-id="101ae-116">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="101ae-116">[itemActivityStat][]</span></span> | <span data-ttu-id="101ae-117">最近七天的分析。</span><span class="sxs-lookup"><span data-stu-id="101ae-117">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md


[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

<!--
{
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemanalytics.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
