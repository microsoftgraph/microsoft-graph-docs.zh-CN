---
title: 更新 windows10EndpointProtectionConfiguration
description: 更新 windows10EndpointProtectionConfiguration 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ad83de42f932cf4b47d7090f6804f7c26555419e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514089"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="45808-103">更新 windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="45808-103">Update windows10EndpointProtectionConfiguration</span></span>

<span data-ttu-id="45808-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45808-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45808-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="45808-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45808-106">更新 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="45808-106">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45808-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="45808-107">Prerequisites</span></span>
<span data-ttu-id="45808-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45808-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45808-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="45808-110">Permission type</span></span>|<span data-ttu-id="45808-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="45808-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45808-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45808-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45808-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45808-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="45808-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45808-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45808-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="45808-115">Not supported.</span></span>|
|<span data-ttu-id="45808-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="45808-116">Application</span></span>|<span data-ttu-id="45808-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="45808-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45808-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45808-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="45808-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="45808-119">Request headers</span></span>
|<span data-ttu-id="45808-120">标头</span><span class="sxs-lookup"><span data-stu-id="45808-120">Header</span></span>|<span data-ttu-id="45808-121">值</span><span class="sxs-lookup"><span data-stu-id="45808-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45808-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="45808-122">Authorization</span></span>|<span data-ttu-id="45808-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="45808-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45808-124">接受</span><span class="sxs-lookup"><span data-stu-id="45808-124">Accept</span></span>|<span data-ttu-id="45808-125">application/json</span><span class="sxs-lookup"><span data-stu-id="45808-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45808-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="45808-126">Request body</span></span>
<span data-ttu-id="45808-127">在请求正文中，提供 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45808-127">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="45808-128">下表显示了创建 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="45808-128">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="45808-129">属性</span><span class="sxs-lookup"><span data-stu-id="45808-129">Property</span></span>|<span data-ttu-id="45808-130">类型</span><span class="sxs-lookup"><span data-stu-id="45808-130">Type</span></span>|<span data-ttu-id="45808-131">说明</span><span class="sxs-lookup"><span data-stu-id="45808-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45808-132">id</span><span class="sxs-lookup"><span data-stu-id="45808-132">id</span></span>|<span data-ttu-id="45808-133">字符串</span><span class="sxs-lookup"><span data-stu-id="45808-133">String</span></span>|<span data-ttu-id="45808-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="45808-134">Key of the entity.</span></span> <span data-ttu-id="45808-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45808-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45808-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45808-136">lastModifiedDateTime</span></span>|<span data-ttu-id="45808-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45808-137">DateTimeOffset</span></span>|<span data-ttu-id="45808-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="45808-138">DateTime the object was last modified.</span></span> <span data-ttu-id="45808-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45808-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45808-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45808-140">createdDateTime</span></span>|<span data-ttu-id="45808-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45808-141">DateTimeOffset</span></span>|<span data-ttu-id="45808-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="45808-142">DateTime the object was created.</span></span> <span data-ttu-id="45808-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45808-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45808-144">说明</span><span class="sxs-lookup"><span data-stu-id="45808-144">description</span></span>|<span data-ttu-id="45808-145">String</span><span class="sxs-lookup"><span data-stu-id="45808-145">String</span></span>|<span data-ttu-id="45808-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="45808-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="45808-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45808-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45808-148">displayName</span><span class="sxs-lookup"><span data-stu-id="45808-148">displayName</span></span>|<span data-ttu-id="45808-149">字符串</span><span class="sxs-lookup"><span data-stu-id="45808-149">String</span></span>|<span data-ttu-id="45808-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="45808-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="45808-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45808-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45808-152">version</span><span class="sxs-lookup"><span data-stu-id="45808-152">version</span></span>|<span data-ttu-id="45808-153">Int32</span><span class="sxs-lookup"><span data-stu-id="45808-153">Int32</span></span>|<span data-ttu-id="45808-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="45808-154">Version of the device configuration.</span></span> <span data-ttu-id="45808-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45808-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45808-156">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="45808-156">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="45808-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-157">Boolean</span></span>|<span data-ttu-id="45808-158">阻止到设备的有状态 FTP 连接</span><span class="sxs-lookup"><span data-stu-id="45808-158">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="45808-159">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="45808-159">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="45808-160">Int32</span><span class="sxs-lookup"><span data-stu-id="45808-160">Int32</span></span>|<span data-ttu-id="45808-161">配置安全关联的空闲超时（以秒为单位），值范围为 300 到 3600（包括这两个值）。</span><span class="sxs-lookup"><span data-stu-id="45808-161">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="45808-162">这是一个时间段，在此之后安全关联将过期并被删除。</span><span class="sxs-lookup"><span data-stu-id="45808-162">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="45808-163">有效值为 300 至 3600</span><span class="sxs-lookup"><span data-stu-id="45808-163">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="45808-164">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="45808-164">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="45808-165">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="45808-165">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="45808-166">选择要使用的预共享密钥编码。</span><span class="sxs-lookup"><span data-stu-id="45808-166">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="45808-167">可取值为：`deviceDefault`、`none`、`utF8`。</span><span class="sxs-lookup"><span data-stu-id="45808-167">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="45808-168">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="45808-168">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="45808-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-169">Boolean</span></span>|<span data-ttu-id="45808-170">配置 IPSec 免除项以允许邻居发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="45808-170">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="45808-171">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="45808-171">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="45808-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-172">Boolean</span></span>|<span data-ttu-id="45808-173">配置 IPSec 免除项以允许 ICMP</span><span class="sxs-lookup"><span data-stu-id="45808-173">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="45808-174">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="45808-174">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="45808-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-175">Boolean</span></span>|<span data-ttu-id="45808-176">配置 IPSec 免除项以允许路由器发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="45808-176">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="45808-177">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="45808-177">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="45808-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-178">Boolean</span></span>|<span data-ttu-id="45808-179">配置 IPSec 免除项以允许 IPv4 和 IPv6 DHCP 通信</span><span class="sxs-lookup"><span data-stu-id="45808-179">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="45808-180">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="45808-180">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="45808-181">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="45808-181">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="45808-182">指定如何强制执行证书吊销列表。</span><span class="sxs-lookup"><span data-stu-id="45808-182">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="45808-183">可取值为：`deviceDefault`、`none`、`attempt`、`require`。</span><span class="sxs-lookup"><span data-stu-id="45808-183">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="45808-184">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="45808-184">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="45808-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-185">Boolean</span></span>|<span data-ttu-id="45808-186">如果键控模块不完全支持身份验证集，请指示模块仅忽略不受支持的身份验证套件而不是整个集</span><span class="sxs-lookup"><span data-stu-id="45808-186">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="45808-187">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="45808-187">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="45808-188">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="45808-188">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="45808-189">配置如何在隧道网关应用场景中应用数据包排队。</span><span class="sxs-lookup"><span data-stu-id="45808-189">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="45808-190">可取值为：`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth`。</span><span class="sxs-lookup"><span data-stu-id="45808-190">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="45808-191">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="45808-191">firewallProfileDomain</span></span>|[<span data-ttu-id="45808-192">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="45808-192">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="45808-193">配置域网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="45808-193">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="45808-194">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="45808-194">firewallProfilePublic</span></span>|[<span data-ttu-id="45808-195">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="45808-195">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="45808-196">配置公用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="45808-196">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="45808-197">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="45808-197">firewallProfilePrivate</span></span>|[<span data-ttu-id="45808-198">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="45808-198">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="45808-199">配置专用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="45808-199">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="45808-200">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="45808-200">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="45808-201">String collection</span><span class="sxs-lookup"><span data-stu-id="45808-201">String collection</span></span>|<span data-ttu-id="45808-202">要从攻击面减少规则中排除的 exe 文件和文件夹的列表</span><span class="sxs-lookup"><span data-stu-id="45808-202">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="45808-203">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="45808-203">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="45808-204">String collection</span><span class="sxs-lookup"><span data-stu-id="45808-204">String collection</span></span>|<span data-ttu-id="45808-205">允许访问受保护文件夹的 exe 路径列表</span><span class="sxs-lookup"><span data-stu-id="45808-205">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="45808-206">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="45808-206">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="45808-207">String 集合</span><span class="sxs-lookup"><span data-stu-id="45808-207">String collection</span></span>|<span data-ttu-id="45808-208">要添加到受保护文件夹列表的文件夹路径列表</span><span class="sxs-lookup"><span data-stu-id="45808-208">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="45808-209">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="45808-209">defenderExploitProtectionXml</span></span>|<span data-ttu-id="45808-210">Binary</span><span class="sxs-lookup"><span data-stu-id="45808-210">Binary</span></span>|<span data-ttu-id="45808-211">包含有关 Exploit Protection 详细信息的 xml 内容。</span><span class="sxs-lookup"><span data-stu-id="45808-211">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="45808-212">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="45808-212">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="45808-213">String</span><span class="sxs-lookup"><span data-stu-id="45808-213">String</span></span>|<span data-ttu-id="45808-214">从中获取 DefenderExploitProtectionXml 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="45808-214">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="45808-215">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="45808-215">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="45808-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-216">Boolean</span></span>|<span data-ttu-id="45808-217">指示是否阻止用户覆盖 Exploit Protection 设置。</span><span class="sxs-lookup"><span data-stu-id="45808-217">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="45808-218">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="45808-218">appLockerApplicationControl</span></span>|[<span data-ttu-id="45808-219">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="45808-219">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="45808-220">使管理员能够选择在设备上允许哪些类型的应用。</span><span class="sxs-lookup"><span data-stu-id="45808-220">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="45808-221">可取值为：`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker`。</span><span class="sxs-lookup"><span data-stu-id="45808-221">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="45808-222">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="45808-222">smartScreenEnableInShell</span></span>|<span data-ttu-id="45808-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-223">Boolean</span></span>|<span data-ttu-id="45808-224">允许 IT 管理员配置适用于 Windows 的 SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="45808-224">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="45808-225">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="45808-225">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="45808-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-226">Boolean</span></span>|<span data-ttu-id="45808-227">允许 IT 管理员控制用户是否可以忽略 SmartScreen 警告并运行恶意文件。</span><span class="sxs-lookup"><span data-stu-id="45808-227">Allows IT Admins to control whether users can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="45808-228">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="45808-228">applicationGuardEnabled</span></span>|<span data-ttu-id="45808-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-229">Boolean</span></span>|<span data-ttu-id="45808-230">启用 Windows Defender 应用程序防护</span><span class="sxs-lookup"><span data-stu-id="45808-230">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="45808-231">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="45808-231">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="45808-232">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="45808-232">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="45808-233">阻止剪贴板传输图像文件、文本文件或二者都不。</span><span class="sxs-lookup"><span data-stu-id="45808-233">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="45808-234">可取值为：`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile`。</span><span class="sxs-lookup"><span data-stu-id="45808-234">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="45808-235">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="45808-235">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="45808-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-236">Boolean</span></span>|<span data-ttu-id="45808-237">阻止企业站点加载非企业内容，例如第三方插件</span><span class="sxs-lookup"><span data-stu-id="45808-237">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="45808-238">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="45808-238">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="45808-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-239">Boolean</span></span>|<span data-ttu-id="45808-240">允许 App Guard 容器（收藏夹、Cookie、Web 密码等）内的持久用户生成数据</span><span class="sxs-lookup"><span data-stu-id="45808-240">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="45808-241">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="45808-241">applicationGuardForceAuditing</span></span>|<span data-ttu-id="45808-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-242">Boolean</span></span>|<span data-ttu-id="45808-243">强制审核将存留 Windows 日志和事件以满足安全/符合性条件（示例事件是用户登录注销、特权使用、软件安装、系统更改等）</span><span class="sxs-lookup"><span data-stu-id="45808-243">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="45808-244">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="45808-244">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="45808-245">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="45808-245">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="45808-246">阻止剪贴板将数据从主机共享到容器或从容器共享到主机，或阻止两种方式，或两种方式均不阻止。</span><span class="sxs-lookup"><span data-stu-id="45808-246">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="45808-247">可取值为：`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone`。</span><span class="sxs-lookup"><span data-stu-id="45808-247">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="45808-248">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="45808-248">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="45808-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-249">Boolean</span></span>|<span data-ttu-id="45808-250">允许从容器打印为 PDF 格式</span><span class="sxs-lookup"><span data-stu-id="45808-250">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="45808-251">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="45808-251">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="45808-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-252">Boolean</span></span>|<span data-ttu-id="45808-253">允许从容器打印为 XPS 格式</span><span class="sxs-lookup"><span data-stu-id="45808-253">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="45808-254">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="45808-254">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="45808-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-255">Boolean</span></span>|<span data-ttu-id="45808-256">允许从容器打印到本地打印机</span><span class="sxs-lookup"><span data-stu-id="45808-256">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="45808-257">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="45808-257">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="45808-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-258">Boolean</span></span>|<span data-ttu-id="45808-259">允许从容器打印到网络打印机</span><span class="sxs-lookup"><span data-stu-id="45808-259">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="45808-260">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="45808-260">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="45808-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-261">Boolean</span></span>|<span data-ttu-id="45808-262">允许管理员禁用对用户计算机上其他磁盘加密的警告提示。</span><span class="sxs-lookup"><span data-stu-id="45808-262">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="45808-263">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="45808-263">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="45808-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-264">Boolean</span></span>|<span data-ttu-id="45808-265">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="45808-265">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="45808-266">此策略仅适用于移动 SKU。</span><span class="sxs-lookup"><span data-stu-id="45808-266">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="45808-267">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="45808-267">bitLockerEncryptDevice</span></span>|<span data-ttu-id="45808-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="45808-268">Boolean</span></span>|<span data-ttu-id="45808-269">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="45808-269">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="45808-270">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="45808-270">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="45808-271">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="45808-271">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="45808-272">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="45808-272">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="45808-273">响应</span><span class="sxs-lookup"><span data-stu-id="45808-273">Response</span></span>
<span data-ttu-id="45808-274">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="45808-274">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45808-275">示例</span><span class="sxs-lookup"><span data-stu-id="45808-275">Example</span></span>

### <a name="request"></a><span data-ttu-id="45808-276">请求</span><span class="sxs-lookup"><span data-stu-id="45808-276">Request</span></span>
<span data-ttu-id="45808-277">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="45808-277">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="45808-278">响应</span><span class="sxs-lookup"><span data-stu-id="45808-278">Response</span></span>
<span data-ttu-id="45808-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="45808-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




