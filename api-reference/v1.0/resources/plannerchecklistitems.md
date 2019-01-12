---
title: plannerChecklistItems 资源类型
description: '**plannerChecklistItemCollection** 资源表示任务上的清单项集合。它是开放类型。它是任务详细信息对象的组成部分。该属性值对中的值是 checklistItem 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 17c1d8c0529e0d85ebc784d25c2dc284f1775c0f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982699"
---
# <a name="plannerchecklistitems-resource-type"></a>plannerChecklistItems 资源类型

**plannerChecklistItemCollection** 资源表示任务上的清单项集合。它是开放类型。它是[任务详细信息](plannertaskdetails.md)对象的组成部分。该属性值对中的值是 [checklistItem](plannerchecklistitem.md) 对象。


## <a name="properties"></a>属性
开放类型的属性可以由客户端定义。在这种情况下，客户端应将 **GUID** 作为属性，并且其值必须为 [checklistItem](plannerchecklistitem.md) 对象。下面是一个示例。若要删除清单中的项，请将该属性值设置为 `null`。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
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
// 示例

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItems resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
