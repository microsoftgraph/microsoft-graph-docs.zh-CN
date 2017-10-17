---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListInfo
ms.openlocfilehash: eb4952c1a49c41dfae6683153753711158c70f01
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="listinfo-resource"></a>ListInfo 资源

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
| **contentTypesEnabled** | Boolean | 如果值为 `true`，则表示为此列表启用了内容类型。
| **hidden**              | Boolean | 如果值为 `true`，则表示该列表在 SharePoint 用户体验中通常不可见。
| **template**            | String  | 枚举值，表示创建列表时使用的基本列表模板。 可能的值包括 `documentLibrary`、`genericList`、`task`、`survey`、`announcements`、`contacts` 等。

### <a name="remarks"></a>备注

虽然用户创建的大多数列表将具有上面列出的其中一个值，但也可以使用其他值。
应用应准备好处理此处未列出的任何值。
对于熟悉 SharePoint 的 CSOM API 的开发者，`template` 值对应于 `SPListTemplateType` 枚举。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
