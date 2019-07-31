---
title: 更新 macOSVpnConfiguration
description: 更新 macOSVpnConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 92b0593347cb115bb5a9b065422fae725d672964
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35946960"
---
# <a name="update-macosvpnconfiguration"></a><span data-ttu-id="a857e-103">更新 macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a857e-103">Update macOSVpnConfiguration</span></span>

> <span data-ttu-id="a857e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a857e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a857e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a857e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a857e-106">更新[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a857e-106">Update the properties of a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a857e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a857e-107">Prerequisites</span></span>
<span data-ttu-id="a857e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a857e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a857e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a857e-110">Permission type</span></span>|<span data-ttu-id="a857e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a857e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a857e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a857e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a857e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a857e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a857e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a857e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a857e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a857e-115">Not supported.</span></span>|
|<span data-ttu-id="a857e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a857e-116">Application</span></span>|<span data-ttu-id="a857e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a857e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a857e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a857e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a857e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a857e-119">Request headers</span></span>
|<span data-ttu-id="a857e-120">标头</span><span class="sxs-lookup"><span data-stu-id="a857e-120">Header</span></span>|<span data-ttu-id="a857e-121">值</span><span class="sxs-lookup"><span data-stu-id="a857e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a857e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a857e-122">Authorization</span></span>|<span data-ttu-id="a857e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a857e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a857e-124">接受</span><span class="sxs-lookup"><span data-stu-id="a857e-124">Accept</span></span>|<span data-ttu-id="a857e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a857e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a857e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a857e-126">Request body</span></span>
<span data-ttu-id="a857e-127">在请求正文中, 提供[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a857e-127">In the request body, supply a JSON representation for the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="a857e-128">下表显示创建[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a857e-128">The following table shows the properties that are required when you create the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

|<span data-ttu-id="a857e-129">属性</span><span class="sxs-lookup"><span data-stu-id="a857e-129">Property</span></span>|<span data-ttu-id="a857e-130">类型</span><span class="sxs-lookup"><span data-stu-id="a857e-130">Type</span></span>|<span data-ttu-id="a857e-131">说明</span><span class="sxs-lookup"><span data-stu-id="a857e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a857e-132">id</span><span class="sxs-lookup"><span data-stu-id="a857e-132">id</span></span>|<span data-ttu-id="a857e-133">字符串</span><span class="sxs-lookup"><span data-stu-id="a857e-133">String</span></span>|<span data-ttu-id="a857e-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a857e-134">Key of the entity.</span></span> <span data-ttu-id="a857e-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a857e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a857e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a857e-137">DateTimeOffset</span></span>|<span data-ttu-id="a857e-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a857e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a857e-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a857e-140">roleScopeTagIds</span></span>|<span data-ttu-id="a857e-141">String collection</span><span class="sxs-lookup"><span data-stu-id="a857e-141">String collection</span></span>|<span data-ttu-id="a857e-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a857e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a857e-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a857e-144">supportsScopeTags</span></span>|<span data-ttu-id="a857e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a857e-145">Boolean</span></span>|<span data-ttu-id="a857e-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="a857e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a857e-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="a857e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a857e-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="a857e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a857e-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a857e-149">This property is read-only.</span></span> <span data-ttu-id="a857e-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a857e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a857e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a857e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a857e-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="a857e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a857e-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a857e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a857e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a857e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a857e-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a857e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a857e-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a857e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a857e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a857e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a857e-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a857e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a857e-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a857e-163">createdDateTime</span></span>|<span data-ttu-id="a857e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a857e-164">DateTimeOffset</span></span>|<span data-ttu-id="a857e-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a857e-165">DateTime the object was created.</span></span> <span data-ttu-id="a857e-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-167">说明</span><span class="sxs-lookup"><span data-stu-id="a857e-167">description</span></span>|<span data-ttu-id="a857e-168">String</span><span class="sxs-lookup"><span data-stu-id="a857e-168">String</span></span>|<span data-ttu-id="a857e-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a857e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a857e-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a857e-171">displayName</span></span>|<span data-ttu-id="a857e-172">String</span><span class="sxs-lookup"><span data-stu-id="a857e-172">String</span></span>|<span data-ttu-id="a857e-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a857e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a857e-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-175">version</span><span class="sxs-lookup"><span data-stu-id="a857e-175">version</span></span>|<span data-ttu-id="a857e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a857e-176">Int32</span></span>|<span data-ttu-id="a857e-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a857e-177">Version of the device configuration.</span></span> <span data-ttu-id="a857e-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-179">connectionName</span><span class="sxs-lookup"><span data-stu-id="a857e-179">connectionName</span></span>|<span data-ttu-id="a857e-180">String</span><span class="sxs-lookup"><span data-stu-id="a857e-180">String</span></span>|<span data-ttu-id="a857e-181">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="a857e-181">Connection name displayed to the user.</span></span> <span data-ttu-id="a857e-182">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-182">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="a857e-183">connectionType</span></span>|[<span data-ttu-id="a857e-184">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="a857e-184">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="a857e-185">连接类型。</span><span class="sxs-lookup"><span data-stu-id="a857e-185">Connection type.</span></span> <span data-ttu-id="a857e-186">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="a857e-186">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="a857e-187">可能的值为`ciscoAnyConnect`: `pulseSecure`、 `f5EdgeClient`、 `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `ikEv2`、、 `zscalerPrivateAccess`、、、、、、、、、、。 `paloAltoGlobalProtect` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2`</span><span class="sxs-lookup"><span data-stu-id="a857e-187">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`.</span></span>|
|<span data-ttu-id="a857e-188">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="a857e-188">loginGroupOrDomain</span></span>|<span data-ttu-id="a857e-189">String</span><span class="sxs-lookup"><span data-stu-id="a857e-189">String</span></span>|<span data-ttu-id="a857e-190">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="a857e-190">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="a857e-191">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-191">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-192">role</span><span class="sxs-lookup"><span data-stu-id="a857e-192">role</span></span>|<span data-ttu-id="a857e-193">String</span><span class="sxs-lookup"><span data-stu-id="a857e-193">String</span></span>|<span data-ttu-id="a857e-194">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="a857e-194">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="a857e-195">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-195">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-196">型</span><span class="sxs-lookup"><span data-stu-id="a857e-196">realm</span></span>|<span data-ttu-id="a857e-197">String</span><span class="sxs-lookup"><span data-stu-id="a857e-197">String</span></span>|<span data-ttu-id="a857e-198">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="a857e-198">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="a857e-199">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-199">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-200">服务器主板</span><span class="sxs-lookup"><span data-stu-id="a857e-200">server</span></span>|[<span data-ttu-id="a857e-201">vpnServer</span><span class="sxs-lookup"><span data-stu-id="a857e-201">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="a857e-202">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="a857e-202">VPN Server on the network.</span></span> <span data-ttu-id="a857e-203">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="a857e-203">Make sure end users can access this network location.</span></span> <span data-ttu-id="a857e-204">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-205">标识符</span><span class="sxs-lookup"><span data-stu-id="a857e-205">identifier</span></span>|<span data-ttu-id="a857e-206">String</span><span class="sxs-lookup"><span data-stu-id="a857e-206">String</span></span>|<span data-ttu-id="a857e-207">当连接类型设置为自定义 VPN 时, 由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="a857e-207">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="a857e-208">例如: Cisco AnyConnect 使用从[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)继承的 AnyConnect applevpn 的标识符。</span><span class="sxs-lookup"><span data-stu-id="a857e-208">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-209">customData</span><span class="sxs-lookup"><span data-stu-id="a857e-209">customData</span></span>|<span data-ttu-id="a857e-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a857e-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="a857e-211">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="a857e-211">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="a857e-212">使用此字段启用 Intune 不支持的功能, 但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="a857e-212">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="a857e-213">请与你的 VPN 供应商联系, 了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="a857e-213">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="a857e-214">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="a857e-214">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="a857e-215">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-216">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="a857e-216">customKeyValueData</span></span>|<span data-ttu-id="a857e-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a857e-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a857e-218">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="a857e-218">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="a857e-219">使用此字段启用 Intune 不支持的功能, 但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="a857e-219">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="a857e-220">请与你的 VPN 供应商联系, 了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="a857e-220">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="a857e-221">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="a857e-221">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="a857e-222">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-222">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-223">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="a857e-223">enableSplitTunneling</span></span>|<span data-ttu-id="a857e-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="a857e-224">Boolean</span></span>|<span data-ttu-id="a857e-225">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="a857e-225">Send all network traffic through VPN.</span></span> <span data-ttu-id="a857e-226">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-226">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-227">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a857e-227">authenticationMethod</span></span>|[<span data-ttu-id="a857e-228">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a857e-228">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="a857e-229">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="a857e-229">Authentication method for this VPN connection.</span></span> <span data-ttu-id="a857e-230">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="a857e-230">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="a857e-231">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="a857e-231">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="a857e-232">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="a857e-232">enablePerApp</span></span>|<span data-ttu-id="a857e-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="a857e-233">Boolean</span></span>|<span data-ttu-id="a857e-234">将此设置为 true 将创建每个应用程序 VPN 有效负载, 以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="a857e-234">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="a857e-235">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-235">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-236">safariDomains</span><span class="sxs-lookup"><span data-stu-id="a857e-236">safariDomains</span></span>|<span data-ttu-id="a857e-237">String collection</span><span class="sxs-lookup"><span data-stu-id="a857e-237">String collection</span></span>|<span data-ttu-id="a857e-238">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="a857e-238">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="a857e-239">除了与此 VPN 关联的应用程序之外, 此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="a857e-239">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="a857e-240">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-240">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-241">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="a857e-241">onDemandRules</span></span>|<span data-ttu-id="a857e-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="a857e-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="a857e-243">按需规则。</span><span class="sxs-lookup"><span data-stu-id="a857e-243">On-Demand Rules.</span></span> <span data-ttu-id="a857e-244">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="a857e-244">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a857e-245">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-245">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-246">proxyServer</span><span class="sxs-lookup"><span data-stu-id="a857e-246">proxyServer</span></span>|[<span data-ttu-id="a857e-247">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="a857e-247">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="a857e-248">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="a857e-248">Proxy Server.</span></span> <span data-ttu-id="a857e-249">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-249">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a857e-250">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="a857e-250">optInToDeviceIdSharing</span></span>|<span data-ttu-id="a857e-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="a857e-251">Boolean</span></span>|<span data-ttu-id="a857e-252">选择将设备的 Id 共享到第三方 vpn 客户端, 以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="a857e-252">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="a857e-253">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a857e-253">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a857e-254">响应</span><span class="sxs-lookup"><span data-stu-id="a857e-254">Response</span></span>
<span data-ttu-id="a857e-255">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a857e-255">If successful, this method returns a `200 OK` response code and an updated [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a857e-256">示例</span><span class="sxs-lookup"><span data-stu-id="a857e-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="a857e-257">请求</span><span class="sxs-lookup"><span data-stu-id="a857e-257">Request</span></span>
<span data-ttu-id="a857e-258">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a857e-258">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2630

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
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
  "optInToDeviceIdSharing": true
}
```

### <a name="response"></a><span data-ttu-id="a857e-259">响应</span><span class="sxs-lookup"><span data-stu-id="a857e-259">Response</span></span>
<span data-ttu-id="a857e-p129">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a857e-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2802

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "id": "8ce00178-0178-8ce0-7801-e08c7801e08c",
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
  "optInToDeviceIdSharing": true
}
```





