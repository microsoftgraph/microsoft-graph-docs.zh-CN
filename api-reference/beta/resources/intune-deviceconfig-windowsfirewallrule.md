---
title: windowsFirewallRule 资源类型
description: 通过 Windows 防火墙控制流量的规则。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b0576c68ad1db2153d085349037db3beaafe8237
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525556"
---
# <a name="windowsfirewallrule-resource-type"></a>windowsFirewallRule 资源类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

通过 Windows 防火墙控制流量的规则。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|规则的显示名称。 不需要是唯一的。|
|说明|String|规则的说明。|
|packageFamilyName|String|受防火墙规则影响的 Microsoft Store 应用程序的程序包系列名称。|
|路径|String|受防火墙规则影响的应用程序的完整文件路径。|
|serviceName|String|当服务（而不是应用程序）发送或接收通信时使用的名称。|
|协议|Int32|0-255 表示 IP 协议（TCP = 6，UDP = 17）的数字。 如果未指定，则默认值为 All。 有效值为0至255|
|localPortRanges|String 集合|本地端口范围的列表。 例如，"100-120"，"200"，"300-320"。 如果未指定，则默认值为 All。|
|remotePortRanges|String 集合|远程端口范围的列表。 例如，"100-120"，"200"，"300-320"。 如果未指定，则默认值为 All。|
|localAddressRanges|String 集合|规则所涵盖的本地地址的列表。 默认值为任意地址。 有效令牌包括：<ul><li>"*" 表示任何本地地址。 如果存在此标记，则必须是包含的唯一标记。</li><li>可以使用子网掩码或网络前缀表示法指定子网。 如果不指定子网掩码和网络前缀，则子网掩码默认为255.255.255.255。</li><li>有效的 IPv6 地址。</li><li>不包含空格的 IPv4 地址范围，格式为 "起始地址-结束地址"。</li><li>不包含空格的 IPv6 地址范围，格式为 "起始地址-结束地址"。</li></ul>|
|remoteAddressRanges|String 集合|指定规则所涵盖的远程地址的令牌列表。 标记不区分大小写。 默认值为任意地址。 有效令牌包括：<ul><li>"*" 表示任何远程地址。 如果存在此标记，则必须是包含的唯一标记。</li><li>"Defaultgateway"</li><li>LDHCP</li><li>DN</li><li>首选</li><li>"Intranet" （在 Windows 版本 1809 + 上受支持）</li><li>"RmtIntranet" （在 Windows 版本 1809 + 上受支持）</li><li>"Internet" （在 Windows 版本 1809 + 上受支持）</li><li>"Ply2Renders" （在 Windows 版本 1809 + 上受支持）</li><li>"LocalSubnet" 指示本地子网上的任何本地地址。</li><li>可以使用子网掩码或网络前缀表示法指定子网。 如果不指定子网掩码和网络前缀，则子网掩码默认为255.255.255.255。</li><li>有效的 IPv6 地址。</li><li>不包含空格的 IPv4 地址范围，格式为 "起始地址-结束地址"。</li><li>不包含空格的 IPv6 地址范围，格式为 "起始地址-结束地址"。</li></ul>|
|profileTypes|[windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)|指定规则所属的配置文件。 如果未指定，则默认值为 All。 可取值为：`notConfigured`、`domain`、`private`、`public`。|
|action|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|规则强制执行的操作。 如果未指定，则允许使用默认值。 可取值为：`notConfigured`、`blocked`、`allowed`。|
|trafficDirection|[windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)|启用了规则的流量方向。 如果未指定，则默认值为 Out。可能的值为`notConfigured`： `out`、 `in`、。|
|interfaceTypes|[windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)|规则的接口类型。 可取值为：`notConfigured`、`remoteAccess`、`wireless`、`lan`。|
|edgeTraversal|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|指示是否为此规则启用或禁用边缘遍历。 EdgeTraversal 设置指示允许特定入站流量通过 Nat 和使用 Teredo 隧道技术的其他边缘设备进行隧道传递。 为了使此设置正常工作，具有入站防火墙规则的应用程序或服务需要支持 IPv6。 此设置的主应用程序允许主机上的侦听器通过 Teredo IPv6 地址进行全局寻址。 默认情况下，新规则已禁用 EdgeTraversal 属性。 可取值为：`notConfigured`、`blocked`、`allowed`。|
|localUserAuthorizations|String|指定应用程序容器的授权本地用户的列表。 这是安全描述符定义语言（SDDL）格式的字符串。|

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



