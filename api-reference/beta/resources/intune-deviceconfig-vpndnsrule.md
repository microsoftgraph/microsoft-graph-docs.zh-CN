---
title: vpnDnsRule 资源类型
description: VPN DNS 规则定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1277bb254a9485bc2adc26859185adfe5d22ad5b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58793871"
---
# <a name="vpndnsrule-resource-type"></a>vpnDnsRule 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN DNS 规则定义。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|name|String|名称。|
|服务器|字符串集合|服务器。|
|proxyServerUri|String|代理服务器 Uri。|
|autoTrigger|布尔值|设备连接到此域时自动连接到 VPN：默认值 False。|
|persistent|Boolean|即使 VPN 未连接，也保持此规则处于活动状态：默认值 False|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String",
  "autoTrigger": true,
  "persistent": true
}
```



