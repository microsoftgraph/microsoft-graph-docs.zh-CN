---
author: daspek
description: ItemActivityStat 资源提供有关在一段时间内发生的活动的信息。
ms.date: 09/14/2017
title: ItemActivityStat
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c21183911e111b2070d463f4552f913d93780493
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075656"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="2b72d-103">itemActivityStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b72d-103">itemActivityStat resource type</span></span>

<span data-ttu-id="2b72d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b72d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b72d-105">**ItemActivityStat**资源提供有关在一段时间内发生的活动的信息。</span><span class="sxs-lookup"><span data-stu-id="2b72d-105">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b72d-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b72d-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2b72d-107">属性</span><span class="sxs-lookup"><span data-stu-id="2b72d-107">Properties</span></span>

| <span data-ttu-id="2b72d-108">属性</span><span class="sxs-lookup"><span data-stu-id="2b72d-108">Property</span></span>         | <span data-ttu-id="2b72d-109">类型</span><span class="sxs-lookup"><span data-stu-id="2b72d-109">Type</span></span>                    | <span data-ttu-id="2b72d-110">说明</span><span class="sxs-lookup"><span data-stu-id="2b72d-110">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="2b72d-111">incompleteData</span><span class="sxs-lookup"><span data-stu-id="2b72d-111">incompleteData</span></span>   | <span data-ttu-id="2b72d-112">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="2b72d-112">[incompleteData][]</span></span>      | <span data-ttu-id="2b72d-113">指示此时间间隔中的统计信息基于不完整的数据。</span><span class="sxs-lookup"><span data-stu-id="2b72d-113">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="2b72d-114">只读。</span><span class="sxs-lookup"><span data-stu-id="2b72d-114">Read-only.</span></span>
| <span data-ttu-id="2b72d-115">isTrending</span><span class="sxs-lookup"><span data-stu-id="2b72d-115">isTrending</span></span>       | <span data-ttu-id="2b72d-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b72d-116">Boolean</span></span>                 | <span data-ttu-id="2b72d-117">指示项目是否为 "趋势"。</span><span class="sxs-lookup"><span data-stu-id="2b72d-117">Indicates whether the item is "trending."</span></span> <span data-ttu-id="2b72d-118">只读。</span><span class="sxs-lookup"><span data-stu-id="2b72d-118">Read-only.</span></span>
| <span data-ttu-id="2b72d-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2b72d-119">startDateTime</span></span>    | <span data-ttu-id="2b72d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b72d-120">DateTimeOffset</span></span>          | <span data-ttu-id="2b72d-121">时间间隔开始时。</span><span class="sxs-lookup"><span data-stu-id="2b72d-121">When the interval starts.</span></span> <span data-ttu-id="2b72d-122">只读。</span><span class="sxs-lookup"><span data-stu-id="2b72d-122">Read-only.</span></span>
| <span data-ttu-id="2b72d-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="2b72d-123">endDateTime</span></span>      | <span data-ttu-id="2b72d-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b72d-124">DateTimeOffset</span></span>          | <span data-ttu-id="2b72d-125">时间间隔结束时。</span><span class="sxs-lookup"><span data-stu-id="2b72d-125">When the interval ends.</span></span> <span data-ttu-id="2b72d-126">只读。</span><span class="sxs-lookup"><span data-stu-id="2b72d-126">Read-only.</span></span>
| <span data-ttu-id="2b72d-127">create</span><span class="sxs-lookup"><span data-stu-id="2b72d-127">create</span></span>           | <span data-ttu-id="2b72d-128">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="2b72d-128">[itemActionStat][]</span></span>      | <span data-ttu-id="2b72d-129">有关此间隔中的 **创建** 操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="2b72d-129">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="2b72d-130">只读。</span><span class="sxs-lookup"><span data-stu-id="2b72d-130">Read-only.</span></span>
| <span data-ttu-id="2b72d-131">edit</span><span class="sxs-lookup"><span data-stu-id="2b72d-131">edit</span></span>             | <span data-ttu-id="2b72d-132">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="2b72d-132">[itemActionStat][]</span></span>      | <span data-ttu-id="2b72d-133">有关此间隔中的 **编辑** 操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="2b72d-133">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="2b72d-134">只读。</span><span class="sxs-lookup"><span data-stu-id="2b72d-134">Read-only.</span></span>
| <span data-ttu-id="2b72d-135">delete</span><span class="sxs-lookup"><span data-stu-id="2b72d-135">delete</span></span>           | <span data-ttu-id="2b72d-136">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="2b72d-136">[itemActionStat][]</span></span>      | <span data-ttu-id="2b72d-137">有关此间隔中的 **删除** 操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="2b72d-137">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="2b72d-138">只读。</span><span class="sxs-lookup"><span data-stu-id="2b72d-138">Read-only.</span></span>
| <span data-ttu-id="2b72d-139">move</span><span class="sxs-lookup"><span data-stu-id="2b72d-139">move</span></span>             | <span data-ttu-id="2b72d-140">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="2b72d-140">[itemActionStat][]</span></span>      | <span data-ttu-id="2b72d-141">有关此间隔中 **移动** 操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="2b72d-141">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="2b72d-142">只读。</span><span class="sxs-lookup"><span data-stu-id="2b72d-142">Read-only.</span></span>
| <span data-ttu-id="2b72d-143">访问</span><span class="sxs-lookup"><span data-stu-id="2b72d-143">access</span></span>           | <span data-ttu-id="2b72d-144">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="2b72d-144">[itemActionStat][]</span></span>      | <span data-ttu-id="2b72d-145">有关此间隔中的 **访问** 操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="2b72d-145">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="2b72d-146">只读。</span><span class="sxs-lookup"><span data-stu-id="2b72d-146">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="2b72d-149">关系</span><span class="sxs-lookup"><span data-stu-id="2b72d-149">Relationships</span></span>

| <span data-ttu-id="2b72d-150">关系名称</span><span class="sxs-lookup"><span data-stu-id="2b72d-150">Relationship name</span></span> | <span data-ttu-id="2b72d-151">类型</span><span class="sxs-lookup"><span data-stu-id="2b72d-151">Type</span></span>                        | <span data-ttu-id="2b72d-152">说明</span><span class="sxs-lookup"><span data-stu-id="2b72d-152">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="2b72d-153">activities</span><span class="sxs-lookup"><span data-stu-id="2b72d-153">activities</span></span>        | <span data-ttu-id="2b72d-154">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="2b72d-154">[itemActivity][] collection</span></span> | <span data-ttu-id="2b72d-155">公开此**itemActivityStat**资源中表示的**itemActivities** 。</span><span class="sxs-lookup"><span data-stu-id="2b72d-155">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="2b72d-157">注解</span><span class="sxs-lookup"><span data-stu-id="2b72d-157">Remarks</span></span>

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


