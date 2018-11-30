---
title: plannerProgressTaskBoardTaskFormat 资源类型
description: '**plannerProgressTaskBoardTaskFormat** 资源表示用于在“任务板”的“进度”视图（由任务对象上的 PercentComplete 字段的状态组成的视图，包含“未启动”、“正在进行”和“完成”列）下正确呈现任务的信息。每个任务均将有一个与其相关联的 **plannerProgressTaskBoardTaskFormat** 对象。'
ms.openlocfilehash: 8ff6f536920bafb8734f63ef9fe9b72f8c2b1acb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043658"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="de93c-104">plannerProgressTaskBoardTaskFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="de93c-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

> <span data-ttu-id="de93c-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="de93c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de93c-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="de93c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="de93c-p103">**plannerProgressTaskBoardTaskFormat** 资源表示用于在“任务板”的“进度”视图（由任务对象上的 PercentComplete 字段的状态组成的视图，包含“未启动”、“正在进行”和“完成”列）下正确呈现任务的信息。每个[任务](plannertask.md)均将有一个与其相关联的 **plannerProgressTaskBoardTaskFormat** 对象。</span><span class="sxs-lookup"><span data-stu-id="de93c-p103">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete). Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="de93c-109">方法</span><span class="sxs-lookup"><span data-stu-id="de93c-109">Methods</span></span>

| <span data-ttu-id="de93c-110">方法</span><span class="sxs-lookup"><span data-stu-id="de93c-110">Method</span></span>           | <span data-ttu-id="de93c-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="de93c-111">Return Type</span></span>    |<span data-ttu-id="de93c-112">说明</span><span class="sxs-lookup"><span data-stu-id="de93c-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="de93c-113">Get plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="de93c-113">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="de93c-114">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="de93c-114">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="de93c-115">读取 **plannerProgressTaskBoardTaskFormat** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="de93c-115">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="de93c-116">Update</span><span class="sxs-lookup"><span data-stu-id="de93c-116">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="de93c-117">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="de93c-117">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="de93c-118">更新 **plannerProgressTaskBoardTaskFormat** 对象。</span><span class="sxs-lookup"><span data-stu-id="de93c-118">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="de93c-119">属性</span><span class="sxs-lookup"><span data-stu-id="de93c-119">Properties</span></span>
| <span data-ttu-id="de93c-120">属性</span><span class="sxs-lookup"><span data-stu-id="de93c-120">Property</span></span>     | <span data-ttu-id="de93c-121">类型</span><span class="sxs-lookup"><span data-stu-id="de93c-121">Type</span></span>   |<span data-ttu-id="de93c-122">说明</span><span class="sxs-lookup"><span data-stu-id="de93c-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de93c-123">id</span><span class="sxs-lookup"><span data-stu-id="de93c-123">id</span></span>|<span data-ttu-id="de93c-124">String</span><span class="sxs-lookup"><span data-stu-id="de93c-124">String</span></span>| <span data-ttu-id="de93c-125">只读。</span><span class="sxs-lookup"><span data-stu-id="de93c-125">Read-only.</span></span> <span data-ttu-id="de93c-126">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="de93c-126">ID of the resource.</span></span> <span data-ttu-id="de93c-127">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="de93c-127">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="de93c-128">服务上执行[格式验证](tasks-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="de93c-128">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="de93c-129">orderHint</span><span class="sxs-lookup"><span data-stu-id="de93c-129">orderHint</span></span>|<span data-ttu-id="de93c-130">String</span><span class="sxs-lookup"><span data-stu-id="de93c-130">String</span></span>|<span data-ttu-id="de93c-p105">用于对任务板进度视图上的任务进行排序的提示值。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="de93c-p105">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="de93c-133">关系</span><span class="sxs-lookup"><span data-stu-id="de93c-133">Relationships</span></span>
<span data-ttu-id="de93c-134">无</span><span class="sxs-lookup"><span data-stu-id="de93c-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="de93c-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de93c-135">JSON representation</span></span>
<span data-ttu-id="de93c-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de93c-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
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
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->