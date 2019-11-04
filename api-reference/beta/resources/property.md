---
title: 属性资源类型
description: Microsoft 搜索连接的架构属性定义。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: df535b89d238f31185ff187b207671337d05fd75
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939086"
---
# <a name="property-resource-type"></a>属性资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft 搜索[连接](externalconnection.md)的[架构](schema.md)属性定义。

## <a name="properties"></a>属性

| 属性      | 类型    | 描述                                        |
|:--------------|:--------|:---------------------------------------------------|
| isQueryable   | Boolean | 指定属性是否为可查询属性。 可查询属性可在[关键字查询语言（KQL）查询](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)中使用。 可选。  |
| isRetrievable | Boolean | 指定属性是否可检索。 当搜索 API 返回项目时，将在结果集中返回可检索的属性。 可检索属性也可用于添加到用于呈现搜索结果的显示模板。 可选。 |
| isSearchable  | Boolean | 指定属性是否可搜索。 仅可搜索的`String`类型`Collection(String)`或属性的属性。 不可搜索的属性不会添加到搜索索引中。 可选。 |
| name          | String  | 属性的名称。 最多32个字符。 不得包含`:`控制字符、空白或以下任何内容：、 `;`、 `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*`、、、、、、、、、、、、、 `=``&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`. 此为必需属性。                |
| type          | 字符串  | 属性的数据类型。 可取值为：`String`、`Int64`、`Double`、`DateTime`、`Boolean`、`Collection(String)`、`Collection(Int64)`、`Collection(Double)`、`Collection(DateTime)`。 必填。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.property",
  "baseType": null
}-->

```json
{
  "isQueryable": true,
  "isRetrievable": true,
  "isSearchable": true,
  "name": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "property resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
