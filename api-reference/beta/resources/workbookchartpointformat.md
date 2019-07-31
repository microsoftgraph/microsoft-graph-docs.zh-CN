---
title: workbookChartPointFormat 资源类型
description: 表示图表点的格式化对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9c3d968c4d36b8220d505edb6b7503a2b1206416
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007233"
---
# <a name="workbookchartpointformat-resource-type"></a>workbookChartPointFormat 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示图表点的格式化对象。


## <a name="methods"></a>方法
无

## <a name="properties"></a>属性
无

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|fill|[workbookChartFill](workbookchartfill.md)|表示图表的填充格式，包括背景格式信息。 只读。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill"
    ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
