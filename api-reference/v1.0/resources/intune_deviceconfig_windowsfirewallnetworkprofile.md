# <a name="windowsfirewallnetworkprofile-resource-type"></a>windowsFirewallNetworkProfile 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Windows 防火墙配置文件策略。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|打开防火墙和高级的安全实施。 可取值为：`notConfigured`、`blocked`、`allowed`。|
|stealthModeBlocked|布尔值|防止服务器在隐藏模式下运行|
|incomingTrafficBlocked|布尔值|配置防火墙以阻止所有传入通信，无论其他策略设置为何|
|unicastResponsesToMulticastBroadcastsBlocked|布尔值|配置防火墙以阻止对多播广播通信的单播响应|
|inboundNotificationsBlocked|布尔值|阻止应用程序在端口上侦听时，避免防火墙显示通知|
|authorizedApplicationRulesFromGroupPolicyMerged|布尔值|配置防火墙，将组策略中的授权应用程序规则与本地存储合并，而不是忽略本地存储规则|
|globalPortRulesFromGroupPolicyMerged|布尔值|配置防火墙，将组策略中的全局端口规则与本地存储合并，而不是忽略本地存储规则|
|connectionSecurityRulesFromGroupPolicyMerged|布尔值|配置防火墙，将组策略中的连接安全规则与本地存储合并，而不是忽略本地存储规则|
|outboundConnectionsBlocked|布尔值|配置防火墙，在默认情况下阻止所有传出连接|
|inboundConnectionsBlocked|布尔值|配置防火墙，在默认情况下阻止所有传入连接|
|securedPacketExemptionAllowed|布尔值|配置防火墙，允许主机计算机响应未经请求的网络通信（如果该通信受 IPSec 保护），即使 stealthModeBlocked 设置为 true|
|policyRulesFromGroupPolicyMerged|布尔值|配置防火墙，将组策略中的防火墙规则与本地存储合并，而不是忽略本地存储规则|

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



