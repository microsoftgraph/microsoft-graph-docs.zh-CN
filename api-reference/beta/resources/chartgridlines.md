---
title: ChartGridlines 资源类型
description: 代表图表坐标轴的主要或次要网格线。
author: lumine2008
ms.openlocfilehash: 263bbefad519fef8b12080cb7b2bfd74ce1a331f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319556"
---
# <a name="chartgridlines-resource-type"></a>ChartGridlines 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表图表坐标轴的主要或次要网格线。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 ChartGridlines](../api/chartgridlines-get.md) | [ChartGridlines](chartgridlines.md) |读取 chartGridlines 对象的属性和关系。|
|[Update](../api/chartgridlines-update.md) | [ChartGridlines](chartgridlines.md)    |更新 ChartGridlines 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|visible|boolean|表示坐标轴网格线是否可见的布尔值。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|format|[ChartGridlinesFormat](chartgridlinesformat.md)|表示图表网格线的格式。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartGridLines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->