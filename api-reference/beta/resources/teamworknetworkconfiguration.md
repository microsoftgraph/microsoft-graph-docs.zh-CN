---
title: teamworkNetworkConfiguration 资源类型
description: 表示有关已启用网络的设备Microsoft Teams配置的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5f08d5d3263917adfb9bc20ca5f964972281ecbb
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262305"
---
# <a name="teamworknetworkconfiguration-resource-type"></a>teamworkNetworkConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关已启用网络的设备Microsoft Teams配置[的详细信息](../resources/teamworkdevice.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|defaultGateway|String|默认网关是在目标对设备未知时用于传递信息的路径。|
|domainName|String|设备的网络域，例如 contoso.com。|
|hostName|String|网络上设备的名称。|
|ipAddress|String|IP 地址是一个数字标签，用于唯一标识连接到 Internet 的每台设备。|
|isDhcpEnabled|Boolean|`True` 如果已启用 DHCP。|
|isPCPortEnabled|Boolean|`True` 如果电脑端口已启用。|
|primaryDns|String|主 DNS 是设备的第一个联系点，用于将主机名转换为 IP 地址。|
|secondaryDns|字符串|当主 DNS 不可用时，使用辅助 DNS。|
|subnetMask|String|子网掩码是一个数字，用于区分 IP 地址中的网络地址和主机地址。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkNetworkConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkNetworkConfiguration",
  "defaultGateway": "String",
  "domainName": "String",
  "hostName": "String",
  "ipAddress": "String",
  "isDhcpEnabled": "Boolean",
  "isPCPortEnabled": "Boolean",
  "primaryDns": "String",
  "secondaryDns": "String",
  "subnetMask": "String"
}
```

