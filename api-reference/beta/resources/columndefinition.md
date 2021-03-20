---
author: JeremyKelley
description: 下面是 columnDefinition 资源的 JSON 表示形式。
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: cddab6ee01cea34902ee892e593e0e81b3cde8af
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961298"
---
# <a name="columndefinition-resource-type"></a>columnDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示网站、[列表或][] [contentType][][中的][]列。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出网站中的列](../api/site-list-columns.md)|[columnDefinition](../resources/columndefinition.md) 集合|获取网站中的 [columnDefinition](../resources/columndefinition.md) 对象及其属性 [的列表](../resources/site.md)。|
|[列出列表中的列](../api/list-list-columns.md)|[columnDefinition](../resources/columndefinition.md) 集合|在列表中获取 [columnDefinition](../resources/columndefinition.md) 对象及其属性 [的列表](../resources/list.md)。|
|[列出内容类型中的列](../api/contenttype-list-columns.md)|[columnDefinition](../resources/columndefinition.md) 集合|获取内容类型中的 [columnDefinition](../resources/columndefinition.md) 对象及其 [属性的列表](../resources/contenttype.md)。|
|[为网站创建 columnDefinition](../api/site-post-columns.md)|[columnDefinition](../resources/columndefinition.md)|在网站 [中创建新的 columnDefinition](../resources/columndefinition.md) [对象](../resources/site.md)。|
|[为列表创建 columnDefinition](../api/list-post-columns.md)|[columnDefinition](../resources/columndefinition.md)|在列表中 [创建新的 columnDefinition](../resources/columndefinition.md) [对象](../resources/list.md)。|
|[为内容类型创建 columnDefinition](../api/contenttype-post-columns.md)|[columnDefinition](../resources/columndefinition.md)|在内容类型 [中创建新的 columnDefinition](../resources/columndefinition.md) [对象](../resources/contenttype.md)。|
|[获取 columnDefinition](../api/columndefinition-get.md)|[columnDefinition](../resources/columndefinition.md)|读取 [columnDefinition 对象的属性和](../resources/columndefinition.md) 关系。|
|[更新 columnDefinition](../api/columndefinition-update.md)|[columnDefinition](../resources/columndefinition.md)|更新 [columnDefinition 对象](../resources/columndefinition.md) 的属性。|
|[删除 columnDefinition](../api/columndefinition-delete.md)|无|删除 [columnDefinition](../resources/columndefinition.md) 对象。|

## <a name="json-representation"></a>JSON 表示形式

下面是 columnDefinition 资源的 JSON 表示形式。

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
  "enforceUniqueValues": true,
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
  "text": { "@odata.type": "microsoft.graph.textColumn" },
  "isDeletable" : false,
  "propagateChanges": false,
  "isReorderable": false,
  "isSealed": false,
  "validation": { "@odata.type": "microsoft.graph.columnValidation" },
  "hyperlinkOrPicture": { "@odata.type": "microsoft.graph.hyperlinkOrPictureColumn" },
  "term": { "@odata.type": "microsoft.graph.termColumn" },
  "sourceContentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "thumbnail": { "@odata.type": "microsoft.graph.thumbnailColumn" },
  "type": { "@odata.type": "microsoft.graph.columnTypes" },
  "contentApprovalStatus": { "@odata.type": "microsoft.graph.contentApprovalStatusColumn" }
}
```

## <a name="properties"></a>属性

列可以包含各种类型的数据。
以下属性表示列存储的数据类型以及该数据的其他设置。
与类型相关的属性 (布尔、计算、选项、货币、dateTime、lookup、number、personOrGroup、text) 是互斥的 -列只能指定其中一个。

| 属性名称           | 类型    | 说明
|:------------------------|:--------|:-----------------------------------------
| **columnGroup**         | string  | 对于网站列，此列所属的组的名称。 可以帮助组织相关的列。
| **说明**         | string  | 面向用户的列描述。
| **displayName**         | string  | 面向用户的列名称。
| **enforceUniqueValues** | Boolean | 如果为 true，则此列不能有两个列表项具有相同的值。
| **hidden**              | Boolean | 指定列是否显示在用户界面中。
| **id**                  | string  | 列的唯一标识符。
| **indexed**             | Boolean | 指定列值是否可用于排序和搜索。
| **名称**                | string  | 在 [listItem][] 上的 [fields][] 中显示的面向 API 的列名称。 对于面向用户的名称，请参阅 **displayName**。
| **readOnly**            | Boolean    | 指定是否可以修改列值。
| **required**            | Boolean | 指定列值是否不可选。
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
| **isDeletable**       | Boolean | 指示是否可以删除此列。
| **propagateChanges**     | Boolean | 如果"True"，则对此列所做的更改将传播到实现该列的列表。 
| **isReorderable**         | Boolean | 指示是否可以对列中的值进行重新排序。 只读。
| **isSealed**              | Boolean | 指定是否可以更改列。
| **validation**   |  [columnValidation][]    | 此列存储该列的验证公式和消息。 
| **hyperlinkOrPicture**  | [hyperlinkOrPictureColumn][] | 此列存储超链接或图片值。 
| **term**     | [termColumn][] | 此列存储分类术语。
| **sourceContentType**   |[contentTypeInfo][]  | 从其继承此列的 ContentType。 仅在提取 contentTypes 列时使用。
| **thumbnail**           |[thumbnailColumn][]      | 此列存储缩略图值。
| **类型**         | columnTypes  | 对于网站栏，列的类型。 只读
| **contentApprovalStatus**| [contentApprovalStatusColumn][]     | 此列存储内容审批状态。

## <a name="relationships"></a>关系

| 属性名称   | 类型                      | 说明
|:----------------|:--------------------------|:-------------------------------
| **sourceColumn** | [columnDefinition][] | 内容类型列的源列。

>**注意：** 这些属性对应于 SharePoint 的 [SPFieldType][] 枚举。
虽然上表中显示了最常见的字段类型，但此 beta API 仍缺少一些。
在这些情况下，不会填充列类型 facet，列将仅具有其基本属性。

## <a name="remarks"></a>备注

默认情况下，不显示 `hidden` 列的 ColumnDefinitions 和字段值。
若要在列出 **columnDefinitions** 时看到这些内容，请在 `$select` 语句中添加 `hidden`。
若要在 [listItems][listItem] 上显示 **字段** 值时看到这些内容，请在 `$select` 语句中添加名称所需的列。

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[columnDefinition]: columnDefinition.md
[contentType]: contenttype.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[geolocationColumn]: geolocationcolumn.md
[列表]: list.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[site]: site.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md
[termColumn]: termColumn.md
[contentApprovalStatusColumn]: contentApprovalStatusColumn.md
[thumbnailColumn]: thumbnailColumn.md
[hyperlinkOrPictureColumn]: hyperlinkOrPictureColumn.md
[columnValidation]: columnValidation.md
[contentTypeInfo]: contentTypeInfo.md


  [SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition",
  "suppressions": []
}
-->