---
title: 键值资源类型
description: 提供有关登录请求的其他相关信息
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 46914cfd74eac45726bc17fc0661a861ad402534
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523021"
---
# <a name="keyvalue-resource-type"></a>键值资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供其他身份验证处理信息，如服务器名称和登录和域的提示的存在。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|Key|String|包含与值相关联的字段的名称。 当登录请求中包含登录或域提示时，相应的字段作为键值对包含。 可能的键`Login hint present`： `Domain hint present`、。|
|value|String|包含指定键的相应值。 如果登录请求`true`中包含登录提示，则值为; 否则为。否则`false`为。 值是`true`在登录请求中包含域提示;否则`false`为。|

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
