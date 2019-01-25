---
title: plannerBucket 资源类型
description: ) 中的 Office 365 中的计划任务。 它包含在 plannerPlan，并且可以具有的 plannerTasks 集合。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 85cf30bc13b3236928e662807a144f81614adbd7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524455"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="9d489-104">plannerBucket 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d489-104">plannerBucket resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d489-p102">**plannerBucket** 资源表示 Office 365 计划中的任务的存储桶（或“自定义列”）。它包含在 [plannerPlan](plannerplan.md) 之中，并且可能具有 [plannerTasks](plannertask.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="9d489-p102">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="9d489-107">方法</span><span class="sxs-lookup"><span data-stu-id="9d489-107">Methods</span></span>

| <span data-ttu-id="9d489-108">方法</span><span class="sxs-lookup"><span data-stu-id="9d489-108">Method</span></span>           | <span data-ttu-id="9d489-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9d489-109">Return Type</span></span>    |<span data-ttu-id="9d489-110">说明</span><span class="sxs-lookup"><span data-stu-id="9d489-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9d489-111">Get plannerBucket</span><span class="sxs-lookup"><span data-stu-id="9d489-111">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="9d489-112">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="9d489-112">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="9d489-113">读取 **plannerBucket** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9d489-113">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="9d489-114">List plannerTasks</span><span class="sxs-lookup"><span data-stu-id="9d489-114">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="9d489-115">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9d489-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="9d489-116">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9d489-116">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="9d489-117">Create</span><span class="sxs-lookup"><span data-stu-id="9d489-117">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="9d489-118">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="9d489-118">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="9d489-119">新建 **plannerBucket** 对象。</span><span class="sxs-lookup"><span data-stu-id="9d489-119">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="9d489-120">Update</span><span class="sxs-lookup"><span data-stu-id="9d489-120">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="9d489-121">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="9d489-121">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="9d489-122">更新 **plannerBucket** 对象。</span><span class="sxs-lookup"><span data-stu-id="9d489-122">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="9d489-123">Delete</span><span class="sxs-lookup"><span data-stu-id="9d489-123">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="9d489-124">无</span><span class="sxs-lookup"><span data-stu-id="9d489-124">None</span></span> |<span data-ttu-id="9d489-125">删除 **plannerBucket** 对象。</span><span class="sxs-lookup"><span data-stu-id="9d489-125">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9d489-126">属性</span><span class="sxs-lookup"><span data-stu-id="9d489-126">Properties</span></span>
| <span data-ttu-id="9d489-127">属性</span><span class="sxs-lookup"><span data-stu-id="9d489-127">Property</span></span>     | <span data-ttu-id="9d489-128">类型</span><span class="sxs-lookup"><span data-stu-id="9d489-128">Type</span></span>   |<span data-ttu-id="9d489-129">说明</span><span class="sxs-lookup"><span data-stu-id="9d489-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d489-130">id</span><span class="sxs-lookup"><span data-stu-id="9d489-130">id</span></span>|<span data-ttu-id="9d489-131">String</span><span class="sxs-lookup"><span data-stu-id="9d489-131">String</span></span>| <span data-ttu-id="9d489-132">只读。</span><span class="sxs-lookup"><span data-stu-id="9d489-132">Read-only.</span></span> <span data-ttu-id="9d489-133">存储桶的 ID。</span><span class="sxs-lookup"><span data-stu-id="9d489-133">ID of the bucket.</span></span> <span data-ttu-id="9d489-134">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="9d489-134">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="9d489-135">服务上执行[格式验证](tasks-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="9d489-135">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="9d489-136">name</span><span class="sxs-lookup"><span data-stu-id="9d489-136">name</span></span>|<span data-ttu-id="9d489-137">String</span><span class="sxs-lookup"><span data-stu-id="9d489-137">String</span></span>|<span data-ttu-id="9d489-138">存储桶的名称。</span><span class="sxs-lookup"><span data-stu-id="9d489-138">Name of the bucket.</span></span>|
|<span data-ttu-id="9d489-139">orderHint</span><span class="sxs-lookup"><span data-stu-id="9d489-139">orderHint</span></span>|<span data-ttu-id="9d489-140">String</span><span class="sxs-lookup"><span data-stu-id="9d489-140">String</span></span>|<span data-ttu-id="9d489-p104">用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="9d489-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="9d489-143">planId</span><span class="sxs-lookup"><span data-stu-id="9d489-143">planId</span></span>|<span data-ttu-id="9d489-144">String</span><span class="sxs-lookup"><span data-stu-id="9d489-144">String</span></span>|<span data-ttu-id="9d489-145">此存储桶所属的计划 ID。</span><span class="sxs-lookup"><span data-stu-id="9d489-145">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d489-146">关系</span><span class="sxs-lookup"><span data-stu-id="9d489-146">Relationships</span></span>
| <span data-ttu-id="9d489-147">关系</span><span class="sxs-lookup"><span data-stu-id="9d489-147">Relationship</span></span> | <span data-ttu-id="9d489-148">类型</span><span class="sxs-lookup"><span data-stu-id="9d489-148">Type</span></span>   |<span data-ttu-id="9d489-149">说明</span><span class="sxs-lookup"><span data-stu-id="9d489-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d489-150">tasks</span><span class="sxs-lookup"><span data-stu-id="9d489-150">tasks</span></span>|<span data-ttu-id="9d489-151">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="9d489-151">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="9d489-p105">只读。可为 NULL。存储桶中的任务集合。</span><span class="sxs-lookup"><span data-stu-id="9d489-p105">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d489-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d489-155">JSON representation</span></span>
<span data-ttu-id="9d489-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d489-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerbucket.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
