---
title: stringKeyObjectValuePair 资源类型
description: 表示其中的密钥是一个字符串，值是一个任意 JSON 对象的键 / 值对。 这是认为应该有一个名为属性 OData 打开类型`value`，它是一个有效的 JSON 对象。
localization_priority: Normal
ms.openlocfilehash: 8545a4ef5a4931d3b886c95b4f39218bc418f53d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831449"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a>stringKeyObjectValuePair 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示其中的密钥是一个字符串，值是一个任意 JSON 对象的键 / 值对。 这是认为应该有一个名为属性 OData 打开类型`value`，它是一个有效的 JSON 对象。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|Key|字符串|键。|
|值|任意|任意的 JSON 对象。|

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
  "key": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
