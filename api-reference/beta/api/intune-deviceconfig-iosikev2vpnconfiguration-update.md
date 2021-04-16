---
title: Update iosikEv2VpnConfiguration
description: 更新 iosikEv2VpnConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 68893c36fc8fdf760c166f32e199f66130bb4edc
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867999"
---
# <a name="update-iosikev2vpnconfiguration"></a><span data-ttu-id="0cdde-103">Update iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0cdde-103">Update iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="0cdde-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cdde-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0cdde-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0cdde-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cdde-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0cdde-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cdde-107">更新 [iosikEv2VpnConfiguration 对象](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="0cdde-107">Update the properties of a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cdde-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0cdde-108">Prerequisites</span></span>
<span data-ttu-id="0cdde-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0cdde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cdde-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0cdde-111">Permission type</span></span>|<span data-ttu-id="0cdde-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0cdde-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cdde-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0cdde-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0cdde-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cdde-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0cdde-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0cdde-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cdde-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cdde-116">Not supported.</span></span>|
|<span data-ttu-id="0cdde-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0cdde-117">Application</span></span>|<span data-ttu-id="0cdde-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cdde-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cdde-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0cdde-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0cdde-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0cdde-120">Request headers</span></span>
|<span data-ttu-id="0cdde-121">标头</span><span class="sxs-lookup"><span data-stu-id="0cdde-121">Header</span></span>|<span data-ttu-id="0cdde-122">值</span><span class="sxs-lookup"><span data-stu-id="0cdde-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cdde-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cdde-123">Authorization</span></span>|<span data-ttu-id="0cdde-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0cdde-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cdde-125">接受</span><span class="sxs-lookup"><span data-stu-id="0cdde-125">Accept</span></span>|<span data-ttu-id="0cdde-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0cdde-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cdde-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0cdde-127">Request body</span></span>
<span data-ttu-id="0cdde-128">在请求正文中，提供 [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0cdde-128">In the request body, supply a JSON representation for the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

<span data-ttu-id="0cdde-129">下表显示创建 [iosikEv2VpnConfiguration 时所需的属性](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="0cdde-129">The following table shows the properties that are required when you create the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span></span>

|<span data-ttu-id="0cdde-130">属性</span><span class="sxs-lookup"><span data-stu-id="0cdde-130">Property</span></span>|<span data-ttu-id="0cdde-131">类型</span><span class="sxs-lookup"><span data-stu-id="0cdde-131">Type</span></span>|<span data-ttu-id="0cdde-132">说明</span><span class="sxs-lookup"><span data-stu-id="0cdde-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cdde-133">id</span><span class="sxs-lookup"><span data-stu-id="0cdde-133">id</span></span>|<span data-ttu-id="0cdde-134">String</span><span class="sxs-lookup"><span data-stu-id="0cdde-134">String</span></span>|<span data-ttu-id="0cdde-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0cdde-135">Key of the entity.</span></span> <span data-ttu-id="0cdde-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0cdde-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0cdde-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cdde-138">DateTimeOffset</span></span>|<span data-ttu-id="0cdde-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0cdde-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0cdde-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0cdde-141">roleScopeTagIds</span></span>|<span data-ttu-id="0cdde-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="0cdde-142">String collection</span></span>|<span data-ttu-id="0cdde-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0cdde-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0cdde-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0cdde-145">supportsScopeTags</span></span>|<span data-ttu-id="0cdde-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cdde-146">Boolean</span></span>|<span data-ttu-id="0cdde-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="0cdde-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0cdde-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="0cdde-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0cdde-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="0cdde-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0cdde-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0cdde-150">This property is read-only.</span></span> <span data-ttu-id="0cdde-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0cdde-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0cdde-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0cdde-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0cdde-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="0cdde-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0cdde-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0cdde-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0cdde-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0cdde-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0cdde-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0cdde-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0cdde-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0cdde-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0cdde-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0cdde-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0cdde-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0cdde-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0cdde-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0cdde-164">createdDateTime</span></span>|<span data-ttu-id="0cdde-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cdde-165">DateTimeOffset</span></span>|<span data-ttu-id="0cdde-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0cdde-166">DateTime the object was created.</span></span> <span data-ttu-id="0cdde-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-168">说明</span><span class="sxs-lookup"><span data-stu-id="0cdde-168">description</span></span>|<span data-ttu-id="0cdde-169">String</span><span class="sxs-lookup"><span data-stu-id="0cdde-169">String</span></span>|<span data-ttu-id="0cdde-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0cdde-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0cdde-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-172">displayName</span><span class="sxs-lookup"><span data-stu-id="0cdde-172">displayName</span></span>|<span data-ttu-id="0cdde-173">String</span><span class="sxs-lookup"><span data-stu-id="0cdde-173">String</span></span>|<span data-ttu-id="0cdde-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0cdde-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0cdde-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-176">version</span><span class="sxs-lookup"><span data-stu-id="0cdde-176">version</span></span>|<span data-ttu-id="0cdde-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0cdde-177">Int32</span></span>|<span data-ttu-id="0cdde-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0cdde-178">Version of the device configuration.</span></span> <span data-ttu-id="0cdde-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="0cdde-180">connectionName</span></span>|<span data-ttu-id="0cdde-181">String</span><span class="sxs-lookup"><span data-stu-id="0cdde-181">String</span></span>|<span data-ttu-id="0cdde-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="0cdde-182">Connection name displayed to the user.</span></span> <span data-ttu-id="0cdde-183">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="0cdde-184">connectionType</span></span>|[<span data-ttu-id="0cdde-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="0cdde-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="0cdde-186">连接类型。</span><span class="sxs-lookup"><span data-stu-id="0cdde-186">Connection type.</span></span> <span data-ttu-id="0cdde-187">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="0cdde-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="0cdde-188">可能的值是 `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` ：、、、、、、、、 `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` 。</span><span class="sxs-lookup"><span data-stu-id="0cdde-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="0cdde-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="0cdde-189">loginGroupOrDomain</span></span>|<span data-ttu-id="0cdde-190">String</span><span class="sxs-lookup"><span data-stu-id="0cdde-190">String</span></span>|<span data-ttu-id="0cdde-191">连接类型设置为 Dell SonicWALL 移动连接时登录组或域。</span><span class="sxs-lookup"><span data-stu-id="0cdde-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="0cdde-192">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-193">role</span><span class="sxs-lookup"><span data-stu-id="0cdde-193">role</span></span>|<span data-ttu-id="0cdde-194">String</span><span class="sxs-lookup"><span data-stu-id="0cdde-194">String</span></span>|<span data-ttu-id="0cdde-195">将连接类型设置为 Pulse Secure 时的角色。</span><span class="sxs-lookup"><span data-stu-id="0cdde-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="0cdde-196">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-197">realm</span><span class="sxs-lookup"><span data-stu-id="0cdde-197">realm</span></span>|<span data-ttu-id="0cdde-198">String</span><span class="sxs-lookup"><span data-stu-id="0cdde-198">String</span></span>|<span data-ttu-id="0cdde-199">将连接类型设置为 Pulse Secure 时的领域。</span><span class="sxs-lookup"><span data-stu-id="0cdde-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="0cdde-200">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-201">server</span><span class="sxs-lookup"><span data-stu-id="0cdde-201">server</span></span>|[<span data-ttu-id="0cdde-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="0cdde-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="0cdde-203">VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="0cdde-203">VPN Server on the network.</span></span> <span data-ttu-id="0cdde-204">确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="0cdde-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="0cdde-205">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-206">标识符</span><span class="sxs-lookup"><span data-stu-id="0cdde-206">identifier</span></span>|<span data-ttu-id="0cdde-207">String</span><span class="sxs-lookup"><span data-stu-id="0cdde-207">String</span></span>|<span data-ttu-id="0cdde-208">连接类型设置为自定义 VPN 时 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="0cdde-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0cdde-209">例如：Cisco AnyConnect 使用 com.cisco.anyconnect.applevpn.plugin 形式的标识符 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-210">customData</span><span class="sxs-lookup"><span data-stu-id="0cdde-210">customData</span></span>|<span data-ttu-id="0cdde-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0cdde-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="0cdde-212">连接类型设置为自定义 VPN 时自定义数据。</span><span class="sxs-lookup"><span data-stu-id="0cdde-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0cdde-213">使用此字段启用 Intune 不支持但在 VPN 解决方案中提供的功能。</span><span class="sxs-lookup"><span data-stu-id="0cdde-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="0cdde-214">请联系 VPN 供应商，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="0cdde-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="0cdde-215">此集合最多可包含 25 个元素。</span><span class="sxs-lookup"><span data-stu-id="0cdde-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="0cdde-216">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="0cdde-217">customKeyValueData</span></span>|<span data-ttu-id="0cdde-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0cdde-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0cdde-219">连接类型设置为自定义 VPN 时自定义数据。</span><span class="sxs-lookup"><span data-stu-id="0cdde-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0cdde-220">使用此字段启用 Intune 不支持但在 VPN 解决方案中提供的功能。</span><span class="sxs-lookup"><span data-stu-id="0cdde-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="0cdde-221">请联系 VPN 供应商，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="0cdde-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="0cdde-222">此集合最多可包含 25 个元素。</span><span class="sxs-lookup"><span data-stu-id="0cdde-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="0cdde-223">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="0cdde-224">enableSplitTunneling</span></span>|<span data-ttu-id="0cdde-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cdde-225">Boolean</span></span>|<span data-ttu-id="0cdde-226">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="0cdde-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="0cdde-227">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0cdde-228">authenticationMethod</span></span>|[<span data-ttu-id="0cdde-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0cdde-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="0cdde-230">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="0cdde-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="0cdde-231">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="0cdde-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="0cdde-232">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="0cdde-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="0cdde-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="0cdde-233">enablePerApp</span></span>|<span data-ttu-id="0cdde-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cdde-234">Boolean</span></span>|<span data-ttu-id="0cdde-235">如果设置为 true，Per-App VPN 有效负载，稍后可关联到可在最终用户的 iOS 设备上触发此 VPN 连接的应用。</span><span class="sxs-lookup"><span data-stu-id="0cdde-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="0cdde-236">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="0cdde-237">safariDomains</span></span>|<span data-ttu-id="0cdde-238">String 集合</span><span class="sxs-lookup"><span data-stu-id="0cdde-238">String collection</span></span>|<span data-ttu-id="0cdde-239">启用"每个应用此 VPN"设置时，Safari 域。</span><span class="sxs-lookup"><span data-stu-id="0cdde-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="0cdde-240">除了与此 VPN 关联的应用之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="0cdde-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="0cdde-241">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="0cdde-242">onDemandRules</span></span>|<span data-ttu-id="0cdde-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0cdde-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="0cdde-244">按需规则。</span><span class="sxs-lookup"><span data-stu-id="0cdde-244">On-Demand Rules.</span></span> <span data-ttu-id="0cdde-245">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0cdde-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0cdde-246">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-247">providerType</span><span class="sxs-lookup"><span data-stu-id="0cdde-247">providerType</span></span>|[<span data-ttu-id="0cdde-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="0cdde-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="0cdde-249">每个应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="0cdde-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="0cdde-250">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="0cdde-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="0cdde-251">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="0cdde-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="0cdde-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="0cdde-252">associatedDomains</span></span>|<span data-ttu-id="0cdde-253">String 集合</span><span class="sxs-lookup"><span data-stu-id="0cdde-253">String collection</span></span>|<span data-ttu-id="0cdde-254">关联域 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="0cdde-255">excludedDomains</span></span>|<span data-ttu-id="0cdde-256">String 集合</span><span class="sxs-lookup"><span data-stu-id="0cdde-256">String collection</span></span>|<span data-ttu-id="0cdde-257">通过公共 Internet 而不是 VPN 访问的域，即使已激活每应用 VPN 也是如此。继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="0cdde-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="0cdde-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cdde-259">Boolean</span></span>|<span data-ttu-id="0cdde-260">切换以阻止用户在"设置"应用中禁用自动 VPN 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-261">disconnectOnIdle</span><span class="sxs-lookup"><span data-stu-id="0cdde-261">disconnectOnIdle</span></span>|<span data-ttu-id="0cdde-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cdde-262">Boolean</span></span>|<span data-ttu-id="0cdde-263">是否在按需连接空闲后断开连接 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-263">Whether to disconnect after on-demand connection idles Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-264">disconnectOnIdleTimerInSeconds</span><span class="sxs-lookup"><span data-stu-id="0cdde-264">disconnectOnIdleTimerInSeconds</span></span>|<span data-ttu-id="0cdde-265">Int32</span><span class="sxs-lookup"><span data-stu-id="0cdde-265">Int32</span></span>|<span data-ttu-id="0cdde-266">断开按需连接之前要等待的时间长度（秒）。</span><span class="sxs-lookup"><span data-stu-id="0cdde-266">The length of time in seconds to wait before disconnecting an on-demand connection.</span></span> <span data-ttu-id="0cdde-267">有效值 0 至 65535 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-267">Valid values 0 to 65535 Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-268">proxyServer</span><span class="sxs-lookup"><span data-stu-id="0cdde-268">proxyServer</span></span>|[<span data-ttu-id="0cdde-269">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="0cdde-269">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="0cdde-270">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="0cdde-270">Proxy Server.</span></span> <span data-ttu-id="0cdde-271">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-271">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-272">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="0cdde-272">optInToDeviceIdSharing</span></span>|<span data-ttu-id="0cdde-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cdde-273">Boolean</span></span>|<span data-ttu-id="0cdde-274">Opt-In将设备 ID 共享给第三方 vpn 客户端，以在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="0cdde-274">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="0cdde-275">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-275">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-276">userDomain</span><span class="sxs-lookup"><span data-stu-id="0cdde-276">userDomain</span></span>|<span data-ttu-id="0cdde-277">String</span><span class="sxs-lookup"><span data-stu-id="0cdde-277">String</span></span>|<span data-ttu-id="0cdde-278">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="0cdde-278">Zscaler only.</span></span> <span data-ttu-id="0cdde-279">输入静态域，以在 Zscaler 应用中预填充登录字段。</span><span class="sxs-lookup"><span data-stu-id="0cdde-279">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="0cdde-280">如果为空，将改为使用用户的 Azure Active Directory 域。</span><span class="sxs-lookup"><span data-stu-id="0cdde-280">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="0cdde-281">继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-281">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-282">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="0cdde-282">strictEnforcement</span></span>|<span data-ttu-id="0cdde-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cdde-283">Boolean</span></span>|<span data-ttu-id="0cdde-284">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="0cdde-284">Zscaler only.</span></span> <span data-ttu-id="0cdde-285">阻止网络流量，直到用户登录 Zscaler 应用。</span><span class="sxs-lookup"><span data-stu-id="0cdde-285">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="0cdde-286">"True"表示流量被阻止。</span><span class="sxs-lookup"><span data-stu-id="0cdde-286">"True" means traffic is blocked.</span></span> <span data-ttu-id="0cdde-287">继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-287">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-288">cloudName</span><span class="sxs-lookup"><span data-stu-id="0cdde-288">cloudName</span></span>|<span data-ttu-id="0cdde-289">String</span><span class="sxs-lookup"><span data-stu-id="0cdde-289">String</span></span>|<span data-ttu-id="0cdde-290">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="0cdde-290">Zscaler only.</span></span> <span data-ttu-id="0cdde-291">用户分配到的 Zscaler 云。</span><span class="sxs-lookup"><span data-stu-id="0cdde-291">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="0cdde-292">继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-292">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-293">excludeList</span><span class="sxs-lookup"><span data-stu-id="0cdde-293">excludeList</span></span>|<span data-ttu-id="0cdde-294">String 集合</span><span class="sxs-lookup"><span data-stu-id="0cdde-294">String collection</span></span>|<span data-ttu-id="0cdde-295">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="0cdde-295">Zscaler only.</span></span> <span data-ttu-id="0cdde-296">未通过 Zscaler 云发送的网络地址列表。</span><span class="sxs-lookup"><span data-stu-id="0cdde-296">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="0cdde-297">继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-297">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-298">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="0cdde-298">targetedMobileApps</span></span>|<span data-ttu-id="0cdde-299">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0cdde-299">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="0cdde-300">目标移动应用。</span><span class="sxs-lookup"><span data-stu-id="0cdde-300">Targeted mobile apps.</span></span> <span data-ttu-id="0cdde-301">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0cdde-301">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0cdde-302">继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-302">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-303">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="0cdde-303">microsoftTunnelSiteId</span></span>|<span data-ttu-id="0cdde-304">String</span><span class="sxs-lookup"><span data-stu-id="0cdde-304">String</span></span>|<span data-ttu-id="0cdde-305">Microsoft 隧道站点 ID。</span><span class="sxs-lookup"><span data-stu-id="0cdde-305">Microsoft Tunnel site ID.</span></span> <span data-ttu-id="0cdde-306">继承自 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cdde-306">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0cdde-307">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0cdde-307">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="0cdde-308">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0cdde-308">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="0cdde-309">子安全关联参数</span><span class="sxs-lookup"><span data-stu-id="0cdde-309">Child Security Association Parameters</span></span>|
|<span data-ttu-id="0cdde-310">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="0cdde-310">clientAuthenticationType</span></span>|[<span data-ttu-id="0cdde-311">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="0cdde-311">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="0cdde-312">VPN 客户端将使用的客户端身份验证的类型。</span><span class="sxs-lookup"><span data-stu-id="0cdde-312">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="0cdde-313">可取值为：`userAuthentication`、`deviceAuthentication`。</span><span class="sxs-lookup"><span data-stu-id="0cdde-313">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="0cdde-314">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="0cdde-314">deadPeerDetectionRate</span></span>|[<span data-ttu-id="0cdde-315">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="0cdde-315">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="0cdde-316">确定检查对等连接是否仍处于活动状态频繁。</span><span class="sxs-lookup"><span data-stu-id="0cdde-316">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="0cdde-317">.</span><span class="sxs-lookup"><span data-stu-id="0cdde-317">.</span></span> <span data-ttu-id="0cdde-318">可取值为：`medium`、`none`、`low`、`high`。</span><span class="sxs-lookup"><span data-stu-id="0cdde-318">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="0cdde-319">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="0cdde-319">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="0cdde-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cdde-320">Boolean</span></span>|<span data-ttu-id="0cdde-321">禁用 MOBIKE</span><span class="sxs-lookup"><span data-stu-id="0cdde-321">Disable MOBIKE</span></span>|
|<span data-ttu-id="0cdde-322">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="0cdde-322">disableRedirect</span></span>|<span data-ttu-id="0cdde-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cdde-323">Boolean</span></span>|<span data-ttu-id="0cdde-324">禁用重定向</span><span class="sxs-lookup"><span data-stu-id="0cdde-324">Disable Redirect</span></span>|
|<span data-ttu-id="0cdde-325">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="0cdde-325">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="0cdde-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cdde-326">Boolean</span></span>|<span data-ttu-id="0cdde-327">启用最佳吊销检查;服务器响应超时不会导致失败</span><span class="sxs-lookup"><span data-stu-id="0cdde-327">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="0cdde-328">enableEAP</span><span class="sxs-lookup"><span data-stu-id="0cdde-328">enableEAP</span></span>|<span data-ttu-id="0cdde-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cdde-329">Boolean</span></span>|<span data-ttu-id="0cdde-330">启用仅 EAP 身份验证</span><span class="sxs-lookup"><span data-stu-id="0cdde-330">Enables EAP only authentication</span></span>|
|<span data-ttu-id="0cdde-331">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="0cdde-331">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="0cdde-332">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cdde-332">Boolean</span></span>|<span data-ttu-id="0cdde-333">启用"完全向前保密" (PFS) 。</span><span class="sxs-lookup"><span data-stu-id="0cdde-333">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="0cdde-334">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="0cdde-334">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="0cdde-335">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cdde-335">Boolean</span></span>|<span data-ttu-id="0cdde-336">启用"使用内部子网属性"。</span><span class="sxs-lookup"><span data-stu-id="0cdde-336">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="0cdde-337">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="0cdde-337">localIdentifier</span></span>|[<span data-ttu-id="0cdde-338">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="0cdde-338">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="0cdde-339">用于标识尝试通过 VPN 连接的客户端的方法。</span><span class="sxs-lookup"><span data-stu-id="0cdde-339">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="0cdde-340">.</span><span class="sxs-lookup"><span data-stu-id="0cdde-340">.</span></span> <span data-ttu-id="0cdde-341">可取值为：`deviceFQDN`、`empty`、`clientCertificateSubjectName`。</span><span class="sxs-lookup"><span data-stu-id="0cdde-341">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="0cdde-342">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="0cdde-342">remoteIdentifier</span></span>|<span data-ttu-id="0cdde-343">String</span><span class="sxs-lookup"><span data-stu-id="0cdde-343">String</span></span>|<span data-ttu-id="0cdde-344">IKEv2 服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="0cdde-344">Address of the IKEv2 server.</span></span> <span data-ttu-id="0cdde-345">必须是 FQDN、UserFQDN、网络地址或 ASN1DN</span><span class="sxs-lookup"><span data-stu-id="0cdde-345">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="0cdde-346">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0cdde-346">securityAssociationParameters</span></span>|[<span data-ttu-id="0cdde-347">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0cdde-347">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="0cdde-348">安全关联参数</span><span class="sxs-lookup"><span data-stu-id="0cdde-348">Security Association Parameters</span></span>|
|<span data-ttu-id="0cdde-349">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="0cdde-349">serverCertificateCommonName</span></span>|<span data-ttu-id="0cdde-350">String</span><span class="sxs-lookup"><span data-stu-id="0cdde-350">String</span></span>|<span data-ttu-id="0cdde-351">服务器身份验证中使用的 IKEv2 服务器证书的公用名</span><span class="sxs-lookup"><span data-stu-id="0cdde-351">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="0cdde-352">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="0cdde-352">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="0cdde-353">String</span><span class="sxs-lookup"><span data-stu-id="0cdde-353">String</span></span>|<span data-ttu-id="0cdde-354">颁发者 身份验证中使用的 IKEv2 服务器证书颁发者公用名</span><span class="sxs-lookup"><span data-stu-id="0cdde-354">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="0cdde-355">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="0cdde-355">serverCertificateType</span></span>|[<span data-ttu-id="0cdde-356">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="0cdde-356">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="0cdde-357">VPN 服务器将呈现给 VPN 客户端以进行身份验证的证书类型。</span><span class="sxs-lookup"><span data-stu-id="0cdde-357">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="0cdde-358">可取值为：`rsa`、`ecdsa256`、`ecdsa384`、`ecdsa521`。</span><span class="sxs-lookup"><span data-stu-id="0cdde-358">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="0cdde-359">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="0cdde-359">sharedSecret</span></span>|<span data-ttu-id="0cdde-360">String</span><span class="sxs-lookup"><span data-stu-id="0cdde-360">String</span></span>|<span data-ttu-id="0cdde-361">在选择"共享密码身份验证"时使用</span><span class="sxs-lookup"><span data-stu-id="0cdde-361">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="0cdde-362">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0cdde-362">tlsMaximumVersion</span></span>|<span data-ttu-id="0cdde-363">String</span><span class="sxs-lookup"><span data-stu-id="0cdde-363">String</span></span>|<span data-ttu-id="0cdde-364">要与 EAP-TLS 身份验证一同使用的最大 TLS 版本</span><span class="sxs-lookup"><span data-stu-id="0cdde-364">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="0cdde-365">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0cdde-365">tlsMinimumVersion</span></span>|<span data-ttu-id="0cdde-366">String</span><span class="sxs-lookup"><span data-stu-id="0cdde-366">String</span></span>|<span data-ttu-id="0cdde-367">要与 EAP-TLS 身份验证一起使用的最低 TLS 版本</span><span class="sxs-lookup"><span data-stu-id="0cdde-367">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="0cdde-368">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0cdde-368">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="0cdde-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cdde-369">Boolean</span></span>|<span data-ttu-id="0cdde-370">除非明确指定，否则允许使用安全关联参数，具体方法为将所有参数设置为设备默认值。</span><span class="sxs-lookup"><span data-stu-id="0cdde-370">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="0cdde-371">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0cdde-371">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="0cdde-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cdde-372">Boolean</span></span>|<span data-ttu-id="0cdde-373">除非明确指定，否则允许使用子安全关联参数，具体方法为将所有参数设置为设备默认值。</span><span class="sxs-lookup"><span data-stu-id="0cdde-373">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="0cdde-374">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0cdde-374">alwaysOnConfiguration</span></span>|[<span data-ttu-id="0cdde-375">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0cdde-375">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="0cdde-376">AlwaysOn 配置</span><span class="sxs-lookup"><span data-stu-id="0cdde-376">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="0cdde-377">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0cdde-377">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="0cdde-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cdde-378">Boolean</span></span>|<span data-ttu-id="0cdde-379">确定是否启用始终启用 VPN</span><span class="sxs-lookup"><span data-stu-id="0cdde-379">Determines if Always on VPN is enabled</span></span>|
|<span data-ttu-id="0cdde-380">mtuSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="0cdde-380">mtuSizeInBytes</span></span>|<span data-ttu-id="0cdde-381">Int32</span><span class="sxs-lookup"><span data-stu-id="0cdde-381">Int32</span></span>|<span data-ttu-id="0cdde-382">最大传输单元数。</span><span class="sxs-lookup"><span data-stu-id="0cdde-382">Maximum transmission unit.</span></span> <span data-ttu-id="0cdde-383">有效值为 1280 至 1400</span><span class="sxs-lookup"><span data-stu-id="0cdde-383">Valid values 1280 to 1400</span></span>|



## <a name="response"></a><span data-ttu-id="0cdde-384">响应</span><span class="sxs-lookup"><span data-stu-id="0cdde-384">Response</span></span>
<span data-ttu-id="0cdde-385">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0cdde-385">If successful, this method returns a `200 OK` response code and an updated [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cdde-386">示例</span><span class="sxs-lookup"><span data-stu-id="0cdde-386">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cdde-387">请求</span><span class="sxs-lookup"><span data-stu-id="0cdde-387">Request</span></span>
<span data-ttu-id="0cdde-388">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0cdde-388">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 5562

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
  "associatedDomains": [
    "Associated Domains value"
  ],
  "excludedDomains": [
    "Excluded Domains value"
  ],
  "disableOnDemandUserOverride": true,
  "disconnectOnIdle": true,
  "disconnectOnIdleTimerInSeconds": 14,
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

### <a name="response"></a><span data-ttu-id="0cdde-389">响应</span><span class="sxs-lookup"><span data-stu-id="0cdde-389">Response</span></span>
<span data-ttu-id="0cdde-p143">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0cdde-p143">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5734

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
  "associatedDomains": [
    "Associated Domains value"
  ],
  "excludedDomains": [
    "Excluded Domains value"
  ],
  "disableOnDemandUserOverride": true,
  "disconnectOnIdle": true,
  "disconnectOnIdleTimerInSeconds": 14,
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




