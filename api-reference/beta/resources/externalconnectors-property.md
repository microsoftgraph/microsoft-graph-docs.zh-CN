---
title: 属性资源类型
description: 连接架构属性Microsoft 搜索定义。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 68dfe94d81f4ae5347322ba17c02eb3dab5c15d7
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467663"
---
# <a name="property-resource-type"></a>属性资源类型

命名空间：microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

连接[架构](externalconnectors-schema.md)的架构Microsoft 搜索[定义](externalconnectors-externalconnection.md)。

## <a name="properties"></a>属性

| 属性      | 类型              | 说明                                        |
|:--------------|:------------------|:---------------------------------------------------|
| aliases       | 字符串集合 | 属性的一组别名或友好名称。 最多 32 个字符。 每个字符串不得包含控制字符、空格或以下任何字符： `:` 、 、 `;` `,` 、 `(` `)` 、 `[` `]` 、 `{` 、 `}` 、 `%` `$` `+` `!` 、 `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` 。 可选。  |
| isQueryable   | boolean           | 指定属性是否可查询。 可查询属性可用于关键字查询语言 [ (KQL) 查询](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)。 可选。  |
| isRefinable   | boolean           | 指定属性是否可精简。  可精简属性可用于筛选搜索[API](search-api-overview.md)中的搜索结果，在用户体验中Microsoft 搜索精简程序控件。 可选。  |
| isRetrievable | boolean           | 指定属性是否可检索。 当搜索 API 返回项目结果集可检索属性将返回在搜索记录中。 还可将可检索属性添加到用于呈现搜索结果的显示模板。 可选。 |
| isSearchable  | boolean           | 指定属性是否可搜索。 仅类型或 `string` `stringCollection` 可搜索的属性。 不可搜索的属性不会添加到搜索索引。 可选。 |
| labels        | 字符串集合 | 指定针对属性添加的一个或多个已知标记。 标签Microsoft 搜索了解连接中数据的语义。 添加适当的标签可增强搜索体验 (例如，提高相关性) 。 支持的标签 `title` `url` `createdBy` ：、、、、、、、 `lastModifiedBy` `authors` 和 `createdDateTime` `lastModifiedDateTime` `fileName` `fileExtension` `iconUrl` `containerName` `containerUrl` 。 可选。 |
| name          | String            | 属性的名称。 最多 32 个字符。 不得包含控制字符、空格或以下任何 `:` 字符：、 `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` 此为必需属性。                |
| type          | String            | 属性的数据类型。 可取值为：`string`、`int64`、`double`、`dateTime`、`boolean`、`stringCollection`、`int64Collection`、`doubleCollection`、`dateTimeCollection`。 此为必需属性。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.property",
  "baseType": null
}-->

```json
{
  "aliases": [ "String" ],
  "isQueryable": true,
  "isRefinable": true,
  "isRetrievable": true,
  "isSearchable": true,
  "labels": [ "string" ],
  "name": "string",
  "type": "string"
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
