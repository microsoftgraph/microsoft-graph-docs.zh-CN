# <a name="windowsfirewallnetworkprofile-resource-type"></a><span data-ttu-id="0e5c4-101">windowsFirewallNetworkProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e5c4-101">windowsFirewallNetworkProfile resource type</span></span>

> <span data-ttu-id="0e5c4-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0e5c4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e5c4-103">Windows 防火墙配置文件策略。</span><span class="sxs-lookup"><span data-stu-id="0e5c4-103">Windows Firewall Profile Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="0e5c4-104">属性</span><span class="sxs-lookup"><span data-stu-id="0e5c4-104">Properties</span></span>
|<span data-ttu-id="0e5c4-105">属性</span><span class="sxs-lookup"><span data-stu-id="0e5c4-105">Property</span></span>|<span data-ttu-id="0e5c4-106">类型</span><span class="sxs-lookup"><span data-stu-id="0e5c4-106">Type</span></span>|<span data-ttu-id="0e5c4-107">说明</span><span class="sxs-lookup"><span data-stu-id="0e5c4-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e5c4-108">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="0e5c4-108">firewallEnabled</span></span>|[<span data-ttu-id="0e5c4-109">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="0e5c4-109">stateManagementSetting</span></span>](../resources/intune_deviceconfig_statemanagementsetting.md)|<span data-ttu-id="0e5c4-110">打开防火墙和高级的安全实施。</span><span class="sxs-lookup"><span data-stu-id="0e5c4-110">Turn on the firewall and advanced security enforcement Possible values are: , , .</span></span> <span data-ttu-id="0e5c4-111">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="0e5c4-111">The possible values are `notConfigured`, `blocked`, `allowed`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="0e5c4-112">stealthModeBlocked</span><span class="sxs-lookup"><span data-stu-id="0e5c4-112">stealthModeBlocked</span></span>|<span data-ttu-id="0e5c4-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="0e5c4-113">Boolean</span></span>|<span data-ttu-id="0e5c4-114">防止服务器在隐藏模式下运行</span><span class="sxs-lookup"><span data-stu-id="0e5c4-114">Prevent the server from operating in stealth mode</span></span>|
|<span data-ttu-id="0e5c4-115">incomingTrafficBlocked</span><span class="sxs-lookup"><span data-stu-id="0e5c4-115">incomingTrafficBlocked</span></span>|<span data-ttu-id="0e5c4-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="0e5c4-116">Boolean</span></span>|<span data-ttu-id="0e5c4-117">配置防火墙以阻止所有传入通信，无论其他策略设置为何</span><span class="sxs-lookup"><span data-stu-id="0e5c4-117">Configures the firewall to block all incoming traffic regardless of other policy settings</span></span>|
|<span data-ttu-id="0e5c4-118">unicastResponsesToMulticastBroadcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="0e5c4-118">unicastResponsesToMulticastBroadcastsBlocked</span></span>|<span data-ttu-id="0e5c4-119">布尔值</span><span class="sxs-lookup"><span data-stu-id="0e5c4-119">Boolean</span></span>|<span data-ttu-id="0e5c4-120">配置防火墙以阻止对多播广播通信的单播响应</span><span class="sxs-lookup"><span data-stu-id="0e5c4-120">Configures the firewall to block unicast responses to multicast broadcast traffic</span></span>|
|<span data-ttu-id="0e5c4-121">inboundNotificationsBlocked</span><span class="sxs-lookup"><span data-stu-id="0e5c4-121">inboundNotificationsBlocked</span></span>|<span data-ttu-id="0e5c4-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="0e5c4-122">Boolean</span></span>|<span data-ttu-id="0e5c4-123">阻止应用程序在端口上侦听时，避免防火墙显示通知</span><span class="sxs-lookup"><span data-stu-id="0e5c4-123">Prevents the firewall from displaying notifications when an application is blocked from listening on a port</span></span>|
|<span data-ttu-id="0e5c4-124">authorizedApplicationRulesFromGroupPolicyMerged</span><span class="sxs-lookup"><span data-stu-id="0e5c4-124">authorizedApplicationRulesFromGroupPolicyMerged</span></span>|<span data-ttu-id="0e5c4-125">布尔值</span><span class="sxs-lookup"><span data-stu-id="0e5c4-125">Boolean</span></span>|<span data-ttu-id="0e5c4-126">配置防火墙，将组策略中的授权应用程序规则与本地存储合并，而不是忽略本地存储规则</span><span class="sxs-lookup"><span data-stu-id="0e5c4-126">Configures the firewall to merge authorized application rules from group policy with those from local store instead of ignoring the local store rules</span></span>|
|<span data-ttu-id="0e5c4-127">globalPortRulesFromGroupPolicyMerged</span><span class="sxs-lookup"><span data-stu-id="0e5c4-127">globalPortRulesFromGroupPolicyMerged</span></span>|<span data-ttu-id="0e5c4-128">布尔值</span><span class="sxs-lookup"><span data-stu-id="0e5c4-128">Boolean</span></span>|<span data-ttu-id="0e5c4-129">配置防火墙，将组策略中的全局端口规则与本地存储合并，而不是忽略本地存储规则</span><span class="sxs-lookup"><span data-stu-id="0e5c4-129">Configures the firewall to merge global port rules from group policy with those from local store instead of ignoring the local store rules</span></span>|
|<span data-ttu-id="0e5c4-130">connectionSecurityRulesFromGroupPolicyMerged</span><span class="sxs-lookup"><span data-stu-id="0e5c4-130">connectionSecurityRulesFromGroupPolicyMerged</span></span>|<span data-ttu-id="0e5c4-131">布尔值</span><span class="sxs-lookup"><span data-stu-id="0e5c4-131">Boolean</span></span>|<span data-ttu-id="0e5c4-132">配置防火墙，将组策略中的连接安全规则与本地存储合并，而不是忽略本地存储规则</span><span class="sxs-lookup"><span data-stu-id="0e5c4-132">Configures the firewall to merge connection security rules from group policy with those from local store instead of ignoring the local store rules</span></span>|
|<span data-ttu-id="0e5c4-133">outboundConnectionsBlocked</span><span class="sxs-lookup"><span data-stu-id="0e5c4-133">outboundConnectionsBlocked</span></span>|<span data-ttu-id="0e5c4-134">布尔值</span><span class="sxs-lookup"><span data-stu-id="0e5c4-134">Boolean</span></span>|<span data-ttu-id="0e5c4-135">配置防火墙，在默认情况下阻止所有传出连接</span><span class="sxs-lookup"><span data-stu-id="0e5c4-135">Configures the firewall to block all outgoing connections by default</span></span>|
|<span data-ttu-id="0e5c4-136">inboundConnectionsBlocked</span><span class="sxs-lookup"><span data-stu-id="0e5c4-136">inboundConnectionsBlocked</span></span>|<span data-ttu-id="0e5c4-137">布尔值</span><span class="sxs-lookup"><span data-stu-id="0e5c4-137">Boolean</span></span>|<span data-ttu-id="0e5c4-138">配置防火墙，在默认情况下阻止所有传入连接</span><span class="sxs-lookup"><span data-stu-id="0e5c4-138">Configures the firewall to block all incoming connections by default</span></span>|
|<span data-ttu-id="0e5c4-139">securedPacketExemptionAllowed</span><span class="sxs-lookup"><span data-stu-id="0e5c4-139">securedPacketExemptionAllowed</span></span>|<span data-ttu-id="0e5c4-140">布尔值</span><span class="sxs-lookup"><span data-stu-id="0e5c4-140">Boolean</span></span>|<span data-ttu-id="0e5c4-141">配置防火墙，允许主机计算机响应未经请求的网络通信（如果该通信受 IPSec 保护），即使 stealthModeBlocked 设置为 true</span><span class="sxs-lookup"><span data-stu-id="0e5c4-141">Configures the firewall to allow the host computer to respond to unsolicited network traffic of that traffic is secured by IPSec even when stealthModeBlocked is set to true</span></span>|
|<span data-ttu-id="0e5c4-142">policyRulesFromGroupPolicyMerged</span><span class="sxs-lookup"><span data-stu-id="0e5c4-142">policyRulesFromGroupPolicyMerged</span></span>|<span data-ttu-id="0e5c4-143">布尔值</span><span class="sxs-lookup"><span data-stu-id="0e5c4-143">Boolean</span></span>|<span data-ttu-id="0e5c4-144">配置防火墙，将组策略中的防火墙规则与本地存储合并，而不是忽略本地存储规则</span><span class="sxs-lookup"><span data-stu-id="0e5c4-144">Configures the firewall to merge Firewall Rule policies from group policy with those from local store instead of ignoring the local store rules</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e5c4-145">关系</span><span class="sxs-lookup"><span data-stu-id="0e5c4-145">Relationships</span></span>
<span data-ttu-id="0e5c4-146">无</span><span class="sxs-lookup"><span data-stu-id="0e5c4-146">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0e5c4-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e5c4-147">JSON Representation</span></span>
<span data-ttu-id="0e5c4-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e5c4-148">Here is a JSON representation of the resource.</span></span>
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



