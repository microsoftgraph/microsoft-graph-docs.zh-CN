---
title: alteredQueryToken 资源类型
description: 表示与原始用户查询相关的已更改的段。
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: edd8a8d121fb28d129fb9a21bf18112ea37f545c
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2022
ms.locfileid: "62879271"
---
# <a name="alteredquerytoken-resource-type"></a>alteredQueryToken 资源类型

命名空间：microsoft.graph

表示与原始用户查询相关的已更改的段。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|length|Int32| 定义已更改的线段的长度。|
|offset|Int32| 定义更改的线段的偏移量。|
|suggestion|字符串| 表示更正的线段字符串。|

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
  "length": "Int32",
  "offset": "Int32",
  "suggestion": "String"
}
```
