---
title: alteredQueryToken 资源类型
description: 表示与原始用户查询有关更改的线段。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 03e6f010fdcd77e07fc6ce3cc7e8c8c285fde73f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067993"
---
# <a name="alteredquerytoken-resource-type"></a>alteredQueryToken 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与原始用户查询有关更改的线段。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|offset|Int32| 定义更改的线段的偏移量。|
|length|Int32| 定义已更改的线段的长度。|
|suggestion|String| 表示更正的线段字符串。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alteredQueryToken",
  "baseType": null
}-->

```json
{
  "offset": 0,
  "length": 6,
  "suggestion": "String"
}
```
