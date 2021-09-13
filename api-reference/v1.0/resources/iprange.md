---
title: ipRange 资源类型
description: 表示 IPV4 和 IPV6 地址范围的 IP 范围基类。
ms.localizationpriority: medium
author: videor
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: b0bb1aba5e0a8f26e12aa8d8f1e273dd58617f68
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089380"
---
# <a name="iprange-resource-type"></a>ipRange 资源类型

命名空间：microsoft.graph

用于配置[ipNamedLocation](ipnamedlocation.md)对象的[iPv4CidrRange](ipv4cidrrange.md)和[iPv6CidrRange](ipv6cidrrange.md)资源类型的 IP 范围抽象类型。

[iPv4CidrRange](ipv4cidrrange.md)派生类型用于配置 IPv4 地址范围，而[iPv6CidrRange](ipv6cidrrange.md)派生类型用于配置 IPv6 地址范围。

## <a name="properties"></a>属性

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ipRange"
}-->

```json
{
    "@odata.type": "#microsoft.graph.ipRange"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ipRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

