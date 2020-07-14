---
title: 创建 iosikEv2VpnConfiguration
description: 创建新的 iosikEv2VpnConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aff0878c6bd2a921fc5f1c40a072555a6524d383
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123125"
---
# <a name="create-iosikev2vpnconfiguration"></a><span data-ttu-id="c944d-103">创建 iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c944d-103">Create iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="c944d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c944d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c944d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c944d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c944d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c944d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c944d-107">创建新的[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c944d-107">Create a new [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c944d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c944d-108">Prerequisites</span></span>
<span data-ttu-id="c944d-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c944d-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c944d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c944d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c944d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c944d-111">Permission type</span></span>|<span data-ttu-id="c944d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c944d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c944d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c944d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c944d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c944d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c944d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c944d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c944d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c944d-116">Not supported.</span></span>|
|<span data-ttu-id="c944d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c944d-117">Application</span></span>|<span data-ttu-id="c944d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c944d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c944d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c944d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c944d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c944d-120">Request headers</span></span>
|<span data-ttu-id="c944d-121">标头</span><span class="sxs-lookup"><span data-stu-id="c944d-121">Header</span></span>|<span data-ttu-id="c944d-122">值</span><span class="sxs-lookup"><span data-stu-id="c944d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c944d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c944d-123">Authorization</span></span>|<span data-ttu-id="c944d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c944d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c944d-125">接受</span><span class="sxs-lookup"><span data-stu-id="c944d-125">Accept</span></span>|<span data-ttu-id="c944d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c944d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c944d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c944d-127">Request body</span></span>
<span data-ttu-id="c944d-128">在请求正文中，提供 iosikEv2VpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c944d-128">In the request body, supply a JSON representation for the iosikEv2VpnConfiguration object.</span></span>

<span data-ttu-id="c944d-129">下表显示创建 iosikEv2VpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c944d-129">The following table shows the properties that are required when you create the iosikEv2VpnConfiguration.</span></span>

