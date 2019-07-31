---
title: plannerChecklistItems 资源类型
description: '**PlannerChecklistItemCollection**资源表示任务上的检查表项的集合。 它是开放类型。 它是任务详细信息对象的一部分。 属性-值对中的值是 checklistItem 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: bebec56f57f546dcfc0b16eedb1fb9635d0fb16f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966000"
---
# <a name="plannerchecklistitems-resource-type"></a>plannerChecklistItems 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**PlannerChecklistItemCollection**资源表示任务上的检查表项的集合。 它是开放类型。 它是[任务详细信息](plannertaskdetails.md)对象的一部分。 属性-值对中的值是[checklistItem](plannerchecklistitem.md)对象。


## <a name="properties"></a>属性
可由客户端定义打开类型的属性。 在这种情况下, 客户端应将**guid**作为属性提供, 并且它们的值必须是[checklistItem](plannerchecklistitem.md)对象。 示例如下所示。 若要删除检查表中的项目, 请将该属性的值`null`设置为。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItems"
}-->

```json
{
  "String-value":
  {
    "isChecked": true,
    "lastModifiedBy": "String-value",
    "lastModifiedByDateTime": "String(timestamp)",
    "orderHint": "String-value",
    "title": "String-value"
  }
}
```
示例

```json
{
  "3a73c9dd-fb47-4230-9c0f-b80788fb0f9b": // client-generated GUID
  {
    "@odata.type": "microsoft.graph.checklistItem", // required in PATCH requests to edit the checklist on a task
    "isChecked": true,
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedByDateTime": "2015-09-21T17:45:12.039Z",
    "orderHint": "0009005756397228702",
    "title": "Get stamps"
  },
  "5f36f5b2-1ec0-4c48-9c75-ed59429516c5":
  {
     "@odata.type": "microsoft.graph.checklistItem",
    "isChecked": false,
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedByDateTime": "2015-09-21T17:45:12.039Z",
    "orderHint": "0004105723397228784",
    "title": "Mail card at UPS"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerChecklistItems resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
