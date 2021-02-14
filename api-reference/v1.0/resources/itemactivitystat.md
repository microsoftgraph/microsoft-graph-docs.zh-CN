---
author: daspek
title: itemActivityStat 资源类型
description: ItemActivityStat 对象提供有关在项目上发生的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a33453fc884fc6dba7bd5b8fbcf4edc0261c11cb
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238678"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="fdb55-103">itemActivityStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="fdb55-103">itemActivityStat resource type</span></span>

<span data-ttu-id="fdb55-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdb55-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fdb55-105">**itemActivityStat** 资源提供有关时间间隔内发生的活动的信息。</span><span class="sxs-lookup"><span data-stu-id="fdb55-105">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="properties"></a><span data-ttu-id="fdb55-106">属性</span><span class="sxs-lookup"><span data-stu-id="fdb55-106">Properties</span></span>

| <span data-ttu-id="fdb55-107">属性</span><span class="sxs-lookup"><span data-stu-id="fdb55-107">Property</span></span>         | <span data-ttu-id="fdb55-108">类型</span><span class="sxs-lookup"><span data-stu-id="fdb55-108">Type</span></span>                    | <span data-ttu-id="fdb55-109">说明</span><span class="sxs-lookup"><span data-stu-id="fdb55-109">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="fdb55-110">incompleteData</span><span class="sxs-lookup"><span data-stu-id="fdb55-110">incompleteData</span></span>   | <span data-ttu-id="fdb55-111">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="fdb55-111">[incompleteData][]</span></span>      | <span data-ttu-id="fdb55-112">指示此间隔中的统计信息基于不完整的数据。</span><span class="sxs-lookup"><span data-stu-id="fdb55-112">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="fdb55-113">只读。</span><span class="sxs-lookup"><span data-stu-id="fdb55-113">Read-only.</span></span>
| <span data-ttu-id="fdb55-114">isTrending</span><span class="sxs-lookup"><span data-stu-id="fdb55-114">isTrending</span></span>       | <span data-ttu-id="fdb55-115">布尔</span><span class="sxs-lookup"><span data-stu-id="fdb55-115">Boolean</span></span>                 | <span data-ttu-id="fdb55-116">指示项目是否是"趋势"。</span><span class="sxs-lookup"><span data-stu-id="fdb55-116">Indicates whether the item is "trending."</span></span> <span data-ttu-id="fdb55-117">只读。</span><span class="sxs-lookup"><span data-stu-id="fdb55-117">Read-only.</span></span>
| <span data-ttu-id="fdb55-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fdb55-118">startDateTime</span></span>    | <span data-ttu-id="fdb55-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdb55-119">DateTimeOffset</span></span>          | <span data-ttu-id="fdb55-120">间隔开始时。</span><span class="sxs-lookup"><span data-stu-id="fdb55-120">When the interval starts.</span></span> <span data-ttu-id="fdb55-121">只读。</span><span class="sxs-lookup"><span data-stu-id="fdb55-121">Read-only.</span></span>
| <span data-ttu-id="fdb55-122">endDateTime</span><span class="sxs-lookup"><span data-stu-id="fdb55-122">endDateTime</span></span>      | <span data-ttu-id="fdb55-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdb55-123">DateTimeOffset</span></span>          | <span data-ttu-id="fdb55-124">时间间隔何时结束。</span><span class="sxs-lookup"><span data-stu-id="fdb55-124">When the interval ends.</span></span> <span data-ttu-id="fdb55-125">只读。</span><span class="sxs-lookup"><span data-stu-id="fdb55-125">Read-only.</span></span>
| <span data-ttu-id="fdb55-126">create</span><span class="sxs-lookup"><span data-stu-id="fdb55-126">create</span></span>           | <span data-ttu-id="fdb55-127">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="fdb55-127">[itemActionStat][]</span></span>      | <span data-ttu-id="fdb55-128">有关此 **间隔中的** 创建操作统计信息。</span><span class="sxs-lookup"><span data-stu-id="fdb55-128">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="fdb55-129">只读。</span><span class="sxs-lookup"><span data-stu-id="fdb55-129">Read-only.</span></span>
| <span data-ttu-id="fdb55-130">edit</span><span class="sxs-lookup"><span data-stu-id="fdb55-130">edit</span></span>             | <span data-ttu-id="fdb55-131">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="fdb55-131">[itemActionStat][]</span></span>      | <span data-ttu-id="fdb55-132">有关此 **间隔中的** 编辑操作统计信息。</span><span class="sxs-lookup"><span data-stu-id="fdb55-132">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="fdb55-133">只读。</span><span class="sxs-lookup"><span data-stu-id="fdb55-133">Read-only.</span></span>
| <span data-ttu-id="fdb55-134">delete</span><span class="sxs-lookup"><span data-stu-id="fdb55-134">delete</span></span>           | <span data-ttu-id="fdb55-135">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="fdb55-135">[itemActionStat][]</span></span>      | <span data-ttu-id="fdb55-136">有关此 **间隔中的** 删除操作统计信息。</span><span class="sxs-lookup"><span data-stu-id="fdb55-136">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="fdb55-137">只读。</span><span class="sxs-lookup"><span data-stu-id="fdb55-137">Read-only.</span></span>
| <span data-ttu-id="fdb55-138">move</span><span class="sxs-lookup"><span data-stu-id="fdb55-138">move</span></span>             | <span data-ttu-id="fdb55-139">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="fdb55-139">[itemActionStat][]</span></span>      | <span data-ttu-id="fdb55-140">有关此 **间隔中的** 移动操作统计信息。</span><span class="sxs-lookup"><span data-stu-id="fdb55-140">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="fdb55-141">只读。</span><span class="sxs-lookup"><span data-stu-id="fdb55-141">Read-only.</span></span>
| <span data-ttu-id="fdb55-142">access</span><span class="sxs-lookup"><span data-stu-id="fdb55-142">access</span></span>           | <span data-ttu-id="fdb55-143">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="fdb55-143">[itemActionStat][]</span></span>      | <span data-ttu-id="fdb55-144">有关此 **间隔中的** 访问操作统计信息。</span><span class="sxs-lookup"><span data-stu-id="fdb55-144">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="fdb55-145">只读。</span><span class="sxs-lookup"><span data-stu-id="fdb55-145">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="fdb55-148">关系</span><span class="sxs-lookup"><span data-stu-id="fdb55-148">Relationships</span></span>

| <span data-ttu-id="fdb55-149">关系名称</span><span class="sxs-lookup"><span data-stu-id="fdb55-149">Relationship name</span></span> | <span data-ttu-id="fdb55-150">类型</span><span class="sxs-lookup"><span data-stu-id="fdb55-150">Type</span></span>                        | <span data-ttu-id="fdb55-151">说明</span><span class="sxs-lookup"><span data-stu-id="fdb55-151">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="fdb55-152">activities</span><span class="sxs-lookup"><span data-stu-id="fdb55-152">activities</span></span>        | <span data-ttu-id="fdb55-153">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="fdb55-153">[itemActivity][] collection</span></span> | <span data-ttu-id="fdb55-154">公开此 **itemActivityStat** 资源中表示的 **itemActivities。**</span><span class="sxs-lookup"><span data-stu-id="fdb55-154">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="fdb55-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fdb55-156">JSON representation</span></span>

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