|<span data-ttu-id="c944d-130">属性</span><span class="sxs-lookup"><span data-stu-id="c944d-130">Property</span></span>|<span data-ttu-id="c944d-131">类型</span><span class="sxs-lookup"><span data-stu-id="c944d-131">Type</span></span>|<span data-ttu-id="c944d-132">说明</span><span class="sxs-lookup"><span data-stu-id="c944d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c944d-133">id</span><span class="sxs-lookup"><span data-stu-id="c944d-133">id</span></span>|<span data-ttu-id="c944d-134">字符串</span><span class="sxs-lookup"><span data-stu-id="c944d-134">String</span></span>|<span data-ttu-id="c944d-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c944d-135">Key of the entity.</span></span> <span data-ttu-id="c944d-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c944d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c944d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c944d-138">DateTimeOffset</span></span>|<span data-ttu-id="c944d-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c944d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c944d-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c944d-141">roleScopeTagIds</span></span>|<span data-ttu-id="c944d-142">String collection</span><span class="sxs-lookup"><span data-stu-id="c944d-142">String collection</span></span>|<span data-ttu-id="c944d-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c944d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c944d-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c944d-145">supportsScopeTags</span></span>|<span data-ttu-id="c944d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c944d-146">Boolean</span></span>|<span data-ttu-id="c944d-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="c944d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c944d-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="c944d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c944d-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="c944d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c944d-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c944d-150">This property is read-only.</span></span> <span data-ttu-id="c944d-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c944d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c944d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c944d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c944d-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="c944d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c944d-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c944d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c944d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c944d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c944d-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c944d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c944d-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c944d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c944d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c944d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c944d-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c944d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c944d-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c944d-164">createdDateTime</span></span>|<span data-ttu-id="c944d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c944d-165">DateTimeOffset</span></span>|<span data-ttu-id="c944d-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c944d-166">DateTime the object was created.</span></span> <span data-ttu-id="c944d-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-168">说明</span><span class="sxs-lookup"><span data-stu-id="c944d-168">description</span></span>|<span data-ttu-id="c944d-169">String</span><span class="sxs-lookup"><span data-stu-id="c944d-169">String</span></span>|<span data-ttu-id="c944d-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c944d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c944d-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c944d-172">displayName</span></span>|<span data-ttu-id="c944d-173">String</span><span class="sxs-lookup"><span data-stu-id="c944d-173">String</span></span>|<span data-ttu-id="c944d-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c944d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c944d-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-176">version</span><span class="sxs-lookup"><span data-stu-id="c944d-176">version</span></span>|<span data-ttu-id="c944d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c944d-177">Int32</span></span>|<span data-ttu-id="c944d-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c944d-178">Version of the device configuration.</span></span> <span data-ttu-id="c944d-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="c944d-180">connectionName</span></span>|<span data-ttu-id="c944d-181">String</span><span class="sxs-lookup"><span data-stu-id="c944d-181">String</span></span>|<span data-ttu-id="c944d-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="c944d-182">Connection name displayed to the user.</span></span> <span data-ttu-id="c944d-183">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="c944d-184">connectionType</span></span>|[<span data-ttu-id="c944d-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="c944d-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="c944d-186">连接类型。</span><span class="sxs-lookup"><span data-stu-id="c944d-186">Connection type.</span></span> <span data-ttu-id="c944d-187">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="c944d-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="c944d-188">可能的值是：、、、、、、、、、、、、、、、、 `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` 。</span><span class="sxs-lookup"><span data-stu-id="c944d-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`.</span></span>|
|<span data-ttu-id="c944d-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="c944d-189">loginGroupOrDomain</span></span>|<span data-ttu-id="c944d-190">String</span><span class="sxs-lookup"><span data-stu-id="c944d-190">String</span></span>|<span data-ttu-id="c944d-191">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="c944d-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="c944d-192">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-193">role</span><span class="sxs-lookup"><span data-stu-id="c944d-193">role</span></span>|<span data-ttu-id="c944d-194">String</span><span class="sxs-lookup"><span data-stu-id="c944d-194">String</span></span>|<span data-ttu-id="c944d-195">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="c944d-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="c944d-196">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-197">型</span><span class="sxs-lookup"><span data-stu-id="c944d-197">realm</span></span>|<span data-ttu-id="c944d-198">String</span><span class="sxs-lookup"><span data-stu-id="c944d-198">String</span></span>|<span data-ttu-id="c944d-199">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="c944d-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="c944d-200">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-201">服务器主板</span><span class="sxs-lookup"><span data-stu-id="c944d-201">server</span></span>|[<span data-ttu-id="c944d-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="c944d-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="c944d-203">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="c944d-203">VPN Server on the network.</span></span> <span data-ttu-id="c944d-204">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="c944d-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="c944d-205">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-206">标识符</span><span class="sxs-lookup"><span data-stu-id="c944d-206">identifier</span></span>|<span data-ttu-id="c944d-207">String</span><span class="sxs-lookup"><span data-stu-id="c944d-207">String</span></span>|<span data-ttu-id="c944d-208">当连接类型设置为自定义 VPN 时，由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="c944d-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="c944d-209">例如： Cisco AnyConnect 使用从[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)继承的 AnyConnect applevpn 的标识符。</span><span class="sxs-lookup"><span data-stu-id="c944d-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-210">customData</span><span class="sxs-lookup"><span data-stu-id="c944d-210">customData</span></span>|<span data-ttu-id="c944d-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c944d-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="c944d-212">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="c944d-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="c944d-213">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="c944d-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="c944d-214">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="c944d-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="c944d-215">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="c944d-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="c944d-216">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="c944d-217">customKeyValueData</span></span>|<span data-ttu-id="c944d-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c944d-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c944d-219">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="c944d-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="c944d-220">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="c944d-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="c944d-221">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="c944d-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="c944d-222">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="c944d-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="c944d-223">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="c944d-224">enableSplitTunneling</span></span>|<span data-ttu-id="c944d-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="c944d-225">Boolean</span></span>|<span data-ttu-id="c944d-226">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="c944d-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="c944d-227">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c944d-228">authenticationMethod</span></span>|[<span data-ttu-id="c944d-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c944d-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="c944d-230">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="c944d-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="c944d-231">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="c944d-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="c944d-232">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="c944d-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="c944d-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="c944d-233">enablePerApp</span></span>|<span data-ttu-id="c944d-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="c944d-234">Boolean</span></span>|<span data-ttu-id="c944d-235">将此设置为 true 将创建每个应用程序 VPN 有效负载，以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="c944d-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="c944d-236">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="c944d-237">safariDomains</span></span>|<span data-ttu-id="c944d-238">String collection</span><span class="sxs-lookup"><span data-stu-id="c944d-238">String collection</span></span>|<span data-ttu-id="c944d-239">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="c944d-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="c944d-240">除了与此 VPN 关联的应用程序之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="c944d-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="c944d-241">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="c944d-242">onDemandRules</span></span>|<span data-ttu-id="c944d-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="c944d-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="c944d-244">按需规则。</span><span class="sxs-lookup"><span data-stu-id="c944d-244">On-Demand Rules.</span></span> <span data-ttu-id="c944d-245">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c944d-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c944d-246">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-247">proxyServer</span><span class="sxs-lookup"><span data-stu-id="c944d-247">proxyServer</span></span>|[<span data-ttu-id="c944d-248">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="c944d-248">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="c944d-249">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="c944d-249">Proxy Server.</span></span> <span data-ttu-id="c944d-250">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-251">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="c944d-251">optInToDeviceIdSharing</span></span>|<span data-ttu-id="c944d-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="c944d-252">Boolean</span></span>|<span data-ttu-id="c944d-253">选择将设备的 Id 共享到第三方 vpn 客户端，以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="c944d-253">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="c944d-254">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-254">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-255">providerType</span><span class="sxs-lookup"><span data-stu-id="c944d-255">providerType</span></span>|[<span data-ttu-id="c944d-256">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="c944d-256">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="c944d-257">每应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="c944d-257">Provider type for per-app VPN.</span></span> <span data-ttu-id="c944d-258">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="c944d-258">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="c944d-259">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="c944d-259">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="c944d-260">userDomain</span><span class="sxs-lookup"><span data-stu-id="c944d-260">userDomain</span></span>|<span data-ttu-id="c944d-261">String</span><span class="sxs-lookup"><span data-stu-id="c944d-261">String</span></span>|<span data-ttu-id="c944d-262">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="c944d-262">Zscaler only.</span></span> <span data-ttu-id="c944d-263">输入一个静态域，以便在 Zscaler 应用程序中预填充 "登录" 字段。</span><span class="sxs-lookup"><span data-stu-id="c944d-263">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="c944d-264">如果保留为空，则将改用用户的 Azure Active Directory 域。</span><span class="sxs-lookup"><span data-stu-id="c944d-264">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="c944d-265">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-265">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-266">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="c944d-266">strictEnforcement</span></span>|<span data-ttu-id="c944d-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="c944d-267">Boolean</span></span>|<span data-ttu-id="c944d-268">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="c944d-268">Zscaler only.</span></span> <span data-ttu-id="c944d-269">阻止网络流量，直到用户登录到 Zscaler 应用程序。</span><span class="sxs-lookup"><span data-stu-id="c944d-269">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="c944d-270">"True" 表示阻止流量。</span><span class="sxs-lookup"><span data-stu-id="c944d-270">"True" means traffic is blocked.</span></span> <span data-ttu-id="c944d-271">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-271">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-272">cloudName</span><span class="sxs-lookup"><span data-stu-id="c944d-272">cloudName</span></span>|<span data-ttu-id="c944d-273">String</span><span class="sxs-lookup"><span data-stu-id="c944d-273">String</span></span>|<span data-ttu-id="c944d-274">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="c944d-274">Zscaler only.</span></span> <span data-ttu-id="c944d-275">用户分配到的 Zscaler 云。</span><span class="sxs-lookup"><span data-stu-id="c944d-275">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="c944d-276">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-276">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-277">excludeList</span><span class="sxs-lookup"><span data-stu-id="c944d-277">excludeList</span></span>|<span data-ttu-id="c944d-278">String collection</span><span class="sxs-lookup"><span data-stu-id="c944d-278">String collection</span></span>|<span data-ttu-id="c944d-279">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="c944d-279">Zscaler only.</span></span> <span data-ttu-id="c944d-280">不通过 Zscaler 云发送的网络地址的列表。</span><span class="sxs-lookup"><span data-stu-id="c944d-280">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="c944d-281">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-281">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-282">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="c944d-282">targetedMobileApps</span></span>|<span data-ttu-id="c944d-283">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c944d-283">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c944d-284">目标移动应用。</span><span class="sxs-lookup"><span data-stu-id="c944d-284">Targeted mobile apps.</span></span> <span data-ttu-id="c944d-285">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c944d-285">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c944d-286">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c944d-286">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c944d-287">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="c944d-287">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="c944d-288">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="c944d-288">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="c944d-289">子安全关联参数</span><span class="sxs-lookup"><span data-stu-id="c944d-289">Child Security Association Parameters</span></span>|
|<span data-ttu-id="c944d-290">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="c944d-290">clientAuthenticationType</span></span>|[<span data-ttu-id="c944d-291">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="c944d-291">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="c944d-292">VPN 客户端将使用的客户端身份验证的类型。</span><span class="sxs-lookup"><span data-stu-id="c944d-292">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="c944d-293">可取值为：`userAuthentication`、`deviceAuthentication`。</span><span class="sxs-lookup"><span data-stu-id="c944d-293">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="c944d-294">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="c944d-294">deadPeerDetectionRate</span></span>|[<span data-ttu-id="c944d-295">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="c944d-295">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="c944d-296">确定检查等连接是否仍处于活动状态的频率。</span><span class="sxs-lookup"><span data-stu-id="c944d-296">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="c944d-297">.</span><span class="sxs-lookup"><span data-stu-id="c944d-297">.</span></span> <span data-ttu-id="c944d-298">可取值为：`medium`、`none`、`low`、`high`。</span><span class="sxs-lookup"><span data-stu-id="c944d-298">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="c944d-299">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="c944d-299">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="c944d-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="c944d-300">Boolean</span></span>|<span data-ttu-id="c944d-301">禁用 MOBIKE</span><span class="sxs-lookup"><span data-stu-id="c944d-301">Disable MOBIKE</span></span>|
|<span data-ttu-id="c944d-302">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="c944d-302">disableRedirect</span></span>|<span data-ttu-id="c944d-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="c944d-303">Boolean</span></span>|<span data-ttu-id="c944d-304">禁用重定向</span><span class="sxs-lookup"><span data-stu-id="c944d-304">Disable Redirect</span></span>|
|<span data-ttu-id="c944d-305">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="c944d-305">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="c944d-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="c944d-306">Boolean</span></span>|<span data-ttu-id="c944d-307">启用尽力吊销检查;服务器响应超时不会导致它失败</span><span class="sxs-lookup"><span data-stu-id="c944d-307">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="c944d-308">enableEAP</span><span class="sxs-lookup"><span data-stu-id="c944d-308">enableEAP</span></span>|<span data-ttu-id="c944d-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="c944d-309">Boolean</span></span>|<span data-ttu-id="c944d-310">启用仅 EAP 身份验证</span><span class="sxs-lookup"><span data-stu-id="c944d-310">Enables EAP only authentication</span></span>|
|<span data-ttu-id="c944d-311">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="c944d-311">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="c944d-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="c944d-312">Boolean</span></span>|<span data-ttu-id="c944d-313">启用完全向前保密 (PFS) 。</span><span class="sxs-lookup"><span data-stu-id="c944d-313">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="c944d-314">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="c944d-314">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="c944d-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="c944d-315">Boolean</span></span>|<span data-ttu-id="c944d-316">启用 "使用内部子网属性"。</span><span class="sxs-lookup"><span data-stu-id="c944d-316">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="c944d-317">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="c944d-317">localIdentifier</span></span>|[<span data-ttu-id="c944d-318">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="c944d-318">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="c944d-319">标识尝试通过 VPN 连接的客户端的方法。</span><span class="sxs-lookup"><span data-stu-id="c944d-319">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="c944d-320">.</span><span class="sxs-lookup"><span data-stu-id="c944d-320">.</span></span> <span data-ttu-id="c944d-321">可取值为：`deviceFQDN`、`empty`、`clientCertificateSubjectName`。</span><span class="sxs-lookup"><span data-stu-id="c944d-321">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="c944d-322">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="c944d-322">remoteIdentifier</span></span>|<span data-ttu-id="c944d-323">String</span><span class="sxs-lookup"><span data-stu-id="c944d-323">String</span></span>|<span data-ttu-id="c944d-324">IKEv2 服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="c944d-324">Address of the IKEv2 server.</span></span> <span data-ttu-id="c944d-325">必须是 FQDN、UserFQDN、网络地址或 ASN1DN</span><span class="sxs-lookup"><span data-stu-id="c944d-325">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="c944d-326">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="c944d-326">securityAssociationParameters</span></span>|[<span data-ttu-id="c944d-327">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="c944d-327">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="c944d-328">安全关联参数</span><span class="sxs-lookup"><span data-stu-id="c944d-328">Security Association Parameters</span></span>|
|<span data-ttu-id="c944d-329">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="c944d-329">serverCertificateCommonName</span></span>|<span data-ttu-id="c944d-330">String</span><span class="sxs-lookup"><span data-stu-id="c944d-330">String</span></span>|<span data-ttu-id="c944d-331">服务器身份验证中使用的 IKEv2 服务器证书的公用名</span><span class="sxs-lookup"><span data-stu-id="c944d-331">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="c944d-332">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="c944d-332">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="c944d-333">String</span><span class="sxs-lookup"><span data-stu-id="c944d-333">String</span></span>|<span data-ttu-id="c944d-334">身份验证中使用的 IKEv2 服务器证书颁发者的颁发者公用名称</span><span class="sxs-lookup"><span data-stu-id="c944d-334">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="c944d-335">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="c944d-335">serverCertificateType</span></span>|[<span data-ttu-id="c944d-336">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="c944d-336">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="c944d-337">VPN 服务器将提供给 VPN 客户端进行身份验证的证书类型。</span><span class="sxs-lookup"><span data-stu-id="c944d-337">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="c944d-338">可取值为：`rsa`、`ecdsa256`、`ecdsa384`、`ecdsa521`。</span><span class="sxs-lookup"><span data-stu-id="c944d-338">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="c944d-339">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="c944d-339">sharedSecret</span></span>|<span data-ttu-id="c944d-340">String</span><span class="sxs-lookup"><span data-stu-id="c944d-340">String</span></span>|<span data-ttu-id="c944d-341">在选择共享密钥身份验证时使用</span><span class="sxs-lookup"><span data-stu-id="c944d-341">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="c944d-342">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c944d-342">tlsMaximumVersion</span></span>|<span data-ttu-id="c944d-343">String</span><span class="sxs-lookup"><span data-stu-id="c944d-343">String</span></span>|<span data-ttu-id="c944d-344">要与 EAP-TLS 身份验证一起使用的最大 TLS 版本</span><span class="sxs-lookup"><span data-stu-id="c944d-344">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="c944d-345">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c944d-345">tlsMinimumVersion</span></span>|<span data-ttu-id="c944d-346">String</span><span class="sxs-lookup"><span data-stu-id="c944d-346">String</span></span>|<span data-ttu-id="c944d-347">与 EAP-TLS 身份验证一起使用的最小 TLS 版本</span><span class="sxs-lookup"><span data-stu-id="c944d-347">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="c944d-348">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="c944d-348">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="c944d-349">Boolean</span><span class="sxs-lookup"><span data-stu-id="c944d-349">Boolean</span></span>|<span data-ttu-id="c944d-350">允许使用安全关联参数，具体方法是将所有参数设置为设备的默认值，除非明确指定。</span><span class="sxs-lookup"><span data-stu-id="c944d-350">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="c944d-351">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="c944d-351">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="c944d-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="c944d-352">Boolean</span></span>|<span data-ttu-id="c944d-353">允许使用子安全关联参数，具体方法是将所有参数设置为设备的默认值，除非明确指定。</span><span class="sxs-lookup"><span data-stu-id="c944d-353">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="c944d-354">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c944d-354">alwaysOnConfiguration</span></span>|[<span data-ttu-id="c944d-355">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c944d-355">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="c944d-356">AlwaysOn 配置</span><span class="sxs-lookup"><span data-stu-id="c944d-356">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="c944d-357">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c944d-357">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="c944d-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="c944d-358">Boolean</span></span>|<span data-ttu-id="c944d-359">确定是否始终启用 VPN</span><span class="sxs-lookup"><span data-stu-id="c944d-359">Determines if Always on VPN is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="c944d-360">响应</span><span class="sxs-lookup"><span data-stu-id="c944d-360">Response</span></span>
<span data-ttu-id="c944d-361">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c944d-361">If successful, this method returns a `201 Created` response code and a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c944d-362">示例</span><span class="sxs-lookup"><span data-stu-id="c944d-362">Example</span></span>

### <a name="request"></a><span data-ttu-id="c944d-363">请求</span><span class="sxs-lookup"><span data-stu-id="c944d-363">Request</span></span>
<span data-ttu-id="c944d-364">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c944d-364">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 5241

{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ],
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "clientAuthenticationType": "deviceAuthentication",
  "deadPeerDetectionRate": "none",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "empty",
  "remoteIdentifier": "Remote Identifier value",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "serverCertificateCommonName": "Server Certificate Common Name value",
  "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
  "serverCertificateType": "ecdsa256",
  "sharedSecret": "Shared Secret value",
  "tlsMaximumVersion": "Tls Maximum Version value",
  "tlsMinimumVersion": "Tls Minimum Version value",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true,
  "alwaysOnConfiguration": {
    "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration",
    "tunnelConfiguration": "cellular",
    "userToggleEnabled": true,
    "voicemailExceptionAction": "allowTrafficOutside",
    "airPrintExceptionAction": "allowTrafficOutside",
    "cellularExceptionAction": "allowTrafficOutside",
    "allowAllCaptiveNetworkPlugins": true,
    "allowedCaptiveNetworkPlugins": {
      "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
      "allowedBundleIdentifiers": [
        "Allowed Bundle Identifiers value"
      ]
    },
    "allowCaptiveWebSheet": true,
    "natKeepAliveIntervalInSeconds": 13,
    "natKeepAliveOffloadEnable": true
  },
  "enableAlwaysOnConfiguration": true
}
```

### <a name="response"></a><span data-ttu-id="c944d-365">响应</span><span class="sxs-lookup"><span data-stu-id="c944d-365">Response</span></span>
<span data-ttu-id="c944d-366">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="c944d-366">Here is an example of the response.</span></span> <span data-ttu-id="c944d-367">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="c944d-367">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c944d-368">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="c944d-368">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 5413

{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
  "id": "b87b0327-0327-b87b-2703-7bb827037bb8",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ],
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "clientAuthenticationType": "deviceAuthentication",
  "deadPeerDetectionRate": "none",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "empty",
  "remoteIdentifier": "Remote Identifier value",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "serverCertificateCommonName": "Server Certificate Common Name value",
  "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
  "serverCertificateType": "ecdsa256",
  "sharedSecret": "Shared Secret value",
  "tlsMaximumVersion": "Tls Maximum Version value",
  "tlsMinimumVersion": "Tls Minimum Version value",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true,
  "alwaysOnConfiguration": {
    "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration",
    "tunnelConfiguration": "cellular",
    "userToggleEnabled": true,
    "voicemailExceptionAction": "allowTrafficOutside",
    "airPrintExceptionAction": "allowTrafficOutside",
    "cellularExceptionAction": "allowTrafficOutside",
    "allowAllCaptiveNetworkPlugins": true,
    "allowedCaptiveNetworkPlugins": {
      "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
      "allowedBundleIdentifiers": [
        "Allowed Bundle Identifiers value"
      ]
    },
    "allowCaptiveWebSheet": true,
    "natKeepAliveIntervalInSeconds": 13,
    "natKeepAliveOffloadEnable": true
  },
  "enableAlwaysOnConfiguration": true
}
```



