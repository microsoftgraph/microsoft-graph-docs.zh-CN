---
title: plannerBucketTaskBoardTaskFormat 资源类型
description: '**PlannerBucketTaskBoardTaskFormat**资源表示用于在任务板的 bucket 视图 (按其分配的存储桶中的任务组织的视图) 中正确呈现任务的信息。 每个任务都有一个与之关联的**plannerBucketTaskBoardTaskFormat**对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b9e9713dca07e8eff0b320fcc50c8c48cc46f489
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009102"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="11eaa-104">plannerBucketTaskBoardTaskFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="11eaa-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11eaa-105">**PlannerBucketTaskBoardTaskFormat**资源表示用于在任务板的 bucket 视图 (按其分配的存储桶中的任务组织的视图) 中正确呈现任务的信息。</span><span class="sxs-lookup"><span data-stu-id="11eaa-105">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to).</span></span> <span data-ttu-id="11eaa-106">每个[任务](plannertask.md)都有一个与之关联的**plannerBucketTaskBoardTaskFormat**对象。</span><span class="sxs-lookup"><span data-stu-id="11eaa-106">Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="11eaa-107">方法</span><span class="sxs-lookup"><span data-stu-id="11eaa-107">Methods</span></span>

| <span data-ttu-id="11eaa-108">方法</span><span class="sxs-lookup"><span data-stu-id="11eaa-108">Method</span></span>           | <span data-ttu-id="11eaa-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="11eaa-109">Return Type</span></span>    |<span data-ttu-id="11eaa-110">说明</span><span class="sxs-lookup"><span data-stu-id="11eaa-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="11eaa-111">获取 plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="11eaa-111">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="11eaa-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="11eaa-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="11eaa-113">读取**plannerBucketTaskBoardTaskFormat**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="11eaa-113">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="11eaa-114">更新</span><span class="sxs-lookup"><span data-stu-id="11eaa-114">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="11eaa-115">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="11eaa-115">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="11eaa-116">更新**plannerBucketTaskBoardTaskFormat**对象。</span><span class="sxs-lookup"><span data-stu-id="11eaa-116">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="11eaa-117">属性</span><span class="sxs-lookup"><span data-stu-id="11eaa-117">Properties</span></span>
| <span data-ttu-id="11eaa-118">属性</span><span class="sxs-lookup"><span data-stu-id="11eaa-118">Property</span></span>     | <span data-ttu-id="11eaa-119">类型</span><span class="sxs-lookup"><span data-stu-id="11eaa-119">Type</span></span>   |<span data-ttu-id="11eaa-120">说明</span><span class="sxs-lookup"><span data-stu-id="11eaa-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11eaa-121">id</span><span class="sxs-lookup"><span data-stu-id="11eaa-121">id</span></span>|<span data-ttu-id="11eaa-122">String</span><span class="sxs-lookup"><span data-stu-id="11eaa-122">String</span></span>| <span data-ttu-id="11eaa-123">只读。</span><span class="sxs-lookup"><span data-stu-id="11eaa-123">Read-only.</span></span> <span data-ttu-id="11eaa-124">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="11eaa-124">ID of the resource.</span></span> <span data-ttu-id="11eaa-125">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="11eaa-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="11eaa-126">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="11eaa-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="11eaa-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="11eaa-127">orderHint</span></span>|<span data-ttu-id="11eaa-128">String</span><span class="sxs-lookup"><span data-stu-id="11eaa-128">String</span></span>|<span data-ttu-id="11eaa-p104">用于为任务板存储桶视图中的任务进行排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="11eaa-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="11eaa-131">关系</span><span class="sxs-lookup"><span data-stu-id="11eaa-131">Relationships</span></span>
<span data-ttu-id="11eaa-132">无</span><span class="sxs-lookup"><span data-stu-id="11eaa-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="11eaa-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11eaa-133">JSON representation</span></span>
<span data-ttu-id="11eaa-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11eaa-134">Here is a JSON representation of the resource.</span></span>

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
