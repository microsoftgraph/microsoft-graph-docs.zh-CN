---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: 2fd6c08e1cfc28a77019d174763b9d698519b6a2
ms.sourcegitcommit: 9e4dc7745eb1bbbe595afd8c7f3db4c19c6bb4ac
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/29/2018
ms.locfileid: "23271313"
---
# <a name="columndefinition-resource"></a>ColumnDefinition 资源

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
| **columnGroup**         | 字符串  | 对于网站列，此列所属的组的名称。 可以帮助组织相关的列。
| **description**         | 字符串  | 面向用户的列描述。
| **displayName**         | 字符串  | 面向用户的列名称。
| **enforceUniqueValues** | 布尔值 | 如果为 true，则此列不能有两个列表项具有相同的值。
| **hidden**              | 布尔值 | 指定列是否显示在用户界面中。
| **id**                  | 字符串  | 列的唯一标识符。
| **indexed**             | 布尔值 | 指定列值是否可用于排序和搜索。
| **name**                | 字符串  | 在 [listItem][] 上的 [fields][] 中显示的面向 API 的列名称。 对于面向用户的名称，请参阅 **displayName**。
| **readOnly**            | 布尔值    | 指定是否可以修改列值。
| **required**            | 布尔值 | 指定列值是否不可选。

列可以包含各种类型的数据。
以下属性表示列存储的数据类型以及该数据的其他设置。
这些属性是互相排斥的 - 列只能指定其中一个。

| 属性名称     | 类型                    | 说明
|:------------------|:------------------------|:-------------------------------
| **布尔值**       | [booleanColumn][]       | 此列存储布尔值。
| **calculated**    | [calculatedColumn][]    | 根据其他列计算此列的数据。
| **choice**        | [choiceColumn][]        | 此列存储所选列表中的数据。
| **currency**      | [currencyColumn][]      | 此列存储货币值。
| **dateTime**      | [dateTimeColumn][]      | 此列存储日期时间值。
| **defaultValue**  | [defaultColumnValue][]  | 此列的默认值。
| **lookup**        | [lookupColumn][]        | 从网站中的另一个源查找此列的数据。
| **number**        | [numberColumn][]        | 此列存储数值。
| **personOrGroup** | [personOrGroupColumn][] | 此列存储个人或组值。
| **text**          | [textColumn][]          | 此列存储文本值。

注意：这些属性对应于 SharePoint 的 [SPFieldType][] 枚举。
虽然上面体现了最常见的字段类型，此 API 仍缺少一些类型。
在这些情况下，不会填充列类型 facet，列将仅具有其基本属性。

## <a name="remarks"></a>备注

默认情况下，不显示 `hidden` 列的 ColumnDefinitions 和字段值。
若要在列出 **columnDefinitions** 时看到这些内容，请在 `$select` 语句中添加 `hidden`。
若要在 [listItems][listItem] 上显示**字段**值时看到这些内容，请在 `$select` 语句中添加名称所需的列。

[booleanColumn]: booleanColumn.md
[calculatedColumn]: calculatedColumn.md
[choiceColumn]: choiceColumn.md
[currencyColumn]: currencyColumn.md
[dateTimeColumn]: dateTimeColumn.md
[defaultColumnValue]: defaultColumnValue.md
[lookupColumn]: lookupColumn.md
[numberColumn]: numberColumn.md
[personOrGroupColumn]: personOrGroupColumn.md
[textColumn]: textColumn.md
[fieldValueSet]: fieldValueSet.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

[SPFieldType]: https://msdn.microsoft.com/en-us/library/microsoft.sharepoint.spfieldtype.aspx

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
