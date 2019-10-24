---
title: iPv4CidrRange 资源类型
description: 表示使用 CIDR 表示法的 IPv4 范围。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4864388492f3dedec4add271904f2e07a3e85419
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653823"
---
# <a name="ipv4cidrrange-resource-type"></a>iPv4CidrRange 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示使用 CIDR 表示法的 IPv4 范围。

继承自 [ipRange](../resources/iprange.md)

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|cidrAddress|String|CIDR 表示法中的 IPv4 地址|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.iPv4CidrRange",
  "baseType": "microsoft.graph.ipRange"
}-->

```json
{
  "cidrAddress": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "iPv4CidrRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->