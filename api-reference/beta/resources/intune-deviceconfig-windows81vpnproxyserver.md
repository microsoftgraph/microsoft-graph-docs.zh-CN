---
title: windows81VpnProxyServer 资源类型
description: VPN 代理服务器。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 60b8e18be9f50d912020d741cf1d65f1f9d756a4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279148"
---
# <a name="windows81vpnproxyserver-resource-type"></a>windows81VpnProxyServer 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN 代理服务器。


继承自 [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|automaticConfigurationScriptUrl|字符串|代理的自动配置脚本 url。 继承自 [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|address|String|处理. 继承自 [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|端口|Int32|端口. 从[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)继承的有效值为0至65535|
|automaticallyDetectProxySettings|Boolean|自动检测代理设置。|
|bypassProxyServerForLocalAddress|Boolean|对本地地址绕过代理服务器。|

## <a name="relationships"></a>关系
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




