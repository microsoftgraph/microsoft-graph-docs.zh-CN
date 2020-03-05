---
title: stringKeyObjectValuePair 资源类型
description: 表示键值对，其中键是字符串，值是任意的 JSON 对象。 这是一种 OData 开放类型，它应具有一个名`value`为的属性，它是一个有效的 JSON 对象。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c3a86cd4963f8d17fbe9f4c5371e98070f8f8f4e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520091"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a>stringKeyObjectValuePair 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示键值对，其中键是字符串，值是任意的 JSON 对象。 这是一种 OData 开放类型，它应具有一个名`value`为的属性，它是一个有效的 JSON 对象。

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
