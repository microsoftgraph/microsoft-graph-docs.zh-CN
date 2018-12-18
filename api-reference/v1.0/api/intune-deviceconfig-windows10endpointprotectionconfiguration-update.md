---
title: 更新 windows10EndpointProtectionConfiguration
description: 更新 windows10EndpointProtectionConfiguration 对象的属性。
author: tfitzmac
ms.openlocfilehash: 7116f7a6eef8c3ae26d5588191eec471a53373b7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313977"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="88ef8-103">更新 windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="88ef8-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="88ef8-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="88ef8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88ef8-105">更新 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="88ef8-105">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="88ef8-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="88ef8-106">Prerequisites</span></span>
<span data-ttu-id="88ef8-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="88ef8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88ef8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="88ef8-109">Permission type</span></span>|<span data-ttu-id="88ef8-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="88ef8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88ef8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88ef8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="88ef8-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88ef8-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="88ef8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88ef8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88ef8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="88ef8-114">Not supported.</span></span>|
|<span data-ttu-id="88ef8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="88ef8-115">Application</span></span>|<span data-ttu-id="88ef8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="88ef8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88ef8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88ef8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="88ef8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="88ef8-118">Request headers</span></span>
|<span data-ttu-id="88ef8-119">标头</span><span class="sxs-lookup"><span data-stu-id="88ef8-119">Header</span></span>|<span data-ttu-id="88ef8-120">值</span><span class="sxs-lookup"><span data-stu-id="88ef8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88ef8-121">授权</span><span class="sxs-lookup"><span data-stu-id="88ef8-121">Authorization</span></span>|<span data-ttu-id="88ef8-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="88ef8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88ef8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="88ef8-123">Accept</span></span>|<span data-ttu-id="88ef8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="88ef8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88ef8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="88ef8-125">Request body</span></span>
<span data-ttu-id="88ef8-126">在请求正文中，提供 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88ef8-126">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="88ef8-127">下表显示了创建 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="88ef8-127">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="88ef8-128">属性</span><span class="sxs-lookup"><span data-stu-id="88ef8-128">Property</span></span>|<span data-ttu-id="88ef8-129">类型</span><span class="sxs-lookup"><span data-stu-id="88ef8-129">Type</span></span>|<span data-ttu-id="88ef8-130">说明</span><span class="sxs-lookup"><span data-stu-id="88ef8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88ef8-131">id</span><span class="sxs-lookup"><span data-stu-id="88ef8-131">id</span></span>|<span data-ttu-id="88ef8-132">String</span><span class="sxs-lookup"><span data-stu-id="88ef8-132">String</span></span>|<span data-ttu-id="88ef8-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="88ef8-133">Key of the entity.</span></span> <span data-ttu-id="88ef8-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88ef8-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88ef8-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88ef8-135">lastModifiedDateTime</span></span>|<span data-ttu-id="88ef8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88ef8-136">DateTimeOffset</span></span>|<span data-ttu-id="88ef8-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="88ef8-137">DateTime the object was last modified.</span></span> <span data-ttu-id="88ef8-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88ef8-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88ef8-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88ef8-139">createdDateTime</span></span>|<span data-ttu-id="88ef8-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88ef8-140">DateTimeOffset</span></span>|<span data-ttu-id="88ef8-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="88ef8-141">DateTime the object was created.</span></span> <span data-ttu-id="88ef8-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88ef8-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88ef8-143">description</span><span class="sxs-lookup"><span data-stu-id="88ef8-143">description</span></span>|<span data-ttu-id="88ef8-144">String</span><span class="sxs-lookup"><span data-stu-id="88ef8-144">String</span></span>|<span data-ttu-id="88ef8-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="88ef8-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="88ef8-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88ef8-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88ef8-147">displayName</span><span class="sxs-lookup"><span data-stu-id="88ef8-147">displayName</span></span>|<span data-ttu-id="88ef8-148">String</span><span class="sxs-lookup"><span data-stu-id="88ef8-148">String</span></span>|<span data-ttu-id="88ef8-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="88ef8-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="88ef8-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88ef8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88ef8-151">version</span><span class="sxs-lookup"><span data-stu-id="88ef8-151">version</span></span>|<span data-ttu-id="88ef8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="88ef8-152">Int32</span></span>|<span data-ttu-id="88ef8-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="88ef8-153">Version of the device configuration.</span></span> <span data-ttu-id="88ef8-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88ef8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88ef8-155">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="88ef8-155">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="88ef8-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-156">Boolean</span></span>|<span data-ttu-id="88ef8-157">阻止到设备的有状态 FTP 连接</span><span class="sxs-lookup"><span data-stu-id="88ef8-157">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="88ef8-158">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="88ef8-158">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="88ef8-159">Int32</span><span class="sxs-lookup"><span data-stu-id="88ef8-159">Int32</span></span>|<span data-ttu-id="88ef8-160">配置安全关联的空闲超时（以秒为单位），值范围为 300 到 3600（包括这两个值）。</span><span class="sxs-lookup"><span data-stu-id="88ef8-160">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="88ef8-161">这是一个时间段，在此之后安全关联将过期并被删除。</span><span class="sxs-lookup"><span data-stu-id="88ef8-161">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="88ef8-162">有效值为 300 至 3600。</span><span class="sxs-lookup"><span data-stu-id="88ef8-162">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="88ef8-163">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="88ef8-163">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="88ef8-164">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="88ef8-164">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="88ef8-165">选择要使用编码的预共享的键。</span><span class="sxs-lookup"><span data-stu-id="88ef8-165">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="88ef8-166">可取值为：`deviceDefault`、`none`、`utF8`。</span><span class="sxs-lookup"><span data-stu-id="88ef8-166">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="88ef8-167">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="88ef8-167">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="88ef8-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-168">Boolean</span></span>|<span data-ttu-id="88ef8-169">配置 IPSec 免除项以允许邻居发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="88ef8-169">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="88ef8-170">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="88ef8-170">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="88ef8-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-171">Boolean</span></span>|<span data-ttu-id="88ef8-172">配置 IPSec 免除项以允许 ICMP</span><span class="sxs-lookup"><span data-stu-id="88ef8-172">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="88ef8-173">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="88ef8-173">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="88ef8-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-174">Boolean</span></span>|<span data-ttu-id="88ef8-175">配置 IPSec 免除项以允许路由器发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="88ef8-175">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="88ef8-176">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="88ef8-176">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="88ef8-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-177">Boolean</span></span>|<span data-ttu-id="88ef8-178">配置 IPSec 免除项以允许 IPv4 和 IPv6 DHCP 通信</span><span class="sxs-lookup"><span data-stu-id="88ef8-178">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="88ef8-179">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="88ef8-179">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="88ef8-180">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="88ef8-180">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="88ef8-181">指定如何强制实施证书吊销列表。</span><span class="sxs-lookup"><span data-stu-id="88ef8-181">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="88ef8-182">可取值为：`deviceDefault`、`none`、`attempt`、`require`。</span><span class="sxs-lookup"><span data-stu-id="88ef8-182">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="88ef8-183">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="88ef8-183">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="88ef8-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-184">Boolean</span></span>|<span data-ttu-id="88ef8-185">如果键控模块不完全支持身份验证集，请指示模块仅忽略不受支持的身份验证套件而不是整个集</span><span class="sxs-lookup"><span data-stu-id="88ef8-185">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="88ef8-186">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="88ef8-186">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="88ef8-187">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="88ef8-187">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="88ef8-188">配置数据包 queueing 应如何应用隧道网关方案中。</span><span class="sxs-lookup"><span data-stu-id="88ef8-188">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="88ef8-189">可取值为：`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth`。</span><span class="sxs-lookup"><span data-stu-id="88ef8-189">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="88ef8-190">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="88ef8-190">firewallProfileDomain</span></span>|[<span data-ttu-id="88ef8-191">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="88ef8-191">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="88ef8-192">配置域网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="88ef8-192">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="88ef8-193">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="88ef8-193">firewallProfilePublic</span></span>|[<span data-ttu-id="88ef8-194">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="88ef8-194">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="88ef8-195">配置公用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="88ef8-195">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="88ef8-196">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="88ef8-196">firewallProfilePrivate</span></span>|[<span data-ttu-id="88ef8-197">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="88ef8-197">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="88ef8-198">配置专用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="88ef8-198">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="88ef8-199">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="88ef8-199">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="88ef8-200">String 集合</span><span class="sxs-lookup"><span data-stu-id="88ef8-200">String collection</span></span>|<span data-ttu-id="88ef8-201">要从攻击面减少规则中排除的 exe 文件和文件夹的列表</span><span class="sxs-lookup"><span data-stu-id="88ef8-201">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="88ef8-202">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="88ef8-202">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="88ef8-203">String 集合</span><span class="sxs-lookup"><span data-stu-id="88ef8-203">String collection</span></span>|<span data-ttu-id="88ef8-204">允许访问受保护文件夹的 exe 路径列表</span><span class="sxs-lookup"><span data-stu-id="88ef8-204">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="88ef8-205">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="88ef8-205">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="88ef8-206">String 集合</span><span class="sxs-lookup"><span data-stu-id="88ef8-206">String collection</span></span>|<span data-ttu-id="88ef8-207">要添加到受保护文件夹列表的文件夹路径列表</span><span class="sxs-lookup"><span data-stu-id="88ef8-207">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="88ef8-208">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="88ef8-208">defenderExploitProtectionXml</span></span>|<span data-ttu-id="88ef8-209">Binary</span><span class="sxs-lookup"><span data-stu-id="88ef8-209">Binary</span></span>|<span data-ttu-id="88ef8-210">包含有关 Exploit Protection 详细信息的 xml 内容。</span><span class="sxs-lookup"><span data-stu-id="88ef8-210">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="88ef8-211">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="88ef8-211">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="88ef8-212">String</span><span class="sxs-lookup"><span data-stu-id="88ef8-212">String</span></span>|<span data-ttu-id="88ef8-213">从中获取 DefenderExploitProtectionXml 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="88ef8-213">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="88ef8-214">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="88ef8-214">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="88ef8-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-215">Boolean</span></span>|<span data-ttu-id="88ef8-216">指示是否阻止用户覆盖 Exploit Protection 设置。</span><span class="sxs-lookup"><span data-stu-id="88ef8-216">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="88ef8-217">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="88ef8-217">appLockerApplicationControl</span></span>|[<span data-ttu-id="88ef8-218">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="88ef8-218">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="88ef8-219">使管理员能够选择在设备上允许哪些类型的应用。</span><span class="sxs-lookup"><span data-stu-id="88ef8-219">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="88ef8-220">可取值为：`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker`。</span><span class="sxs-lookup"><span data-stu-id="88ef8-220">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="88ef8-221">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="88ef8-221">smartScreenEnableInShell</span></span>|<span data-ttu-id="88ef8-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-222">Boolean</span></span>|<span data-ttu-id="88ef8-223">允许 IT 管理员配置适用于 Windows 的 SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="88ef8-223">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="88ef8-224">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="88ef8-224">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="88ef8-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-225">Boolean</span></span>|<span data-ttu-id="88ef8-226">允许 IT 管理员控制用户是否可以忽略 SmartScreen 警告并运行恶意文件。</span><span class="sxs-lookup"><span data-stu-id="88ef8-226">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="88ef8-227">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="88ef8-227">applicationGuardEnabled</span></span>|<span data-ttu-id="88ef8-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-228">Boolean</span></span>|<span data-ttu-id="88ef8-229">启用 Windows Defender 应用程序防护</span><span class="sxs-lookup"><span data-stu-id="88ef8-229">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="88ef8-230">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="88ef8-230">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="88ef8-231">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="88ef8-231">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="88ef8-232">阻止传输图像文件、 文本文件或两者到剪贴板。</span><span class="sxs-lookup"><span data-stu-id="88ef8-232">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="88ef8-233">可取值为：`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile`。</span><span class="sxs-lookup"><span data-stu-id="88ef8-233">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="88ef8-234">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="88ef8-234">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="88ef8-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-235">Boolean</span></span>|<span data-ttu-id="88ef8-236">阻止企业站点加载非企业内容，例如第三方插件</span><span class="sxs-lookup"><span data-stu-id="88ef8-236">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="88ef8-237">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="88ef8-237">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="88ef8-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-238">Boolean</span></span>|<span data-ttu-id="88ef8-239">允许 App Guard 容器（收藏夹、Cookie、Web 密码等）内的持久用户生成数据</span><span class="sxs-lookup"><span data-stu-id="88ef8-239">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="88ef8-240">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="88ef8-240">applicationGuardForceAuditing</span></span>|<span data-ttu-id="88ef8-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-241">Boolean</span></span>|<span data-ttu-id="88ef8-242">强制审核将存留 Windows 日志和事件以满足安全/符合性条件（示例事件是用户登录注销、特权使用、软件安装、系统更改等）</span><span class="sxs-lookup"><span data-stu-id="88ef8-242">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="88ef8-243">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="88ef8-243">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="88ef8-244">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="88ef8-244">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="88ef8-245">阻止剪贴板将数据从主机共享到容器或从容器共享到主机，或阻止两种方式，或两种方式均不阻止。</span><span class="sxs-lookup"><span data-stu-id="88ef8-245">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="88ef8-246">可取值为：`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone`。</span><span class="sxs-lookup"><span data-stu-id="88ef8-246">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="88ef8-247">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="88ef8-247">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="88ef8-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-248">Boolean</span></span>|<span data-ttu-id="88ef8-249">允许从容器打印为 PDF 格式</span><span class="sxs-lookup"><span data-stu-id="88ef8-249">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="88ef8-250">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="88ef8-250">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="88ef8-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-251">Boolean</span></span>|<span data-ttu-id="88ef8-252">允许从容器打印为 XPS 格式</span><span class="sxs-lookup"><span data-stu-id="88ef8-252">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="88ef8-253">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="88ef8-253">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="88ef8-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-254">Boolean</span></span>|<span data-ttu-id="88ef8-255">允许从容器打印到本地打印机</span><span class="sxs-lookup"><span data-stu-id="88ef8-255">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="88ef8-256">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="88ef8-256">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="88ef8-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-257">Boolean</span></span>|<span data-ttu-id="88ef8-258">允许从容器打印到网络打印机</span><span class="sxs-lookup"><span data-stu-id="88ef8-258">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="88ef8-259">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="88ef8-259">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="88ef8-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-260">Boolean</span></span>|<span data-ttu-id="88ef8-261">允许管理员禁用对用户计算机上其他磁盘加密的警告提示。</span><span class="sxs-lookup"><span data-stu-id="88ef8-261">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="88ef8-262">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="88ef8-262">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="88ef8-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-263">Boolean</span></span>|<span data-ttu-id="88ef8-264">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="88ef8-264">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="88ef8-265">此策略仅适用于移动 SKU。</span><span class="sxs-lookup"><span data-stu-id="88ef8-265">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="88ef8-266">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="88ef8-266">bitLockerEncryptDevice</span></span>|<span data-ttu-id="88ef8-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="88ef8-267">Boolean</span></span>|<span data-ttu-id="88ef8-268">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="88ef8-268">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="88ef8-269">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="88ef8-269">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="88ef8-270">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="88ef8-270">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="88ef8-271">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="88ef8-271">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="88ef8-272">响应</span><span class="sxs-lookup"><span data-stu-id="88ef8-272">Response</span></span>
<span data-ttu-id="88ef8-273">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="88ef8-273">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88ef8-274">示例</span><span class="sxs-lookup"><span data-stu-id="88ef8-274">Example</span></span>
### <a name="request"></a><span data-ttu-id="88ef8-275">请求</span><span class="sxs-lookup"><span data-stu-id="88ef8-275">Request</span></span>
<span data-ttu-id="88ef8-276">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88ef8-276">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4245

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
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

### <a name="response"></a><span data-ttu-id="88ef8-277">响应</span><span class="sxs-lookup"><span data-stu-id="88ef8-277">Response</span></span>
<span data-ttu-id="88ef8-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="88ef8-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



