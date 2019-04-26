---
title: mentionsPreview 资源类型
description: 表示有关在资源实例中提及对象的信息。
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 516560d2a0a8e498c1a0b31a62d8ca4209724767
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342287"
---
# <a name="mentionspreview-resource-type"></a>mentionsPreview 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关在资源实例中[提及](../resources/mention.md)对象的信息。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| isMentioned | Boolean | 如此如果在父资源实例中提到了登录用户。 只读。 支持筛选器。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mentionsPreview"
}-->

```json
{
  "isMentioned": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mentionsPreview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
