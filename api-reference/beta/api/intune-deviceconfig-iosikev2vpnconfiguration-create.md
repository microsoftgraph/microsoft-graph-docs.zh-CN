---
title: 创建 iosikEv2VpnConfiguration
description: 创建新的 iosikEv2VpnConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b80b625c96ef25ca060f4a5225b91dc553158d1c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49220733"
---
# <a name="create-iosikev2vpnconfiguration"></a><span data-ttu-id="63180-103">创建 iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="63180-103">Create iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="63180-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63180-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63180-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="63180-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63180-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63180-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63180-107">创建新的 [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="63180-107">Create a new [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63180-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="63180-108">Prerequisites</span></span>
<span data-ttu-id="63180-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63180-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63180-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="63180-111">Permission type</span></span>|<span data-ttu-id="63180-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="63180-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63180-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63180-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63180-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63180-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="63180-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63180-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63180-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="63180-116">Not supported.</span></span>|
|<span data-ttu-id="63180-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="63180-117">Application</span></span>|<span data-ttu-id="63180-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63180-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63180-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63180-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="63180-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="63180-120">Request headers</span></span>
|<span data-ttu-id="63180-121">标头</span><span class="sxs-lookup"><span data-stu-id="63180-121">Header</span></span>|<span data-ttu-id="63180-122">值</span><span class="sxs-lookup"><span data-stu-id="63180-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63180-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="63180-123">Authorization</span></span>|<span data-ttu-id="63180-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="63180-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63180-125">接受</span><span class="sxs-lookup"><span data-stu-id="63180-125">Accept</span></span>|<span data-ttu-id="63180-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63180-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63180-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="63180-127">Request body</span></span>
<span data-ttu-id="63180-128">在请求正文中，提供 iosikEv2VpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63180-128">In the request body, supply a JSON representation for the iosikEv2VpnConfiguration object.</span></span>

<span data-ttu-id="63180-129">下表显示创建 iosikEv2VpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="63180-129">The following table shows the properties that are required when you create the iosikEv2VpnConfiguration.</span></span>

