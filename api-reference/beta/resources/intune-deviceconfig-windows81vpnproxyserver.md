---
title: windows81VpnProxyServer 资源类型
description: VPN 代理服务器。
author: tfitzmac
ms.openlocfilehash: 015df762d25e1a87a9ce29bd4efbc15e98ed7e08
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349362"
---
# <a name="windows81vpnproxyserver-resource-type"></a>windows81VpnProxyServer 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

VPN 代理服务器。

继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|automaticConfigurationScriptUrl|字符串|代理服务器的自动配置脚本的 url。 继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|address|String|地址。 继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|port|Int32|端口。 有效值 0 到 65535 继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|automaticallyDetectProxySettings|Boolean|自动检测代理设置。|
|bypassProxyServerForLocalAddress|Boolean|对于本地地址绕过代理服务器。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows81VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "automaticallyDetectProxySettings": true,
  "bypassProxyServerForLocalAddress": true
}
```





