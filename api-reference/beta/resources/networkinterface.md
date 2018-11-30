---
title: networkInterface 资源类型
description: 表示与此主机网络接口卡 (NIC)。
ms.openlocfilehash: 7044b4f469e74424b0dc27ffa38c5feb081faa45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042177"
---
# <a name="networkinterface-resource-type"></a>networkInterface 资源类型

表示与此主机网络接口卡 (NIC)。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|说明|字符串|NIC 的说明 (例如以太网适配器，无线 LAN 适配器本地区域连接 * <> # 等。)。|
|ipV4Address|字符串|与此网卡关联的最后一个 IPv4 地址|
|ipV6Address|字符串|最后一个公用 （也称为全局） IPv6 地址与此网卡。|
|localIpV6Address|字符串|最后一个本地 （链接-本地或站点-本地） IPv6 地址与此网卡。|
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