---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
localization_priority: Normal
ms.openlocfilehash: 1362116c0dbe997eda941cb790e00e9ddb078ae4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517629"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="aa63b-102">itemActivityStat 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa63b-102">itemActivityStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa63b-103">**ItemActivityStat**资源提供有关发生的时间间隔内的活动信息。</span><span class="sxs-lookup"><span data-stu-id="aa63b-103">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa63b-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa63b-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="aa63b-105">属性</span><span class="sxs-lookup"><span data-stu-id="aa63b-105">Properties</span></span>

| <span data-ttu-id="aa63b-106">属性</span><span class="sxs-lookup"><span data-stu-id="aa63b-106">Property</span></span>         | <span data-ttu-id="aa63b-107">类型</span><span class="sxs-lookup"><span data-stu-id="aa63b-107">Type</span></span>                    | <span data-ttu-id="aa63b-108">说明</span><span class="sxs-lookup"><span data-stu-id="aa63b-108">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="aa63b-109">incompleteData</span><span class="sxs-lookup"><span data-stu-id="aa63b-109">incompleteData</span></span>   | <span data-ttu-id="aa63b-110">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="aa63b-110">[incompleteData][]</span></span>      | <span data-ttu-id="aa63b-111">指示此间隔中的统计信息基于不完整的数据。</span><span class="sxs-lookup"><span data-stu-id="aa63b-111">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="aa63b-112">只读。</span><span class="sxs-lookup"><span data-stu-id="aa63b-112">Read-only.</span></span>
| <span data-ttu-id="aa63b-113">isTrending</span><span class="sxs-lookup"><span data-stu-id="aa63b-113">isTrending</span></span>       | <span data-ttu-id="aa63b-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa63b-114">Boolean</span></span>                 | <span data-ttu-id="aa63b-115">指示是否项目"趋势。"</span><span class="sxs-lookup"><span data-stu-id="aa63b-115">Indicates whether the item is "trending."</span></span> <span data-ttu-id="aa63b-116">只读。</span><span class="sxs-lookup"><span data-stu-id="aa63b-116">Read-only.</span></span>
| <span data-ttu-id="aa63b-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="aa63b-117">startDateTime</span></span>    | <span data-ttu-id="aa63b-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa63b-118">DateTimeOffset</span></span>          | <span data-ttu-id="aa63b-119">当开始间隔。</span><span class="sxs-lookup"><span data-stu-id="aa63b-119">When the interval starts.</span></span> <span data-ttu-id="aa63b-120">只读。</span><span class="sxs-lookup"><span data-stu-id="aa63b-120">Read-only.</span></span>
| <span data-ttu-id="aa63b-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="aa63b-121">endDateTime</span></span>      | <span data-ttu-id="aa63b-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa63b-122">DateTimeOffset</span></span>          | <span data-ttu-id="aa63b-123">当结束间隔。</span><span class="sxs-lookup"><span data-stu-id="aa63b-123">When the interval ends.</span></span> <span data-ttu-id="aa63b-124">只读。</span><span class="sxs-lookup"><span data-stu-id="aa63b-124">Read-only.</span></span>
| <span data-ttu-id="aa63b-125">create</span><span class="sxs-lookup"><span data-stu-id="aa63b-125">create</span></span>           | <span data-ttu-id="aa63b-126">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="aa63b-126">[itemActionStat][]</span></span>      | <span data-ttu-id="aa63b-127">有关此间隔中的**创建**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="aa63b-127">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="aa63b-128">只读。</span><span class="sxs-lookup"><span data-stu-id="aa63b-128">Read-only.</span></span>
| <span data-ttu-id="aa63b-129">edit</span><span class="sxs-lookup"><span data-stu-id="aa63b-129">edit</span></span>             | <span data-ttu-id="aa63b-130">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="aa63b-130">[itemActionStat][]</span></span>      | <span data-ttu-id="aa63b-131">有关此间隔中的**编辑**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="aa63b-131">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="aa63b-132">只读。</span><span class="sxs-lookup"><span data-stu-id="aa63b-132">Read-only.</span></span>
| <span data-ttu-id="aa63b-133">delete</span><span class="sxs-lookup"><span data-stu-id="aa63b-133">delete</span></span>           | <span data-ttu-id="aa63b-134">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="aa63b-134">[itemActionStat][]</span></span>      | <span data-ttu-id="aa63b-135">有关此间隔中的**删除**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="aa63b-135">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="aa63b-136">只读。</span><span class="sxs-lookup"><span data-stu-id="aa63b-136">Read-only.</span></span>
| <span data-ttu-id="aa63b-137">move</span><span class="sxs-lookup"><span data-stu-id="aa63b-137">move</span></span>             | <span data-ttu-id="aa63b-138">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="aa63b-138">[itemActionStat][]</span></span>      | <span data-ttu-id="aa63b-139">有关此间隔中的**移动**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="aa63b-139">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="aa63b-140">只读。</span><span class="sxs-lookup"><span data-stu-id="aa63b-140">Read-only.</span></span>
| <span data-ttu-id="aa63b-141">Access</span><span class="sxs-lookup"><span data-stu-id="aa63b-141">access</span></span>           | <span data-ttu-id="aa63b-142">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="aa63b-142">[itemActionStat][]</span></span>      | <span data-ttu-id="aa63b-143">有关此间隔中的**访问**操作的统计信息。</span><span class="sxs-lookup"><span data-stu-id="aa63b-143">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="aa63b-144">只读。</span><span class="sxs-lookup"><span data-stu-id="aa63b-144">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="aa63b-147">关系</span><span class="sxs-lookup"><span data-stu-id="aa63b-147">Relationships</span></span>

| <span data-ttu-id="aa63b-148">关系名称</span><span class="sxs-lookup"><span data-stu-id="aa63b-148">Relationship name</span></span> | <span data-ttu-id="aa63b-149">类型</span><span class="sxs-lookup"><span data-stu-id="aa63b-149">Type</span></span>                        | <span data-ttu-id="aa63b-150">说明</span><span class="sxs-lookup"><span data-stu-id="aa63b-150">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="aa63b-151">activities</span><span class="sxs-lookup"><span data-stu-id="aa63b-151">activities</span></span>        | <span data-ttu-id="aa63b-152">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="aa63b-152">[itemActivity][] collection</span></span> | <span data-ttu-id="aa63b-153">公开**itemActivities**此**itemActivityStat**资源中表示。</span><span class="sxs-lookup"><span data-stu-id="aa63b-153">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="aa63b-155">注解</span><span class="sxs-lookup"><span data-stu-id="aa63b-155">Remarks</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactivitystat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
