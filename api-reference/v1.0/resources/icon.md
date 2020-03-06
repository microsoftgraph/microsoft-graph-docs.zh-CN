---
title: 图标资源类型
description: 表示单元格图标。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: af719295a0d3ab46c94877a9cd046f63423e5ed4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532900"
---
# <a name="icon-resource-type"></a>图标资源类型

命名空间：microsoft.graph

表示单元格图标。


## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取图标](../api/icon-get.md) | [Icon](icon.md) |读取 icon 对象的属性和关系。|
|[更新](../api/icon-update.md) | [图标](icon.md)  |更新 icon 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|index|int|表示给定集合中图标的索引。|
|set|string|表示图标所属的集合。 可能的值为： `Invalid`、 `ThreeArrows`、 `ThreeArrowsGray` `ThreeFlags` `ThreeTrafficLights1` `ThreeTrafficLights2` `ThreeSigns` `ThreeSymbols` `ThreeSymbols2` `FourArrows` `FourArrowsGray` `FiveBoxes`、、 `FourRedToBlack`、、、、、、、、、、、、、、、、。 `FourRating` `FourTrafficLights` `FiveArrows` `FiveArrowsGray` `FiveRating` `FiveQuarters` `ThreeStars` `ThreeTriangles`|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookIcon"
}-->

```json
{
  "index": 1024,
  "set": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
