---
title: plannerAssignedToTaskBoardTaskFormat 资源类型
description: '**plannerAssignedToTaskBoardTaskFormat** 资源表示用于在“任务板”的“AssignedTo”视图（由已向其分配任务的用户组成的视图）下正确呈现任务的信息。每个任务均将有一个与其相关联的 **plannerAssignedToTaskBoardTaskFormat** 对象。'
localization_priority: Normal
ms.openlocfilehash: bae551e009faeb40418f10a082bb8955846e8901
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818079"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="5b702-104">plannerAssignedToTaskBoardTaskFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b702-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

> <span data-ttu-id="5b702-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5b702-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b702-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5b702-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b702-p103">**plannerAssignedToTaskBoardTaskFormat** 资源表示用于在“任务板”的“AssignedTo”视图（由已向其分配任务的用户组成的视图）下正确呈现任务的信息。每个[任务](plannertask.md)均将有一个与其相关联的 **plannerAssignedToTaskBoardTaskFormat** 对象。</span><span class="sxs-lookup"><span data-stu-id="5b702-p103">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to). Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="5b702-109">方法</span><span class="sxs-lookup"><span data-stu-id="5b702-109">Methods</span></span>

| <span data-ttu-id="5b702-110">方法</span><span class="sxs-lookup"><span data-stu-id="5b702-110">Method</span></span>           | <span data-ttu-id="5b702-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="5b702-111">Return Type</span></span>    |<span data-ttu-id="5b702-112">说明</span><span class="sxs-lookup"><span data-stu-id="5b702-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5b702-113">Get plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="5b702-113">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | [<span data-ttu-id="5b702-114">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="5b702-114">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="5b702-115">读取 **plannerAssignedToTaskBoardTaskFormat** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5b702-115">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="5b702-116">Update</span><span class="sxs-lookup"><span data-stu-id="5b702-116">Update</span></span>](../api/plannerassignedtotaskboardtaskformat-update.md) | [<span data-ttu-id="5b702-117">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="5b702-117">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="5b702-118">更新 **plannerAssignedToTaskBoardTaskFormat** 对象。</span><span class="sxs-lookup"><span data-stu-id="5b702-118">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5b702-119">属性</span><span class="sxs-lookup"><span data-stu-id="5b702-119">Properties</span></span>
| <span data-ttu-id="5b702-120">属性</span><span class="sxs-lookup"><span data-stu-id="5b702-120">Property</span></span>     | <span data-ttu-id="5b702-121">类型</span><span class="sxs-lookup"><span data-stu-id="5b702-121">Type</span></span>   |<span data-ttu-id="5b702-122">说明</span><span class="sxs-lookup"><span data-stu-id="5b702-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b702-123">id</span><span class="sxs-lookup"><span data-stu-id="5b702-123">id</span></span>|<span data-ttu-id="5b702-124">String</span><span class="sxs-lookup"><span data-stu-id="5b702-124">String</span></span>| <span data-ttu-id="5b702-125">只读。</span><span class="sxs-lookup"><span data-stu-id="5b702-125">Read-only.</span></span> <span data-ttu-id="5b702-126">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="5b702-126">ID of the resource.</span></span> <span data-ttu-id="5b702-127">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="5b702-127">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="5b702-128">服务上执行[格式验证](tasks-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="5b702-128">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="5b702-129">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="5b702-129">orderHintsByAssignee</span></span>|[<span data-ttu-id="5b702-130">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="5b702-130">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="5b702-p105">用于为任务板 AssignedTo 视图上的任务进行排序的提示字典。每个条目的键是任务分配到的用户之一，值为排序提示。[此处](planner-order-hint-format.md)概述了各值的格式。</span><span class="sxs-lookup"><span data-stu-id="5b702-p105">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="5b702-134">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="5b702-134">unassignedOrderHint</span></span>|<span data-ttu-id="5b702-135">字符串</span><span class="sxs-lookup"><span data-stu-id="5b702-135">String</span></span>|<span data-ttu-id="5b702-p106">当任务未分配给任何人，或 orderHintsByAssignee 字典未向分配到任务的用户提供排序提示时，提示值用于为任务板 AssignedTo 视图上的任务排序。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="5b702-p106">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b702-138">关系</span><span class="sxs-lookup"><span data-stu-id="5b702-138">Relationships</span></span>
<span data-ttu-id="5b702-139">无</span><span class="sxs-lookup"><span data-stu-id="5b702-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5b702-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b702-140">JSON representation</span></span>
<span data-ttu-id="5b702-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b702-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHintsByAssignee": {"@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"},
  "unassignedOrderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
