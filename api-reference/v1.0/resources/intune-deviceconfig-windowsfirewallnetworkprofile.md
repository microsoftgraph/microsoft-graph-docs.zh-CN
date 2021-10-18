---
title: windowsFirewallNetworkProfile 资源类型
description: Windows 防火墙配置文件策略。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 27e38c473a8f37b35a74dd29872607428dddd042
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60455216"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>windowsFirewallNetworkProfile 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 防火墙配置文件策略。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|配置主机设备以允许或阻止网络配置文件的防火墙和高级安全实施。 可取值为：`notConfigured`、`blocked`、`allowed`。|
|stealthModeBlocked|布尔值|阻止服务器在隐藏模式下运行。 当为 True 时，如果一个为 True，则使用一个表示为"为"的"为"。如果为"一个"，则"将具有优先级"。如果为"完成"，则使用"完成"模式时，如果为"完成"，则使用"确定"。|
|incomingTrafficBlocked|布尔值|配置防火墙以阻止所有传入流量，而不考虑其他策略设置。 当 IncomingTrafficRequired 和 IncomingTrafficBlocked 都为 true 时，IncomingTrafficBlocked 优先。|
|unicastResponsesToMulticastBroadcastsBlocked|布尔值|配置防火墙以阻止对多播广播流量的单播响应。 当 UnicastResponsesToMulticastBroadcastsRequired 和 UnicastResponsesToMulticastBroadcastsBlocked 都为 true 时，UnicastResponsesToMulticastBroadcastsBlocked 将优先。|
|inboundNotificationsBlocked|布尔值|阻止应用程序在端口上侦听时，阻止防火墙显示通知。 当 InboundNotificationsRequired 和 InboundNotificationsBlocked 都为 true 时，InboundNotificationsBlocked 优先。|
|authorizedApplicationRulesFromGroupPolicyMerged|布尔值|配置防火墙以将组策略中的授权应用程序规则与本地存储合并，而不是忽略本地存储规则。 当 AuthorizedApplicationRulesFromGroupPolicyNotMerged 和 AuthorizedApplicationRulesFromGroupPolicyMerged 都为 true 时，AuthorizedApplicationRulesFromGroupPolicyMerged 将优先。|
|globalPortRulesFromGroupPolicyMerged|布尔值|配置防火墙以将组策略中的全局端口规则与本地存储中的端口规则合并，而不是忽略本地存储规则。 当 GlobalPortRulesFromGroupPolicyNotMerged 和 GlobalPortRulesFromGroupPolicyMerged 都为 true 时，GlobalPortRulesFromGroupPolicyMerged 将具有优先级。|
|connectionSecurityRulesFromGroupPolicyMerged|布尔值|配置防火墙以将组策略中的连接安全规则与本地存储中的连接安全规则合并，而不是忽略本地存储规则。 当 ConnectionSecurityRulesFromGroupPolicyNotMerged 和 ConnectionSecurityRulesFromGroupPolicyMerged 都为 true 时，ConnectionSecurityRulesFromGroupPolicyMerged 将优先。|
|outboundConnectionsBlocked|布尔值|默认情况下，配置防火墙以阻止所有传出连接。 当 OutboundConnectionsRequired 和 OutboundConnectionsBlocked 都为 true 时，OutboundConnectionsBlocked 优先。 此设置将应用于 1809 Windows版本 1809 及以上的版本。|
|inboundConnectionsBlocked|布尔值|将防火墙配置为默认情况下阻止所有传入连接。 当 InboundConnectionsRequired 和 InboundConnectionsBlocked 都为 true 时，InboundConnectionsBlocked 优先。|
|securedPacketExemptionAllowed|布尔值|配置防火墙以允许主计算机响应该流量的未经请求的网络流量，即使将"用户"模式Blocked 设置为 true 也是如此。 当 SecuredPacketExemptionBlocked 和 SecuredPacketExemptionAllowed 都为 true 时，SecuredPacketExemptionAllowed 优先。|
|policyRulesFromGroupPolicyMerged|布尔值|配置防火墙以将组策略中的防火墙规则策略与本地存储中的防火墙规则合并，而不是忽略本地存储规则。 当 PolicyRulesFromGroupPolicyNotMerged 和 PolicyRulesFromGroupPolicyMerged 都为 true 时，PolicyRulesFromGroupPolicyMerged 将优先。|

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
  "stealthModeBlocked": true,
  "incomingTrafficBlocked": true,
  "unicastResponsesToMulticastBroadcastsBlocked": true,
  "inboundNotificationsBlocked": true,
  "authorizedApplicationRulesFromGroupPolicyMerged": true,
  "globalPortRulesFromGroupPolicyMerged": true,
  "connectionSecurityRulesFromGroupPolicyMerged": true,
  "outboundConnectionsBlocked": true,
  "inboundConnectionsBlocked": true,
  "securedPacketExemptionAllowed": true,
  "policyRulesFromGroupPolicyMerged": true
}
```



