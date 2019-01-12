---
title: RangeFill 资源类型
description: 表示 range 对象的背景。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4043122f4c35c3e7f1c6f9d3919687833d35b9b3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974341"
---
# <a name="rangefill-resource-type"></a>RangeFill 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示 range 对象的背景。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 RangeFill](../api/rangefill-get.md) | [RangeFill](rangefill.md) |读取 rangeFill 对象的属性和关系。|
|[Update](../api/rangefill-update.md) | [RangeFill](rangefill.md)   |更新 RangeFill 对象 |
|[Clear](../api/rangefill-clear.md)|无|重置区域背景。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|color|string|表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。|

## <a name="relationships"></a>Relationships
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
