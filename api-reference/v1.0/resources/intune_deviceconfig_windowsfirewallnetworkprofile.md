# <a name="windowsfirewallnetworkprofile-resource-type"></a><span data-ttu-id="e1b3d-101">windowsFirewallNetworkProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1b3d-101">windowsFirewallNetworkProfile resource type</span></span>

> <span data-ttu-id="e1b3d-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e1b3d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1b3d-103">Windows 防火墙配置文件策略。</span><span class="sxs-lookup"><span data-stu-id="e1b3d-103">Windows Firewall Profile Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="e1b3d-104">属性</span><span class="sxs-lookup"><span data-stu-id="e1b3d-104">Properties</span></span>
|<span data-ttu-id="e1b3d-105">属性</span><span class="sxs-lookup"><span data-stu-id="e1b3d-105">Property</span></span>|<span data-ttu-id="e1b3d-106">类型</span><span class="sxs-lookup"><span data-stu-id="e1b3d-106">Type</span></span>|<span data-ttu-id="e1b3d-107">说明</span><span class="sxs-lookup"><span data-stu-id="e1b3d-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1b3d-108">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="e1b3d-108">firewallEnabled</span></span>|<span data-ttu-id="e1b3d-109">String</span><span class="sxs-lookup"><span data-stu-id="e1b3d-109">String</span></span>|<span data-ttu-id="e1b3d-110">打开防火墙和高级安全执行 可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="e1b3d-110">Turn on the firewall and advanced security enforcement Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="e1b3d-111">stealthModeBlocked</span><span class="sxs-lookup"><span data-stu-id="e1b3d-111">stealthModeBlocked</span></span>|<span data-ttu-id="e1b3d-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="e1b3d-112">Boolean</span></span>|<span data-ttu-id="e1b3d-113">防止服务器在隐藏模式下运行</span><span class="sxs-lookup"><span data-stu-id="e1b3d-113">Prevent the server from operating in stealth mode</span></span>|
|<span data-ttu-id="e1b3d-114">incomingTrafficBlocked</span><span class="sxs-lookup"><span data-stu-id="e1b3d-114">incomingTrafficBlocked</span></span>|<span data-ttu-id="e1b3d-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="e1b3d-115">Boolean</span></span>|<span data-ttu-id="e1b3d-116">配置防火墙以阻止所有传入通信，无论其他策略设置为何</span><span class="sxs-lookup"><span data-stu-id="e1b3d-116">Configures the firewall to block all incoming traffic regardless of other policy settings</span></span>|
|<span data-ttu-id="e1b3d-117">unicastResponsesToMulticastBroadcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="e1b3d-117">unicastResponsesToMulticastBroadcastsBlocked</span></span>|<span data-ttu-id="e1b3d-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="e1b3d-118">Boolean</span></span>|<span data-ttu-id="e1b3d-119">配置防火墙以阻止对多播广播通信的单播响应</span><span class="sxs-lookup"><span data-stu-id="e1b3d-119">Configures the firewall to block unicast responses to multicast broadcast traffic</span></span>|
|<span data-ttu-id="e1b3d-120">inboundNotificationsBlocked</span><span class="sxs-lookup"><span data-stu-id="e1b3d-120">inboundNotificationsBlocked</span></span>|<span data-ttu-id="e1b3d-121">布尔值</span><span class="sxs-lookup"><span data-stu-id="e1b3d-121">Boolean</span></span>|<span data-ttu-id="e1b3d-122">阻止应用程序在端口上侦听时，避免防火墙显示通知</span><span class="sxs-lookup"><span data-stu-id="e1b3d-122">Prevents the firewall from displaying notifications when an application is blocked from listening on a port</span></span>|
|<span data-ttu-id="e1b3d-123">authorizedApplicationRulesFromGroupPolicyMerged</span><span class="sxs-lookup"><span data-stu-id="e1b3d-123">authorizedApplicationRulesFromGroupPolicyMerged</span></span>|<span data-ttu-id="e1b3d-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="e1b3d-124">Boolean</span></span>|<span data-ttu-id="e1b3d-125">配置防火墙，将组策略中的授权应用程序规则与本地存储合并，而不是忽略本地存储规则</span><span class="sxs-lookup"><span data-stu-id="e1b3d-125">Configures the firewall to merge authorized application rules from group policy with those from local store instead of ignoring the local store rules</span></span>|
|<span data-ttu-id="e1b3d-126">globalPortRulesFromGroupPolicyMerged</span><span class="sxs-lookup"><span data-stu-id="e1b3d-126">globalPortRulesFromGroupPolicyMerged</span></span>|<span data-ttu-id="e1b3d-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="e1b3d-127">Boolean</span></span>|<span data-ttu-id="e1b3d-128">配置防火墙，将组策略中的全局端口规则与本地存储合并，而不是忽略本地存储规则</span><span class="sxs-lookup"><span data-stu-id="e1b3d-128">Configures the firewall to merge global port rules from group policy with those from local store instead of ignoring the local store rules</span></span>|
|<span data-ttu-id="e1b3d-129">connectionSecurityRulesFromGroupPolicyMerged</span><span class="sxs-lookup"><span data-stu-id="e1b3d-129">connectionSecurityRulesFromGroupPolicyMerged</span></span>|<span data-ttu-id="e1b3d-130">布尔值</span><span class="sxs-lookup"><span data-stu-id="e1b3d-130">Boolean</span></span>|<span data-ttu-id="e1b3d-131">配置防火墙，将组策略中的连接安全规则与本地存储合并，而不是忽略本地存储规则</span><span class="sxs-lookup"><span data-stu-id="e1b3d-131">Configures the firewall to merge connection security rules from group policy with those from local store instead of ignoring the local store rules</span></span>|
|<span data-ttu-id="e1b3d-132">outboundConnectionsBlocked</span><span class="sxs-lookup"><span data-stu-id="e1b3d-132">outboundConnectionsBlocked</span></span>|<span data-ttu-id="e1b3d-133">布尔值</span><span class="sxs-lookup"><span data-stu-id="e1b3d-133">Boolean</span></span>|<span data-ttu-id="e1b3d-134">配置防火墙，在默认情况下阻止所有传出连接</span><span class="sxs-lookup"><span data-stu-id="e1b3d-134">Configures the firewall to block all outgoing connections by default</span></span>|
|<span data-ttu-id="e1b3d-135">inboundConnectionsBlocked</span><span class="sxs-lookup"><span data-stu-id="e1b3d-135">inboundConnectionsBlocked</span></span>|<span data-ttu-id="e1b3d-136">布尔值</span><span class="sxs-lookup"><span data-stu-id="e1b3d-136">Boolean</span></span>|<span data-ttu-id="e1b3d-137">配置防火墙，在默认情况下阻止所有传入连接</span><span class="sxs-lookup"><span data-stu-id="e1b3d-137">Configures the firewall to block all incoming connections by default</span></span>|
|<span data-ttu-id="e1b3d-138">securedPacketExemptionAllowed</span><span class="sxs-lookup"><span data-stu-id="e1b3d-138">securedPacketExemptionAllowed</span></span>|<span data-ttu-id="e1b3d-139">布尔值</span><span class="sxs-lookup"><span data-stu-id="e1b3d-139">Boolean</span></span>|<span data-ttu-id="e1b3d-140">配置防火墙，允许主机计算机响应未经请求的网络通信（如果该通信受 IPSec 保护），即使 stealthModeBlocked 设置为 true</span><span class="sxs-lookup"><span data-stu-id="e1b3d-140">Configures the firewall to allow the host computer to respond to unsolicited network traffic of that traffic is secured by IPSec even when stealthModeBlocked is set to true</span></span>|
|<span data-ttu-id="e1b3d-141">policyRulesFromGroupPolicyMerged</span><span class="sxs-lookup"><span data-stu-id="e1b3d-141">policyRulesFromGroupPolicyMerged</span></span>|<span data-ttu-id="e1b3d-142">布尔值</span><span class="sxs-lookup"><span data-stu-id="e1b3d-142">Boolean</span></span>|<span data-ttu-id="e1b3d-143">配置防火墙，将组策略中的防火墙规则与本地存储合并，而不是忽略本地存储规则</span><span class="sxs-lookup"><span data-stu-id="e1b3d-143">Configures the firewall to merge Firewall Rule policies from group policy with those from local store instead of ignoring the local store rules</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1b3d-144">关系</span><span class="sxs-lookup"><span data-stu-id="e1b3d-144">Relationships</span></span>
<span data-ttu-id="e1b3d-145">无</span><span class="sxs-lookup"><span data-stu-id="e1b3d-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e1b3d-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1b3d-146">JSON Representation</span></span>
<span data-ttu-id="e1b3d-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1b3d-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



