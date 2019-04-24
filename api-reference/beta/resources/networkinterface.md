---
title: networkInterface 资源类型
description: 表示与此主机相关联的网络接口卡 (NIC)。
localization_priority: Normal
ms.openlocfilehash: 92ea26b76de8fa6ffbcdcf0bc64b85a08d0f51af
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457065"
---
# <a name="networkinterface-resource-type"></a>networkInterface 资源类型

表示与此主机相关联的网络接口卡 (NIC)。

## <a name="properties"></a>属性

| 属性   | 类型 |描述|
|:---------------|:--------|:----------|
|说明|字符串|NIC 的说明 (例如, 以太网适配器、无线局域网适配器本地区域连接 * < # > 等)。|
|ipV4Address|字符串|与此 NIC 关联的最后一个 IPv4 地址。|
|ipV6Address|字符串|与此 NIC 关联的最后一个公共 (也称为全局) IPv6 地址。|
|localIpV6Address|字符串|与此 NIC 关联的最后一个本地 (链接本地或站点本地) IPv6 地址。|
|macAddress|字符串|此主机上的 NIC 的 MAC 地址。|

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
