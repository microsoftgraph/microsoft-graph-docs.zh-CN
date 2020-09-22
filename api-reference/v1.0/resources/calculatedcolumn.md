---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
description: columnDefinition 资源上的 calculatedColumn 指出列数据基于站点中的其他列计算。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 29699b5f220f4b9e46258a42c3b353cc9712ac6d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066529"
---
# <a name="calculatedcolumn-resource-type"></a>CalculatedColumn 资源类型

命名空间：microsoft.graph

[columnDefinition](columndefinition.md) 资源上的 **calculatedColumn** 指出列数据基于站点中的其他列计算。

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
| **format**     | string  | 对于`dateTime` 输出类型，值的格式。 必须为 `dateOnly` 或 `dateTime` 的其中一个。
| **formula**    | string  | 用于计算此列的值的公式。
| **outputType** | string  | 用于设置此列中值的格式的输出类型。 必须为 `boolean`、`currency`、`dateTime`、`number` 或 `text`.的其中一个。

SharePoint 公式使用一种类似于 Excel 公式的语法。
有关详细信息，请参阅 [SharePoint 列表中常见公式的示例][SPFormulas] 。

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/calculatedcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(dateOnly,dateTime) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/calculatedcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(boolean,currency,dateTime,number,text) are in resource, but () are in table"
  ],
  "tocPath": "Resources/CalculatedColumn"
} -->

