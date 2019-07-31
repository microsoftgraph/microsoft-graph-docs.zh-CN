---
author: daspek
description: ItemAnalytics 资源提供有关项目上发生的活动的分析。 此资源目前仅适用于 SharePoint 和 OneDrive for business。
ms.date: 09/14/2017
title: ItemAnalytics
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d2be5c7665961248e989101a1a9bd21eb805e6e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967093"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="28096-104">itemAnalytics 资源类型</span><span class="sxs-lookup"><span data-stu-id="28096-104">itemAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28096-105">**ItemAnalytics**资源提供有关项目上发生的活动的分析。</span><span class="sxs-lookup"><span data-stu-id="28096-105">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="28096-106">此资源目前仅适用于 SharePoint 和 OneDrive for business。</span><span class="sxs-lookup"><span data-stu-id="28096-106">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="28096-107">您还可以使用[getActivitiesByInterval][] API 检索自定义时间范围或时间间隔内的分析。</span><span class="sxs-lookup"><span data-stu-id="28096-107">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="28096-108">**注意:\*\*\*\*ItemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。</span><span class="sxs-lookup"><span data-stu-id="28096-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="28096-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28096-109">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="28096-110">属性</span><span class="sxs-lookup"><span data-stu-id="28096-110">Properties</span></span>

| <span data-ttu-id="28096-111">属性</span><span class="sxs-lookup"><span data-stu-id="28096-111">Property</span></span>      | <span data-ttu-id="28096-112">类型</span><span class="sxs-lookup"><span data-stu-id="28096-112">Type</span></span>                 | <span data-ttu-id="28096-113">说明</span><span class="sxs-lookup"><span data-stu-id="28096-113">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="28096-114">allTime</span><span class="sxs-lookup"><span data-stu-id="28096-114">allTime</span></span>       | <span data-ttu-id="28096-115">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="28096-115">[itemActivityStat][]</span></span> | <span data-ttu-id="28096-116">对项目生命周期的分析。</span><span class="sxs-lookup"><span data-stu-id="28096-116">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="28096-117">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="28096-117">lastSevenDays</span></span> | <span data-ttu-id="28096-118">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="28096-118">[itemActivityStat][]</span></span> | <span data-ttu-id="28096-119">最近七天的分析。</span><span class="sxs-lookup"><span data-stu-id="28096-119">Analytics for the last seven days.</span></span>

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
