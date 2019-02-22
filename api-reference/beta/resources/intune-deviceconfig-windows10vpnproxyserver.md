---
title: windows10VpnProxyServer 资源类型
description: VPN 代理服务器。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4686049e2f3525409e81ec1492dcb052ab9f3657
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140689"
---
# <a name="windows10vpnproxyserver-resource-type"></a>windows10VpnProxyServer 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN 代理服务器。


继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|automaticConfigurationScriptUrl|字符串|代理的自动配置脚本 url。 继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|address|String|处理. 继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|port|Int32|端口. 从[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)继承的有效值为0至65535|
|bypassProxyServerForLocalAddress|布尔|对本地地址绕过代理服务器。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "bypassProxyServerForLocalAddress": true
}
```




