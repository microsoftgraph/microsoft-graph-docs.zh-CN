---
title: windows81VpnProxyServer 资源类型
description: VPN 代理服务器。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b9ced7586870dc0b9dc5f3df2c95000d1342cc93
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033656"
---
# <a name="windows81vpnproxyserver-resource-type"></a>windows81VpnProxyServer 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN 代理服务器。


继承自 [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|automaticConfigurationScriptUrl|String|代理的自动配置脚本 URL。 继承自 [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|address|String|地址。 继承自 [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|端口|Int32|端口。 有效值 0 至 65535 继承自 [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|automaticallyDetectProxySettings|Boolean|自动检测代理设置。|
|bypassProxyServerForLocalAddress|Boolean|对于本地地址，绕过代理服务器。|

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



