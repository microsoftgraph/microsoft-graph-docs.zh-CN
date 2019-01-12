---
title: ChartTitle 资源类型
description: 表示图表的 chart title 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: db0b95e0e01fcbf1c962689a1615066692700992
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977561"
---
# <a name="charttitle-resource-type"></a>ChartTitle 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示图表的 chart title 对象。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 ChartTitle](../api/charttitle-get.md) | [ChartTitle](charttitle.md) |读取 chartTitle 对象的属性和关系。|
|[Update](../api/charttitle-update.md) | [ChartTitle](charttitle.md)    |更新 ChartTitle 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|overlay|boolean|表示图表标题是否将叠加在图表上的布尔值。|
|text|string|表示图表的标题文本。|
|visible|boolean|表示 chart title 对象的可见性的布尔值。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|format|[ChartTitleFormat](charttitleformat.md)|表示图表标题的格式，包括填充和字体格式。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartTitle"
}-->

```json
{
  "overlay": true,
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
