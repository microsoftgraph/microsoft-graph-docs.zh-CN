---
title: windowsFirewallNetworkProfile 资源类型
description: Windows 防火墙配置文件策略。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6bab7f12749d0467ac6435be23ee7a49dac89af6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58802486"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>windowsFirewallNetworkProfile 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 防火墙配置文件策略。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|配置主机设备以允许或阻止网络配置文件的防火墙和高级安全实施。 可取值为：`notConfigured`、`blocked`、`allowed`。|
|quiredModeRequired|Boolean|允许服务器在隐藏模式下运行。 当为 True 时，如果一个为 True，则使用一个表示为"为"的"为"。如果为"一个"，则"将具有优先级"。如果为"完成"，则使用"完成"模式时，如果为"完成"，则使用"确定"。|
|stealthModeBlocked|布尔值|阻止服务器在隐藏模式下运行。 当为 True 时，如果一个为 True，则使用一个表示为"为"的"为"。如果为"一个"，则"将具有优先级"。如果为"完成"，则使用"完成"模式时，如果为"完成"，则使用"确定"。|
|incomingTrafficRequired|Boolean|配置防火墙以允许传入流量符合其他策略设置。 当 IncomingTrafficRequired 和 IncomingTrafficBlocked 都为 true 时，IncomingTrafficBlocked 优先。|
|incomingTrafficBlocked|布尔值|配置防火墙以阻止所有传入流量，而不考虑其他策略设置。 当 IncomingTrafficRequired 和 IncomingTrafficBlocked 都为 true 时，IncomingTrafficBlocked 优先。|
|unicastResponsesToMulticastBroadcastsRequired|Boolean|配置防火墙以允许单播响应多播广播流量。 当 UnicastResponsesToMulticastBroadcastsRequired 和 UnicastResponsesToMulticastBroadcastsBlocked 都为 true 时，UnicastResponsesToMulticastBroadcastsBlocked 将优先。|
|unicastResponsesToMulticastBroadcastsBlocked|布尔值|配置防火墙以阻止对多播广播流量的单播响应。 当 UnicastResponsesToMulticastBroadcastsRequired 和 UnicastResponsesToMulticastBroadcastsBlocked 都为 true 时，UnicastResponsesToMulticastBroadcastsBlocked 将优先。|
|inboundNotificationsRequired|Boolean|允许防火墙在阻止应用程序侦听端口时显示通知。 当 InboundNotificationsRequired 和 InboundNotificationsBlocked 都为 true 时，InboundNotificationsBlocked 优先。|
|inboundNotificationsBlocked|布尔值|阻止应用程序在端口上侦听时，阻止防火墙显示通知。 当 InboundNotificationsRequired 和 InboundNotificationsBlocked 都为 true 时，InboundNotificationsBlocked 优先。|
|authorizedApplicationRulesFromGroupPolicyMerged|布尔值|配置防火墙以将组策略中的授权应用程序规则与本地存储合并，而不是忽略本地存储规则。 当 AuthorizedApplicationRulesFromGroupPolicyNotMerged 和 AuthorizedApplicationRulesFromGroupPolicyMerged 都为 true 时，AuthorizedApplicationRulesFromGroupPolicyMerged 将优先。|
|authorizedApplicationRulesFromGroupPolicyNotMerged|布尔值|配置防火墙以防止将组策略中的授权应用程序规则与本地存储合并，而不是忽略本地存储规则。 当 AuthorizedApplicationRulesFromGroupPolicyNotMerged 和 AuthorizedApplicationRulesFromGroupPolicyMerged 都为 true 时，AuthorizedApplicationRulesFromGroupPolicyMerged 将优先。|
|globalPortRulesFromGroupPolicyMerged|布尔值|配置防火墙以将组策略中的全局端口规则与本地存储中的端口规则合并，而不是忽略本地存储规则。 当 GlobalPortRulesFromGroupPolicyNotMerged 和 GlobalPortRulesFromGroupPolicyMerged 都为 true 时，GlobalPortRulesFromGroupPolicyMerged 将具有优先级。|
|globalPortRulesFromGroupPolicyNotMerged|Boolean|配置防火墙以防止将组策略中的全局端口规则与本地存储中的端口规则合并，而不是忽略本地存储规则。 当 GlobalPortRulesFromGroupPolicyNotMerged 和 GlobalPortRulesFromGroupPolicyMerged 都为 true 时，GlobalPortRulesFromGroupPolicyMerged 将具有优先级。|
|connectionSecurityRulesFromGroupPolicyMerged|布尔值|配置防火墙以将组策略中的连接安全规则与本地存储中的连接安全规则合并，而不是忽略本地存储规则。 当 ConnectionSecurityRulesFromGroupPolicyNotMerged 和 ConnectionSecurityRulesFromGroupPolicyMerged 都为 true 时，ConnectionSecurityRulesFromGroupPolicyMerged 将优先。|
|connectionSecurityRulesFromGroupPolicyNotMerged|布尔值|配置防火墙以防止将组策略中的连接安全规则与本地存储中的连接安全规则合并，而不是忽略本地存储规则。 当 ConnectionSecurityRulesFromGroupPolicyNotMerged 和 ConnectionSecurityRulesFromGroupPolicyMerged 都为 true 时，ConnectionSecurityRulesFromGroupPolicyMerged 将优先。|
|outboundConnectionsRequired|布尔值|配置防火墙以默认允许所有传出连接。 当 OutboundConnectionsRequired 和 OutboundConnectionsBlocked 都为 true 时，OutboundConnectionsBlocked 优先。 此设置将应用于 Windows版本 1809 及以上版本。|
|outboundConnectionsBlocked|布尔值|默认情况下，配置防火墙以阻止所有传出连接。 当 OutboundConnectionsRequired 和 OutboundConnectionsBlocked 都为 true 时，OutboundConnectionsBlocked 优先。 此设置将应用于 Windows版本 1809 及以上版本。|
|inboundConnectionsRequired|布尔值|配置防火墙以默认允许所有传入连接。 当 InboundConnectionsRequired 和 InboundConnectionsBlocked 都为 true 时，InboundConnectionsBlocked 优先。|
|inboundConnectionsBlocked|布尔值|将防火墙配置为默认情况下阻止所有传入连接。 当 InboundConnectionsRequired 和 InboundConnectionsBlocked 都为 true 时，InboundConnectionsBlocked 优先。|
|securedPacketExemptionAllowed|布尔值|配置防火墙以允许主计算机响应该流量的未经请求的网络流量，即使将"用户"模式Blocked 设置为 true 也是如此。 当 SecuredPacketExemptionBlocked 和 SecuredPacketExemptionAllowed 都为 true 时，SecuredPacketExemptionAllowed 优先。|
|securedPacketExemptionBlocked|Boolean|配置防火墙以阻止主计算机响应该通信的未经请求的网络流量，即使将"系统锁定"设置为 true，IPSec 也保护此通信。 当 SecuredPacketExemptionBlocked 和 SecuredPacketExemptionAllowed 都为 true 时，SecuredPacketExemptionAllowed 优先。|
|policyRulesFromGroupPolicyMerged|布尔值|配置防火墙以将组策略中的防火墙规则策略与本地存储中的防火墙规则合并，而不是忽略本地存储规则。 当 PolicyRulesFromGroupPolicyNotMerged 和 PolicyRulesFromGroupPolicyMerged 都为 true 时，PolicyRulesFromGroupPolicyMerged 将优先。|
|policyRulesFromGroupPolicyNotMerged|Boolean|配置防火墙以防止将组策略中的防火墙规则策略与本地存储中的策略合并，而不是忽略本地存储规则。 当 PolicyRulesFromGroupPolicyNotMerged 和 PolicyRulesFromGroupPolicyMerged 都为 true 时，PolicyRulesFromGroupPolicyMerged 将优先。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallNetworkProfile",
  "firewallEnabled": "String",
  "stealthModeRequired": true,
  "stealthModeBlocked": true,
  "incomingTrafficRequired": true,
  "incomingTrafficBlocked": true,
  "unicastResponsesToMulticastBroadcastsRequired": true,
  "unicastResponsesToMulticastBroadcastsBlocked": true,
  "inboundNotificationsRequired": true,
  "inboundNotificationsBlocked": true,
  "authorizedApplicationRulesFromGroupPolicyMerged": true,
  "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
  "globalPortRulesFromGroupPolicyMerged": true,
  "globalPortRulesFromGroupPolicyNotMerged": true,
  "connectionSecurityRulesFromGroupPolicyMerged": true,
  "connectionSecurityRulesFromGroupPolicyNotMerged": true,
  "outboundConnectionsRequired": true,
  "outboundConnectionsBlocked": true,
  "inboundConnectionsRequired": true,
  "inboundConnectionsBlocked": true,
  "securedPacketExemptionAllowed": true,
  "securedPacketExemptionBlocked": true,
  "policyRulesFromGroupPolicyMerged": true,
  "policyRulesFromGroupPolicyNotMerged": true
}
```



