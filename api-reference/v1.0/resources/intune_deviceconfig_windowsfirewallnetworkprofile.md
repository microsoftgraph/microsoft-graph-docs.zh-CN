# <a name="windowsfirewallnetworkprofile-resource-type"></a>windowsFirewallNetworkProfile 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Windows 防火墙配置文件策略。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|配置主机设备，以允许或阻止针对网络配置文件的防火墙和高级安全措施的实施。 可取值为：`notConfigured`、`blocked`、`allowed`。|
|stealthModeBlocked|布尔值|防止服务器在隐藏模式下运行。 当 StealthModeRequired 和 StealthModeBlocked 均为 true时，则 StealthModeBlocked 优先。|
|incomingTrafficBlocked|布尔值|配置防火墙以阻止所有传入通信，无论其他策略设置为何。 当 IncomingTrafficRequired 和 IncomingTrafficBlocked 均为 true时，则 IncomingTrafficBlocked 优先。|
|unicastResponsesToMulticastBroadcastsBlocked|布尔值|配置防火墙以阻止对多播广播通信的单播响应。 当 UnicastResponsesToMulticastBroadcastsRequired 和 UnicastResponsesToMulticastBroadcastsBlocked 均为 true时，则 UnicastResponsesToMulticastBroadcastsBlocked 优先。|
|inboundNotificationsBlocked|布尔值|防止防火墙在应用程序受阻无法在端口侦听时显示通知。 当 InboundNotificationsRequired 和 InboundNotificationsBlocked 均为 true时，则 InboundNotificationsBlocked 优先。|
|authorizedApplicationRulesFromGroupPolicyMerged|布尔值|配置防火墙，将组策略中的授权应用程序规则与本地存储的规则合并，而不是忽略本地存储规则 当 AuthorizedApplicationRulesFromGroupPolicyNotMerged 和 AuthorizedApplicationRulesFromGroupPolicyMerged 均为 true时，则 AuthorizedApplicationRulesFromGroupPolicyMerged 优先。|
|globalPortRulesFromGroupPolicyMerged|布尔值|配置防火墙，将组策略中的全局端口规则与本地存储规则合并，而不是忽略本地存储规则。 当 GlobalPortRulesFromGroupPolicyNotMerged 和 GlobalPortRulesFromGroupPolicyMerged 均为 true，则 GlobalPortRulesFromGroupPolicyMerged 优先。|
|connectionSecurityRulesFromGroupPolicyMerged|布尔值|配置防火墙，将组策略中的连接安全规则与本地存储规则合并，而不是忽略本地存储规则。 当 ConnectionSecurityRulesFromGroupPolicyNotMerged 和 ConnectionSecurityRulesFromGroupPolicyMerged 均为 true时，则 ConnectionSecurityRulesFromGroupPolicyMerged 优先。|
|outboundConnectionsBlocked|布尔值|配置防火墙，在默认情况下阻止所有传出连接。 当 OutboundConnectionsRequired 和 OutboundConnectionsBlocked 均为 true时，则 OutboundConnectionsBlocked 优先。|
|inboundConnectionsBlocked|布尔值|配置防火墙，在默认情况下阻止所有传入连接。 当 InboundConnectionsRequired 和 InboundConnectionsBlocked 均为 true时，则 InboundConnectionsBlocked 优先。|
|securedPacketExemptionAllowed|布尔值|配置防火墙，允许主机计算机响应未经请求的网络通信（如果该通信受 IPSec 保护），即使 stealthModeBlocked 设置为 true。 当 SecuredPacketExemptionBlocked 和 SecuredPacketExemptionAllowed 均为 true时，则 SecuredPacketExemptionAllowed 优先。|
|policyRulesFromGroupPolicyMerged|布尔值|配置防火墙，将组策略中的防火墙规则与本地存储规则合并，而不是忽略本地存储规则。 当 PolicyRulesFromGroupPolicyNotMerged 和 PolicyRulesFromGroupPolicyMerged 均为 true时，则 PolicyRulesFromGroupPolicyMerged 优先。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile"
}-->
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








