---
title: windowsFirewallNetworkProfile 资源类型
description: Windows 防火墙配置文件策略。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9ed6011844daedc5fe4140b04851605529921c99
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66729998"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>windowsFirewallNetworkProfile 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 防火墙配置文件策略。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|将主机设备配置为允许或阻止防火墙和高级安全强制网络配置文件。 可取值为：`notConfigured`、`blocked`、`allowed`。|
|stealthModeBlocked|布尔值|阻止服务器在隐身模式下运行。 当 StealthModeRequired 和 StealthModeBlocked 均为 true 时，StealthModeBlocked 优先。|
|incomingTrafficBlocked|布尔值|将防火墙配置为阻止所有传入流量，而不考虑其他策略设置。 当 IncomingTrafficRequired 和 IncomingTrafficBlocked 均为 true 时，IncomingTrafficBlocked 优先级。|
|unicastResponsesToMulticastBroadcastsBlocked|布尔值|将防火墙配置为阻止对多播广播流量的单播响应。 当 UnicastResponsesToMulticastBroadcastsRequired 和 UnicastResponsesToMulticastBroadcastsBlocked 均为 true 时，UnicastResponsesToMulticastBroadcastsBlocked 优先。|
|inboundNotificationsBlocked|布尔值|当阻止应用程序侦听端口时，防止防火墙显示通知。 当 InboundNotificationsRequired 和 InboundNotificationsBlocked 均为 true 时，InboundNotificationsBlocked 优先级。|
|authorizedApplicationRulesFromGroupPolicyMerged|布尔值|将防火墙配置为将组策略中的授权应用程序规则与本地存储中的授权应用程序规则合并，而不是忽略本地存储规则。 当 AuthorizedApplicationRulesFromGroupPolicyNotMerged 和 AuthorizedApplicationRulesFromGroupPolicyMerged 均为 true 时，AuthorizedApplicationRulesFromGroupPolicyMerged 将优先处理。|
|globalPortRulesFromGroupPolicyMerged|布尔值|将防火墙配置为将组策略中的全局端口规则与本地存储中的全局端口规则合并，而不是忽略本地存储规则。 当 GlobalPortRulesFromGroupPolicyNotMerged 和 GlobalPortRulesFromGroupPolicyMerged 均为 true 时，GlobalPortRulesFromGroupPolicyMerged 优先。|
|connectionSecurityRulesFromGroupPolicyMerged|布尔值|将防火墙配置为将组策略中的连接安全规则与本地存储中的连接安全规则合并，而不是忽略本地存储规则。 当 ConnectionSecurityRulesFromGroupPolicyNotMerged 和 ConnectionSecurityRulesFromGroupPolicyMerged 均为 true 时，ConnectionSecurityRulesFromGroupPolicyMerged 将优先执行。|
|outboundConnectionsBlocked|布尔值|默认情况下，将防火墙配置为阻止所有传出连接。 当 OutboundConnectionsRequired 和 OutboundConnectionsBlocked 均为 true 时，OutboundConnectionsBlocked 将优先执行。 此设置将应用于 Windows 版本 1809 及更高版本。|
|inboundConnectionsBlocked|布尔值|默认情况下，将防火墙配置为阻止所有传入连接。 当 InboundConnectionsRequired 和 InboundConnectionsBlocked 均为 true 时，InboundConnectionsBlocked 优先级。|
|securedPacketExemptionAllowed|布尔值|将防火墙配置为允许主机响应未经请求的网络流量，即使将 stealthModeBlocked 设置为 true，IPSec 也可保护该流量。 当 SecuredPacketExemptionBlocked 和 SecuredPacketExemptionAllowed 均为 true 时，SecuredPacketExemptionAllowed 优先处理。|
|policyRulesFromGroupPolicyMerged|布尔值|将防火墙配置为将组策略中的防火墙规则策略与本地存储中的策略合并，而不是忽略本地存储规则。 当 PolicyRulesFromGroupPolicyNotMerged 和 PolicyRulesFromGroupPolicyMerged 均为 true 时，PolicyRulesFromGroupPolicyMerged 将优先级。|

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





