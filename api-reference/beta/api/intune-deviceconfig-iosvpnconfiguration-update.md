---
title: 更新 iosVpnConfiguration
description: 更新 iosVpnConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eaca743801259af26ff414707b07553b142f2e60
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790901"
---
# <a name="update-iosvpnconfiguration"></a><span data-ttu-id="83254-103">更新 iosVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="83254-103">Update iosVpnConfiguration</span></span>

<span data-ttu-id="83254-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83254-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83254-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="83254-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83254-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="83254-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83254-107">更新 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="83254-107">Update the properties of a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83254-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="83254-108">Prerequisites</span></span>
<span data-ttu-id="83254-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="83254-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83254-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="83254-111">Permission type</span></span>|<span data-ttu-id="83254-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="83254-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83254-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83254-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83254-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83254-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="83254-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83254-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83254-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="83254-116">Not supported.</span></span>|
|<span data-ttu-id="83254-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="83254-117">Application</span></span>|<span data-ttu-id="83254-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83254-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="83254-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83254-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="83254-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="83254-120">Request headers</span></span>
|<span data-ttu-id="83254-121">标头</span><span class="sxs-lookup"><span data-stu-id="83254-121">Header</span></span>|<span data-ttu-id="83254-122">值</span><span class="sxs-lookup"><span data-stu-id="83254-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83254-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83254-123">Authorization</span></span>|<span data-ttu-id="83254-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="83254-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83254-125">接受</span><span class="sxs-lookup"><span data-stu-id="83254-125">Accept</span></span>|<span data-ttu-id="83254-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83254-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83254-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="83254-127">Request body</span></span>
<span data-ttu-id="83254-128">在请求正文中，提供 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83254-128">In the request body, supply a JSON representation for the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="83254-129">下表显示创建 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="83254-129">The following table shows the properties that are required when you create the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span>

