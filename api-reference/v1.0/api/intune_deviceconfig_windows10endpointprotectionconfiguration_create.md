# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="78f26-101">创建 windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="78f26-101">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="78f26-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="78f26-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78f26-103">创建新的 [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="78f26-103">Create a new [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="78f26-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="78f26-104">Prerequisites</span></span>
<span data-ttu-id="78f26-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="78f26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="78f26-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="78f26-107">Permission type</span></span>|<span data-ttu-id="78f26-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="78f26-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78f26-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78f26-109">Delegated (work or school account)</span></span>|<span data-ttu-id="78f26-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f26-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="78f26-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78f26-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78f26-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="78f26-112">Not supported.</span></span>|
|<span data-ttu-id="78f26-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="78f26-113">Application</span></span>|<span data-ttu-id="78f26-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="78f26-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78f26-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78f26-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="78f26-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="78f26-116">Request headers</span></span>
|<span data-ttu-id="78f26-117">标头</span><span class="sxs-lookup"><span data-stu-id="78f26-117">Header</span></span>|<span data-ttu-id="78f26-118">值</span><span class="sxs-lookup"><span data-stu-id="78f26-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78f26-119">授权</span><span class="sxs-lookup"><span data-stu-id="78f26-119">Authorization</span></span>|<span data-ttu-id="78f26-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="78f26-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78f26-121">接受</span><span class="sxs-lookup"><span data-stu-id="78f26-121">Accept</span></span>|<span data-ttu-id="78f26-122">application/json</span><span class="sxs-lookup"><span data-stu-id="78f26-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78f26-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="78f26-123">Request body</span></span>
<span data-ttu-id="78f26-124">在请求正文中，提供 windows10EndpointProtectionConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78f26-124">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="78f26-125">下表显示了创建 windows10EndpointProtectionConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="78f26-125">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="78f26-126">属性</span><span class="sxs-lookup"><span data-stu-id="78f26-126">Property</span></span>|<span data-ttu-id="78f26-127">类型</span><span class="sxs-lookup"><span data-stu-id="78f26-127">Type</span></span>|<span data-ttu-id="78f26-128">说明</span><span class="sxs-lookup"><span data-stu-id="78f26-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78f26-129">ID</span><span class="sxs-lookup"><span data-stu-id="78f26-129">id</span></span>|<span data-ttu-id="78f26-130">字符串</span><span class="sxs-lookup"><span data-stu-id="78f26-130">String</span></span>|<span data-ttu-id="78f26-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="78f26-131">Key of the entity.</span></span> <span data-ttu-id="78f26-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="78f26-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78f26-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78f26-133">lastModifiedDateTime</span></span>|<span data-ttu-id="78f26-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78f26-134">DateTimeOffset</span></span>|<span data-ttu-id="78f26-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="78f26-135">DateTime the object was last modified.</span></span> <span data-ttu-id="78f26-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="78f26-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78f26-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="78f26-137">createdDateTime</span></span>|<span data-ttu-id="78f26-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78f26-138">DateTimeOffset</span></span>|<span data-ttu-id="78f26-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="78f26-139">DateTime the object was created.</span></span> <span data-ttu-id="78f26-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="78f26-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78f26-141">说明</span><span class="sxs-lookup"><span data-stu-id="78f26-141">description</span></span>|<span data-ttu-id="78f26-142">字符串</span><span class="sxs-lookup"><span data-stu-id="78f26-142">String</span></span>|<span data-ttu-id="78f26-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="78f26-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="78f26-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="78f26-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78f26-145">displayName</span><span class="sxs-lookup"><span data-stu-id="78f26-145">displayName</span></span>|<span data-ttu-id="78f26-146">字符串</span><span class="sxs-lookup"><span data-stu-id="78f26-146">String</span></span>|<span data-ttu-id="78f26-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="78f26-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="78f26-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="78f26-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78f26-149">版本</span><span class="sxs-lookup"><span data-stu-id="78f26-149">version</span></span>|<span data-ttu-id="78f26-150">Int32</span><span class="sxs-lookup"><span data-stu-id="78f26-150">Int32</span></span>|<span data-ttu-id="78f26-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="78f26-151">Version of the device configuration.</span></span> <span data-ttu-id="78f26-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="78f26-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="78f26-153">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="78f26-153">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="78f26-154">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-154">Boolean</span></span>|<span data-ttu-id="78f26-155">阻止到设备的有状态 FTP 连接</span><span class="sxs-lookup"><span data-stu-id="78f26-155">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="78f26-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="78f26-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="78f26-157">Int32</span><span class="sxs-lookup"><span data-stu-id="78f26-157">Int32</span></span>|<span data-ttu-id="78f26-158">配置安全关联的空闲超时（以秒为单位），值范围为 300 到 3600（包括这两个值）。</span><span class="sxs-lookup"><span data-stu-id="78f26-158">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="78f26-159">这是一个时间段，在此之后安全关联将过期并被删除。</span><span class="sxs-lookup"><span data-stu-id="78f26-159">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="78f26-160">有效值为 300 至 3600。</span><span class="sxs-lookup"><span data-stu-id="78f26-160">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="78f26-161">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="78f26-161">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="78f26-162">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="78f26-162">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune_deviceconfig_firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="78f26-163">选择要使用的预共享密钥编码。</span><span class="sxs-lookup"><span data-stu-id="78f26-163">Select the preshared key encoding to be used Possible values are: , , .</span></span> <span data-ttu-id="78f26-164">可取值为：`deviceDefault`、`none`、`utF8`。</span><span class="sxs-lookup"><span data-stu-id="78f26-164">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="78f26-165">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="78f26-165">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="78f26-166">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-166">Boolean</span></span>|<span data-ttu-id="78f26-167">配置 IPSec 免除项以允许邻居发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="78f26-167">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="78f26-168">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="78f26-168">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="78f26-169">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-169">Boolean</span></span>|<span data-ttu-id="78f26-170">配置 IPSec 免除项以允许 ICMP</span><span class="sxs-lookup"><span data-stu-id="78f26-170">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="78f26-171">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="78f26-171">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="78f26-172">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-172">Boolean</span></span>|<span data-ttu-id="78f26-173">配置 IPSec 免除项以允许路由器发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="78f26-173">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="78f26-174">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="78f26-174">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="78f26-175">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-175">Boolean</span></span>|<span data-ttu-id="78f26-176">配置 IPSec 免除项以允许 IPv4 和 IPv6 DHCP 通信</span><span class="sxs-lookup"><span data-stu-id="78f26-176">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="78f26-177">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="78f26-177">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="78f26-178">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="78f26-178">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune_deviceconfig_firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="78f26-179">指定如何强制执行证书吊销列表。</span><span class="sxs-lookup"><span data-stu-id="78f26-179">Specify how the certificate revocation list is to be enforced Possible values are: , , , .</span></span> <span data-ttu-id="78f26-180">可取值为：`deviceDefault`、`none`、`attempt`、`require`。</span><span class="sxs-lookup"><span data-stu-id="78f26-180">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="78f26-181">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="78f26-181">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="78f26-182">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-182">Boolean</span></span>|<span data-ttu-id="78f26-183">如果键控模块不完全支持身份验证集，请指示模块仅忽略不受支持的身份验证套件而不是整个集</span><span class="sxs-lookup"><span data-stu-id="78f26-183">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="78f26-184">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="78f26-184">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="78f26-185">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="78f26-185">firewallPacketQueueingMethodType</span></span>](../resources/intune_deviceconfig_firewallpacketqueueingmethodtype.md)|<span data-ttu-id="78f26-186">配置数据包排队如何在隧道网关方案中应用。</span><span class="sxs-lookup"><span data-stu-id="78f26-186">Configures how packet queueing should be applied in the tunnel gateway scenario Possible values are: , , , , .</span></span> <span data-ttu-id="78f26-187">可取值为：`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth`。</span><span class="sxs-lookup"><span data-stu-id="78f26-187">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="78f26-188">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="78f26-188">firewallProfileDomain</span></span>|[<span data-ttu-id="78f26-189">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="78f26-189">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="78f26-190">配置域网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="78f26-190">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="78f26-191">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="78f26-191">firewallProfilePublic</span></span>|[<span data-ttu-id="78f26-192">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="78f26-192">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="78f26-193">配置公用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="78f26-193">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="78f26-194">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="78f26-194">firewallProfilePrivate</span></span>|[<span data-ttu-id="78f26-195">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="78f26-195">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="78f26-196">配置专用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="78f26-196">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="78f26-197">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="78f26-197">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="78f26-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="78f26-198">String collection</span></span>|<span data-ttu-id="78f26-199">要从攻击面减少规则中排除的 exe 文件和文件夹的列表</span><span class="sxs-lookup"><span data-stu-id="78f26-199">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="78f26-200">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="78f26-200">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="78f26-201">String 集合</span><span class="sxs-lookup"><span data-stu-id="78f26-201">String collection</span></span>|<span data-ttu-id="78f26-202">允许访问受保护文件夹的 exe 路径列表</span><span class="sxs-lookup"><span data-stu-id="78f26-202">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="78f26-203">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="78f26-203">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="78f26-204">String 集合</span><span class="sxs-lookup"><span data-stu-id="78f26-204">String collection</span></span>|<span data-ttu-id="78f26-205">要添加到受保护文件夹列表的文件夹路径列表</span><span class="sxs-lookup"><span data-stu-id="78f26-205">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="78f26-206">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="78f26-206">defenderExploitProtectionXml</span></span>|<span data-ttu-id="78f26-207">二进制</span><span class="sxs-lookup"><span data-stu-id="78f26-207">Binary</span></span>|<span data-ttu-id="78f26-208">包含有关 Exploit Protection 详细信息的 xml 内容。</span><span class="sxs-lookup"><span data-stu-id="78f26-208">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="78f26-209">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="78f26-209">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="78f26-210">字符串</span><span class="sxs-lookup"><span data-stu-id="78f26-210">String</span></span>|<span data-ttu-id="78f26-211">从中获取 DefenderExploitProtectionXml 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="78f26-211">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="78f26-212">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="78f26-212">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="78f26-213">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-213">Boolean</span></span>|<span data-ttu-id="78f26-214">指示是否阻止用户覆盖 Exploit Protection 设置。</span><span class="sxs-lookup"><span data-stu-id="78f26-214">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="78f26-215">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="78f26-215">appLockerApplicationControl</span></span>|[<span data-ttu-id="78f26-216">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="78f26-216">appLockerApplicationControlType</span></span>](../resources/intune_deviceconfig_applockerapplicationcontroltype.md)|<span data-ttu-id="78f26-217">使管理员能够选择在设备上允许哪些类型的应用。</span><span class="sxs-lookup"><span data-stu-id="78f26-217">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="78f26-218">可取值为：`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker`。</span><span class="sxs-lookup"><span data-stu-id="78f26-218">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="78f26-219">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="78f26-219">smartScreenEnableInShell</span></span>|<span data-ttu-id="78f26-220">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-220">Boolean</span></span>|<span data-ttu-id="78f26-221">允许 IT 管理员配置适用于 Windows 的 SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="78f26-221">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="78f26-222">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="78f26-222">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="78f26-223">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-223">Boolean</span></span>|<span data-ttu-id="78f26-224">允许 IT 管理员控制用户是否可以忽略 SmartScreen 警告并运行恶意文件。</span><span class="sxs-lookup"><span data-stu-id="78f26-224">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="78f26-225">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="78f26-225">applicationGuardEnabled</span></span>|<span data-ttu-id="78f26-226">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-226">Boolean</span></span>|<span data-ttu-id="78f26-227">启用 Windows Defender 应用程序防护</span><span class="sxs-lookup"><span data-stu-id="78f26-227">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="78f26-228">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="78f26-228">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="78f26-229">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="78f26-229">applicationGuardBlockFileTransferType</span></span>](../resources/intune_deviceconfig_applicationguardblockfiletransfertype.md)|<span data-ttu-id="78f26-230">阻止剪贴板传输图像文件或文本文件或两者均不阻止。</span><span class="sxs-lookup"><span data-stu-id="78f26-230">Block clipboard to transfer image file, text file or neither of them Possible values are: , , , , .</span></span> <span data-ttu-id="78f26-231">可取值为：`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile`。</span><span class="sxs-lookup"><span data-stu-id="78f26-231">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="78f26-232">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="78f26-232">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="78f26-233">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-233">Boolean</span></span>|<span data-ttu-id="78f26-234">阻止企业站点加载非企业内容，例如第三方插件</span><span class="sxs-lookup"><span data-stu-id="78f26-234">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="78f26-235">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="78f26-235">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="78f26-236">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-236">Boolean</span></span>|<span data-ttu-id="78f26-237">允许 App Guard 容器（收藏夹、Cookie、Web 密码等）内的持久用户生成数据</span><span class="sxs-lookup"><span data-stu-id="78f26-237">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="78f26-238">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="78f26-238">applicationGuardForceAuditing</span></span>|<span data-ttu-id="78f26-239">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-239">Boolean</span></span>|<span data-ttu-id="78f26-240">强制审核将存留 Windows 日志和事件以满足安全/符合性条件（示例事件是用户登录注销、特权使用、软件安装、系统更改等）</span><span class="sxs-lookup"><span data-stu-id="78f26-240">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="78f26-241">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="78f26-241">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="78f26-242">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="78f26-242">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune_deviceconfig_applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="78f26-243">阻止剪贴板将数据从主机共享到容器或从容器共享到主机，或阻止两种方式，或两种方式均不阻止。</span><span class="sxs-lookup"><span data-stu-id="78f26-243">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="78f26-244">可取值为：`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone`。</span><span class="sxs-lookup"><span data-stu-id="78f26-244">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="78f26-245">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="78f26-245">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="78f26-246">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-246">Boolean</span></span>|<span data-ttu-id="78f26-247">允许从容器打印为 PDF 格式</span><span class="sxs-lookup"><span data-stu-id="78f26-247">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="78f26-248">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="78f26-248">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="78f26-249">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-249">Boolean</span></span>|<span data-ttu-id="78f26-250">允许从容器打印为 XPS 格式</span><span class="sxs-lookup"><span data-stu-id="78f26-250">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="78f26-251">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="78f26-251">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="78f26-252">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-252">Boolean</span></span>|<span data-ttu-id="78f26-253">允许从容器打印到本地打印机</span><span class="sxs-lookup"><span data-stu-id="78f26-253">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="78f26-254">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="78f26-254">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="78f26-255">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-255">Boolean</span></span>|<span data-ttu-id="78f26-256">允许从容器打印到网络打印机</span><span class="sxs-lookup"><span data-stu-id="78f26-256">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="78f26-257">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="78f26-257">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="78f26-258">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-258">Boolean</span></span>|<span data-ttu-id="78f26-259">允许管理员禁用对用户计算机上其他磁盘加密的警告提示。</span><span class="sxs-lookup"><span data-stu-id="78f26-259">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="78f26-260">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="78f26-260">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="78f26-261">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-261">Boolean</span></span>|<span data-ttu-id="78f26-262">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="78f26-262">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="78f26-263">此策略仅适用于移动 SKU。</span><span class="sxs-lookup"><span data-stu-id="78f26-263">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="78f26-264">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="78f26-264">bitLockerEncryptDevice</span></span>|<span data-ttu-id="78f26-265">布尔值</span><span class="sxs-lookup"><span data-stu-id="78f26-265">Boolean</span></span>|<span data-ttu-id="78f26-266">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="78f26-266">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="78f26-267">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="78f26-267">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="78f26-268">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="78f26-268">bitLockerRemovableDrivePolicy</span></span>](../resources/intune_deviceconfig_bitlockerremovabledrivepolicy.md)|<span data-ttu-id="78f26-269">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="78f26-269">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="78f26-270">响应</span><span class="sxs-lookup"><span data-stu-id="78f26-270">Response</span></span>
<span data-ttu-id="78f26-271">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="78f26-271">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78f26-272">示例</span><span class="sxs-lookup"><span data-stu-id="78f26-272">Example</span></span>
### <a name="request"></a><span data-ttu-id="78f26-273">请求</span><span class="sxs-lookup"><span data-stu-id="78f26-273">Request</span></span>
<span data-ttu-id="78f26-274">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="78f26-274">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4309

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
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
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
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
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
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
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```

### <a name="response"></a><span data-ttu-id="78f26-275">响应</span><span class="sxs-lookup"><span data-stu-id="78f26-275">Response</span></span>
<span data-ttu-id="78f26-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="78f26-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4417

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "09709403-9403-0970-0394-700903947009",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
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
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
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
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
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
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```








