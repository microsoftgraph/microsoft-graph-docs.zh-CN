---
title: plannerAssignedToTaskBoardTaskFormat 资源类型
description: '**PlannerAssignedToTaskBoardTaskFormat**资源表示用于在任务板的 "分配器" 视图中正确呈现任务的信息，该信息 (将任务分配给其) 的用户组织的视图。 每个任务都有一个与之关联的 **plannerAssignedToTaskBoardTaskFormat** 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: aca03e2a82d7fe42aa229c2f53d0c1dd066a30bc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037617"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="54392-104">plannerAssignedToTaskBoardTaskFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="54392-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="54392-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54392-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="54392-106">**PlannerAssignedToTaskBoardTaskFormat**资源表示用于在任务板的 "分配器" 视图中正确呈现任务的信息，该信息 (将任务分配给其) 的用户组织的视图。</span><span class="sxs-lookup"><span data-stu-id="54392-106">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to).</span></span> <span data-ttu-id="54392-107">每个 [任务](plannertask.md) 都有一个与之关联的 **plannerAssignedToTaskBoardTaskFormat** 对象。</span><span class="sxs-lookup"><span data-stu-id="54392-107">Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="54392-108">方法</span><span class="sxs-lookup"><span data-stu-id="54392-108">Methods</span></span>

| <span data-ttu-id="54392-109">方法</span><span class="sxs-lookup"><span data-stu-id="54392-109">Method</span></span>           | <span data-ttu-id="54392-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="54392-110">Return Type</span></span>    |<span data-ttu-id="54392-111">说明</span><span class="sxs-lookup"><span data-stu-id="54392-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="54392-112">获取 plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="54392-112">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | [<span data-ttu-id="54392-113">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="54392-113">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="54392-114">读取 **plannerAssignedToTaskBoardTaskFormat** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="54392-114">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="54392-115">更新</span><span class="sxs-lookup"><span data-stu-id="54392-115">Update</span></span>](../api/plannerassignedtotaskboardtaskformat-update.md) | [<span data-ttu-id="54392-116">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="54392-116">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="54392-117">更新 **plannerAssignedToTaskBoardTaskFormat** 对象。</span><span class="sxs-lookup"><span data-stu-id="54392-117">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="54392-118">属性</span><span class="sxs-lookup"><span data-stu-id="54392-118">Properties</span></span>
| <span data-ttu-id="54392-119">属性</span><span class="sxs-lookup"><span data-stu-id="54392-119">Property</span></span>     | <span data-ttu-id="54392-120">类型</span><span class="sxs-lookup"><span data-stu-id="54392-120">Type</span></span>   |<span data-ttu-id="54392-121">说明</span><span class="sxs-lookup"><span data-stu-id="54392-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54392-122">id</span><span class="sxs-lookup"><span data-stu-id="54392-122">id</span></span>|<span data-ttu-id="54392-123">String</span><span class="sxs-lookup"><span data-stu-id="54392-123">String</span></span>| <span data-ttu-id="54392-124">只读。</span><span class="sxs-lookup"><span data-stu-id="54392-124">Read-only.</span></span> <span data-ttu-id="54392-125">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="54392-125">ID of the resource.</span></span> <span data-ttu-id="54392-126">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="54392-126">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="54392-127">[格式验证](planner-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="54392-127">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="54392-128">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="54392-128">orderHintsByAssignee</span></span>|[<span data-ttu-id="54392-129">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="54392-129">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="54392-p104">用于为任务板 AssignedTo 视图上的任务进行排序的提示字典。每个条目的键是任务分配到的用户之一，值为排序提示。[此处](planner-order-hint-format.md)概述了各值的格式。</span><span class="sxs-lookup"><span data-stu-id="54392-p104">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="54392-133">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="54392-133">unassignedOrderHint</span></span>|<span data-ttu-id="54392-134">字符串</span><span class="sxs-lookup"><span data-stu-id="54392-134">String</span></span>|<span data-ttu-id="54392-p105">当任务未分配给任何人，或 orderHintsByAssignee 字典未向分配到任务的用户提供排序提示时，用于为任务板 AssignedTo 视图上的任务进行排序的提示值。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="54392-p105">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="54392-137">关系</span><span class="sxs-lookup"><span data-stu-id="54392-137">Relationships</span></span>
<span data-ttu-id="54392-138">无</span><span class="sxs-lookup"><span data-stu-id="54392-138">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="54392-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54392-139">JSON representation</span></span>
<span data-ttu-id="54392-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54392-140">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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

