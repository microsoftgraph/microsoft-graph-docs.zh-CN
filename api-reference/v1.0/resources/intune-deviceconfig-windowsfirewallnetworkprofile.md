---
title: windowsFirewallNetworkProfile 资源类型
description: Windows 防火墙配置文件策略。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e30f01031d46babf066b6778edf7801de7eac46c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917957"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>windowsFirewallNetworkProfile 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Windows 防火墙配置文件策略。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|配置主机设备，以允许或阻止的防火墙和高级的安全实施的网络配置文件。 可取值为：`notConfigured`、`blocked`、`allowed`。|
|stealthModeBlocked|布尔值|防止服务器操作系统中隐藏模式。 当 StealthModeRequired 和 StealthModeBlocked 均为 true，则 StealthModeBlocked 优先。|
|incomingTrafficBlocked|布尔值|配置防火墙以阻止所有传入通信，无论其他策略设置。 当 IncomingTrafficRequired 和 IncomingTrafficBlocked 均为 true，则 IncomingTrafficBlocked 优先。|
|unicastResponsesToMulticastBroadcastsBlocked|布尔值|配置为阻止单播 エ ・ 复 ハ 多播广播通信防火墙。 当 UnicastResponsesToMulticastBroadcastsRequired 和 UnicastResponsesToMulticastBroadcastsBlocked 均为 true，则 UnicastResponsesToMulticastBroadcastsBlocked 优先。|
|inboundNotificationsBlocked|布尔值|防止防火墙阻止侦听端口应用程序时显示通知。 当 InboundNotificationsRequired 和 InboundNotificationsBlocked 均为 true，则 InboundNotificationsBlocked 优先。|
|authorizedApplicationRulesFromGroupPolicyMerged|布尔值|配置防火墙合并与从本地存储而不是忽略的本地存储规则组策略中的授权的应用程序规则。 当 AuthorizedApplicationRulesFromGroupPolicyNotMerged 和 AuthorizedApplicationRulesFromGroupPolicyMerged 均为 true，则 AuthorizedApplicationRulesFromGroupPolicyMerged 优先。|
|globalPortRulesFromGroupPolicyMerged|布尔值|配置防火墙合并与从本地存储而不是忽略的本地存储规则组策略中的全局端口规则。 当 GlobalPortRulesFromGroupPolicyNotMerged 和 GlobalPortRulesFromGroupPolicyMerged 均为 true，则 GlobalPortRulesFromGroupPolicyMerged 优先。|
|connectionSecurityRulesFromGroupPolicyMerged|布尔值|配置防火墙合并与从本地存储而不是忽略的本地存储规则的组策略中的连接安全规则。 当 ConnectionSecurityRulesFromGroupPolicyNotMerged 和 ConnectionSecurityRulesFromGroupPolicyMerged 均为 true，则 ConnectionSecurityRulesFromGroupPolicyMerged 优先。|
|outboundConnectionsBlocked|布尔值|配置防火墙以阻止默认情况下所有传出连接。 当 OutboundConnectionsRequired 和 OutboundConnectionsBlocked 均为 true，则 OutboundConnectionsBlocked 优先。|
|inboundConnectionsBlocked|布尔值|配置防火墙以阻止默认情况下的所有传入连接。 当 InboundConnectionsRequired 和 InboundConnectionsBlocked 均为 true，则 InboundConnectionsBlocked 优先。|
|securedPacketExemptionAllowed|布尔值|配置防火墙以允许主机计算机响应的未经请求的网络通信，即使设置 stealthModeBlocked ipsec 保护通信为 true。 当 SecuredPacketExemptionBlocked 和 SecuredPacketExemptionAllowed 均为 true，则 SecuredPacketExemptionAllowed 优先。|
|policyRulesFromGroupPolicyMerged|布尔值|配置防火墙合并与从本地存储而不是忽略的本地存储规则的防火墙规则策略组策略中。 当 PolicyRulesFromGroupPolicyNotMerged 和 PolicyRulesFromGroupPolicyMerged 均为 true，则 PolicyRulesFromGroupPolicyMerged 优先。|

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



