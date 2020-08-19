---
title: networkInterface 资源类型
description: 表示与此主机关联 (NIC) 的网络接口卡。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 4f19c2fae729e437ec2d9e91a0c6be5694a85214
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812784"
---
# <a name="networkinterface-resource-type"></a>networkInterface 资源类型

命名空间：microsoft.graph

表示与此主机关联 (NIC) 的网络接口卡。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|说明|String|NIC 的说明 (例如，以太网适配器、无线局域网适配器本地区域连接 * < # > 等 ) 。|
|ipV4Address|String|与此 NIC 关联的最后一个 IPv4 地址。|
|ipV6Address|String|最后一个公共 (也称为全局) 与此 NIC 关联的 IPv6 地址。|
|localIpV6Address|String|上次本地 (与此 NIC 关联的本地或站点本地) IPv6 地址。|
|macAddress|String|此主机上的 NIC 的 MAC 地址。|

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
