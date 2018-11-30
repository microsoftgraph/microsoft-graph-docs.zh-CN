---
title: plannerOrderHintsByAssignee 资源类型
description: '**PlannerOrderHintsByAssignee**是包含订购提示 plannerTask 资源，以指示分配给任务板视图中的任务顺序中的代理人的资源。'
ms.openlocfilehash: b83abd3d3d08fc4d30f9f664af621bebad397b3e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010256"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a>plannerOrderHintsByAssignee 资源类型

**plannerOrderHintsByAssignee** 是包含[排序提示](planner-order-hint-format.md)的资源，适用于 [plannerTask](plannertask.md) 资源中的代理人，用于指示“任务板”的“分配到”视图中的任务顺序。此类型是开放类型。其属性是已分配到任务的用户 ID，其值是排序提示。

## <a name="properties"></a>属性
开放类型的属性可以由客户端定义。在这种情况下，客户必须将已分配到任务的用户 ID 作为属性名称，并且将有效的[排序提示](planner-order-hint-format.md)作为值。无法从此类型中删除属性。更新对包含的 [plannerTask](plannertask.md) 的分配后服务将自动删除值。

示例：

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