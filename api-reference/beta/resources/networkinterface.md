---
title: networkInterface 资源类型
description: 表示与此主机关联的网络接口卡 (NIC) 。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-pc
ms.technology: microsoft-graph
author: preetikr
ms.openlocfilehash: 9c2d2b8558730a832d6658ce6ef137d609a13d04
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176810"
---
# <a name="networkinterface-resource-type"></a>networkInterface 资源类型

命名空间：microsoft.graph

表示与此主机关联的网络接口卡 (NIC) 。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|说明|String|NIC (说明，例如以太网适配器、无线 LAN 适配器局部区域连接 *<#> 等) 。|
|ipV4Address|String|与此 NIC 关联的最后一个 IPv4 地址。|
|ipV6Address|String|与此 NIC 关联的最后一个公共 (又名全局) IPv6 地址。|
|localIpV6Address|String|与此 NIC 关联的最后一个本地 (链接本地或站点本地) IPv6 地址。|
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


