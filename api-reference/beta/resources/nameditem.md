---
title: NamedItem 资源类型
description: 表示单元格区域或值的定义名称。名称可以为基元的已命名对象（如以下类型中所示）、range 对象或对区域的引用。此对象可用于获取与名称相关的 range 对象。
ms.openlocfilehash: 11ca12e0ae094f0e682cfde5fb1fe1feecabdb9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045162"
---
# <a name="nameditem-resource-type"></a>NamedItem 资源类型

表示单元格区域或值的定义名称。名称可以为基元的已命名对象（如以下类型中所示）、range 对象或对区域的引用。此对象可用于获取与名称相关的 range 对象。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Add](../api/nameditem-add.md)|[NamedItem](nameditem.md)|将新名称添加到给定范围的集合。|
|[AddFormulaLocal](../api/nameditem-addformulalocal.md)|[NamedItem](nameditem.md)|使用用户的公式区域设置，将新名称添加到给定范围的集合。|
|[获取 NamedItem](../api/nameditem-get.md) | [NamedItem](nameditem.md) |读取 nameditem 对象的属性和关系。|
|[更新](../api/nameditem-update.md) | [NamedItem](nameditem.md)   |更新 NamedItem 对象。 |
|[区域](../api/nameditem-range.md)|[Range](range.md)|返回与名称相关的 range 对象。如果已命名项目的类型不是区域，将引发异常。|
|[列出](../api/nameditem-list.md) | [NamedItem](nameditem.md) 集合 |获取 namedItem 对象集合。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|name|string|对象的名称。只读。|
|注释|string|表示与此名称相关联的注释。|
|scope|string|指明是否将 name 限定到工作簿或特定工作表。只读。|
|type|string|指示与名称相关的引用类型。可能的值是：`String`、`Integer`、`Double`、`Boolean`、`Range`。只读。|
|值|string|表示名称定义为引用的公式。例如 =Sheet14!$B$2:$H$12、=4.75 等。只读。|
|visible|boolean|指定对象是否可见。|

## <a name="relationships"></a>Relationships
| 关系     | 类型   |说明|
|:---------------|:--------|:----------|
|worksheet|[worksheet](worksheet.md)|返回已命名项限定到的工作表。仅在该项目的作用域为工作表时才可用。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": "string",
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
