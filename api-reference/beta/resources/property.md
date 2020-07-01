---
title: 属性资源类型
description: Microsoft 搜索连接的架构属性定义。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9862170dfcca0960ebd319089da70cca93782875
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990262"
---
# <a name="property-resource-type"></a>属性资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft 搜索[连接](externalconnection.md)的[架构](schema.md)属性定义。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>属性

| 属性      | 类型              | 说明                                        |
|:--------------|:------------------|:---------------------------------------------------|
| 别名       | String collection | 一组别名或属性的友好名称。 最多32个字符。 每个字符串不得包含控制字符、空白或以下任何内容：、、、、、、、、、、、、、、、、、、、、、、、、、、 `:` `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` 。 可选。  |
| isQueryable   | Boolean           | 指定属性是否为可查询属性。 可查询属性可在[关键字查询语言（KQL）查询](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)中使用。 可选。  |
| isRefinable   | Boolean           | 指定属性是否为可精简。  可精简属性可用于筛选[搜索 API](search-api-overview.md)中的搜索结果，并在 Microsoft search 用户体验中添加精简条件控件。 可选。  |
| isRetrievable | Boolean           | 指定属性是否可检索。 当搜索 API 返回项目时，将在结果集中返回可检索的属性。 可检索属性也可用于添加到用于呈现搜索结果的显示模板。 可选。 |
| isSearchable  | Boolean           | 指定属性是否可搜索。 仅可搜索的类型或属性的属性 `String` `StringCollection` 。 不可搜索的属性不会添加到搜索索引中。 可选。 |
| 标题        | String collection | 指定针对属性添加的一个或多个已知标记。 标签可帮助 Microsoft 搜索了解连接中的数据的语义。 添加适当的标签将导致增强的搜索体验（如更好的相关性）。 支持的标签：、、、、、、 `title` `url` `createdBy` `lastModifiedBy` `authors` `createdDateTime` `lastModifiedDateTime` `fileName` 和 `fileExtension` 。 可选。 |
| name          | String            | 属性的名称。 最多32个字符。 不得包含控制字符、空白或以下任何内容：、、、、、、、、、、、、、、、、、、、、、、、、、、、 `:` `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` 。 此为必需属性。                |
| type          | String            | 属性的数据类型。 可取值为：`String`、`Int64`、`Double`、`DateTime`、`Boolean`、`StringCollection`、`Int64Collection`、`DoubleCollection`、`DateTimeCollection`。 必需。 |

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
  "aliases": [ "String" ],
  "isQueryable": true,
  "isRefinable": true,
  "isRetrievable": true,
  "isSearchable": true,
  "labels": [ "String" ],
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
