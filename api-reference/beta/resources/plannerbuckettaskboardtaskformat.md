---
title: plannerBucketTaskBoardTaskFormat 资源类型
description: '**plannerBucketTaskBoardTaskFormat** 资源表示用于在“任务板”的“存储桶”视图（由被分配到的存储桶中的任务组成的视图）下正确呈现任务的信息。每个任务均将有一个与其相关联的 **plannerBucketTaskBoardTaskFormat** 对象。'
ms.openlocfilehash: 2fa91a4900a12f4c7433049c8ee4be94cdaa7b06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047587"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="2f040-104">plannerBucketTaskBoardTaskFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f040-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

> <span data-ttu-id="2f040-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2f040-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f040-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2f040-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2f040-p103">**plannerBucketTaskBoardTaskFormat** 资源表示用于在“任务板”的“存储桶”视图（由被分配到的存储桶中的任务组成的视图）下正确呈现任务的信息。每个[任务](plannertask.md)均将有一个与其相关联的 **plannerBucketTaskBoardTaskFormat** 对象。</span><span class="sxs-lookup"><span data-stu-id="2f040-p103">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="2f040-109">方法</span><span class="sxs-lookup"><span data-stu-id="2f040-109">Methods</span></span>

| <span data-ttu-id="2f040-110">方法</span><span class="sxs-lookup"><span data-stu-id="2f040-110">Method</span></span>           | <span data-ttu-id="2f040-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="2f040-111">Return Type</span></span>    |<span data-ttu-id="2f040-112">说明</span><span class="sxs-lookup"><span data-stu-id="2f040-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2f040-113">Get plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="2f040-113">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="2f040-114">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="2f040-114">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="2f040-115">读取 **plannerBucketTaskBoardTaskFormat** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2f040-115">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="2f040-116">Update</span><span class="sxs-lookup"><span data-stu-id="2f040-116">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="2f040-117">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="2f040-117">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="2f040-118">更新 **plannerBucketTaskBoardTaskFormat** 对象</span><span class="sxs-lookup"><span data-stu-id="2f040-118">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2f040-119">属性</span><span class="sxs-lookup"><span data-stu-id="2f040-119">Properties</span></span>
| <span data-ttu-id="2f040-120">属性</span><span class="sxs-lookup"><span data-stu-id="2f040-120">Property</span></span>     | <span data-ttu-id="2f040-121">类型</span><span class="sxs-lookup"><span data-stu-id="2f040-121">Type</span></span>   |<span data-ttu-id="2f040-122">说明</span><span class="sxs-lookup"><span data-stu-id="2f040-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f040-123">id</span><span class="sxs-lookup"><span data-stu-id="2f040-123">id</span></span>|<span data-ttu-id="2f040-124">String</span><span class="sxs-lookup"><span data-stu-id="2f040-124">String</span></span>| <span data-ttu-id="2f040-125">只读。</span><span class="sxs-lookup"><span data-stu-id="2f040-125">Read-only.</span></span> <span data-ttu-id="2f040-126">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="2f040-126">ID of the resource.</span></span> <span data-ttu-id="2f040-127">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="2f040-127">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="2f040-128">服务上执行[格式验证](tasks-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="2f040-128">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="2f040-129">orderHint</span><span class="sxs-lookup"><span data-stu-id="2f040-129">orderHint</span></span>|<span data-ttu-id="2f040-130">String</span><span class="sxs-lookup"><span data-stu-id="2f040-130">String</span></span>|<span data-ttu-id="2f040-p105">用于对任务板存储桶视图中的任务进行排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="2f040-p105">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f040-133">关系</span><span class="sxs-lookup"><span data-stu-id="2f040-133">Relationships</span></span>
<span data-ttu-id="2f040-134">无</span><span class="sxs-lookup"><span data-stu-id="2f040-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2f040-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f040-135">JSON representation</span></span>
<span data-ttu-id="2f040-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f040-136">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->