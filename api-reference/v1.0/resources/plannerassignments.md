---
title: plannerAssignments 资源类型
description: '**plannerAssignments** 资源表示 plannerTask 资源的工作分配。 此类型是开放类型。 此类型的每个属性名称 '
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: c6c90a607622dc47f7fd3a3d77b7b42b2c39b6e5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044340"
---
# <a name="plannerassignments-resource-type"></a>plannerAssignments 资源类型

命名空间：microsoft.graph

**plannerAssignments** 资源表示 [plannerTask](plannertask.md)资源的工作分配。 此类型是开放类型。 此类型的每个属性名称都是任务分配到的用户对象的 ID。 可以将用户分配给创建具有其 ID 的新属性的任务，并将 orderHint 属性填充为值的 [plannerassignment](plannerassignment.md) 对象。 通过使用其 ID 命名的属性设置为 null，可以从任务中取消分配被分配者。


## <a name="properties"></a>属性
开放类型的属性可通过客户端定义。 但在这种情况下，客户端必须提供分配的用户 ID 作为属性名称。 必须将属性设置为 **plannerAssignment** 对象，以创建或修改被分配者，并将 该属性设置为 null 以删除它们。

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
此示例从任务的分配者列表中删除 ID 为 ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 的用户，同时更改用户 ID 为 4e98f8f1-bb03-4015-b8e0-19bb370949d8 的被分派人的顺序。 如果任务尚未分配给 ID 为 4e98f8f1-bb03-4015-b8e0-19bb370949d8 的用户，则使用此值更新工作分配将任务分配给此用户。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

