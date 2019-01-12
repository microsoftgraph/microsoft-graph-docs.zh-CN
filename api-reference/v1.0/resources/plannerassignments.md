---
title: plannerAssignments 资源类型
description: '**PlannerAssignments**资源表示 plannerTask 资源的分配。 此类型为打开的类型。 在这种类型的每个属性名称 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: bf079cbf91e0c9b8b1a8c92403324b301bbde923
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966816"
---
# <a name="plannerassignments-resource-type"></a>plannerAssignments 资源类型

**plannerAssignments** 资源表示 [plannerTask](plannertask.md) 资源的分配。此类型是开放类型。此类型中的每个属性名称均是任务被分配到的用户对象的 ID。可以通过新建以用户 ID 命名的属性并将包含 orderHint 属性的 [plannerassignment](plannerassignment.md) 对象填充为其值来向任务分配用户。可以通过将以代理人 ID 命名的属性设置为 null 来在任务中取消分配代理人。


## <a name="properties"></a>属性
开放类型的属性可以由客户端定义。但是在这种情况下，客户必须将分配用户的 ID 作为属性名称。必须将属性设置为 **plannerAssignment** 对象才能创建或修改代理人，必须将其设置为 null 才能删除代理人。

示例：

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47", "4e98f8f1-bb03-4015-b8e0-19bb370949d8" ],
  "@odata.type": "microsoft.graph.plannerAssignments"
}-->
```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": null,
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": { 
      "@odata.type": "microsoft.graph.plannerAssignment",
      "orderHint": "String"
    }
}
```
该示例将从任务的代理人列表中删除 ID 为 ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 的用户，并更改用户 ID 为 4e98f8f1-bb03-4015-b8e0-19bb370949d8 的代理人顺序。如果尚未将任务分配给 ID 为 4e98f8f1-bb03-4015-b8e0-19bb370949d8 的用户，则使用此值更新分配会将此任务分配给该用户。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
