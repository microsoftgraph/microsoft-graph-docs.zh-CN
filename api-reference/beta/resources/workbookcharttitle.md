---
title: workbookChartTitle 资源类型
description: 表示图表的图表标题对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2e9cf5de45ae45b336bc6b6bf8456700b5c53495
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348615"
---
# <a name="workbookcharttitle-resource-type"></a>workbookChartTitle 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示图表的图表标题对象。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 workbookChartTitle](../api/charttitle-get.md) | [workbookChartTitle](workbookcharttitle.md) |读取 chartTitle 对象的属性和关系。|
|[更新](../api/charttitle-update.md) | [workbookChartTitle](workbookcharttitle.md)    |更新 ChartTitle 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|overlay|布尔|表示图表标题是否将叠加在图表上的布尔值。|
|text|string|表示图表的标题文本。|
|visible|布尔|表示 chart title 对象的可见性的布尔值。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|format|[workbookChartTitleFormat](workbookcharttitleformat.md)|表示图表标题的格式，包括填充和字体格式。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartTitle"
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
