---
author: daspek
description: ItemAnalytics 资源提供有关项目上发生的活动的分析。 此资源目前仅适用于 SharePoint 和 OneDrive for business。
ms.date: 09/14/2017
title: ItemAnalytics
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 4035ff821927d520ed457c3040be01bd9368240c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523098"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="73f90-104">itemAnalytics 资源类型</span><span class="sxs-lookup"><span data-stu-id="73f90-104">itemAnalytics resource type</span></span>

<span data-ttu-id="73f90-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="73f90-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73f90-106">**ItemAnalytics**资源提供有关项目上发生的活动的分析。</span><span class="sxs-lookup"><span data-stu-id="73f90-106">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="73f90-107">此资源目前仅适用于 SharePoint 和 OneDrive for business。</span><span class="sxs-lookup"><span data-stu-id="73f90-107">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="73f90-108">您还可以使用[getActivitiesByInterval][] API 检索自定义时间范围或时间间隔内的分析。</span><span class="sxs-lookup"><span data-stu-id="73f90-108">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="73f90-109">**注意：\*\*\*\*ItemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。</span><span class="sxs-lookup"><span data-stu-id="73f90-109">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="73f90-110">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73f90-110">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="73f90-111">属性</span><span class="sxs-lookup"><span data-stu-id="73f90-111">Properties</span></span>

| <span data-ttu-id="73f90-112">属性</span><span class="sxs-lookup"><span data-stu-id="73f90-112">Property</span></span>      | <span data-ttu-id="73f90-113">类型</span><span class="sxs-lookup"><span data-stu-id="73f90-113">Type</span></span>                 | <span data-ttu-id="73f90-114">说明</span><span class="sxs-lookup"><span data-stu-id="73f90-114">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="73f90-115">allTime</span><span class="sxs-lookup"><span data-stu-id="73f90-115">allTime</span></span>       | <span data-ttu-id="73f90-116">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="73f90-116">[itemActivityStat][]</span></span> | <span data-ttu-id="73f90-117">对项目生命周期的分析。</span><span class="sxs-lookup"><span data-stu-id="73f90-117">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="73f90-118">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="73f90-118">lastSevenDays</span></span> | <span data-ttu-id="73f90-119">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="73f90-119">[itemActivityStat][]</span></span> | <span data-ttu-id="73f90-120">最近七天的分析。</span><span class="sxs-lookup"><span data-stu-id="73f90-120">Analytics for the last seven days.</span></span>

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
