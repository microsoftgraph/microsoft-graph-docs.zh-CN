---
author: daspek
description: ItemActivityStat 资源提供有关在一段时间内发生的活动的信息。
ms.date: 09/14/2017
title: ItemActivityStat
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 612acf6ef619f13b0c334dd2046041b25020f450
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523112"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="6920e-103">itemActivityStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="6920e-103">itemActivityStat resource type</span></span>

<span data-ttu-id="6920e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6920e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6920e-105">**ItemActivityStat**资源提供有关在一段时间内发生的活动的信息。</span><span class="sxs-lookup"><span data-stu-id="6920e-105">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6920e-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6920e-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6920e-107">属性</span><span class="sxs-lookup"><span data-stu-id="6920e-107">Properties</span></span>

| <span data-ttu-id="6920e-108">属性</span><span class="sxs-lookup"><span data-stu-id="6920e-108">Property</span></span>         | <span data-ttu-id="6920e-109">类型</span><span class="sxs-lookup"><span data-stu-id="6920e-109">Type</span></span>                    | <span data-ttu-id="6920e-110">说明</span><span class="sxs-lookup"><span data-stu-id="6920e-110">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="6920e-111">incompleteData</span><span class="sxs-lookup"><span data-stu-id="6920e-111">incompleteData</span></span>   | <span data-ttu-id="6920e-112">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="6920e-112">[incompleteData][]</span></span>      | <span data-ttu-id="6920e-113">指示此时间间隔中的统计信息基于不完整的数据。</span><span class="sxs-lookup"><span data-stu-id="6920e-113">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="6920e-114">只读。</span><span class="sxs-lookup"><span data-stu-id="6920e-114">Read-only.</span></span>
| <span data-ttu-id="6920e-115">isTrending</span><span class="sxs-lookup"><span data-stu-id="6920e-115">isTrending</span></span>       | <span data-ttu-id="6920e-116">布尔</span><span class="sxs-lookup"><span data-stu-id="6920e-116">Boolean</span></span>                 | <span data-ttu-id="6920e-117">指示项目是否为 "趋势"。</span><span class="sxs-lookup"><span data-stu-id="6920e-117">Indicates whether the item is "trending."</span></span> <span data-ttu-id="6920e-118">只读。</span><span class="sxs-lookup"><span data-stu-id="6920e-118">Read-only.</span></span>
| <span data-ttu-id="6920e-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6920e-119">startDateTime</span></span>    | <span data-ttu-id="6920e-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6920e-120">DateTimeOffset</span></span>          | <span data-ttu-id="6920e-121">时间间隔开始时。</span><span class="sxs-lookup"><span data-stu-id="6920e-121">When the interval starts.</span></span> <span data-ttu-id="6920e-122">只读。</span><span class="sxs-lookup"><span data-stu-id="6920e-122">Read-only.</span></span>
| <span data-ttu-id="6920e-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6920e-123">endDateTime</span></span>      | <span data-ttu-id="6920e-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6920e-124">DateTimeOffset</span></span>          | <span data-ttu-id="6920e-125">时间间隔结束时。</span><span class="sxs-lookup"><span data-stu-id="6920e-125">When the interval ends.</span></span> <span data-ttu-id="6920e-126">只读。</span><span class="sxs-lookup"><span data-stu-id="6920e-126">Read-only.</span></span>
| <span data-ttu-id="6920e-127">create</span><span class="sxs-lookup"><span data-stu-id="6920e-127">create</span></span>           | <span data-ttu-id="6920e-128">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="6920e-128">[itemActionStat][]</span></span>      | <span data-ttu-id="6920e-129">有关此间隔中的**创建**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="6920e-129">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="6920e-130">只读。</span><span class="sxs-lookup"><span data-stu-id="6920e-130">Read-only.</span></span>
| <span data-ttu-id="6920e-131">edit</span><span class="sxs-lookup"><span data-stu-id="6920e-131">edit</span></span>             | <span data-ttu-id="6920e-132">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="6920e-132">[itemActionStat][]</span></span>      | <span data-ttu-id="6920e-133">有关此间隔中的**编辑**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="6920e-133">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="6920e-134">只读。</span><span class="sxs-lookup"><span data-stu-id="6920e-134">Read-only.</span></span>
| <span data-ttu-id="6920e-135">delete</span><span class="sxs-lookup"><span data-stu-id="6920e-135">delete</span></span>           | <span data-ttu-id="6920e-136">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="6920e-136">[itemActionStat][]</span></span>      | <span data-ttu-id="6920e-137">有关此间隔中的**删除**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="6920e-137">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="6920e-138">只读。</span><span class="sxs-lookup"><span data-stu-id="6920e-138">Read-only.</span></span>
| <span data-ttu-id="6920e-139">move</span><span class="sxs-lookup"><span data-stu-id="6920e-139">move</span></span>             | <span data-ttu-id="6920e-140">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="6920e-140">[itemActionStat][]</span></span>      | <span data-ttu-id="6920e-141">有关此间隔中**移动**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="6920e-141">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="6920e-142">只读。</span><span class="sxs-lookup"><span data-stu-id="6920e-142">Read-only.</span></span>
| <span data-ttu-id="6920e-143">访问</span><span class="sxs-lookup"><span data-stu-id="6920e-143">access</span></span>           | <span data-ttu-id="6920e-144">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="6920e-144">[itemActionStat][]</span></span>      | <span data-ttu-id="6920e-145">有关此间隔中的**访问**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="6920e-145">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="6920e-146">只读。</span><span class="sxs-lookup"><span data-stu-id="6920e-146">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="6920e-149">关系</span><span class="sxs-lookup"><span data-stu-id="6920e-149">Relationships</span></span>

| <span data-ttu-id="6920e-150">关系名称</span><span class="sxs-lookup"><span data-stu-id="6920e-150">Relationship name</span></span> | <span data-ttu-id="6920e-151">类型</span><span class="sxs-lookup"><span data-stu-id="6920e-151">Type</span></span>                        | <span data-ttu-id="6920e-152">说明</span><span class="sxs-lookup"><span data-stu-id="6920e-152">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="6920e-153">activities</span><span class="sxs-lookup"><span data-stu-id="6920e-153">activities</span></span>        | <span data-ttu-id="6920e-154">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="6920e-154">[itemActivity][] collection</span></span> | <span data-ttu-id="6920e-155">公开此**itemActivityStat**资源中表示的**itemActivities** 。</span><span class="sxs-lookup"><span data-stu-id="6920e-155">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="6920e-157">注解</span><span class="sxs-lookup"><span data-stu-id="6920e-157">Remarks</span></span>

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
