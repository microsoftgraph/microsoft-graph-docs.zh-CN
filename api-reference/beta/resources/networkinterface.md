---
title: networkInterface 资源类型
description: 表示与此主机 (NIC) 网络接口卡。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 7ba1efe14cfd4bce099960406ae31392c10529ba862c388e379ef234c786d6be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54224255"
---
# <a name="networkinterface-resource-type"></a>networkInterface 资源类型

命名空间：microsoft.graph

表示与此主机 (NIC) 网络接口卡。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|说明|String|NIC (描述，例如以太网适配器、无线 LAN 适配器局域网连接 *<#> 等) 。|
|ipV4Address|字符串|与此 NIC 关联的最后一个 IPv4 地址。|
|ipV6Address|字符串|Last Public (aka global) IPv6 address associated with this NIC.|
|localIpV6Address|String|上次本地 (与此 NIC 关联的链接本地或站点) IPv6 地址。|
|macAddress|String|此主机上 NIC 的 MAC 地址。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkInterface"
}-->

```json
{
  "description": "String",
  "ipV4Address": "String",
  "ipV6Address": "String",
  "localIpV6Address": "String",
  "macAddress": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkInterface resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


