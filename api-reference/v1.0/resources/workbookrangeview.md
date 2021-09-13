---
title: rangeView 资源类型
description: RangeView 表示父范围的一组可见单元格。
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9e49392b8a8ef6f79c199d7e7ce7bf2aba22f114
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139420"
---
# <a name="rangeview-resource-type"></a>rangeView 资源类型

命名空间：microsoft.graph RangeView 表示父范围的一组可见单元格。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[List rows](../api/workbookrangeview-list-rows.md) |[workbookRangeView](workbookrangeview.md) 集合| 获取一组 workbookRangeView 对象。|
|[Itemat](../api/workbookrangeview-itemat.md)|[workbookRangeView](workbookrangeview.md)|按索引获取范围视图项。|
|[Range](../api/workbookrangeview-range.md)|[workbookRange](range.md)|返回与范围视图相关联的范围对象|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|cellAddresses|Json|表示单元格地址
|columnCount|Int32|返回可见列数。只读。|
|formulas|Json|表示采用 A1 表示法的公式。 |
|formulasLocal|Json|表示采用 A1 表示法的公式，使用用户语言和数字格式区域设置。例如，英语中的公式 "=SUM(A1, 1.5)" 在德语中变为 "=SUMME(A1; 1,5)"。    |
|formulasR1C1|Json|表示采用 R1C1 样式表示法的公式。   |
|index|Int32|范围的索引。|
|numberFormat|Json|表示 Excel 中指定单元格的数字格式代码。只读。 |
|rowCount|Int32|返回可见行数。只读。  |
|text|Json|指定区域的文本值。文本值与单元格宽度无关。在 Excel UI 中替代 # 符号不会影响 API 返回的文本值。只读。    |
|valueTypes|Json|表示每个单元格的数据类型。 只读。 可能的值包括：Unknown、Empty、String、Integer、Double、Boolean、Error。 |
|values|Json|表示指定的 RangeView 的原始值。返回的数据可能是字符串、数字，也可能是布尔值。包含错误的单元格将返回错误字符串。   |

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|rows|[workbookRangeView](workbookrangeview.md) 集合| 表示一组与范围相关联的范围视图。只读。  只读。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookRangeView"
}-->
```json
{
  "cellAddresses": "Json",
  "columnCount": 1024,
  "formulas": "Json",
  "formulasLocal": "Json",
  "formulasR1C1": "Json",
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```

