---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
ms.openlocfilehash: 067cf88773b5f5d69b2b3538a2ddeab6741631a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041799"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="1618c-102">itemActivityStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="1618c-102">itemActivityStat resource type</span></span>

> <span data-ttu-id="1618c-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1618c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1618c-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1618c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1618c-105">**ItemActivityStat**资源提供有关发生的时间间隔内的活动信息。</span><span class="sxs-lookup"><span data-stu-id="1618c-105">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1618c-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1618c-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="1618c-107">属性</span><span class="sxs-lookup"><span data-stu-id="1618c-107">Properties</span></span>

| <span data-ttu-id="1618c-108">属性</span><span class="sxs-lookup"><span data-stu-id="1618c-108">Property</span></span>         | <span data-ttu-id="1618c-109">类型</span><span class="sxs-lookup"><span data-stu-id="1618c-109">Type</span></span>                    | <span data-ttu-id="1618c-110">说明</span><span class="sxs-lookup"><span data-stu-id="1618c-110">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="1618c-111">incompleteData</span><span class="sxs-lookup"><span data-stu-id="1618c-111">incompleteData</span></span>   | <span data-ttu-id="1618c-112">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="1618c-112">[incompleteData][]</span></span>      | <span data-ttu-id="1618c-113">指示此间隔中的统计信息基于不完整的数据。</span><span class="sxs-lookup"><span data-stu-id="1618c-113">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="1618c-114">只读。</span><span class="sxs-lookup"><span data-stu-id="1618c-114">Read-only.</span></span>
| <span data-ttu-id="1618c-115">isTrending</span><span class="sxs-lookup"><span data-stu-id="1618c-115">isTrending</span></span>       | <span data-ttu-id="1618c-116">布尔</span><span class="sxs-lookup"><span data-stu-id="1618c-116">Boolean</span></span>                 | <span data-ttu-id="1618c-117">指示是否项目"趋势。"</span><span class="sxs-lookup"><span data-stu-id="1618c-117">Indicates whether the item is "trending."</span></span> <span data-ttu-id="1618c-118">只读。</span><span class="sxs-lookup"><span data-stu-id="1618c-118">Read-only.</span></span>
| <span data-ttu-id="1618c-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1618c-119">startDateTime</span></span>    | <span data-ttu-id="1618c-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1618c-120">DateTimeOffset</span></span>          | <span data-ttu-id="1618c-121">当开始间隔。</span><span class="sxs-lookup"><span data-stu-id="1618c-121">When the interval starts.</span></span> <span data-ttu-id="1618c-122">只读。</span><span class="sxs-lookup"><span data-stu-id="1618c-122">Read-only.</span></span>
| <span data-ttu-id="1618c-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="1618c-123">endDateTime</span></span>      | <span data-ttu-id="1618c-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1618c-124">DateTimeOffset</span></span>          | <span data-ttu-id="1618c-125">当结束间隔。</span><span class="sxs-lookup"><span data-stu-id="1618c-125">When the interval ends.</span></span> <span data-ttu-id="1618c-126">只读。</span><span class="sxs-lookup"><span data-stu-id="1618c-126">Read-only.</span></span>
| <span data-ttu-id="1618c-127">create</span><span class="sxs-lookup"><span data-stu-id="1618c-127">create</span></span>           | <span data-ttu-id="1618c-128">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="1618c-128">[itemActionStat][]</span></span>      | <span data-ttu-id="1618c-129">有关此间隔中的**创建**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="1618c-129">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="1618c-130">只读。</span><span class="sxs-lookup"><span data-stu-id="1618c-130">Read-only.</span></span>
| <span data-ttu-id="1618c-131">edit</span><span class="sxs-lookup"><span data-stu-id="1618c-131">edit</span></span>             | <span data-ttu-id="1618c-132">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="1618c-132">[itemActionStat][]</span></span>      | <span data-ttu-id="1618c-133">有关此间隔中的**编辑**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="1618c-133">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="1618c-134">只读。</span><span class="sxs-lookup"><span data-stu-id="1618c-134">Read-only.</span></span>
| <span data-ttu-id="1618c-135">delete</span><span class="sxs-lookup"><span data-stu-id="1618c-135">delete</span></span>           | <span data-ttu-id="1618c-136">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="1618c-136">[itemActionStat][]</span></span>      | <span data-ttu-id="1618c-137">有关此间隔中的**删除**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="1618c-137">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="1618c-138">只读。</span><span class="sxs-lookup"><span data-stu-id="1618c-138">Read-only.</span></span>
| <span data-ttu-id="1618c-139">move</span><span class="sxs-lookup"><span data-stu-id="1618c-139">move</span></span>             | <span data-ttu-id="1618c-140">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="1618c-140">[itemActionStat][]</span></span>      | <span data-ttu-id="1618c-141">有关此间隔中的**移动**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="1618c-141">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="1618c-142">只读。</span><span class="sxs-lookup"><span data-stu-id="1618c-142">Read-only.</span></span>
| <span data-ttu-id="1618c-143">访问</span><span class="sxs-lookup"><span data-stu-id="1618c-143">access</span></span>           | <span data-ttu-id="1618c-144">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="1618c-144">[itemActionStat][]</span></span>      | <span data-ttu-id="1618c-145">有关此间隔中的**访问**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="1618c-145">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="1618c-146">只读。</span><span class="sxs-lookup"><span data-stu-id="1618c-146">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="1618c-149">关系</span><span class="sxs-lookup"><span data-stu-id="1618c-149">Relationships</span></span>

| <span data-ttu-id="1618c-150">关系名称</span><span class="sxs-lookup"><span data-stu-id="1618c-150">Relationship name</span></span> | <span data-ttu-id="1618c-151">类型</span><span class="sxs-lookup"><span data-stu-id="1618c-151">Type</span></span>                        | <span data-ttu-id="1618c-152">说明</span><span class="sxs-lookup"><span data-stu-id="1618c-152">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="1618c-153">activities</span><span class="sxs-lookup"><span data-stu-id="1618c-153">activities</span></span>        | <span data-ttu-id="1618c-154">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="1618c-154">[itemActivity][] collection</span></span> | <span data-ttu-id="1618c-155">公开**itemActivities**此**itemActivityStat**资源中表示。</span><span class="sxs-lookup"><span data-stu-id="1618c-155">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="1618c-157">注解</span><span class="sxs-lookup"><span data-stu-id="1618c-157">Remarks</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat"
} -->
