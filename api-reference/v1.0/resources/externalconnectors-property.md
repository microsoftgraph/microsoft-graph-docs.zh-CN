---
title: 属性资源类型
description: 连接架构属性Microsoft 搜索定义。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 2595f222410b96b2c2586d8cfd06ccc0722a1911
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453308"
---
# <a name="property-resource-type"></a>属性资源类型

命名空间：microsoft.graph.externalConnectors



连接[架构](externalconnectors-schema.md)的架构Microsoft 搜索[定义](externalconnectors-externalconnection.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|aliases|字符串集合|属性的一组别名或友好名称。 最多 32 个字符。 仅允许字母数字字符。 例如，每个字符串不能包含控制字符、空格或以下任一 `:` 字符：、。 `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `` ` `` `^` 可选。|
|isQueryable|Boolean|指定属性是否可查询。 可查询属性可用于关键字查询语言 [ (KQL) 查询](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)。 可选。|
|isRefinable|Boolean|指定属性是否可精简。  可精简属性可用于筛选搜索[API](search-api-overview.md)中的搜索结果，并添加用户体验Microsoft 搜索控件。 可选。|
|isRetrievable|Boolean|指定属性是否可检索。 当搜索 API 返回项目结果集可检索属性将返回在搜索记录中。 还可将可检索属性添加到用于呈现搜索结果的显示模板。 可选。|
|isSearchable|Boolean|指定属性是否可搜索。 仅类型或 `String` `StringCollection` 可搜索的属性。 不可搜索的属性不会添加到搜索索引。 可选。|
|labels|microsoft.graph.externalConnectors.label 集合|指定针对属性添加的一个或多个已知标记。 标签Microsoft 搜索了解连接中数据的语义。 添加适当的标签可增强搜索体验 (例如，提高相关性) 。 可取值包括：`title`、`url`、`createdBy`、`lastModifiedBy`、`authors`、`createdDateTime`、`lastModifiedDateTime`、`fileName`、`fileExtension`、`unknownFutureValue`。 可选。|
|name|String|属性的名称。 最多 32 个字符。 仅允许字母数字字符。 例如，每个字符串不能包含控制字符、空格或以下任一 `:` 字符：、。 `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `` ` `` `^`  此为必需属性。|
|type|microsoft.graph.externalConnectors.propertyType|属性的数据类型。 可取值为：`string`、`int64`、`double`、`dateTime`、`boolean`、`stringCollection`、`int64Collection`、`doubleCollection`、`dateTimeCollection`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.property"
}
-->
``` json
{
  "name": "String",
  "type": "String",
  "isSearchable": "Boolean",
  "isRetrievable": "Boolean",
  "isQueryable": "Boolean",
  "isRefinable": "Boolean",
  "aliases": [
    "String"
  ],
  "labels": [
    "String"
  ]
}
```

