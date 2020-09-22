---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
description: listInfo 复杂类型提供有关 list 的其他信息。
doc_type: resourcePageType
ms.openlocfilehash: a7a0a7d400d54ce27dc2f0c8a3397def301fa7aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025260"
---
# <a name="listinfo-resource"></a>ListInfo 资源

命名空间：microsoft.graph

**listInfo** 复杂类型提供有关 [list][] 的其他信息。

[list]: list.md

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.listInfo"
}-->

```json
{
  "contentTypesEnabled": false,
  "hidden": false,
  "template": "documentLibrary | genericList | tasks | survey | links | announcements | contacts | ..."
}
```

## <a name="properties"></a>属性

| 属性名称           | 类型    | 说明
|:------------------------|:--------|:------------------------------------------------
| **contentTypesEnabled** | Boolean | 如果为 `true`，则表明已为此列表启用内容类型。
| **hidden**              | Boolean | 如果为 `true`，则表明该列表通常在 SharePoint 用户体验中不可见。
| **template**            | String  | 一个枚举值，表示创建列表时使用的基本列表模板。 可能的值包括 `documentLibrary`、`genericList`、`task`、`survey`、`announcements`、`contacts` 等。

### <a name="remarks"></a>注解

虽然用户创建的大多数列表都有上面列出的一个值，但也可能包含其他值。
应用应准备好处理未在此处列出的任何值。
对于熟悉 SharePoint CSOM API 的开发人员，`template` 值与 `SPListTemplateType` 枚举对应。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/listinfo.md:
      Found potential enums in resource example that weren't defined in a table:(documentLibrary,genericList,tasks,survey,links,announcements,contacts,...) are in resource, but () are in table"
  ],
  "tocPath": ""
}-->

