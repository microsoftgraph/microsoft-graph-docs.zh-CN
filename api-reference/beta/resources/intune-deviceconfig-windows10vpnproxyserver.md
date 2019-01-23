---
title: windows10VpnProxyServer 资源类型
description: VPN 代理服务器。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d4f8975a08e60105c37e0959ac72e24a1dd639cd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407121"
---
# <a name="windows10vpnproxyserver-resource-type"></a>windows10VpnProxyServer 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN 代理服务器。


继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|automaticConfigurationScriptUrl|String|代理服务器的自动配置脚本的 url。 继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|address|String|地址。 继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|port|Int32|端口。 有效值 0 到 65535 继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|bypassProxyServerForLocalAddress|Boolean|对于本地地址绕过代理服务器。|

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




