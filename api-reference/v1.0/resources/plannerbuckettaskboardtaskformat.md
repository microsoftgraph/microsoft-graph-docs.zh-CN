---
title: plannerBucketTaskBoardTaskFormat 资源类型
description: '**plannerBucketTaskBoardTaskFormat**资源表示用于在任务板的 bucket 视图 (按其分配的存储桶中的任务组织的视图) 中正确呈现任务的信息。 每个任务都有一个与之关联的**plannerBucketTaskBoardTaskFormat**对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 4982b0b539412058d6d598893b698f12d88bd671
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462240"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="d7470-104">plannerBucketTaskBoardTaskFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7470-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="d7470-105">**plannerBucketTaskBoardTaskFormat**资源表示用于在任务板的 bucket 视图 (按其分配的存储桶中的任务组织的视图) 中正确呈现任务的信息。</span><span class="sxs-lookup"><span data-stu-id="d7470-105">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to).</span></span> <span data-ttu-id="d7470-106">每个[任务](plannertask.md)都有一个与之关联的**plannerBucketTaskBoardTaskFormat**对象。</span><span class="sxs-lookup"><span data-stu-id="d7470-106">Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="d7470-107">方法</span><span class="sxs-lookup"><span data-stu-id="d7470-107">Methods</span></span>

| <span data-ttu-id="d7470-108">方法</span><span class="sxs-lookup"><span data-stu-id="d7470-108">Method</span></span>           | <span data-ttu-id="d7470-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d7470-109">Return Type</span></span>    |<span data-ttu-id="d7470-110">说明</span><span class="sxs-lookup"><span data-stu-id="d7470-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d7470-111">获取 plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d7470-111">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="d7470-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d7470-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="d7470-113">读取**plannerBucketTaskBoardTaskFormat**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d7470-113">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="d7470-114">更新</span><span class="sxs-lookup"><span data-stu-id="d7470-114">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="d7470-115">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d7470-115">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="d7470-116">更新**plannerBucketTaskBoardTaskFormat**对象。</span><span class="sxs-lookup"><span data-stu-id="d7470-116">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d7470-117">属性</span><span class="sxs-lookup"><span data-stu-id="d7470-117">Properties</span></span>
| <span data-ttu-id="d7470-118">属性</span><span class="sxs-lookup"><span data-stu-id="d7470-118">Property</span></span>     | <span data-ttu-id="d7470-119">类型</span><span class="sxs-lookup"><span data-stu-id="d7470-119">Type</span></span>   |<span data-ttu-id="d7470-120">说明</span><span class="sxs-lookup"><span data-stu-id="d7470-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7470-121">id</span><span class="sxs-lookup"><span data-stu-id="d7470-121">id</span></span>|<span data-ttu-id="d7470-122">String</span><span class="sxs-lookup"><span data-stu-id="d7470-122">String</span></span>| <span data-ttu-id="d7470-123">只读。</span><span class="sxs-lookup"><span data-stu-id="d7470-123">Read-only.</span></span> <span data-ttu-id="d7470-124">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="d7470-124">ID of the resource.</span></span> <span data-ttu-id="d7470-125">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="d7470-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="d7470-126">[格式验证](planner-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="d7470-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="d7470-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="d7470-127">orderHint</span></span>|<span data-ttu-id="d7470-128">String</span><span class="sxs-lookup"><span data-stu-id="d7470-128">String</span></span>|<span data-ttu-id="d7470-p104">用于为任务板存储桶视图中的任务进行排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="d7470-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7470-131">关系</span><span class="sxs-lookup"><span data-stu-id="d7470-131">Relationships</span></span>
<span data-ttu-id="d7470-132">无</span><span class="sxs-lookup"><span data-stu-id="d7470-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d7470-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7470-133">JSON representation</span></span>
<span data-ttu-id="d7470-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7470-134">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
