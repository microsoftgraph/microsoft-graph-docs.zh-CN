---
author: daspek
ms.author: dspektor
title: itemActivityStat 资源类型
description: ItemActivityStat 对象提供有关项目上发生的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 11b19e4b953d4353382aec15071c6589b5bb23c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447666"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="99d48-103">itemActivityStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="99d48-103">itemActivityStat resource type</span></span>

<span data-ttu-id="99d48-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="99d48-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="99d48-105">**ItemActivityStat**资源提供有关在一段时间内发生的活动的信息。</span><span class="sxs-lookup"><span data-stu-id="99d48-105">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="properties"></a><span data-ttu-id="99d48-106">属性</span><span class="sxs-lookup"><span data-stu-id="99d48-106">Properties</span></span>

| <span data-ttu-id="99d48-107">属性</span><span class="sxs-lookup"><span data-stu-id="99d48-107">Property</span></span>         | <span data-ttu-id="99d48-108">类型</span><span class="sxs-lookup"><span data-stu-id="99d48-108">Type</span></span>                    | <span data-ttu-id="99d48-109">说明</span><span class="sxs-lookup"><span data-stu-id="99d48-109">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="99d48-110">incompleteData</span><span class="sxs-lookup"><span data-stu-id="99d48-110">incompleteData</span></span>   | <span data-ttu-id="99d48-111">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="99d48-111">[incompleteData][]</span></span>      | <span data-ttu-id="99d48-112">指示此时间间隔中的统计信息基于不完整的数据。</span><span class="sxs-lookup"><span data-stu-id="99d48-112">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="99d48-113">只读。</span><span class="sxs-lookup"><span data-stu-id="99d48-113">Read-only.</span></span>
| <span data-ttu-id="99d48-114">isTrending</span><span class="sxs-lookup"><span data-stu-id="99d48-114">isTrending</span></span>       | <span data-ttu-id="99d48-115">布尔</span><span class="sxs-lookup"><span data-stu-id="99d48-115">Boolean</span></span>                 | <span data-ttu-id="99d48-116">指示项目是否为 "趋势"。</span><span class="sxs-lookup"><span data-stu-id="99d48-116">Indicates whether the item is "trending."</span></span> <span data-ttu-id="99d48-117">只读。</span><span class="sxs-lookup"><span data-stu-id="99d48-117">Read-only.</span></span>
| <span data-ttu-id="99d48-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="99d48-118">startDateTime</span></span>    | <span data-ttu-id="99d48-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99d48-119">DateTimeOffset</span></span>          | <span data-ttu-id="99d48-120">时间间隔开始时。</span><span class="sxs-lookup"><span data-stu-id="99d48-120">When the interval starts.</span></span> <span data-ttu-id="99d48-121">只读。</span><span class="sxs-lookup"><span data-stu-id="99d48-121">Read-only.</span></span>
| <span data-ttu-id="99d48-122">endDateTime</span><span class="sxs-lookup"><span data-stu-id="99d48-122">endDateTime</span></span>      | <span data-ttu-id="99d48-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99d48-123">DateTimeOffset</span></span>          | <span data-ttu-id="99d48-124">时间间隔结束时。</span><span class="sxs-lookup"><span data-stu-id="99d48-124">When the interval ends.</span></span> <span data-ttu-id="99d48-125">只读。</span><span class="sxs-lookup"><span data-stu-id="99d48-125">Read-only.</span></span>
| <span data-ttu-id="99d48-126">create</span><span class="sxs-lookup"><span data-stu-id="99d48-126">create</span></span>           | <span data-ttu-id="99d48-127">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="99d48-127">[itemActionStat][]</span></span>      | <span data-ttu-id="99d48-128">有关此间隔中的**创建**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="99d48-128">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="99d48-129">只读。</span><span class="sxs-lookup"><span data-stu-id="99d48-129">Read-only.</span></span>
| <span data-ttu-id="99d48-130">edit</span><span class="sxs-lookup"><span data-stu-id="99d48-130">edit</span></span>             | <span data-ttu-id="99d48-131">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="99d48-131">[itemActionStat][]</span></span>      | <span data-ttu-id="99d48-132">有关此间隔中的**编辑**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="99d48-132">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="99d48-133">只读。</span><span class="sxs-lookup"><span data-stu-id="99d48-133">Read-only.</span></span>
| <span data-ttu-id="99d48-134">delete</span><span class="sxs-lookup"><span data-stu-id="99d48-134">delete</span></span>           | <span data-ttu-id="99d48-135">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="99d48-135">[itemActionStat][]</span></span>      | <span data-ttu-id="99d48-136">有关此间隔中的**删除**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="99d48-136">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="99d48-137">只读。</span><span class="sxs-lookup"><span data-stu-id="99d48-137">Read-only.</span></span>
| <span data-ttu-id="99d48-138">move</span><span class="sxs-lookup"><span data-stu-id="99d48-138">move</span></span>             | <span data-ttu-id="99d48-139">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="99d48-139">[itemActionStat][]</span></span>      | <span data-ttu-id="99d48-140">有关此间隔中**移动**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="99d48-140">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="99d48-141">只读。</span><span class="sxs-lookup"><span data-stu-id="99d48-141">Read-only.</span></span>
| <span data-ttu-id="99d48-142">访问</span><span class="sxs-lookup"><span data-stu-id="99d48-142">access</span></span>           | <span data-ttu-id="99d48-143">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="99d48-143">[itemActionStat][]</span></span>      | <span data-ttu-id="99d48-144">有关此间隔中的**访问**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="99d48-144">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="99d48-145">只读。</span><span class="sxs-lookup"><span data-stu-id="99d48-145">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="99d48-148">关系</span><span class="sxs-lookup"><span data-stu-id="99d48-148">Relationships</span></span>

| <span data-ttu-id="99d48-149">关系名称</span><span class="sxs-lookup"><span data-stu-id="99d48-149">Relationship name</span></span> | <span data-ttu-id="99d48-150">类型</span><span class="sxs-lookup"><span data-stu-id="99d48-150">Type</span></span>                        | <span data-ttu-id="99d48-151">说明</span><span class="sxs-lookup"><span data-stu-id="99d48-151">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="99d48-152">activities</span><span class="sxs-lookup"><span data-stu-id="99d48-152">activities</span></span>        | <span data-ttu-id="99d48-153">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="99d48-153">[itemActivity][] collection</span></span> | <span data-ttu-id="99d48-154">公开此**itemActivityStat**资源中表示的**itemActivities** 。</span><span class="sxs-lookup"><span data-stu-id="99d48-154">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="99d48-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99d48-156">JSON representation</span></span>

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
