---
title: windowsFirewallRule 资源类型
description: 通过 Windows 防火墙控制流量的规则。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 77df7da501aee80b534accbe4c0d33dcf0e8df63
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570213"
---
# <a name="windowsfirewallrule-resource-type"></a>windowsFirewallRule 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

通过 Windows 防火墙控制流量的规则。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|规则的显示名称。 不需要是唯一的。|
|说明|String|规则的说明。|
|packageFamilyName|String|受防火墙规则影响的 Microsoft Store 应用程序的程序包系列名称。|
|路径|String|受防火墙规则影响的应用程序的完整文件路径。|
|serviceName|String|当服务 (而不是应用程序) 发送或接收通信时使用的名称。|
|协议|Int32|0-255 表示 IP 协议 (TCP = 6, UDP = 17) 的数字。 如果未指定, 则默认值为 All。 有效值为0至255|
|localPortRanges|String collection|本地端口范围的列表。 例如, "100-120", "200", "300-320"。 如果未指定, 则默认值为 All。|
|remotePortRanges|String collection|远程端口范围的列表。 例如, "100-120", "200", "300-320"。 如果未指定, 则默认值为 All。|
|localAddressRanges|String collection|规则所涵盖的本地地址的列表。 有效令牌包括:
- "*" 表示任何本地地址。 如果存在此标记, 则必须是包含的唯一标记。
- 可以使用子网掩码或网络前缀表示法指定子网。 如果不指定子网掩码和网络前缀, 则子网掩码默认为255.255.255.255。
- 有效的 IPv6 地址。
- 不包含空格的 IPv4 地址范围, 格式为 "起始地址-结束地址"。
- 不包含空格的 IPv6 地址范围, 格式为 "起始地址-结束地址"。
默认值为任意地址。 || remoteAddressRanges |字符串集合 |指定规则所涵盖的远程地址的令牌列表。 标记不区分大小写。 有效令牌包括:
- "*" 表示任何远程地址。 如果存在此标记, 则必须是包含的唯一标记。
- "Defaultgateway"
- ldhcp
- dn
- 首选
- "Intranet" (在 Windows 版本 1809 + 上受支持)
- "RmtIntranet" (在 Windows 版本 1809 + 上受支持)
- "Internet" (在 Windows 版本 1809 + 上受支持)
- "Ply2Renders" (在 Windows 版本 1809 + 上受支持)
- "LocalSubnet" 指示本地子网上的任何本地地址。
- 可以使用子网掩码或网络前缀表示法指定子网。 如果不指定子网掩码和网络前缀, 则子网掩码默认为255.255.255.255。
- 有效的 IPv6 地址。
- 不包含空格的 IPv4 地址范围, 格式为 "起始地址-结束地址"。
- 不包含空格的 IPv6 地址范围, 格式为 "起始地址-结束地址"。
默认值为任意地址。 || profileTypes |[windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)|指定规则所属的配置文件。 如果未指定, 则默认值为 All。 可能的值为`notConfigured`: `domain`、 `private`、 `public`、。 || 操作 |[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|规则强制执行的操作。 如果未指定, 则允许使用默认值。 可能的值为`notConfigured`: `blocked`、 `allowed`、。 || trafficDirection |[windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)|启用了规则的流量方向。 如果未指定, 则默认值为 Out。可能的值为`notConfigured`: `out`、 `in`、。 || interfaceTypes |[windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)|规则的接口类型。 可能的值为`notConfigured`: `remoteAccess`、 `wireless`、 `lan`、。 || localUserAuthorizations |String |指定应用程序容器的授权本地用户的列表。 这是安全描述符定义语言 (SDDL) 格式的字符串。 |

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
  "localUserAuthorizations": "String"
}
```





