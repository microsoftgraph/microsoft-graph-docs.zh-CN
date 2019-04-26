---
title: metadataEntry 资源类型
description: 给定对象的元数据。
localization_priority: Normal
ms.openlocfilehash: 829dc5fbbf3d73dbabb2e9e69bfff28814cc203a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345576"
---
# <a name="metadataentry-resource-type"></a>metadataEntry 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

给定对象的元数据。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|Key|String|元数据属性的名称。|
|value|String|元数据属性的值。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataEntry"
}-->

```json
{
  "key": "String",
  "value": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "metadataEntry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
