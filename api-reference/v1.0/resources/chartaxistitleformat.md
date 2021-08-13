---
title: ChartAxisTitleFormat 资源类型
description: 表示图表坐标轴标题格式。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 96b5bb7cf0865a8ae859d392c9d59d8dce78580870807adaebfcd802655d88c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230828"
---
# <a name="chartaxistitleformat-resource-type"></a>ChartAxisTitleFormat 资源类型

命名空间：microsoft.graph

表示图表坐标轴标题格式。


## <a name="methods"></a>方法
无

## <a name="properties"></a>属性
无

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|font|[WorkbookChartFont](chartfont.md)|表示图表坐标轴标题对象的字体属性，例如字体名称、字体大小、颜色等。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

