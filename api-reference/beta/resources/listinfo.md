---
author: JeremyKelley
description: listInfo 复杂类型提供有关 list 的其他信息。
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 3a066505348b1a1014b27ca3c83e0ee2f97f41a5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522951"
---
# <a name="listinfo-resource"></a>ListInfo 资源

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| **contentTypesEnabled** | 布尔 | 如果为 `true`，则表明已为此列表启用内容类型。
| **hidden**              | Boolean | 如果为 `true`，则表明该列表通常在 SharePoint 用户体验中不可见。
| **template**            | String  | 一个枚举值，表示创建列表时使用的基本列表模板。 可能的值包括 `documentLibrary`、`genericList`、`task`、`survey`、`announcements`、`contacts` 等。

### <a name="remarks"></a>注解

虽然用户创建的大多数列表都有上面列出的一个值，但也可能包含其他值。
应用应准备好处理未在此处列出的任何值。
对于熟悉 SharePoint CSOM API 的开发人员，`template` 值与 `SPListTemplateType` 枚举对应。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
