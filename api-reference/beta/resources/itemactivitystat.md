---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
localization_priority: Normal
ms.openlocfilehash: 08bbfd414a32e8eb8a0144d879ede55c71c19b89
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339872"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="77ae5-102">itemActivityStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="77ae5-102">itemActivityStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77ae5-103">**itemActivityStat**资源提供有关在一段时间内发生的活动的信息。</span><span class="sxs-lookup"><span data-stu-id="77ae5-103">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="77ae5-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77ae5-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="77ae5-105">属性</span><span class="sxs-lookup"><span data-stu-id="77ae5-105">Properties</span></span>

| <span data-ttu-id="77ae5-106">属性</span><span class="sxs-lookup"><span data-stu-id="77ae5-106">Property</span></span>         | <span data-ttu-id="77ae5-107">类型</span><span class="sxs-lookup"><span data-stu-id="77ae5-107">Type</span></span>                    | <span data-ttu-id="77ae5-108">说明</span><span class="sxs-lookup"><span data-stu-id="77ae5-108">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="77ae5-109">incompleteData</span><span class="sxs-lookup"><span data-stu-id="77ae5-109">incompleteData</span></span>   | <span data-ttu-id="77ae5-110">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="77ae5-110">[incompleteData][]</span></span>      | <span data-ttu-id="77ae5-111">指示此时间间隔中的统计信息基于不完整的数据。</span><span class="sxs-lookup"><span data-stu-id="77ae5-111">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="77ae5-112">只读。</span><span class="sxs-lookup"><span data-stu-id="77ae5-112">Read-only.</span></span>
| <span data-ttu-id="77ae5-113">isTrending</span><span class="sxs-lookup"><span data-stu-id="77ae5-113">isTrending</span></span>       | <span data-ttu-id="77ae5-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="77ae5-114">Boolean</span></span>                 | <span data-ttu-id="77ae5-115">指示项目是否为 "趋势"。</span><span class="sxs-lookup"><span data-stu-id="77ae5-115">Indicates whether the item is "trending."</span></span> <span data-ttu-id="77ae5-116">只读。</span><span class="sxs-lookup"><span data-stu-id="77ae5-116">Read-only.</span></span>
| <span data-ttu-id="77ae5-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="77ae5-117">startDateTime</span></span>    | <span data-ttu-id="77ae5-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77ae5-118">DateTimeOffset</span></span>          | <span data-ttu-id="77ae5-119">时间间隔开始时。</span><span class="sxs-lookup"><span data-stu-id="77ae5-119">When the interval starts.</span></span> <span data-ttu-id="77ae5-120">只读。</span><span class="sxs-lookup"><span data-stu-id="77ae5-120">Read-only.</span></span>
| <span data-ttu-id="77ae5-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="77ae5-121">endDateTime</span></span>      | <span data-ttu-id="77ae5-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77ae5-122">DateTimeOffset</span></span>          | <span data-ttu-id="77ae5-123">时间间隔结束时。</span><span class="sxs-lookup"><span data-stu-id="77ae5-123">When the interval ends.</span></span> <span data-ttu-id="77ae5-124">只读。</span><span class="sxs-lookup"><span data-stu-id="77ae5-124">Read-only.</span></span>
| <span data-ttu-id="77ae5-125">create</span><span class="sxs-lookup"><span data-stu-id="77ae5-125">create</span></span>           | <span data-ttu-id="77ae5-126">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="77ae5-126">[itemActionStat][]</span></span>      | <span data-ttu-id="77ae5-127">有关此间隔中的**创建**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="77ae5-127">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="77ae5-128">只读。</span><span class="sxs-lookup"><span data-stu-id="77ae5-128">Read-only.</span></span>
| <span data-ttu-id="77ae5-129">edit</span><span class="sxs-lookup"><span data-stu-id="77ae5-129">edit</span></span>             | <span data-ttu-id="77ae5-130">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="77ae5-130">[itemActionStat][]</span></span>      | <span data-ttu-id="77ae5-131">有关此间隔中的**编辑**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="77ae5-131">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="77ae5-132">只读。</span><span class="sxs-lookup"><span data-stu-id="77ae5-132">Read-only.</span></span>
| <span data-ttu-id="77ae5-133">delete</span><span class="sxs-lookup"><span data-stu-id="77ae5-133">delete</span></span>           | <span data-ttu-id="77ae5-134">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="77ae5-134">[itemActionStat][]</span></span>      | <span data-ttu-id="77ae5-135">有关此间隔中的**删除**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="77ae5-135">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="77ae5-136">只读。</span><span class="sxs-lookup"><span data-stu-id="77ae5-136">Read-only.</span></span>
| <span data-ttu-id="77ae5-137">move</span><span class="sxs-lookup"><span data-stu-id="77ae5-137">move</span></span>             | <span data-ttu-id="77ae5-138">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="77ae5-138">[itemActionStat][]</span></span>      | <span data-ttu-id="77ae5-139">有关此间隔中**移动**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="77ae5-139">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="77ae5-140">只读。</span><span class="sxs-lookup"><span data-stu-id="77ae5-140">Read-only.</span></span>
| <span data-ttu-id="77ae5-141">访问</span><span class="sxs-lookup"><span data-stu-id="77ae5-141">access</span></span>           | <span data-ttu-id="77ae5-142">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="77ae5-142">[itemActionStat][]</span></span>      | <span data-ttu-id="77ae5-143">有关此间隔中的**访问**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="77ae5-143">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="77ae5-144">只读。</span><span class="sxs-lookup"><span data-stu-id="77ae5-144">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="77ae5-147">关系</span><span class="sxs-lookup"><span data-stu-id="77ae5-147">Relationships</span></span>

| <span data-ttu-id="77ae5-148">关系名称</span><span class="sxs-lookup"><span data-stu-id="77ae5-148">Relationship name</span></span> | <span data-ttu-id="77ae5-149">类型</span><span class="sxs-lookup"><span data-stu-id="77ae5-149">Type</span></span>                        | <span data-ttu-id="77ae5-150">说明</span><span class="sxs-lookup"><span data-stu-id="77ae5-150">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="77ae5-151">activities</span><span class="sxs-lookup"><span data-stu-id="77ae5-151">activities</span></span>        | <span data-ttu-id="77ae5-152">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="77ae5-152">[itemActivity][] collection</span></span> | <span data-ttu-id="77ae5-153">公开此**itemActivityStat**资源中表示的**itemActivities** 。</span><span class="sxs-lookup"><span data-stu-id="77ae5-153">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="77ae5-155">注解</span><span class="sxs-lookup"><span data-stu-id="77ae5-155">Remarks</span></span>

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
