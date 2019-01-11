---
title: plannerOrderHintsByAssignee 资源类型
description: '**PlannerOrderHintsByAssignee**是包含订购提示 plannerTask 资源，以指示分配给任务板视图中的任务顺序中的代理人的资源。'
localization_priority: Normal
ms.openlocfilehash: cdc254eab43972d321e01e646880b3087f3af6f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863943"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a><span data-ttu-id="194c5-103">plannerOrderHintsByAssignee 资源类型</span><span class="sxs-lookup"><span data-stu-id="194c5-103">plannerOrderHintsByAssignee resource type</span></span>

> <span data-ttu-id="194c5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="194c5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="194c5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="194c5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="194c5-p102">**plannerOrderHintsByAssignee** 是包含[排序提示](planner-order-hint-format.md)的资源，适用于 [plannerTask](plannertask.md) 资源中的代理人，用于指示“任务板”的“分配到”视图中的任务顺序。此类型是开放类型。其属性是已分配到任务的用户 ID，其值是排序提示。</span><span class="sxs-lookup"><span data-stu-id="194c5-p102">The **plannerOrderHintsByAssignee** is a resource that contains [ordering hints](planner-order-hint-format.md) for assignees in a [plannerTask](plannertask.md) resource, to indicate the order of the task in Assigned To view of the Task Board. This type is an open type. The properties are the ids of users assigned to the task, and the values are order hints.</span></span>

## <a name="properties"></a><span data-ttu-id="194c5-109">属性</span><span class="sxs-lookup"><span data-stu-id="194c5-109">Properties</span></span>
<span data-ttu-id="194c5-p103">开放类型的属性可以由客户端定义。在这种情况下，客户必须将已分配到任务的用户 ID 作为属性名称，并且将有效的[排序提示](planner-order-hint-format.md)作为值。无法从此类型中删除属性。更新对包含的 [plannerTask](plannertask.md) 的分配后服务将自动删除值。</span><span class="sxs-lookup"><span data-stu-id="194c5-p103">Properties of an Open Type can be defined by the client. In this case, the client must provide ids of users assigned to the task as property names, and a valid [order hint](planner-order-hint-format.md) as the value. Properties cannot be removed from this type. The service will automatically remove values as the assignments on the containing [plannerTask](plannertask.md) are updated.</span></span>

<span data-ttu-id="194c5-114">示例：</span><span class="sxs-lookup"><span data-stu-id="194c5-114">Example:</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
