---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CalculatedColumn
ms.openlocfilehash: 44700ba7606243002798ec0ec84c3be30d38ef1f
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="calculatedcolumn-resource-type"></a>CalculatedColumn 资源类型

[columnDefinition](columnDefinition.md) 资源上的 **calculatedColumn** 指示基于网站中的其他列计算的列数据。

## <a name="json-representation"></a>JSON 表示形式

下面是 **calculatedColumn** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a>属性

| 属性名称  | 类型    | 说明
|:---------------|:--------|:--------------------------------------------------
| **format**     | string  | 对于 `dateTime` 输出类型，是值的格式。 必须是 `dateOnly` 或 `dateTime` 的其中一个。
| **formula**    | string  | 用于计算此列的值的公式。
| **outputType** | string  | 用于设置此列中值的格式的输出类型。 必须为 `boolean`、`currency`、`dateTime`、`number` 或 `text` 的其中一个。

SharePoint 公式使用一种类似于 Excel 公式的语法。
请参阅 [SharePoint 列表中的常用公式示例][SPFormulas]，了解详细信息。

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn"
} -->
