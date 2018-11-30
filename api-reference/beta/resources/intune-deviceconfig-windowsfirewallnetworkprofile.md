---
title: windowsFirewallNetworkProfile 资源类型
description: Windows 防火墙配置文件策略。
ms.openlocfilehash: eb27eefb636abfa274cd018a637ccc364ef227c9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045434"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>windowsFirewallNetworkProfile 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Windows 防火墙配置文件策略。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|配置主机设备，以允许或阻止的防火墙和高级的安全实施的网络配置文件。 可取值为：`notConfigured`、`blocked`、`allowed`。|
|stealthModeRequired|布尔|允许服务器在隐藏模式下运行。 当 StealthModeRequired 和 StealthModeBlocked 均为 true，则 StealthModeBlocked 优先。|
|stealthModeBlocked|布尔值|防止服务器操作系统中隐藏模式。 当 StealthModeRequired 和 StealthModeBlocked 均为 true，则 StealthModeBlocked 优先。|
|incomingTrafficRequired|布尔|配置防火墙以允许传入通信的保密协议其他策略设置。 当 IncomingTrafficRequired 和 IncomingTrafficBlocked 均为 true，则 IncomingTrafficBlocked 优先。|
|incomingTrafficBlocked|布尔值|配置防火墙以阻止所有传入通信，无论其他策略设置。 当 IncomingTrafficRequired 和 IncomingTrafficBlocked 均为 true，则 IncomingTrafficBlocked 优先。|
|unicastResponsesToMulticastBroadcastsRequired|布尔|配置防火墙以允许单播 エ ・ 复 ハ 多播广播通信。 当 UnicastResponsesToMulticastBroadcastsRequired 和 UnicastResponsesToMulticastBroadcastsBlocked 均为 true，则 UnicastResponsesToMulticastBroadcastsBlocked 优先。|
|unicastResponsesToMulticastBroadcastsBlocked|布尔值|配置为阻止单播 エ ・ 复 ハ 多播广播通信防火墙。 当 UnicastResponsesToMulticastBroadcastsRequired 和 UnicastResponsesToMulticastBroadcastsBlocked 均为 true，则 UnicastResponsesToMulticastBroadcastsBlocked 优先。|
|inboundNotificationsRequired|布尔|允许防火墙以阻止侦听端口应用程序时显示通知。 当 InboundNotificationsRequired 和 InboundNotificationsBlocked 均为 true，则 InboundNotificationsBlocked 优先。|
|inboundNotificationsBlocked|布尔值|防止防火墙阻止侦听端口应用程序时显示通知。 当 InboundNotificationsRequired 和 InboundNotificationsBlocked 均为 true，则 InboundNotificationsBlocked 优先。|
|authorizedApplicationRulesFromGroupPolicyMerged|布尔值|配置防火墙合并与从本地存储而不是忽略的本地存储规则组策略中的授权的应用程序规则。 当 AuthorizedApplicationRulesFromGroupPolicyNotMerged 和 AuthorizedApplicationRulesFromGroupPolicyMerged 均为 true，则 AuthorizedApplicationRulesFromGroupPolicyMerged 优先。|
|authorizedApplicationRulesFromGroupPolicyNotMerged|布尔|配置防火墙以阻止合并授权应用程序与从本地存储而不是忽略本地组策略中的规则存储规则。 当 AuthorizedApplicationRulesFromGroupPolicyNotMerged 和 AuthorizedApplicationRulesFromGroupPolicyMerged 均为 true，则 AuthorizedApplicationRulesFromGroupPolicyMerged 优先。|
|globalPortRulesFromGroupPolicyMerged|布尔值|配置防火墙合并与从本地存储而不是忽略的本地存储规则组策略中的全局端口规则。 当 GlobalPortRulesFromGroupPolicyNotMerged 和 GlobalPortRulesFromGroupPolicyMerged 均为 true，则 GlobalPortRulesFromGroupPolicyMerged 优先。|
|globalPortRulesFromGroupPolicyNotMerged|布尔|配置防火墙以阻止合并与从本地存储而不是忽略的本地存储规则组策略中的全局端口规则。 当 GlobalPortRulesFromGroupPolicyNotMerged 和 GlobalPortRulesFromGroupPolicyMerged 均为 true，则 GlobalPortRulesFromGroupPolicyMerged 优先。|
|connectionSecurityRulesFromGroupPolicyMerged|布尔值|配置防火墙合并与从本地存储而不是忽略的本地存储规则的组策略中的连接安全规则。 当 ConnectionSecurityRulesFromGroupPolicyNotMerged 和 ConnectionSecurityRulesFromGroupPolicyMerged 均为 true，则 ConnectionSecurityRulesFromGroupPolicyMerged 优先。|
|connectionSecurityRulesFromGroupPolicyNotMerged|布尔|配置防火墙以阻止合并组策略中的连接安全规则与从本地存储而不是忽略本地存储规则。 当 ConnectionSecurityRulesFromGroupPolicyNotMerged 和 ConnectionSecurityRulesFromGroupPolicyMerged 均为 true，则 ConnectionSecurityRulesFromGroupPolicyMerged 优先。|
|outboundConnectionsRequired|布尔|配置防火墙以允许默认情况下所有传出连接。 当 OutboundConnectionsRequired 和 OutboundConnectionsBlocked 均为 true，则 OutboundConnectionsBlocked 优先。|
|outboundConnectionsBlocked|布尔值|配置防火墙以阻止默认情况下所有传出连接。 当 OutboundConnectionsRequired 和 OutboundConnectionsBlocked 均为 true，则 OutboundConnectionsBlocked 优先。|
|inboundConnectionsRequired|布尔|配置防火墙以允许默认情况下的所有传入连接。 当 InboundConnectionsRequired 和 InboundConnectionsBlocked 均为 true，则 InboundConnectionsBlocked 优先。|
|inboundConnectionsBlocked|布尔值|配置防火墙以阻止默认情况下的所有传入连接。 当 InboundConnectionsRequired 和 InboundConnectionsBlocked 均为 true，则 InboundConnectionsBlocked 优先。|
|securedPacketExemptionAllowed|布尔值|配置防火墙以允许主机计算机响应的未经请求的网络通信，即使设置 stealthModeBlocked ipsec 保护通信为 true。 当 SecuredPacketExemptionBlocked 和 SecuredPacketExemptionAllowed 均为 true，则 SecuredPacketExemptionAllowed 优先。|
|securedPacketExemptionBlocked|布尔|配置防火墙以阻止主机计算机响应的未经请求的网络通信，即使设置 stealthModeBlocked ipsec 保护通信为 true。 当 SecuredPacketExemptionBlocked 和 SecuredPacketExemptionAllowed 均为 true，则 SecuredPacketExemptionAllowed 优先。|
|policyRulesFromGroupPolicyMerged|布尔值|配置防火墙合并与从本地存储而不是忽略的本地存储规则的防火墙规则策略组策略中。 当 PolicyRulesFromGroupPolicyNotMerged 和 PolicyRulesFromGroupPolicyMerged 均为 true，则 PolicyRulesFromGroupPolicyMerged 优先。|
|policyRulesFromGroupPolicyNotMerged|布尔|配置防火墙以阻止合并防火墙规则与从本地存储而不是忽略本地组策略中的策略存储规则。 当 PolicyRulesFromGroupPolicyNotMerged 和 PolicyRulesFromGroupPolicyMerged 均为 true，则 PolicyRulesFromGroupPolicyMerged 优先。|

## <a name="relationships"></a>Relationships
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





