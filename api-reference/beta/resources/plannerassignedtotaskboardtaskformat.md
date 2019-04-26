---
title: plannerAssignedToTaskBoardTaskFormat 资源类型
description: '**plannerAssignedToTaskBoardTaskFormat**资源表示用于在任务板的 "分配器" 视图 (由任务分配到的用户组织的视图) 中正确呈现任务的信息。 每个任务都有一个与之关联的**plannerAssignedToTaskBoardTaskFormat**对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f67539847cbb8a4adb88137743b4246ced02a521
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344593"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="ab52a-104">plannerAssignedToTaskBoardTaskFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab52a-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab52a-105">**plannerAssignedToTaskBoardTaskFormat**资源表示用于在任务板的 "分配器" 视图 (由任务分配到的用户组织的视图) 中正确呈现任务的信息。</span><span class="sxs-lookup"><span data-stu-id="ab52a-105">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to).</span></span> <span data-ttu-id="ab52a-106">每个[任务](plannertask.md)都有一个与之关联的**plannerAssignedToTaskBoardTaskFormat**对象。</span><span class="sxs-lookup"><span data-stu-id="ab52a-106">Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="ab52a-107">方法</span><span class="sxs-lookup"><span data-stu-id="ab52a-107">Methods</span></span>

| <span data-ttu-id="ab52a-108">方法</span><span class="sxs-lookup"><span data-stu-id="ab52a-108">Method</span></span>           | <span data-ttu-id="ab52a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ab52a-109">Return Type</span></span>    |<span data-ttu-id="ab52a-110">说明</span><span class="sxs-lookup"><span data-stu-id="ab52a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ab52a-111">获取 plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="ab52a-111">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | [<span data-ttu-id="ab52a-112">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="ab52a-112">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="ab52a-113">读取**plannerAssignedToTaskBoardTaskFormat**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ab52a-113">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="ab52a-114">更新</span><span class="sxs-lookup"><span data-stu-id="ab52a-114">Update</span></span>](../api/plannerassignedtotaskboardtaskformat-update.md) | [<span data-ttu-id="ab52a-115">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="ab52a-115">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="ab52a-116">更新**plannerAssignedToTaskBoardTaskFormat**对象。</span><span class="sxs-lookup"><span data-stu-id="ab52a-116">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ab52a-117">属性</span><span class="sxs-lookup"><span data-stu-id="ab52a-117">Properties</span></span>
| <span data-ttu-id="ab52a-118">属性</span><span class="sxs-lookup"><span data-stu-id="ab52a-118">Property</span></span>     | <span data-ttu-id="ab52a-119">类型</span><span class="sxs-lookup"><span data-stu-id="ab52a-119">Type</span></span>   |<span data-ttu-id="ab52a-120">说明</span><span class="sxs-lookup"><span data-stu-id="ab52a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab52a-121">id</span><span class="sxs-lookup"><span data-stu-id="ab52a-121">id</span></span>|<span data-ttu-id="ab52a-122">String</span><span class="sxs-lookup"><span data-stu-id="ab52a-122">String</span></span>| <span data-ttu-id="ab52a-123">只读。</span><span class="sxs-lookup"><span data-stu-id="ab52a-123">Read-only.</span></span> <span data-ttu-id="ab52a-124">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="ab52a-124">ID of the resource.</span></span> <span data-ttu-id="ab52a-125">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="ab52a-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="ab52a-126">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="ab52a-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="ab52a-127">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="ab52a-127">orderHintsByAssignee</span></span>|[<span data-ttu-id="ab52a-128">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="ab52a-128">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="ab52a-p104">用于为任务板 AssignedTo 视图上的任务进行排序的提示字典。每个条目的键是任务分配到的用户之一，值为排序提示。[此处](planner-order-hint-format.md)概述了各值的格式。</span><span class="sxs-lookup"><span data-stu-id="ab52a-p104">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="ab52a-132">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="ab52a-132">unassignedOrderHint</span></span>|<span data-ttu-id="ab52a-133">字符串</span><span class="sxs-lookup"><span data-stu-id="ab52a-133">String</span></span>|<span data-ttu-id="ab52a-p105">当任务未分配给任何人，或 orderHintsByAssignee 字典未向分配到任务的用户提供排序提示时，用于为任务板 AssignedTo 视图上的任务进行排序的提示值。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="ab52a-p105">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab52a-136">关系</span><span class="sxs-lookup"><span data-stu-id="ab52a-136">Relationships</span></span>
<span data-ttu-id="ab52a-137">无</span><span class="sxs-lookup"><span data-stu-id="ab52a-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ab52a-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab52a-138">JSON representation</span></span>
<span data-ttu-id="ab52a-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab52a-139">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
