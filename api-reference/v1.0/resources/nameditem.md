---
title: NamedItem 资源类型
description: 表示单元格区域或值的定义名称。名称可以为基元的已命名对象（如以下类型中所示）、range 对象或对区域的引用。此对象可用于获取与名称相关的 range 对象。
ms.localizationpriority: medium
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6afde3e91f451b146add7e364a3c308959d4eff2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59028812"
---
# <a name="nameditem-resource-type"></a>NamedItem 资源类型

命名空间：microsoft.graph

表示单元格区域或值的定义名称。名称可以为基元的已命名对象（如以下类型中所示）、range 对象或对区域的引用。此对象可用于获取与名称相关的 range 对象。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Add](../api/nameditem-add.md)|[WorkbookNamedItem](nameditem.md)|将新名称添加到给定范围的集合。|
|[AddFormulaLocal](../api/nameditem-addformulalocal.md)|[WorkbookNamedItem](nameditem.md)|使用用户的公式区域设置，将新名称添加到给定范围的集合。|
|[获取 NamedItem](../api/nameditem-get.md) | [WorkbookNamedItem](nameditem.md) |读取 nameditem 对象的属性和关系。|
|[更新](../api/nameditem-update.md) | [WorkbookNamedItem](nameditem.md)   |更新 NamedItem 对象。 |
|[区域](../api/nameditem-range.md)|[区域](range.md)|返回与名称相关的 range 对象。如果已命名项目的类型不是区域，将引发异常。|
|[列出](../api/nameditem-list.md) | [WorkbookNamedItem](nameditem.md) 集合 |获取 namedItem 对象集合。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|name|string|对象的名称。只读。|
|comment|string|表示与此名称相关联的注释。|
|scope|string|指明是否将 name 限定到工作簿或特定工作表。只读。|
|类型|string|指示与名称相关的引用类型。 可能的值包括 `String`、`Integer`、`Double`、`Boolean`、`Range`。 只读。|
|value|Json|表示名称定义为引用的公式。例如 =Sheet14!$B$2:$H$12、=4.75 等。只读。|
|visible|布尔|指定对象是否可见。|

## <a name="relationships"></a>关系
| 关系     | 类型   |说明|
|:---------------|:--------|:----------|
|worksheet|[WorkbookWorksheet](worksheet.md)|返回已命名项限定到的工作表。仅在该项目的作用域为工作表时才可用。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookNamedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": {"@odata.type": "microsoft.graph.Json"},
  "visible": true

}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

