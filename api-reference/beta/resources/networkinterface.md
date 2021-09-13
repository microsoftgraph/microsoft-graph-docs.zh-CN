---
title: networkInterface 资源类型
description: 表示与此主机 (NIC) 网络接口卡。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 914d7f3484762a9b2994fe1eef06d47f4ac09f75
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59105788"
---
# <a name="networkinterface-resource-type"></a>networkInterface 资源类型

命名空间：microsoft.graph

表示与此主机 (NIC) 网络接口卡。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|说明|String|NIC (描述，例如以太网适配器、无线 LAN 适配器局域网连接 *<#> 等) 。|
|ipV4Address|String|与此 NIC 关联的最后一个 IPv4 地址。|
|ipV6Address|String|上次公开 (，也) NIC 关联的 IPv6 地址。|
|localIpV6Address|String|上次本地 (与此 NIC 关联的 IPv6) 本地或站点本地地址。|
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


