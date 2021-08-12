---
title: plannerChecklistItems 资源类型
description: '**plannerChecklistItemCollection** 资源表示任务上的清单项的集合。 它是"打开类型"。 它是任务详细信息对象的一部分。 属性值对中的值是 checklistItem 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: f465adf89e9cb344013e30edccf03513f8fb96065e676ffb78d7cb8fa13f14ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178071"
---
# <a name="plannerchecklistitems-resource-type"></a>plannerChecklistItems 资源类型

命名空间：microsoft.graph

**plannerChecklistItemCollection** 资源表示任务上的清单项的集合。 它是"打开类型"。 它是任务详细信息 [对象的一](plannertaskdetails.md) 部分。 属性值对中的值是 [checklistItem](plannerchecklistitem.md) 对象。


## <a name="properties"></a>属性
开放类型的属性可以通过客户端定义。 在这种情况下，客户端应提供 **GUID** 作为属性，并且其值必须是 [checklistItem](plannerchecklistitem.md) 对象。 示例如下所示。 若要删除清单中的项目，将 属性的值设置为 `null` 。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItems resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

