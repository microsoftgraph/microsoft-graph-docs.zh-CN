---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemAnalytics
localization_priority: Normal
ms.openlocfilehash: 03626b5dad041181558af076b5dc0ac05b684e13
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842411"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="f4a40-102">itemAnalytics 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4a40-102">itemAnalytics resource type</span></span>

> <span data-ttu-id="f4a40-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f4a40-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f4a40-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f4a40-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f4a40-105">**ItemAnalytics**资源提供有关活动项上发生的分析。</span><span class="sxs-lookup"><span data-stu-id="f4a40-105">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="f4a40-106">此资源是当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="f4a40-106">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="f4a40-107">[GetActivitiesByInterval][] API 还可用于检索分析通过自定义的时间范围或时间间隔。</span><span class="sxs-lookup"><span data-stu-id="f4a40-107">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="f4a40-108">**注意：\*\*\*\*ItemAnalytics**资源尚不可用所有[国家/地区的部署](/graph/deployments)中。</span><span class="sxs-lookup"><span data-stu-id="f4a40-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4a40-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4a40-109">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f4a40-110">属性</span><span class="sxs-lookup"><span data-stu-id="f4a40-110">Properties</span></span>

| <span data-ttu-id="f4a40-111">属性</span><span class="sxs-lookup"><span data-stu-id="f4a40-111">Property</span></span>      | <span data-ttu-id="f4a40-112">类型</span><span class="sxs-lookup"><span data-stu-id="f4a40-112">Type</span></span>                 | <span data-ttu-id="f4a40-113">Description</span><span class="sxs-lookup"><span data-stu-id="f4a40-113">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="f4a40-114">allTime</span><span class="sxs-lookup"><span data-stu-id="f4a40-114">allTime</span></span>       | <span data-ttu-id="f4a40-115">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="f4a40-115">[itemActivityStat][]</span></span> | <span data-ttu-id="f4a40-116">通过分析的项目生命周期。</span><span class="sxs-lookup"><span data-stu-id="f4a40-116">Analytics over the the item's lifespan.</span></span>
| <span data-ttu-id="f4a40-117">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="f4a40-117">lastSevenDays</span></span> | <span data-ttu-id="f4a40-118">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="f4a40-118">[itemActivityStat][]</span></span> | <span data-ttu-id="f4a40-119">最近七天的分析。</span><span class="sxs-lookup"><span data-stu-id="f4a40-119">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md


[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

<!-- {
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics"
} -->