|<span data-ttu-id="63180-130">属性</span><span class="sxs-lookup"><span data-stu-id="63180-130">Property</span></span>|<span data-ttu-id="63180-131">类型</span><span class="sxs-lookup"><span data-stu-id="63180-131">Type</span></span>|<span data-ttu-id="63180-132">说明</span><span class="sxs-lookup"><span data-stu-id="63180-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63180-133">id</span><span class="sxs-lookup"><span data-stu-id="63180-133">id</span></span>|<span data-ttu-id="63180-134">String</span><span class="sxs-lookup"><span data-stu-id="63180-134">String</span></span>|<span data-ttu-id="63180-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="63180-135">Key of the entity.</span></span> <span data-ttu-id="63180-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63180-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="63180-137">lastModifiedDateTime</span></span>|<span data-ttu-id="63180-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63180-138">DateTimeOffset</span></span>|<span data-ttu-id="63180-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="63180-139">DateTime the object was last modified.</span></span> <span data-ttu-id="63180-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63180-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="63180-141">roleScopeTagIds</span></span>|<span data-ttu-id="63180-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="63180-142">String collection</span></span>|<span data-ttu-id="63180-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="63180-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="63180-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63180-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="63180-145">supportsScopeTags</span></span>|<span data-ttu-id="63180-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="63180-146">Boolean</span></span>|<span data-ttu-id="63180-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="63180-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="63180-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="63180-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="63180-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="63180-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="63180-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="63180-150">This property is read-only.</span></span> <span data-ttu-id="63180-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63180-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="63180-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="63180-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="63180-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="63180-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="63180-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="63180-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63180-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="63180-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="63180-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="63180-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="63180-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="63180-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="63180-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63180-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="63180-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="63180-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="63180-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="63180-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="63180-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="63180-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63180-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="63180-164">createdDateTime</span></span>|<span data-ttu-id="63180-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63180-165">DateTimeOffset</span></span>|<span data-ttu-id="63180-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="63180-166">DateTime the object was created.</span></span> <span data-ttu-id="63180-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63180-168">description</span><span class="sxs-lookup"><span data-stu-id="63180-168">description</span></span>|<span data-ttu-id="63180-169">String</span><span class="sxs-lookup"><span data-stu-id="63180-169">String</span></span>|<span data-ttu-id="63180-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="63180-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="63180-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63180-172">displayName</span><span class="sxs-lookup"><span data-stu-id="63180-172">displayName</span></span>|<span data-ttu-id="63180-173">String</span><span class="sxs-lookup"><span data-stu-id="63180-173">String</span></span>|<span data-ttu-id="63180-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="63180-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="63180-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63180-176">version</span><span class="sxs-lookup"><span data-stu-id="63180-176">version</span></span>|<span data-ttu-id="63180-177">Int32</span><span class="sxs-lookup"><span data-stu-id="63180-177">Int32</span></span>|<span data-ttu-id="63180-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="63180-178">Version of the device configuration.</span></span> <span data-ttu-id="63180-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63180-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="63180-180">connectionName</span></span>|<span data-ttu-id="63180-181">String</span><span class="sxs-lookup"><span data-stu-id="63180-181">String</span></span>|<span data-ttu-id="63180-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="63180-182">Connection name displayed to the user.</span></span> <span data-ttu-id="63180-183">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="63180-184">connectionType</span></span>|[<span data-ttu-id="63180-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="63180-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="63180-186">连接类型。</span><span class="sxs-lookup"><span data-stu-id="63180-186">Connection type.</span></span> <span data-ttu-id="63180-187">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="63180-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="63180-188">可能的值为：、、、、、、、、、、、、、、、、、、 `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` 。</span><span class="sxs-lookup"><span data-stu-id="63180-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="63180-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="63180-189">loginGroupOrDomain</span></span>|<span data-ttu-id="63180-190">String</span><span class="sxs-lookup"><span data-stu-id="63180-190">String</span></span>|<span data-ttu-id="63180-191">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="63180-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="63180-192">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-193">role</span><span class="sxs-lookup"><span data-stu-id="63180-193">role</span></span>|<span data-ttu-id="63180-194">String</span><span class="sxs-lookup"><span data-stu-id="63180-194">String</span></span>|<span data-ttu-id="63180-195">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="63180-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="63180-196">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-197">型</span><span class="sxs-lookup"><span data-stu-id="63180-197">realm</span></span>|<span data-ttu-id="63180-198">String</span><span class="sxs-lookup"><span data-stu-id="63180-198">String</span></span>|<span data-ttu-id="63180-199">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="63180-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="63180-200">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-201">服务器主板</span><span class="sxs-lookup"><span data-stu-id="63180-201">server</span></span>|[<span data-ttu-id="63180-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="63180-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="63180-203">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="63180-203">VPN Server on the network.</span></span> <span data-ttu-id="63180-204">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="63180-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="63180-205">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-206">标识符</span><span class="sxs-lookup"><span data-stu-id="63180-206">identifier</span></span>|<span data-ttu-id="63180-207">String</span><span class="sxs-lookup"><span data-stu-id="63180-207">String</span></span>|<span data-ttu-id="63180-208">当连接类型设置为自定义 VPN 时，由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="63180-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="63180-209">例如： Cisco AnyConnect 使用从[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)继承的 AnyConnect applevpn 的标识符。</span><span class="sxs-lookup"><span data-stu-id="63180-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-210">customData</span><span class="sxs-lookup"><span data-stu-id="63180-210">customData</span></span>|<span data-ttu-id="63180-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="63180-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="63180-212">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="63180-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="63180-213">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="63180-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="63180-214">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="63180-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="63180-215">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="63180-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="63180-216">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="63180-217">customKeyValueData</span></span>|<span data-ttu-id="63180-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="63180-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="63180-219">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="63180-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="63180-220">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="63180-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="63180-221">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="63180-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="63180-222">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="63180-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="63180-223">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="63180-224">enableSplitTunneling</span></span>|<span data-ttu-id="63180-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="63180-225">Boolean</span></span>|<span data-ttu-id="63180-226">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="63180-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="63180-227">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="63180-228">authenticationMethod</span></span>|[<span data-ttu-id="63180-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="63180-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="63180-230">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="63180-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="63180-231">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="63180-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="63180-232">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="63180-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="63180-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="63180-233">enablePerApp</span></span>|<span data-ttu-id="63180-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="63180-234">Boolean</span></span>|<span data-ttu-id="63180-235">如果将此设置为 true，则会创建 Per-App VPN 有效负载，以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="63180-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="63180-236">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="63180-237">safariDomains</span></span>|<span data-ttu-id="63180-238">String 集合</span><span class="sxs-lookup"><span data-stu-id="63180-238">String collection</span></span>|<span data-ttu-id="63180-239">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="63180-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="63180-240">除了与此 VPN 关联的应用程序之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="63180-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="63180-241">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="63180-242">onDemandRules</span></span>|<span data-ttu-id="63180-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="63180-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="63180-244">按需规则。</span><span class="sxs-lookup"><span data-stu-id="63180-244">On-Demand Rules.</span></span> <span data-ttu-id="63180-245">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="63180-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="63180-246">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-247">providerType</span><span class="sxs-lookup"><span data-stu-id="63180-247">providerType</span></span>|[<span data-ttu-id="63180-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="63180-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="63180-249">每应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="63180-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="63180-250">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="63180-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="63180-251">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="63180-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="63180-252">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="63180-252">excludedDomains</span></span>|<span data-ttu-id="63180-253">String 集合</span><span class="sxs-lookup"><span data-stu-id="63180-253">String collection</span></span>|<span data-ttu-id="63180-254">通过公用 internet 而不是通过 VPN 访问的域，即使已从[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)继承每个应用 VPN 也是如此</span><span class="sxs-lookup"><span data-stu-id="63180-254">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-255">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="63180-255">disableOnDemandUserOverride</span></span>|<span data-ttu-id="63180-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="63180-256">Boolean</span></span>|<span data-ttu-id="63180-257">切换以防止用户在从[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)继承的设置应用程序中禁用自动 VPN</span><span class="sxs-lookup"><span data-stu-id="63180-257">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-258">proxyServer</span><span class="sxs-lookup"><span data-stu-id="63180-258">proxyServer</span></span>|[<span data-ttu-id="63180-259">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="63180-259">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="63180-260">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="63180-260">Proxy Server.</span></span> <span data-ttu-id="63180-261">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-261">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-262">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="63180-262">optInToDeviceIdSharing</span></span>|<span data-ttu-id="63180-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="63180-263">Boolean</span></span>|<span data-ttu-id="63180-264">Opt-In 将设备的 Id 共享到第三方 vpn 客户端，以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="63180-264">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="63180-265">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-265">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-266">userDomain</span><span class="sxs-lookup"><span data-stu-id="63180-266">userDomain</span></span>|<span data-ttu-id="63180-267">String</span><span class="sxs-lookup"><span data-stu-id="63180-267">String</span></span>|<span data-ttu-id="63180-268">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="63180-268">Zscaler only.</span></span> <span data-ttu-id="63180-269">输入一个静态域，以便在 Zscaler 应用程序中预填充 "登录" 字段。</span><span class="sxs-lookup"><span data-stu-id="63180-269">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="63180-270">如果保留为空，则将改用用户的 Azure Active Directory 域。</span><span class="sxs-lookup"><span data-stu-id="63180-270">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="63180-271">继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-271">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-272">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="63180-272">strictEnforcement</span></span>|<span data-ttu-id="63180-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="63180-273">Boolean</span></span>|<span data-ttu-id="63180-274">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="63180-274">Zscaler only.</span></span> <span data-ttu-id="63180-275">阻止网络流量，直到用户登录到 Zscaler 应用程序。</span><span class="sxs-lookup"><span data-stu-id="63180-275">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="63180-276">"True" 表示阻止流量。</span><span class="sxs-lookup"><span data-stu-id="63180-276">"True" means traffic is blocked.</span></span> <span data-ttu-id="63180-277">继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-277">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-278">cloudName</span><span class="sxs-lookup"><span data-stu-id="63180-278">cloudName</span></span>|<span data-ttu-id="63180-279">String</span><span class="sxs-lookup"><span data-stu-id="63180-279">String</span></span>|<span data-ttu-id="63180-280">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="63180-280">Zscaler only.</span></span> <span data-ttu-id="63180-281">用户分配到的 Zscaler 云。</span><span class="sxs-lookup"><span data-stu-id="63180-281">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="63180-282">继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-282">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-283">excludeList</span><span class="sxs-lookup"><span data-stu-id="63180-283">excludeList</span></span>|<span data-ttu-id="63180-284">String 集合</span><span class="sxs-lookup"><span data-stu-id="63180-284">String collection</span></span>|<span data-ttu-id="63180-285">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="63180-285">Zscaler only.</span></span> <span data-ttu-id="63180-286">不通过 Zscaler 云发送的网络地址的列表。</span><span class="sxs-lookup"><span data-stu-id="63180-286">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="63180-287">继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-287">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-288">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="63180-288">targetedMobileApps</span></span>|<span data-ttu-id="63180-289">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="63180-289">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="63180-290">目标移动应用。</span><span class="sxs-lookup"><span data-stu-id="63180-290">Targeted mobile apps.</span></span> <span data-ttu-id="63180-291">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="63180-291">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="63180-292">继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-292">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-293">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="63180-293">microsoftTunnelSiteId</span></span>|<span data-ttu-id="63180-294">String</span><span class="sxs-lookup"><span data-stu-id="63180-294">String</span></span>|<span data-ttu-id="63180-295">Microsoft 隧道站点 ID。</span><span class="sxs-lookup"><span data-stu-id="63180-295">Microsoft Tunnel site ID.</span></span> <span data-ttu-id="63180-296">继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63180-296">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="63180-297">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="63180-297">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="63180-298">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="63180-298">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="63180-299">子安全关联参数</span><span class="sxs-lookup"><span data-stu-id="63180-299">Child Security Association Parameters</span></span>|
|<span data-ttu-id="63180-300">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="63180-300">clientAuthenticationType</span></span>|[<span data-ttu-id="63180-301">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="63180-301">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="63180-302">VPN 客户端将使用的客户端身份验证的类型。</span><span class="sxs-lookup"><span data-stu-id="63180-302">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="63180-303">可取值为：`userAuthentication`、`deviceAuthentication`。</span><span class="sxs-lookup"><span data-stu-id="63180-303">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="63180-304">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="63180-304">deadPeerDetectionRate</span></span>|[<span data-ttu-id="63180-305">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="63180-305">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="63180-306">确定检查等连接是否仍处于活动状态的频率。</span><span class="sxs-lookup"><span data-stu-id="63180-306">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="63180-307">.</span><span class="sxs-lookup"><span data-stu-id="63180-307">.</span></span> <span data-ttu-id="63180-308">可取值为：`medium`、`none`、`low`、`high`。</span><span class="sxs-lookup"><span data-stu-id="63180-308">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="63180-309">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="63180-309">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="63180-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="63180-310">Boolean</span></span>|<span data-ttu-id="63180-311">禁用 MOBIKE</span><span class="sxs-lookup"><span data-stu-id="63180-311">Disable MOBIKE</span></span>|
|<span data-ttu-id="63180-312">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="63180-312">disableRedirect</span></span>|<span data-ttu-id="63180-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="63180-313">Boolean</span></span>|<span data-ttu-id="63180-314">禁用重定向</span><span class="sxs-lookup"><span data-stu-id="63180-314">Disable Redirect</span></span>|
|<span data-ttu-id="63180-315">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="63180-315">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="63180-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="63180-316">Boolean</span></span>|<span data-ttu-id="63180-317">启用尽力吊销检查;服务器响应超时不会导致它失败</span><span class="sxs-lookup"><span data-stu-id="63180-317">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="63180-318">enableEAP</span><span class="sxs-lookup"><span data-stu-id="63180-318">enableEAP</span></span>|<span data-ttu-id="63180-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="63180-319">Boolean</span></span>|<span data-ttu-id="63180-320">启用仅 EAP 身份验证</span><span class="sxs-lookup"><span data-stu-id="63180-320">Enables EAP only authentication</span></span>|
|<span data-ttu-id="63180-321">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="63180-321">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="63180-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="63180-322">Boolean</span></span>|<span data-ttu-id="63180-323">启用完全向前保密 (PFS) 。</span><span class="sxs-lookup"><span data-stu-id="63180-323">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="63180-324">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="63180-324">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="63180-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="63180-325">Boolean</span></span>|<span data-ttu-id="63180-326">启用 "使用内部子网属性"。</span><span class="sxs-lookup"><span data-stu-id="63180-326">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="63180-327">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="63180-327">localIdentifier</span></span>|[<span data-ttu-id="63180-328">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="63180-328">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="63180-329">标识尝试通过 VPN 连接的客户端的方法。</span><span class="sxs-lookup"><span data-stu-id="63180-329">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="63180-330">.</span><span class="sxs-lookup"><span data-stu-id="63180-330">.</span></span> <span data-ttu-id="63180-331">可取值为：`deviceFQDN`、`empty`、`clientCertificateSubjectName`。</span><span class="sxs-lookup"><span data-stu-id="63180-331">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="63180-332">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="63180-332">remoteIdentifier</span></span>|<span data-ttu-id="63180-333">String</span><span class="sxs-lookup"><span data-stu-id="63180-333">String</span></span>|<span data-ttu-id="63180-334">IKEv2 服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="63180-334">Address of the IKEv2 server.</span></span> <span data-ttu-id="63180-335">必须是 FQDN、UserFQDN、网络地址或 ASN1DN</span><span class="sxs-lookup"><span data-stu-id="63180-335">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="63180-336">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="63180-336">securityAssociationParameters</span></span>|[<span data-ttu-id="63180-337">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="63180-337">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="63180-338">安全关联参数</span><span class="sxs-lookup"><span data-stu-id="63180-338">Security Association Parameters</span></span>|
|<span data-ttu-id="63180-339">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="63180-339">serverCertificateCommonName</span></span>|<span data-ttu-id="63180-340">String</span><span class="sxs-lookup"><span data-stu-id="63180-340">String</span></span>|<span data-ttu-id="63180-341">服务器身份验证中使用的 IKEv2 服务器证书的公用名</span><span class="sxs-lookup"><span data-stu-id="63180-341">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="63180-342">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="63180-342">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="63180-343">String</span><span class="sxs-lookup"><span data-stu-id="63180-343">String</span></span>|<span data-ttu-id="63180-344">身份验证中使用的 IKEv2 服务器证书颁发者的颁发者公用名称</span><span class="sxs-lookup"><span data-stu-id="63180-344">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="63180-345">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="63180-345">serverCertificateType</span></span>|[<span data-ttu-id="63180-346">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="63180-346">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="63180-347">VPN 服务器将提供给 VPN 客户端进行身份验证的证书类型。</span><span class="sxs-lookup"><span data-stu-id="63180-347">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="63180-348">可取值为：`rsa`、`ecdsa256`、`ecdsa384`、`ecdsa521`。</span><span class="sxs-lookup"><span data-stu-id="63180-348">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="63180-349">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="63180-349">sharedSecret</span></span>|<span data-ttu-id="63180-350">String</span><span class="sxs-lookup"><span data-stu-id="63180-350">String</span></span>|<span data-ttu-id="63180-351">在选择共享密钥身份验证时使用</span><span class="sxs-lookup"><span data-stu-id="63180-351">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="63180-352">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="63180-352">tlsMaximumVersion</span></span>|<span data-ttu-id="63180-353">String</span><span class="sxs-lookup"><span data-stu-id="63180-353">String</span></span>|<span data-ttu-id="63180-354">要与 EAP-TLS 身份验证一起使用的最大 TLS 版本</span><span class="sxs-lookup"><span data-stu-id="63180-354">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="63180-355">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="63180-355">tlsMinimumVersion</span></span>|<span data-ttu-id="63180-356">String</span><span class="sxs-lookup"><span data-stu-id="63180-356">String</span></span>|<span data-ttu-id="63180-357">与 EAP-TLS 身份验证一起使用的最小 TLS 版本</span><span class="sxs-lookup"><span data-stu-id="63180-357">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="63180-358">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="63180-358">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="63180-359">Boolean</span><span class="sxs-lookup"><span data-stu-id="63180-359">Boolean</span></span>|<span data-ttu-id="63180-360">允许使用安全关联参数，具体方法是将所有参数设置为设备的默认值，除非明确指定。</span><span class="sxs-lookup"><span data-stu-id="63180-360">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="63180-361">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="63180-361">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="63180-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="63180-362">Boolean</span></span>|<span data-ttu-id="63180-363">允许使用子安全关联参数，具体方法是将所有参数设置为设备的默认值，除非明确指定。</span><span class="sxs-lookup"><span data-stu-id="63180-363">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="63180-364">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="63180-364">alwaysOnConfiguration</span></span>|[<span data-ttu-id="63180-365">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="63180-365">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="63180-366">AlwaysOn 配置</span><span class="sxs-lookup"><span data-stu-id="63180-366">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="63180-367">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="63180-367">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="63180-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="63180-368">Boolean</span></span>|<span data-ttu-id="63180-369">确定是否始终启用 VPN</span><span class="sxs-lookup"><span data-stu-id="63180-369">Determines if Always on VPN is enabled</span></span>|
|<span data-ttu-id="63180-370">mtuSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="63180-370">mtuSizeInBytes</span></span>|<span data-ttu-id="63180-371">Int32</span><span class="sxs-lookup"><span data-stu-id="63180-371">Int32</span></span>|<span data-ttu-id="63180-372">最大传输单位。</span><span class="sxs-lookup"><span data-stu-id="63180-372">Maximum transmission unit.</span></span> <span data-ttu-id="63180-373">有效值为1至65536</span><span class="sxs-lookup"><span data-stu-id="63180-373">Valid values 1 to 65536</span></span>|



## <a name="response"></a><span data-ttu-id="63180-374">响应</span><span class="sxs-lookup"><span data-stu-id="63180-374">Response</span></span>
<span data-ttu-id="63180-375">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="63180-375">If successful, this method returns a `201 Created` response code and a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63180-376">示例</span><span class="sxs-lookup"><span data-stu-id="63180-376">Example</span></span>

### <a name="request"></a><span data-ttu-id="63180-377">请求</span><span class="sxs-lookup"><span data-stu-id="63180-377">Request</span></span>
<span data-ttu-id="63180-378">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="63180-378">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 5428

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
  "providerType": "appProxy",
  "excludedDomains": [
    "Excluded Domains value"
  ],
  "disableOnDemandUserOverride": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value",
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
  "enableAlwaysOnConfiguration": true,
  "mtuSizeInBytes": 14
}
```

### <a name="response"></a><span data-ttu-id="63180-379">响应</span><span class="sxs-lookup"><span data-stu-id="63180-379">Response</span></span>
<span data-ttu-id="63180-p142">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="63180-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 5600

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
  "providerType": "appProxy",
  "excludedDomains": [
    "Excluded Domains value"
  ],
  "disableOnDemandUserOverride": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value",
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
  "enableAlwaysOnConfiguration": true,
  "mtuSizeInBytes": 14
}
```




