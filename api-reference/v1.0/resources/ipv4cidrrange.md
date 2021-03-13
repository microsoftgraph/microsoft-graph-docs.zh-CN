---
title: iPv4CidrRange 资源类型
description: 表示使用 CIDR 表示法的 IPv4 范围。
localization_priority: Normal
author: videor
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 0b1af8d424d3e8dfc6f1791fa83a633e571310e6
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760867"
---
# <a name="ipv4cidrrange-resource-type"></a>iPv4CidrRange 资源类型

命名空间：microsoft.graph

表示使用 CIDR 表示法的 IPv4 范围。

继承自 [ipRange](../resources/iprange.md)

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|cidrAddress|字符串|CIDR 表示法中的 IPv4 地址|

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
