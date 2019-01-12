---
title: plannerOrderHintsByAssignee 资源类型
description: '**PlannerOrderHintsByAssignee**是包含订购提示 plannerTask 资源，以指示分配给任务板视图中的任务顺序中的代理人的资源。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b285c4a04d045c8a4e70a574c88772a0981c95e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967747"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a><span data-ttu-id="4e477-103">plannerOrderHintsByAssignee 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e477-103">plannerOrderHintsByAssignee resource type</span></span>

<span data-ttu-id="4e477-p101">**plannerOrderHintsByAssignee** 是包含[排序提示](planner-order-hint-format.md)的资源，适用于 [plannerTask](plannertask.md) 资源中的代理人，用于指示“任务板”的“分配到”视图中的任务顺序。此类型是开放类型。其属性是已分配到任务的用户 ID，其值是排序提示。</span><span class="sxs-lookup"><span data-stu-id="4e477-p101">The **plannerOrderHintsByAssignee** is a resource that contains [ordering hints](planner-order-hint-format.md) for assignees in a [plannerTask](plannertask.md) resource, to indicate the order of the task in Assigned To view of the Task Board. This type is an open type. The properties are the ids of users assigned to the task, and the values are order hints.</span></span>

## <a name="properties"></a><span data-ttu-id="4e477-107">属性</span><span class="sxs-lookup"><span data-stu-id="4e477-107">Properties</span></span>
<span data-ttu-id="4e477-p102">开放类型的属性可以由客户端定义。在这种情况下，客户必须将已分配到任务的用户 ID 作为属性名称，并且将有效的[排序提示](planner-order-hint-format.md)作为值。无法从此类型中删除属性。更新对包含的 [plannerTask](plannertask.md) 的分配后服务将自动删除值。</span><span class="sxs-lookup"><span data-stu-id="4e477-p102">Properties of an Open Type can be defined by the client. In this case, the client must provide ids of users assigned to the task as property names, and a valid [order hint](planner-order-hint-format.md) as the value. Properties cannot be removed from this type. The service will automatically remove values as the assignments on the containing [plannerTask](plannertask.md) are updated.</span></span>

<span data-ttu-id="4e477-112">示例：</span><span class="sxs-lookup"><span data-stu-id="4e477-112">Example:</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47", "4e98f8f1-bb03-4015-b8e0-19bb370949d8" ],
  "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
}-->

```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": "String",
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerOrderHintsByAssignee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
