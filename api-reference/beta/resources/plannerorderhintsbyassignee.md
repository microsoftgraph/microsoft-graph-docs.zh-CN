---
title: plannerOrderHintsByAssignee 资源类型
description: '**plannerOrderHintsByAssignee**是一个资源, 其中包含 plannerTask 资源中的工作负责人的排序提示, 以指示任务的分配对象在任务板中的显示顺序。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 428944f9d622bba8db5d700b8d113a2c5b476301
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344436"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a>plannerOrderHintsByAssignee 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**plannerOrderHintsByAssignee**是一个资源, 其中包含[plannerTask](plannertask.md)资源中的工作负责人的[排序提示](planner-order-hint-format.md), 以指示任务的分配对象在任务板中的显示顺序。
此类型是开放类型。 这些属性是分配给该任务的用户的 id, 并且值是 order 提示。

## <a name="properties"></a>属性
可由客户端定义打开类型的属性。 在这种情况下, 客户端必须提供作为属性名称分配给该任务的用户的 id, 并将有效的[order 提示](planner-order-hint-format.md)作为值。
无法从此类型中删除属性。 该服务将自动删除值, 因为更新了包含的[plannerTask](plannertask.md)上的工作分配。

示例：

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerOrderHintsByAssignee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
