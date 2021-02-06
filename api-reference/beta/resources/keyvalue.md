---
title: keyValue 资源类型
description: 提供有关登录请求的其他相关信息
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3459f827f35049b383e732c805d61371577b2260
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135392"
---
# <a name="keyvalue-resource-type"></a>keyValue 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供其他身份验证处理信息，例如服务器名称和登录和域提示的存在。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|Key|字符串|包含与值关联的字段的名称。 当登录请求中包含登录或域提示时，相应的字段会作为键值对包含在内。 可能的键： `Login hint present` `Domain hint present` ， 。|
|value|String|包含指定键的相应值。 该值是登录请求中是否包含登录提示;否则 `true` `false` 。 该值是 `true` 域提示是否包含在登录请求中;否则 `false` 。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValue",
  "baseType": null
}-->

```json
{
  "key": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