|<span data-ttu-id="83254-130">属性</span><span class="sxs-lookup"><span data-stu-id="83254-130">Property</span></span>|<span data-ttu-id="83254-131">类型</span><span class="sxs-lookup"><span data-stu-id="83254-131">Type</span></span>|<span data-ttu-id="83254-132">说明</span><span class="sxs-lookup"><span data-stu-id="83254-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83254-133">id</span><span class="sxs-lookup"><span data-stu-id="83254-133">id</span></span>|<span data-ttu-id="83254-134">String</span><span class="sxs-lookup"><span data-stu-id="83254-134">String</span></span>|<span data-ttu-id="83254-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="83254-135">Key of the entity.</span></span> <span data-ttu-id="83254-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83254-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83254-137">lastModifiedDateTime</span></span>|<span data-ttu-id="83254-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83254-138">DateTimeOffset</span></span>|<span data-ttu-id="83254-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="83254-139">DateTime the object was last modified.</span></span> <span data-ttu-id="83254-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83254-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="83254-141">roleScopeTagIds</span></span>|<span data-ttu-id="83254-142">字符串集合</span><span class="sxs-lookup"><span data-stu-id="83254-142">String collection</span></span>|<span data-ttu-id="83254-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="83254-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="83254-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83254-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="83254-145">supportsScopeTags</span></span>|<span data-ttu-id="83254-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="83254-146">Boolean</span></span>|<span data-ttu-id="83254-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="83254-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="83254-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="83254-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="83254-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="83254-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="83254-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="83254-150">This property is read-only.</span></span> <span data-ttu-id="83254-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83254-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="83254-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="83254-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="83254-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="83254-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="83254-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="83254-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83254-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="83254-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="83254-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="83254-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="83254-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="83254-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="83254-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83254-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="83254-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="83254-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="83254-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="83254-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="83254-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="83254-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83254-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83254-164">createdDateTime</span></span>|<span data-ttu-id="83254-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83254-165">DateTimeOffset</span></span>|<span data-ttu-id="83254-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="83254-166">DateTime the object was created.</span></span> <span data-ttu-id="83254-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83254-168">description</span><span class="sxs-lookup"><span data-stu-id="83254-168">description</span></span>|<span data-ttu-id="83254-169">String</span><span class="sxs-lookup"><span data-stu-id="83254-169">String</span></span>|<span data-ttu-id="83254-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="83254-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="83254-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83254-172">displayName</span><span class="sxs-lookup"><span data-stu-id="83254-172">displayName</span></span>|<span data-ttu-id="83254-173">String</span><span class="sxs-lookup"><span data-stu-id="83254-173">String</span></span>|<span data-ttu-id="83254-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="83254-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="83254-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83254-176">version</span><span class="sxs-lookup"><span data-stu-id="83254-176">version</span></span>|<span data-ttu-id="83254-177">Int32</span><span class="sxs-lookup"><span data-stu-id="83254-177">Int32</span></span>|<span data-ttu-id="83254-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="83254-178">Version of the device configuration.</span></span> <span data-ttu-id="83254-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83254-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="83254-180">connectionName</span></span>|<span data-ttu-id="83254-181">String</span><span class="sxs-lookup"><span data-stu-id="83254-181">String</span></span>|<span data-ttu-id="83254-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="83254-182">Connection name displayed to the user.</span></span> <span data-ttu-id="83254-183">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="83254-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="83254-184">connectionType</span></span>|[<span data-ttu-id="83254-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="83254-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="83254-186">连接类型。</span><span class="sxs-lookup"><span data-stu-id="83254-186">Connection type.</span></span> <span data-ttu-id="83254-187">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="83254-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="83254-188">可能的值为：、、、、、、、、、、、、、、、、、、 `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` 。</span><span class="sxs-lookup"><span data-stu-id="83254-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="83254-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="83254-189">loginGroupOrDomain</span></span>|<span data-ttu-id="83254-190">String</span><span class="sxs-lookup"><span data-stu-id="83254-190">String</span></span>|<span data-ttu-id="83254-191">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="83254-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="83254-192">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="83254-193">role</span><span class="sxs-lookup"><span data-stu-id="83254-193">role</span></span>|<span data-ttu-id="83254-194">String</span><span class="sxs-lookup"><span data-stu-id="83254-194">String</span></span>|<span data-ttu-id="83254-195">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="83254-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="83254-196">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="83254-197">型</span><span class="sxs-lookup"><span data-stu-id="83254-197">realm</span></span>|<span data-ttu-id="83254-198">String</span><span class="sxs-lookup"><span data-stu-id="83254-198">String</span></span>|<span data-ttu-id="83254-199">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="83254-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="83254-200">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="83254-201">服务器主板</span><span class="sxs-lookup"><span data-stu-id="83254-201">server</span></span>|[<span data-ttu-id="83254-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="83254-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="83254-203">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="83254-203">VPN Server on the network.</span></span> <span data-ttu-id="83254-204">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="83254-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="83254-205">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="83254-206">标识符</span><span class="sxs-lookup"><span data-stu-id="83254-206">identifier</span></span>|<span data-ttu-id="83254-207">String</span><span class="sxs-lookup"><span data-stu-id="83254-207">String</span></span>|<span data-ttu-id="83254-208">当连接类型设置为自定义 VPN 时，由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="83254-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="83254-209">例如： Cisco AnyConnect 使用从[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)继承的 AnyConnect applevpn 的标识符。</span><span class="sxs-lookup"><span data-stu-id="83254-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="83254-210">customData</span><span class="sxs-lookup"><span data-stu-id="83254-210">customData</span></span>|<span data-ttu-id="83254-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83254-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="83254-212">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="83254-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="83254-213">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="83254-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="83254-214">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="83254-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="83254-215">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="83254-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="83254-216">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="83254-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="83254-217">customKeyValueData</span></span>|<span data-ttu-id="83254-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83254-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="83254-219">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="83254-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="83254-220">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="83254-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="83254-221">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="83254-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="83254-222">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="83254-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="83254-223">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="83254-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="83254-224">enableSplitTunneling</span></span>|<span data-ttu-id="83254-225">布尔值</span><span class="sxs-lookup"><span data-stu-id="83254-225">Boolean</span></span>|<span data-ttu-id="83254-226">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="83254-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="83254-227">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="83254-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="83254-228">authenticationMethod</span></span>|[<span data-ttu-id="83254-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="83254-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="83254-230">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="83254-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="83254-231">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="83254-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="83254-232">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="83254-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="83254-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="83254-233">enablePerApp</span></span>|<span data-ttu-id="83254-234">布尔值</span><span class="sxs-lookup"><span data-stu-id="83254-234">Boolean</span></span>|<span data-ttu-id="83254-235">将此设置为 true 将创建每个应用程序 VPN 有效负载，以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="83254-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="83254-236">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="83254-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="83254-237">safariDomains</span></span>|<span data-ttu-id="83254-238">字符串集合</span><span class="sxs-lookup"><span data-stu-id="83254-238">String collection</span></span>|<span data-ttu-id="83254-239">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="83254-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="83254-240">除了与此 VPN 关联的应用程序之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="83254-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="83254-241">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="83254-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="83254-242">onDemandRules</span></span>|<span data-ttu-id="83254-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83254-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="83254-244">按需规则。</span><span class="sxs-lookup"><span data-stu-id="83254-244">On-Demand Rules.</span></span> <span data-ttu-id="83254-245">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="83254-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="83254-246">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="83254-247">providerType</span><span class="sxs-lookup"><span data-stu-id="83254-247">providerType</span></span>|[<span data-ttu-id="83254-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="83254-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="83254-249">每应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="83254-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="83254-250">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="83254-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="83254-251">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="83254-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="83254-252">proxyServer</span><span class="sxs-lookup"><span data-stu-id="83254-252">proxyServer</span></span>|[<span data-ttu-id="83254-253">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="83254-253">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="83254-254">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="83254-254">Proxy Server.</span></span> <span data-ttu-id="83254-255">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-255">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="83254-256">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="83254-256">optInToDeviceIdSharing</span></span>|<span data-ttu-id="83254-257">布尔值</span><span class="sxs-lookup"><span data-stu-id="83254-257">Boolean</span></span>|<span data-ttu-id="83254-258">选择将设备的 Id 共享到第三方 vpn 客户端，以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="83254-258">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="83254-259">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83254-259">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="83254-260">userDomain</span><span class="sxs-lookup"><span data-stu-id="83254-260">userDomain</span></span>|<span data-ttu-id="83254-261">String</span><span class="sxs-lookup"><span data-stu-id="83254-261">String</span></span>|<span data-ttu-id="83254-262">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="83254-262">Zscaler only.</span></span> <span data-ttu-id="83254-263">输入一个静态域，以便在 Zscaler 应用程序中预填充 "登录" 字段。</span><span class="sxs-lookup"><span data-stu-id="83254-263">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="83254-264">如果保留为空，则将改用用户的 Azure Active Directory 域。</span><span class="sxs-lookup"><span data-stu-id="83254-264">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="83254-265">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="83254-265">strictEnforcement</span></span>|<span data-ttu-id="83254-266">布尔值</span><span class="sxs-lookup"><span data-stu-id="83254-266">Boolean</span></span>|<span data-ttu-id="83254-267">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="83254-267">Zscaler only.</span></span> <span data-ttu-id="83254-268">阻止网络流量，直到用户登录到 Zscaler 应用程序。</span><span class="sxs-lookup"><span data-stu-id="83254-268">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="83254-269">"True" 表示阻止流量。</span><span class="sxs-lookup"><span data-stu-id="83254-269">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="83254-270">cloudName</span><span class="sxs-lookup"><span data-stu-id="83254-270">cloudName</span></span>|<span data-ttu-id="83254-271">String</span><span class="sxs-lookup"><span data-stu-id="83254-271">String</span></span>|<span data-ttu-id="83254-272">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="83254-272">Zscaler only.</span></span> <span data-ttu-id="83254-273">用户分配到的 Zscaler 云。</span><span class="sxs-lookup"><span data-stu-id="83254-273">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="83254-274">excludeList</span><span class="sxs-lookup"><span data-stu-id="83254-274">excludeList</span></span>|<span data-ttu-id="83254-275">字符串集合</span><span class="sxs-lookup"><span data-stu-id="83254-275">String collection</span></span>|<span data-ttu-id="83254-276">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="83254-276">Zscaler only.</span></span> <span data-ttu-id="83254-277">不通过 Zscaler 云发送的网络地址的列表。</span><span class="sxs-lookup"><span data-stu-id="83254-277">List of network addresses which are not sent through the Zscaler cloud.</span></span>|
|<span data-ttu-id="83254-278">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="83254-278">targetedMobileApps</span></span>|<span data-ttu-id="83254-279">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83254-279">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="83254-280">目标移动应用。</span><span class="sxs-lookup"><span data-stu-id="83254-280">Targeted mobile apps.</span></span> <span data-ttu-id="83254-281">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="83254-281">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="83254-282">响应</span><span class="sxs-lookup"><span data-stu-id="83254-282">Response</span></span>
<span data-ttu-id="83254-283">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="83254-283">If successful, this method returns a `200 OK` response code and an updated [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83254-284">示例</span><span class="sxs-lookup"><span data-stu-id="83254-284">Example</span></span>

### <a name="request"></a><span data-ttu-id="83254-285">请求</span><span class="sxs-lookup"><span data-stu-id="83254-285">Request</span></span>
<span data-ttu-id="83254-286">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="83254-286">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3072

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="83254-287">响应</span><span class="sxs-lookup"><span data-stu-id="83254-287">Response</span></span>
<span data-ttu-id="83254-p135">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="83254-p135">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3244

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
  "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
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
  ]
}
```



