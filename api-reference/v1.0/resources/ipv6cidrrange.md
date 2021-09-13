---
title: iPv6CidrRange 资源类型
description: 表示使用 CIDR 表示法的 IPv6 范围。
ms.localizationpriority: medium
author: videor
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: d36d19d3d0d10da58a3223c146be542c9f57878c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062479"
---
# <a name="ipv6cidrrange-resource-type"></a>iPv6CidrRange 资源类型

命名空间：microsoft.graph

表示使用无类别域间路由和 CIDR (IPv6) 范围。

继承自 [ipRange](../resources/iprange.md)

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|cidrAddress|String|CIDR 表示法中的 IPv6 地址。 不可为空。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.iPv6CidrRange",
  "baseType": "microsoft.graph.ipRange"
}-->

```json
{
  "@odata.type": "#microsoft.graph.iPv6CidrRange", 
  "cidrAddress": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "iPv6CidrRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
