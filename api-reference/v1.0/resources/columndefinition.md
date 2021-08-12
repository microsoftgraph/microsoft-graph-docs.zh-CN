---
author: JeremyKelley
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
description: 下面是 ColumnDefinition 资源的 JSON 表示形式。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4beefa8523898b4770de217a895426e9cc1f5cf91edbc6835b677d450ffc4943
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126667"
---
# <a name="columndefinition-resource"></a>ColumnDefinition 资源

命名空间：microsoft.graph

## <a name="json-representation"></a>JSON 表示形式

下面是 ColumnDefinition 资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnDefinition"
}-->

```json
{
  "columnGroup": "string",
  "description": "description",
  "displayName": "friendly name",
  "enforceUniqueValues": "true",
  "hidden": false,
  "id": "string",
  "indexed": true,
  "name": "staticNameForApi",
  "readOnly": false,
  "required": false,
  "boolean": { "@odata.type": "microsoft.graph.booleanColumn" },
  "calculated": { "@odata.type": "microsoft.graph.calculatedColumn" },
  "choice": { "@odata.type": "microsoft.graph.choiceColumn" },
  "currency": { "@odata.type": "microsoft.graph.currencyColumn" },
  "dateTime": { "@odata.type": "microsoft.graph.dateTimeColumn" },
  "defaultValue": { "@odata.type": "microsoft.graph.defaultColumnValue" },
  "geolocation": { "@odata.type": "microsoft.graph.geolocationColumn" },
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" }
}
```

## <a name="properties"></a>属性

**columnDefinition** 资源具有以下属性。

| 属性名称           | 类型    | 说明
|:------------------------|:--------|:-----------------------------------------
| **columnGroup**         | string  | 对于网站列，此列所属的组的名称。 可以帮助组织相关的列。
| **说明**         | string  | 面向用户的列描述。
| **displayName**         | string  | 面向用户的列名称。
| **enforceUniqueValues** | boolean | 如果为 true，则此列不能有两个列表项具有相同的值。
| **hidden**              | boolean | 指定列是否显示在用户界面中。
| **id**                  | string  | 列的唯一标识符。
| **indexed**             | boolean | 指定列值是否可用于排序和搜索。
| **名称**                | string  | 在 [listItem][] 上的 [fields][] 中显示的面向 API 的列名称。 对于面向用户的名称，请参阅 **displayName**。
| **readOnly**            | bool    | 指定是否可以修改列值。
| **required**            | boolean | 指定列值是否不可选。

列可以包含各种类型的数据。
以下属性表示列存储的数据类型以及该数据的其他设置。
这些属性是互相排斥的 - 列只能指定其中一个。

| 属性名称     | 类型                    | 说明
|:------------------|:------------------------|:-------------------------------
| **boolean**       | [booleanColumn][]       | 此列存储布尔值。
| **calculated**    | [calculatedColumn][]    | 根据其他列计算此列的数据。
| **choice**        | [choiceColumn][]        | 此列存储所选列表中的数据。
| **currency**      | [currencyColumn][]      | 此列存储货币值。
| **dateTime**      | [dateTimeColumn][]      | 此列存储日期时间值。
| **defaultValue**  | [defaultColumnValue][]  | 此列的默认值。
| **地理位置**   | [geolocationColumn][]   | 此列存储地理位置。
| **lookup**        | [lookupColumn][]        | 从网站中的另一个源查找此列的数据。
| **number**        | [numberColumn][]        | 此列存储数值。
| **personOrGroup** | [personOrGroupColumn][] | 此列存储个人或组值。
| **text**          | [textColumn][]          | 此列存储文本值。

注意：这些属性对应于 SharePoint 的 [SPFieldType][] 枚举。
虽然上面表示的是最常见的字段类型，但此 API 仍缺少一些。
在这些情况下，不会填充列类型 facet，列将仅具有其基本属性。

## <a name="remarks"></a>备注

默认情况下，不显示 `hidden` 列的 ColumnDefinitions 和字段值。
若要在列出 **columnDefinitions** 时看到这些内容，请在 `$select` 语句中添加 `hidden`。
若要在 [listItems][listItem] 上显示 **字段** 值时看到这些内容，请在 `$select` 语句中添加名称所需的列。

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[geolocationColumn]: geolocationcolumn.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md


  [SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->