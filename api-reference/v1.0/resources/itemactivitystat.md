---
author: daspek
ms.author: dspektor
title: itemActivityStat 资源类型
description: ItemActivityStat 对象提供有关项目上发生的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3af10bba565585341d04cdc47702e18e71d8accd
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970640"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="e501e-103">itemActivityStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="e501e-103">itemActivityStat resource type</span></span>

<span data-ttu-id="e501e-104">**ItemActivityStat**资源提供有关在一段时间内发生的活动的信息。</span><span class="sxs-lookup"><span data-stu-id="e501e-104">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="properties"></a><span data-ttu-id="e501e-105">属性</span><span class="sxs-lookup"><span data-stu-id="e501e-105">Properties</span></span>

| <span data-ttu-id="e501e-106">属性</span><span class="sxs-lookup"><span data-stu-id="e501e-106">Property</span></span>         | <span data-ttu-id="e501e-107">类型</span><span class="sxs-lookup"><span data-stu-id="e501e-107">Type</span></span>                    | <span data-ttu-id="e501e-108">说明</span><span class="sxs-lookup"><span data-stu-id="e501e-108">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="e501e-109">incompleteData</span><span class="sxs-lookup"><span data-stu-id="e501e-109">incompleteData</span></span>   | <span data-ttu-id="e501e-110">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="e501e-110">[incompleteData][]</span></span>      | <span data-ttu-id="e501e-111">指示此时间间隔中的统计信息基于不完整的数据。</span><span class="sxs-lookup"><span data-stu-id="e501e-111">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="e501e-112">只读。</span><span class="sxs-lookup"><span data-stu-id="e501e-112">Read-only.</span></span>
| <span data-ttu-id="e501e-113">isTrending</span><span class="sxs-lookup"><span data-stu-id="e501e-113">isTrending</span></span>       | <span data-ttu-id="e501e-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="e501e-114">Boolean</span></span>                 | <span data-ttu-id="e501e-115">指示项目是否为 "趋势"。</span><span class="sxs-lookup"><span data-stu-id="e501e-115">Indicates whether the item is "trending."</span></span> <span data-ttu-id="e501e-116">只读。</span><span class="sxs-lookup"><span data-stu-id="e501e-116">Read-only.</span></span>
| <span data-ttu-id="e501e-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e501e-117">startDateTime</span></span>    | <span data-ttu-id="e501e-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e501e-118">DateTimeOffset</span></span>          | <span data-ttu-id="e501e-119">时间间隔开始时。</span><span class="sxs-lookup"><span data-stu-id="e501e-119">When the interval starts.</span></span> <span data-ttu-id="e501e-120">只读。</span><span class="sxs-lookup"><span data-stu-id="e501e-120">Read-only.</span></span>
| <span data-ttu-id="e501e-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e501e-121">endDateTime</span></span>      | <span data-ttu-id="e501e-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e501e-122">DateTimeOffset</span></span>          | <span data-ttu-id="e501e-123">时间间隔结束时。</span><span class="sxs-lookup"><span data-stu-id="e501e-123">When the interval ends.</span></span> <span data-ttu-id="e501e-124">只读。</span><span class="sxs-lookup"><span data-stu-id="e501e-124">Read-only.</span></span>
| <span data-ttu-id="e501e-125">create</span><span class="sxs-lookup"><span data-stu-id="e501e-125">create</span></span>           | <span data-ttu-id="e501e-126">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="e501e-126">[itemActionStat][]</span></span>      | <span data-ttu-id="e501e-127">有关此间隔中的**创建**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="e501e-127">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="e501e-128">只读。</span><span class="sxs-lookup"><span data-stu-id="e501e-128">Read-only.</span></span>
| <span data-ttu-id="e501e-129">edit</span><span class="sxs-lookup"><span data-stu-id="e501e-129">edit</span></span>             | <span data-ttu-id="e501e-130">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="e501e-130">[itemActionStat][]</span></span>      | <span data-ttu-id="e501e-131">有关此间隔中的**编辑**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="e501e-131">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="e501e-132">只读。</span><span class="sxs-lookup"><span data-stu-id="e501e-132">Read-only.</span></span>
| <span data-ttu-id="e501e-133">delete</span><span class="sxs-lookup"><span data-stu-id="e501e-133">delete</span></span>           | <span data-ttu-id="e501e-134">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="e501e-134">[itemActionStat][]</span></span>      | <span data-ttu-id="e501e-135">有关此间隔中的**删除**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="e501e-135">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="e501e-136">只读。</span><span class="sxs-lookup"><span data-stu-id="e501e-136">Read-only.</span></span>
| <span data-ttu-id="e501e-137">move</span><span class="sxs-lookup"><span data-stu-id="e501e-137">move</span></span>             | <span data-ttu-id="e501e-138">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="e501e-138">[itemActionStat][]</span></span>      | <span data-ttu-id="e501e-139">有关此间隔中**移动**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="e501e-139">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="e501e-140">只读。</span><span class="sxs-lookup"><span data-stu-id="e501e-140">Read-only.</span></span>
| <span data-ttu-id="e501e-141">访问</span><span class="sxs-lookup"><span data-stu-id="e501e-141">access</span></span>           | <span data-ttu-id="e501e-142">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="e501e-142">[itemActionStat][]</span></span>      | <span data-ttu-id="e501e-143">有关此间隔中的**访问**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="e501e-143">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="e501e-144">只读。</span><span class="sxs-lookup"><span data-stu-id="e501e-144">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="e501e-147">关系</span><span class="sxs-lookup"><span data-stu-id="e501e-147">Relationships</span></span>

| <span data-ttu-id="e501e-148">关系名称</span><span class="sxs-lookup"><span data-stu-id="e501e-148">Relationship name</span></span> | <span data-ttu-id="e501e-149">类型</span><span class="sxs-lookup"><span data-stu-id="e501e-149">Type</span></span>                        | <span data-ttu-id="e501e-150">说明</span><span class="sxs-lookup"><span data-stu-id="e501e-150">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="e501e-151">activities</span><span class="sxs-lookup"><span data-stu-id="e501e-151">activities</span></span>        | <span data-ttu-id="e501e-152">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="e501e-152">[itemActivity][] collection</span></span> | <span data-ttu-id="e501e-153">公开此**itemActivityStat**资源中表示的**itemActivities** 。</span><span class="sxs-lookup"><span data-stu-id="e501e-153">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="e501e-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e501e-155">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "baseType": "microsoft.graph.entity",
  "@type": "microsoft.graph.itemActivityStat",
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "incompleteData": {"@odata.type": "microsoft.graph.incompleteData"},
  "isTrending": true,
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "create": {"@odata.type": "microsoft.graph.itemActionStat"},
  "delete": {"@odata.type": "microsoft.graph.itemActionStat"},
  "edit": {"@odata.type": "microsoft.graph.itemActionStat"},
  "move": {"@odata.type": "microsoft.graph.itemActionStat"},
  "access": {"@odata.type": "microsoft.graph.itemActionStat"}
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat",
  "suppressions": []
}
-->
