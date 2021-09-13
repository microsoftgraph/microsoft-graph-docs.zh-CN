---
title: plannerOrderHintsByAssignee 资源类型
description: '**plannerOrderHintsByAssignee** 是包含 plannerTask 资源中被分配者排序提示的资源，用于指示任务板的"分配到"视图中的任务顺序。'
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: cfe6e1ac1bd0611eac9a2a39ce89814374371d19
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019235"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a>plannerOrderHintsByAssignee 资源类型

命名空间：microsoft.graph

**plannerOrderHintsByAssignee** 是包含 [plannerTask](plannertask.md)资源中被分配者排序提示的资源，用于指示任务板的"分配到"视图中的任务顺序。 [](planner-order-hint-format.md)
此类型是开放类型。 属性是分配给任务的用户的 ID，值是排序提示。

## <a name="properties"></a>属性
开放类型的属性可通过客户端定义。 在这种情况下，客户端必须提供分配给任务的用户的 ID 作为属性名称，并提供有效的 [排序](planner-order-hint-format.md) 提示作为值。
无法从此类型中删除属性。 当包含 [plannerTask](plannertask.md) 上的分配更新时，该服务将自动删除值。

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

