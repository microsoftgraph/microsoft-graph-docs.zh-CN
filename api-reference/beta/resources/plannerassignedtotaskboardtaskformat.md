---
title: plannerAssignedToTaskBoardTaskFormat 资源类型
description: '**plannerAssignedToTaskBoardTaskFormat** 资源表示用于在“任务板”的“AssignedTo”视图（由已向其分配任务的用户组成的视图）下正确呈现任务的信息。每个**任务**均将有一个与其相关联的 plannerAssignedToTaskBoardTaskFormat 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 6a7aa230a610ec63559797d058cbc3f64ffe843d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529815"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="d69c9-104">plannerAssignedToTaskBoardTaskFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="d69c9-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d69c9-p102">**plannerAssignedToTaskBoardTaskFormat** 资源表示用于在“任务板”的“AssignedTo”视图（由已向其分配任务的用户组成的视图）下正确呈现任务的信息。每个[任务](plannertask.md)均将有一个与其相关联的 **plannerAssignedToTaskBoardTaskFormat** 对象。</span><span class="sxs-lookup"><span data-stu-id="d69c9-p102">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to). Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="d69c9-107">方法</span><span class="sxs-lookup"><span data-stu-id="d69c9-107">Methods</span></span>

| <span data-ttu-id="d69c9-108">方法</span><span class="sxs-lookup"><span data-stu-id="d69c9-108">Method</span></span>           | <span data-ttu-id="d69c9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d69c9-109">Return Type</span></span>    |<span data-ttu-id="d69c9-110">说明</span><span class="sxs-lookup"><span data-stu-id="d69c9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d69c9-111">Get plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d69c9-111">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | [<span data-ttu-id="d69c9-112">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d69c9-112">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="d69c9-113">读取 **plannerAssignedToTaskBoardTaskFormat** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d69c9-113">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="d69c9-114">Update</span><span class="sxs-lookup"><span data-stu-id="d69c9-114">Update</span></span>](../api/plannerassignedtotaskboardtaskformat-update.md) | [<span data-ttu-id="d69c9-115">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d69c9-115">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="d69c9-116">更新 **plannerAssignedToTaskBoardTaskFormat** 对象。</span><span class="sxs-lookup"><span data-stu-id="d69c9-116">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d69c9-117">属性</span><span class="sxs-lookup"><span data-stu-id="d69c9-117">Properties</span></span>
| <span data-ttu-id="d69c9-118">属性</span><span class="sxs-lookup"><span data-stu-id="d69c9-118">Property</span></span>     | <span data-ttu-id="d69c9-119">类型</span><span class="sxs-lookup"><span data-stu-id="d69c9-119">Type</span></span>   |<span data-ttu-id="d69c9-120">说明</span><span class="sxs-lookup"><span data-stu-id="d69c9-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d69c9-121">id</span><span class="sxs-lookup"><span data-stu-id="d69c9-121">id</span></span>|<span data-ttu-id="d69c9-122">String</span><span class="sxs-lookup"><span data-stu-id="d69c9-122">String</span></span>| <span data-ttu-id="d69c9-123">只读。</span><span class="sxs-lookup"><span data-stu-id="d69c9-123">Read-only.</span></span> <span data-ttu-id="d69c9-124">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="d69c9-124">ID of the resource.</span></span> <span data-ttu-id="d69c9-125">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="d69c9-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="d69c9-126">服务上执行[格式验证](tasks-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="d69c9-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="d69c9-127">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="d69c9-127">orderHintsByAssignee</span></span>|[<span data-ttu-id="d69c9-128">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="d69c9-128">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="d69c9-p104">用于为任务板 AssignedTo 视图上的任务进行排序的提示字典。每个条目的键是任务分配到的用户之一，值为排序提示。[此处](planner-order-hint-format.md)概述了各值的格式。</span><span class="sxs-lookup"><span data-stu-id="d69c9-p104">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="d69c9-132">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="d69c9-132">unassignedOrderHint</span></span>|<span data-ttu-id="d69c9-133">字符串</span><span class="sxs-lookup"><span data-stu-id="d69c9-133">String</span></span>|<span data-ttu-id="d69c9-p105">当任务未分配给任何人，或 orderHintsByAssignee 字典未向分配到任务的用户提供排序提示时，提示值用于为任务板 AssignedTo 视图上的任务排序。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="d69c9-p105">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="d69c9-136">关系</span><span class="sxs-lookup"><span data-stu-id="d69c9-136">Relationships</span></span>
<span data-ttu-id="d69c9-137">无</span><span class="sxs-lookup"><span data-stu-id="d69c9-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d69c9-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d69c9-138">JSON representation</span></span>
<span data-ttu-id="d69c9-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d69c9-139">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerassignedtotaskboardtaskformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
