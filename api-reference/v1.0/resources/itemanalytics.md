---
author: daspek
ms.author: dspektor
title: itemAnalytics 资源类型
description: ItemAnalytics 对象提供有关项目上发生的活动的分析。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0b4ee2bba6cff84a99cf5a0e20dddc09ad87ee59
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447652"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="c1ee1-103">itemAnalytics 资源类型</span><span class="sxs-lookup"><span data-stu-id="c1ee1-103">itemAnalytics resource type</span></span>

<span data-ttu-id="c1ee1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c1ee1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c1ee1-105">**ItemAnalytics**资源提供有关项目上发生的活动的分析。</span><span class="sxs-lookup"><span data-stu-id="c1ee1-105">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="c1ee1-106">此资源目前仅适用于 SharePoint 和 OneDrive for business。</span><span class="sxs-lookup"><span data-stu-id="c1ee1-106">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="c1ee1-107">您还可以使用[getActivitiesByInterval][] API 检索自定义时间范围或时间间隔内的分析。</span><span class="sxs-lookup"><span data-stu-id="c1ee1-107">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="c1ee1-108">**注意：\*\*\*\*ItemAnalytics**资源在所有[国家/地区部署](/graph/deployments)中尚不可用。</span><span class="sxs-lookup"><span data-stu-id="c1ee1-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="properties"></a><span data-ttu-id="c1ee1-109">属性</span><span class="sxs-lookup"><span data-stu-id="c1ee1-109">Properties</span></span>

| <span data-ttu-id="c1ee1-110">属性</span><span class="sxs-lookup"><span data-stu-id="c1ee1-110">Property</span></span>      | <span data-ttu-id="c1ee1-111">类型</span><span class="sxs-lookup"><span data-stu-id="c1ee1-111">Type</span></span>                 | <span data-ttu-id="c1ee1-112">说明</span><span class="sxs-lookup"><span data-stu-id="c1ee1-112">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="c1ee1-113">allTime</span><span class="sxs-lookup"><span data-stu-id="c1ee1-113">allTime</span></span>       | <span data-ttu-id="c1ee1-114">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="c1ee1-114">[itemActivityStat][]</span></span> | <span data-ttu-id="c1ee1-115">对项目生命周期的分析。</span><span class="sxs-lookup"><span data-stu-id="c1ee1-115">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="c1ee1-116">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="c1ee1-116">lastSevenDays</span></span> | <span data-ttu-id="c1ee1-117">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="c1ee1-117">[itemActivityStat][]</span></span> | <span data-ttu-id="c1ee1-118">最近七天的分析。</span><span class="sxs-lookup"><span data-stu-id="c1ee1-118">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="json-representation"></a><span data-ttu-id="c1ee1-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1ee1-121">JSON representation</span></span>

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
