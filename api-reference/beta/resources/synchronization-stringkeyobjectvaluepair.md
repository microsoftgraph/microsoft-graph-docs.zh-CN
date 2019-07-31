---
title: stringKeyObjectValuePair 资源类型
description: 表示键值对, 其中键是字符串, 值是任意的 JSON 对象。 这是一种 OData 开放类型, 它应具有一个名`value`为的属性, 它是一个有效的 JSON 对象。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3ec55eee1f6b5f60e8936f906390d5343fbafbdf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007828"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a>stringKeyObjectValuePair 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示键值对, 其中键是字符串, 值是任意的 JSON 对象。 这是一种 OData 开放类型, 它应具有一个名`value`为的属性, 它是一个有效的 JSON 对象。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|Key|String|键。|
|值|Json|任意 JSON 对象。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
