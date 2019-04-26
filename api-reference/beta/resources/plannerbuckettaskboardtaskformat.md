---
title: plannerBucketTaskBoardTaskFormat 资源类型
description: '**plannerBucketTaskBoardTaskFormat**资源表示用于在任务板的 bucket 视图 (按其分配的存储桶中的任务组织的视图) 中正确呈现任务的信息。 每个任务都有一个与之关联的**plannerBucketTaskBoardTaskFormat**对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: d40234fd729b849fee9fa789b9ae410eb0147f45
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344588"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="e5efe-104">plannerBucketTaskBoardTaskFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5efe-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5efe-105">**plannerBucketTaskBoardTaskFormat**资源表示用于在任务板的 bucket 视图 (按其分配的存储桶中的任务组织的视图) 中正确呈现任务的信息。</span><span class="sxs-lookup"><span data-stu-id="e5efe-105">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to).</span></span> <span data-ttu-id="e5efe-106">每个[任务](plannertask.md)都有一个与之关联的**plannerBucketTaskBoardTaskFormat**对象。</span><span class="sxs-lookup"><span data-stu-id="e5efe-106">Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="e5efe-107">方法</span><span class="sxs-lookup"><span data-stu-id="e5efe-107">Methods</span></span>

| <span data-ttu-id="e5efe-108">方法</span><span class="sxs-lookup"><span data-stu-id="e5efe-108">Method</span></span>           | <span data-ttu-id="e5efe-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e5efe-109">Return Type</span></span>    |<span data-ttu-id="e5efe-110">说明</span><span class="sxs-lookup"><span data-stu-id="e5efe-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e5efe-111">获取 plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e5efe-111">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="e5efe-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e5efe-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="e5efe-113">读取**plannerBucketTaskBoardTaskFormat**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e5efe-113">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="e5efe-114">更新</span><span class="sxs-lookup"><span data-stu-id="e5efe-114">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="e5efe-115">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e5efe-115">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="e5efe-116">更新**plannerBucketTaskBoardTaskFormat**对象。</span><span class="sxs-lookup"><span data-stu-id="e5efe-116">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e5efe-117">属性</span><span class="sxs-lookup"><span data-stu-id="e5efe-117">Properties</span></span>
| <span data-ttu-id="e5efe-118">属性</span><span class="sxs-lookup"><span data-stu-id="e5efe-118">Property</span></span>     | <span data-ttu-id="e5efe-119">类型</span><span class="sxs-lookup"><span data-stu-id="e5efe-119">Type</span></span>   |<span data-ttu-id="e5efe-120">说明</span><span class="sxs-lookup"><span data-stu-id="e5efe-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5efe-121">id</span><span class="sxs-lookup"><span data-stu-id="e5efe-121">id</span></span>|<span data-ttu-id="e5efe-122">String</span><span class="sxs-lookup"><span data-stu-id="e5efe-122">String</span></span>| <span data-ttu-id="e5efe-123">只读。</span><span class="sxs-lookup"><span data-stu-id="e5efe-123">Read-only.</span></span> <span data-ttu-id="e5efe-124">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="e5efe-124">ID of the resource.</span></span> <span data-ttu-id="e5efe-125">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="e5efe-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="e5efe-126">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="e5efe-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="e5efe-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="e5efe-127">orderHint</span></span>|<span data-ttu-id="e5efe-128">String</span><span class="sxs-lookup"><span data-stu-id="e5efe-128">String</span></span>|<span data-ttu-id="e5efe-p104">用于为任务板存储桶视图中的任务进行排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="e5efe-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5efe-131">关系</span><span class="sxs-lookup"><span data-stu-id="e5efe-131">Relationships</span></span>
<span data-ttu-id="e5efe-132">无</span><span class="sxs-lookup"><span data-stu-id="e5efe-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e5efe-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5efe-133">JSON representation</span></span>
<span data-ttu-id="e5efe-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5efe-134">Here is a JSON representation of the resource.</span></span>

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
