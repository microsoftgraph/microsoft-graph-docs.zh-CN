---
title: workbookRangeFill 资源类型
description: 表示 range 对象的背景。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: eea7337fa4aefb1bde607740b9a2fc78264dae91
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348593"
---
# <a name="workbookrangefill-resource-type"></a>workbookRangeFill 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 range 对象的背景。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 workbookRangeFill](../api/rangefill-get.md) | [workbookRangeFill](workbookrangefill.md) |读取 rangeFill 对象的属性和关系。|
|[更新](../api/rangefill-update.md) | [workbookRangeFill](workbookrangefill.md)   |更新 RangeFill 对象 |
|[清除](../api/rangefill-clear.md)|None|重置区域背景。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|color|string|表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
