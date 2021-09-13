---
title: SortField 资源类型
description: 表示排序操作中的条件。
ms.localizationpriority: medium
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ca8acdf09960988cb8da55e45daaf2504ef4e664
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136351"
---
# <a name="sortfield-resource-type"></a>SortField 资源类型

命名空间：microsoft.graph

表示排序操作中的条件。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|ascending|boolean|表示是否以升序方式进行排序。|
|color|string|表示按字体或单元格颜色进行排序时，条件的目标颜色。|
|dataOption|string|表示此字段的其他排序选项。 可能的值是 `Normal` `TextAsNumber` ：、。|
|Key|int|表示条件所在的列（或行，具体取决于排序方向）。表示与第一列（或行）的偏移量。|
|sortOn|string|表示此条件的排序类型。 可能的值包括 `Value`、`CellColor`、`FontColor`、`Icon`。|
|图标|[WorkbookIcon](icon.md)|表示对单元格图标进行排序时，条件的目标图标。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookSortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string",
  "icon": { "@odata.type": "microsoft.graph.workbookIcon" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

