---
title: plannerBucketTaskBoardTaskFormat 资源类型
description: '**plannerBucketTaskBoardTaskFormat** 资源表示用于在“任务板”的“存储桶”视图（由被分配到的存储桶中的任务组成的视图）下正确呈现任务的信息。每个任务均将有一个与其相关联的 **plannerBucketTaskBoardTaskFormat** 对象。'
localization_priority: Normal
ms.openlocfilehash: a4fae04147bb97a7128f7b8ad881ac9b34cb7d8c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836076"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="23e98-104">plannerBucketTaskBoardTaskFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="23e98-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="23e98-p102">**plannerBucketTaskBoardTaskFormat** 资源表示用于在“任务板”的“存储桶”视图（由被分配到的存储桶中的任务组成的视图）下正确呈现任务的信息。每个[任务](plannertask.md)均将有一个与其相关联的 **plannerBucketTaskBoardTaskFormat** 对象。</span><span class="sxs-lookup"><span data-stu-id="23e98-p102">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="23e98-107">方法</span><span class="sxs-lookup"><span data-stu-id="23e98-107">Methods</span></span>

| <span data-ttu-id="23e98-108">方法</span><span class="sxs-lookup"><span data-stu-id="23e98-108">Method</span></span>           | <span data-ttu-id="23e98-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="23e98-109">Return Type</span></span>    |<span data-ttu-id="23e98-110">说明</span><span class="sxs-lookup"><span data-stu-id="23e98-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="23e98-111">Get plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="23e98-111">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="23e98-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="23e98-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="23e98-113">读取 **plannerBucketTaskBoardTaskFormat** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="23e98-113">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="23e98-114">Update</span><span class="sxs-lookup"><span data-stu-id="23e98-114">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="23e98-115">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="23e98-115">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="23e98-116">更新 **plannerBucketTaskBoardTaskFormat** 对象</span><span class="sxs-lookup"><span data-stu-id="23e98-116">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="23e98-117">属性</span><span class="sxs-lookup"><span data-stu-id="23e98-117">Properties</span></span>
| <span data-ttu-id="23e98-118">属性</span><span class="sxs-lookup"><span data-stu-id="23e98-118">Property</span></span>     | <span data-ttu-id="23e98-119">类型</span><span class="sxs-lookup"><span data-stu-id="23e98-119">Type</span></span>   |<span data-ttu-id="23e98-120">说明</span><span class="sxs-lookup"><span data-stu-id="23e98-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23e98-121">id</span><span class="sxs-lookup"><span data-stu-id="23e98-121">id</span></span>|<span data-ttu-id="23e98-122">String</span><span class="sxs-lookup"><span data-stu-id="23e98-122">String</span></span>| <span data-ttu-id="23e98-123">只读。</span><span class="sxs-lookup"><span data-stu-id="23e98-123">Read-only.</span></span> <span data-ttu-id="23e98-124">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="23e98-124">ID of the resource.</span></span> <span data-ttu-id="23e98-125">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="23e98-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="23e98-126">服务上执行[格式验证](planner-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="23e98-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="23e98-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="23e98-127">orderHint</span></span>|<span data-ttu-id="23e98-128">String</span><span class="sxs-lookup"><span data-stu-id="23e98-128">String</span></span>|<span data-ttu-id="23e98-p104">用于对任务板存储桶视图中的任务进行排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="23e98-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="23e98-131">关系</span><span class="sxs-lookup"><span data-stu-id="23e98-131">Relationships</span></span>
<span data-ttu-id="23e98-132">无</span><span class="sxs-lookup"><span data-stu-id="23e98-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="23e98-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23e98-133">JSON representation</span></span>
<span data-ttu-id="23e98-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23e98-134">Here is a JSON representation of the resource.</span></span>

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
