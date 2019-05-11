---
title: vpnDnsRule 资源类型
description: VPN DNS 规则定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bdb362bcbf672f491e22e2ee7d69a7e5c243e812
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944612"
---
# <a name="vpndnsrule-resource-type"></a>vpnDnsRule 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN DNS 规则定义。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|name|String|别名.|
|台|String collection|台.|
|proxyServerUri|String|代理服务器 Uri。|
|autoTrigger|Boolean|当设备连接到此域时自动连接到 VPN: 默认值为 False。|
|保持|Boolean|将此规则保持为活动状态, 即使未连接 VPN 也是如此: 默认值为 False|

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




