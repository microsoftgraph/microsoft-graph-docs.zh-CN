---
title: plannerBucketTaskBoardTaskFormat 资源类型
description: '**PlannerBucketTaskBoardTaskFormat**资源表示用于在任务板的 bucket 视图中正确呈现任务的信息，该信息是按分配给) 的存储桶中的任务组织的视图 (。 每个任务都有一个与之关联的 **plannerBucketTaskBoardTaskFormat** 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: f90d90cd0b625c612b125ffc031fe6c3e252a253
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026529"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="52afc-104">plannerBucketTaskBoardTaskFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="52afc-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="52afc-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52afc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52afc-106">**PlannerBucketTaskBoardTaskFormat**资源表示用于在任务板的 bucket 视图中正确呈现任务的信息，该信息是按分配给) 的存储桶中的任务组织的视图 (。</span><span class="sxs-lookup"><span data-stu-id="52afc-106">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to).</span></span> <span data-ttu-id="52afc-107">每个 [任务](plannertask.md) 都有一个与之关联的 **plannerBucketTaskBoardTaskFormat** 对象。</span><span class="sxs-lookup"><span data-stu-id="52afc-107">Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="52afc-108">方法</span><span class="sxs-lookup"><span data-stu-id="52afc-108">Methods</span></span>

| <span data-ttu-id="52afc-109">方法</span><span class="sxs-lookup"><span data-stu-id="52afc-109">Method</span></span>           | <span data-ttu-id="52afc-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="52afc-110">Return Type</span></span>    |<span data-ttu-id="52afc-111">说明</span><span class="sxs-lookup"><span data-stu-id="52afc-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52afc-112">获取 plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="52afc-112">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="52afc-113">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="52afc-113">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="52afc-114">读取 **plannerBucketTaskBoardTaskFormat** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="52afc-114">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="52afc-115">更新</span><span class="sxs-lookup"><span data-stu-id="52afc-115">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="52afc-116">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="52afc-116">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="52afc-117">更新 **plannerBucketTaskBoardTaskFormat** 对象。</span><span class="sxs-lookup"><span data-stu-id="52afc-117">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="52afc-118">属性</span><span class="sxs-lookup"><span data-stu-id="52afc-118">Properties</span></span>
| <span data-ttu-id="52afc-119">属性</span><span class="sxs-lookup"><span data-stu-id="52afc-119">Property</span></span>     | <span data-ttu-id="52afc-120">类型</span><span class="sxs-lookup"><span data-stu-id="52afc-120">Type</span></span>   |<span data-ttu-id="52afc-121">说明</span><span class="sxs-lookup"><span data-stu-id="52afc-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52afc-122">id</span><span class="sxs-lookup"><span data-stu-id="52afc-122">id</span></span>|<span data-ttu-id="52afc-123">String</span><span class="sxs-lookup"><span data-stu-id="52afc-123">String</span></span>| <span data-ttu-id="52afc-124">只读。</span><span class="sxs-lookup"><span data-stu-id="52afc-124">Read-only.</span></span> <span data-ttu-id="52afc-125">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="52afc-125">ID of the resource.</span></span> <span data-ttu-id="52afc-126">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="52afc-126">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="52afc-127">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="52afc-127">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="52afc-128">orderHint</span><span class="sxs-lookup"><span data-stu-id="52afc-128">orderHint</span></span>|<span data-ttu-id="52afc-129">String</span><span class="sxs-lookup"><span data-stu-id="52afc-129">String</span></span>|<span data-ttu-id="52afc-p104">用于为任务板存储桶视图中的任务进行排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="52afc-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="52afc-132">关系</span><span class="sxs-lookup"><span data-stu-id="52afc-132">Relationships</span></span>
<span data-ttu-id="52afc-133">无</span><span class="sxs-lookup"><span data-stu-id="52afc-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="52afc-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52afc-134">JSON representation</span></span>
<span data-ttu-id="52afc-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52afc-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


