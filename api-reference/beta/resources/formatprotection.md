---
title: FormatProtection 资源类型
description: 表示对范围对象的格式保护。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ruoyingl
ms.openlocfilehash: 3f2f2747c2d5dd5945ada93d53d65241fa3ce6ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973946"
---
# <a name="formatprotection-resource-type"></a>FormatProtection 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示对范围对象的格式保护。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 FormatProtection](../api/formatprotection-get.md) | [FormatProtection](formatprotection.md) |读取 formatProtection 对象的属性和关系。|
|[更新](../api/formatprotection-update.md) | [FormatProtection](formatprotection.md)  |更新 FormatProtection 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|formulaHidden|boolean|表示 Excel 是否隐藏区域中的单元格公式。指示整个区域不具有统一公式隐藏设置的空值。|
|已锁定|boolean|指示 Excel 是否锁定对象中的单元格。指示整个区域不具有统一锁定设置的空值。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.formatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


