---
author: daspek
title: itemAnalytics 资源类型
description: ItemAnalytics 对象提供有关在项目上发生的活动的分析。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 96ad65ef5cc8907663a9ca67e5ea2b7546b8fa03
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238657"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="4cacc-103">itemAnalytics 资源类型</span><span class="sxs-lookup"><span data-stu-id="4cacc-103">itemAnalytics resource type</span></span>

<span data-ttu-id="4cacc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cacc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4cacc-105">**itemAnalytics** 资源提供有关在项目上发生的活动的分析。</span><span class="sxs-lookup"><span data-stu-id="4cacc-105">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="4cacc-106">此资源当前仅适用于 SharePoint 和 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="4cacc-106">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="4cacc-107">您还可以使用 [getActivitiesByInterval][] API 检索自定义时间范围或时间间隔的分析。</span><span class="sxs-lookup"><span data-stu-id="4cacc-107">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="4cacc-108">**注意：\*\*\*\*itemAnalytics** 资源尚未在所有的国家部署 [中可用](/graph/deployments)。</span><span class="sxs-lookup"><span data-stu-id="4cacc-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="properties"></a><span data-ttu-id="4cacc-109">属性</span><span class="sxs-lookup"><span data-stu-id="4cacc-109">Properties</span></span>

| <span data-ttu-id="4cacc-110">属性</span><span class="sxs-lookup"><span data-stu-id="4cacc-110">Property</span></span>      | <span data-ttu-id="4cacc-111">类型</span><span class="sxs-lookup"><span data-stu-id="4cacc-111">Type</span></span>                 | <span data-ttu-id="4cacc-112">说明</span><span class="sxs-lookup"><span data-stu-id="4cacc-112">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="4cacc-113">allTime</span><span class="sxs-lookup"><span data-stu-id="4cacc-113">allTime</span></span>       | <span data-ttu-id="4cacc-114">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="4cacc-114">[itemActivityStat][]</span></span> | <span data-ttu-id="4cacc-115">项目生命周期分析。</span><span class="sxs-lookup"><span data-stu-id="4cacc-115">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="4cacc-116">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="4cacc-116">lastSevenDays</span></span> | <span data-ttu-id="4cacc-117">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="4cacc-117">[itemActivityStat][]</span></span> | <span data-ttu-id="4cacc-118">过去七天的分析。</span><span class="sxs-lookup"><span data-stu-id="4cacc-118">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="json-representation"></a><span data-ttu-id="4cacc-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4cacc-121">JSON representation</span></span>

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

