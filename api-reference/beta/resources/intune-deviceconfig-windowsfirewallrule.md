---
title: windowsFirewallRule 资源类型
description: 控制通过防火墙Windows的规则。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ead732e65cf3119f974f2fa6b29da14cc3dd180b1211dcba1a5dd1db90cc71eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251405"
---
# <a name="windowsfirewallrule-resource-type"></a>windowsFirewallRule 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

控制通过防火墙Windows的规则。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|规则的显示名称。 不需要是唯一的。|
|description|字符串|规则的说明。|
|packageFamilyName|String|受防火墙规则Microsoft Store应用程序包系列名称。|
|filePath|String|受防火墙规则影响的应用的完整文件路径。|
|serviceName|String|在服务（而不是应用程序）发送或接收通信时所使用的名称。|
|协议|Int32|0-255 号码，表示 TCP (6，UDP = 17) 。 如果未指定，则默认值为 All。 有效值为 0 到 255|
|localPortRanges|String collection|本地端口范围的列表。 例如，"100-120"、"200"、"300-320"。 如果未指定，则默认值为 All。|
|remotePortRanges|String collection|远程端口范围列表。 例如，"100-120"、"200"、"300-320"。 如果未指定，则默认值为 All。|
|localAddressRanges|String collection|规则涵盖的本地地址列表。 默认值为任意地址。 有效令牌包括：<ul><li>"*"指示任何本地地址。 如果存在此令牌，则必须是包含的唯一令牌。</li><li>可以使用子网掩码或网络前缀表示法指定子网。 如果未指定子网掩码和网络前缀，则子网掩码默认为 255.255.255.255。</li><li>有效的 IPv6 地址。</li><li>格式为"开始地址 - 结束地址"的 IPv4 地址范围，不包含空格。</li><li>格式为"开始地址 - 结束地址"的 IPv6 地址范围，不包含空格。</li></ul>|
|remoteAddressRanges|String collection|指定规则涵盖的远程地址的令牌列表。 令牌不区分大小写。 默认值为任意地址。 有效令牌包括：<ul><li>"*"指示任何远程地址。 如果存在此令牌，则必须是包含的唯一令牌。</li><li>"Defaultgateway"</li><li>"DHCP"</li><li>"DNS"</li><li>"WINS"</li><li>1809 (版本 1809 Windows支持"Intranet") </li><li>"RmtIntranet" (版本 1809 Windows版本上支持) </li><li>1809 (版本 Windows 1809) 支持"Internet") </li><li>1809 (版本 1809 Windows支持"Ply2Renders") </li><li>"LocalSubnet"指示本地子网上的任何本地地址。</li><li>可以使用子网掩码或网络前缀表示法指定子网。 如果未指定子网掩码和网络前缀，则子网掩码默认为 255.255.255.255。</li><li>有效的 IPv6 地址。</li><li>格式为"开始地址 - 结束地址"的 IPv4 地址范围，不包含空格。</li><li>格式为"开始地址 - 结束地址"的 IPv6 地址范围，不包含空格。</li></ul>|
|profileTypes|[windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)|指定规则所属的配置文件。 如果未指定，则默认值为 All。 可取值为：`notConfigured`、`domain`、`private`、`public`。|
|action|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|规则强制执行的操作。 如果未指定，则默认值为 Allowed。 可取值为：`notConfigured`、`blocked`、`allowed`。|
|trafficDirection|[windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)|为规则启用的流量方向。 如果未指定，则默认值为 Out。可能的值是 `notConfigured` `out` `in` ：、、。|
|interfaceTypes|[windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)|规则的接口类型。 可取值为：`notConfigured`、`remoteAccess`、`wireless`、`lan`。|
|edgeTraversal|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|指示是为此规则启用还是禁用边缘遍历。 EdgeTraversal 设置指示允许特定入站流量使用 Teredo 隧道技术通过 NAT 和其他边缘设备进行隧道传输。 为了使此设置正常工作，具有入站防火墙规则的应用程序或服务需要支持 IPv6。 此设置的主要应用程序允许主机上的侦听器通过 Teredo IPv6 地址进行全局地址处理。 默认情况下，新规则禁用 EdgeTraversal 属性。 可取值为：`notConfigured`、`blocked`、`allowed`。|
|localUserAuthorizations|String|指定应用容器的授权本地用户列表。 这是安全描述符定义语言和 SDDL (格式) 字符串。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallRule",
  "displayName": "String",
  "description": "String",
  "packageFamilyName": "String",
  "filePath": "String",
  "serviceName": "String",
  "protocol": 1024,
  "localPortRanges": [
    "String"
  ],
  "remotePortRanges": [
    "String"
  ],
  "localAddressRanges": [
    "String"
  ],
  "remoteAddressRanges": [
    "String"
  ],
  "profileTypes": "String",
  "action": "String",
  "trafficDirection": "String",
  "interfaceTypes": "String",
  "edgeTraversal": "String",
  "localUserAuthorizations": "String"
}
```




