---
author: daspek
ms.author: dspektor
title: itemActivityStat 资源类型
description: ItemActivityStat 对象提供有关项目上发生的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: bf4396e6da5c56b19d33d7a914d864cb6dd54592
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036671"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="677e7-103">itemActivityStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="677e7-103">itemActivityStat resource type</span></span>

<span data-ttu-id="677e7-104">**ItemActivityStat**资源提供有关在一段时间内发生的活动的信息。</span><span class="sxs-lookup"><span data-stu-id="677e7-104">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="properties"></a><span data-ttu-id="677e7-105">属性</span><span class="sxs-lookup"><span data-stu-id="677e7-105">Properties</span></span>

| <span data-ttu-id="677e7-106">属性</span><span class="sxs-lookup"><span data-stu-id="677e7-106">Property</span></span>         | <span data-ttu-id="677e7-107">类型</span><span class="sxs-lookup"><span data-stu-id="677e7-107">Type</span></span>                    | <span data-ttu-id="677e7-108">说明</span><span class="sxs-lookup"><span data-stu-id="677e7-108">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="677e7-109">incompleteData</span><span class="sxs-lookup"><span data-stu-id="677e7-109">incompleteData</span></span>   | <span data-ttu-id="677e7-110">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="677e7-110">[incompleteData][]</span></span>      | <span data-ttu-id="677e7-111">指示此时间间隔中的统计信息基于不完整的数据。</span><span class="sxs-lookup"><span data-stu-id="677e7-111">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="677e7-112">只读。</span><span class="sxs-lookup"><span data-stu-id="677e7-112">Read-only.</span></span>
| <span data-ttu-id="677e7-113">isTrending</span><span class="sxs-lookup"><span data-stu-id="677e7-113">isTrending</span></span>       | <span data-ttu-id="677e7-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="677e7-114">Boolean</span></span>                 | <span data-ttu-id="677e7-115">指示项目是否为 "趋势"。</span><span class="sxs-lookup"><span data-stu-id="677e7-115">Indicates whether the item is "trending."</span></span> <span data-ttu-id="677e7-116">只读。</span><span class="sxs-lookup"><span data-stu-id="677e7-116">Read-only.</span></span>
| <span data-ttu-id="677e7-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="677e7-117">startDateTime</span></span>    | <span data-ttu-id="677e7-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="677e7-118">DateTimeOffset</span></span>          | <span data-ttu-id="677e7-119">时间间隔开始时。</span><span class="sxs-lookup"><span data-stu-id="677e7-119">When the interval starts.</span></span> <span data-ttu-id="677e7-120">只读。</span><span class="sxs-lookup"><span data-stu-id="677e7-120">Read-only.</span></span>
| <span data-ttu-id="677e7-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="677e7-121">endDateTime</span></span>      | <span data-ttu-id="677e7-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="677e7-122">DateTimeOffset</span></span>          | <span data-ttu-id="677e7-123">时间间隔结束时。</span><span class="sxs-lookup"><span data-stu-id="677e7-123">When the interval ends.</span></span> <span data-ttu-id="677e7-124">只读。</span><span class="sxs-lookup"><span data-stu-id="677e7-124">Read-only.</span></span>
| <span data-ttu-id="677e7-125">create</span><span class="sxs-lookup"><span data-stu-id="677e7-125">create</span></span>           | <span data-ttu-id="677e7-126">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="677e7-126">[itemActionStat][]</span></span>      | <span data-ttu-id="677e7-127">有关此间隔中的**创建**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="677e7-127">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="677e7-128">只读。</span><span class="sxs-lookup"><span data-stu-id="677e7-128">Read-only.</span></span>
| <span data-ttu-id="677e7-129">edit</span><span class="sxs-lookup"><span data-stu-id="677e7-129">edit</span></span>             | <span data-ttu-id="677e7-130">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="677e7-130">[itemActionStat][]</span></span>      | <span data-ttu-id="677e7-131">有关此间隔中的**编辑**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="677e7-131">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="677e7-132">只读。</span><span class="sxs-lookup"><span data-stu-id="677e7-132">Read-only.</span></span>
| <span data-ttu-id="677e7-133">delete</span><span class="sxs-lookup"><span data-stu-id="677e7-133">delete</span></span>           | <span data-ttu-id="677e7-134">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="677e7-134">[itemActionStat][]</span></span>      | <span data-ttu-id="677e7-135">有关此间隔中的**删除**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="677e7-135">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="677e7-136">只读。</span><span class="sxs-lookup"><span data-stu-id="677e7-136">Read-only.</span></span>
| <span data-ttu-id="677e7-137">move</span><span class="sxs-lookup"><span data-stu-id="677e7-137">move</span></span>             | <span data-ttu-id="677e7-138">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="677e7-138">[itemActionStat][]</span></span>      | <span data-ttu-id="677e7-139">有关此间隔中**移动**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="677e7-139">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="677e7-140">只读。</span><span class="sxs-lookup"><span data-stu-id="677e7-140">Read-only.</span></span>
| <span data-ttu-id="677e7-141">访问</span><span class="sxs-lookup"><span data-stu-id="677e7-141">access</span></span>           | <span data-ttu-id="677e7-142">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="677e7-142">[itemActionStat][]</span></span>      | <span data-ttu-id="677e7-143">有关此间隔中的**访问**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="677e7-143">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="677e7-144">只读。</span><span class="sxs-lookup"><span data-stu-id="677e7-144">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="677e7-147">关系</span><span class="sxs-lookup"><span data-stu-id="677e7-147">Relationships</span></span>

| <span data-ttu-id="677e7-148">关系名称</span><span class="sxs-lookup"><span data-stu-id="677e7-148">Relationship name</span></span> | <span data-ttu-id="677e7-149">类型</span><span class="sxs-lookup"><span data-stu-id="677e7-149">Type</span></span>                        | <span data-ttu-id="677e7-150">说明</span><span class="sxs-lookup"><span data-stu-id="677e7-150">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="677e7-151">activities</span><span class="sxs-lookup"><span data-stu-id="677e7-151">activities</span></span>        | <span data-ttu-id="677e7-152">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="677e7-152">[itemActivity][] collection</span></span> | <span data-ttu-id="677e7-153">公开此**itemActivityStat**资源中表示的**itemActivities** 。</span><span class="sxs-lookup"><span data-stu-id="677e7-153">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="677e7-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="677e7-155">JSON representation</span></span>

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
