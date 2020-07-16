---
title: 更新 macOSVpnConfiguration
description: 更新 macOSVpnConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ea226221b4808e5eecf371c449ba236bc3e5019f
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122992"
---
# <a name="update-macosvpnconfiguration"></a><span data-ttu-id="bf4fb-103">更新 macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="bf4fb-103">Update macOSVpnConfiguration</span></span>

<span data-ttu-id="bf4fb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf4fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf4fb-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf4fb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf4fb-107">更新[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-107">Update the properties of a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf4fb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bf4fb-108">Prerequisites</span></span>
<span data-ttu-id="bf4fb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf4fb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf4fb-111">Permission type</span></span>|<span data-ttu-id="bf4fb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bf4fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf4fb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf4fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bf4fb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf4fb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bf4fb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf4fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf4fb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-116">Not supported.</span></span>|
|<span data-ttu-id="bf4fb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf4fb-117">Application</span></span>|<span data-ttu-id="bf4fb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf4fb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf4fb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf4fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bf4fb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf4fb-120">Request headers</span></span>
|<span data-ttu-id="bf4fb-121">标头</span><span class="sxs-lookup"><span data-stu-id="bf4fb-121">Header</span></span>|<span data-ttu-id="bf4fb-122">值</span><span class="sxs-lookup"><span data-stu-id="bf4fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf4fb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf4fb-123">Authorization</span></span>|<span data-ttu-id="bf4fb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf4fb-125">接受</span><span class="sxs-lookup"><span data-stu-id="bf4fb-125">Accept</span></span>|<span data-ttu-id="bf4fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bf4fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf4fb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf4fb-127">Request body</span></span>
<span data-ttu-id="bf4fb-128">在请求正文中，提供[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-128">In the request body, supply a JSON representation for the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="bf4fb-129">下表显示创建[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-129">The following table shows the properties that are required when you create the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

|<span data-ttu-id="bf4fb-130">属性</span><span class="sxs-lookup"><span data-stu-id="bf4fb-130">Property</span></span>|<span data-ttu-id="bf4fb-131">类型</span><span class="sxs-lookup"><span data-stu-id="bf4fb-131">Type</span></span>|<span data-ttu-id="bf4fb-132">说明</span><span class="sxs-lookup"><span data-stu-id="bf4fb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf4fb-133">id</span><span class="sxs-lookup"><span data-stu-id="bf4fb-133">id</span></span>|<span data-ttu-id="bf4fb-134">字符串</span><span class="sxs-lookup"><span data-stu-id="bf4fb-134">String</span></span>|<span data-ttu-id="bf4fb-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-135">Key of the entity.</span></span> <span data-ttu-id="bf4fb-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf4fb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bf4fb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf4fb-138">DateTimeOffset</span></span>|<span data-ttu-id="bf4fb-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bf4fb-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bf4fb-141">roleScopeTagIds</span></span>|<span data-ttu-id="bf4fb-142">String collection</span><span class="sxs-lookup"><span data-stu-id="bf4fb-142">String collection</span></span>|<span data-ttu-id="bf4fb-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bf4fb-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bf4fb-145">supportsScopeTags</span></span>|<span data-ttu-id="bf4fb-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf4fb-146">Boolean</span></span>|<span data-ttu-id="bf4fb-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bf4fb-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bf4fb-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bf4fb-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-150">This property is read-only.</span></span> <span data-ttu-id="bf4fb-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bf4fb-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bf4fb-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bf4fb-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bf4fb-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bf4fb-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bf4fb-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bf4fb-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bf4fb-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bf4fb-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bf4fb-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bf4fb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bf4fb-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bf4fb-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bf4fb-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bf4fb-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bf4fb-164">createdDateTime</span></span>|<span data-ttu-id="bf4fb-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf4fb-165">DateTimeOffset</span></span>|<span data-ttu-id="bf4fb-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-166">DateTime the object was created.</span></span> <span data-ttu-id="bf4fb-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-168">说明</span><span class="sxs-lookup"><span data-stu-id="bf4fb-168">description</span></span>|<span data-ttu-id="bf4fb-169">String</span><span class="sxs-lookup"><span data-stu-id="bf4fb-169">String</span></span>|<span data-ttu-id="bf4fb-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bf4fb-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-172">displayName</span><span class="sxs-lookup"><span data-stu-id="bf4fb-172">displayName</span></span>|<span data-ttu-id="bf4fb-173">String</span><span class="sxs-lookup"><span data-stu-id="bf4fb-173">String</span></span>|<span data-ttu-id="bf4fb-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bf4fb-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-176">version</span><span class="sxs-lookup"><span data-stu-id="bf4fb-176">version</span></span>|<span data-ttu-id="bf4fb-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bf4fb-177">Int32</span></span>|<span data-ttu-id="bf4fb-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-178">Version of the device configuration.</span></span> <span data-ttu-id="bf4fb-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="bf4fb-180">connectionName</span></span>|<span data-ttu-id="bf4fb-181">String</span><span class="sxs-lookup"><span data-stu-id="bf4fb-181">String</span></span>|<span data-ttu-id="bf4fb-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-182">Connection name displayed to the user.</span></span> <span data-ttu-id="bf4fb-183">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="bf4fb-184">connectionType</span></span>|[<span data-ttu-id="bf4fb-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="bf4fb-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="bf4fb-186">连接类型。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-186">Connection type.</span></span> <span data-ttu-id="bf4fb-187">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="bf4fb-188">可能的值是：、、、、、、、、、、、、、、、、 `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` 。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`.</span></span>|
|<span data-ttu-id="bf4fb-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="bf4fb-189">loginGroupOrDomain</span></span>|<span data-ttu-id="bf4fb-190">String</span><span class="sxs-lookup"><span data-stu-id="bf4fb-190">String</span></span>|<span data-ttu-id="bf4fb-191">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="bf4fb-192">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-193">role</span><span class="sxs-lookup"><span data-stu-id="bf4fb-193">role</span></span>|<span data-ttu-id="bf4fb-194">String</span><span class="sxs-lookup"><span data-stu-id="bf4fb-194">String</span></span>|<span data-ttu-id="bf4fb-195">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="bf4fb-196">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-197">型</span><span class="sxs-lookup"><span data-stu-id="bf4fb-197">realm</span></span>|<span data-ttu-id="bf4fb-198">String</span><span class="sxs-lookup"><span data-stu-id="bf4fb-198">String</span></span>|<span data-ttu-id="bf4fb-199">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="bf4fb-200">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-201">服务器主板</span><span class="sxs-lookup"><span data-stu-id="bf4fb-201">server</span></span>|[<span data-ttu-id="bf4fb-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="bf4fb-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="bf4fb-203">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-203">VPN Server on the network.</span></span> <span data-ttu-id="bf4fb-204">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="bf4fb-205">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-206">标识符</span><span class="sxs-lookup"><span data-stu-id="bf4fb-206">identifier</span></span>|<span data-ttu-id="bf4fb-207">String</span><span class="sxs-lookup"><span data-stu-id="bf4fb-207">String</span></span>|<span data-ttu-id="bf4fb-208">当连接类型设置为自定义 VPN 时，由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="bf4fb-209">例如： Cisco AnyConnect 使用从[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)继承的 AnyConnect applevpn 的标识符。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-210">customData</span><span class="sxs-lookup"><span data-stu-id="bf4fb-210">customData</span></span>|<span data-ttu-id="bf4fb-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bf4fb-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="bf4fb-212">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="bf4fb-213">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="bf4fb-214">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="bf4fb-215">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="bf4fb-216">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="bf4fb-217">customKeyValueData</span></span>|<span data-ttu-id="bf4fb-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bf4fb-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="bf4fb-219">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="bf4fb-220">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="bf4fb-221">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="bf4fb-222">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="bf4fb-223">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="bf4fb-224">enableSplitTunneling</span></span>|<span data-ttu-id="bf4fb-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf4fb-225">Boolean</span></span>|<span data-ttu-id="bf4fb-226">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="bf4fb-227">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="bf4fb-228">authenticationMethod</span></span>|[<span data-ttu-id="bf4fb-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="bf4fb-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="bf4fb-230">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="bf4fb-231">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="bf4fb-232">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="bf4fb-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="bf4fb-233">enablePerApp</span></span>|<span data-ttu-id="bf4fb-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf4fb-234">Boolean</span></span>|<span data-ttu-id="bf4fb-235">将此设置为 true 将创建每个应用程序 VPN 有效负载，以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="bf4fb-236">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="bf4fb-237">safariDomains</span></span>|<span data-ttu-id="bf4fb-238">String collection</span><span class="sxs-lookup"><span data-stu-id="bf4fb-238">String collection</span></span>|<span data-ttu-id="bf4fb-239">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="bf4fb-240">除了与此 VPN 关联的应用程序之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="bf4fb-241">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="bf4fb-242">onDemandRules</span></span>|<span data-ttu-id="bf4fb-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf4fb-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="bf4fb-244">按需规则。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-244">On-Demand Rules.</span></span> <span data-ttu-id="bf4fb-245">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="bf4fb-246">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-247">proxyServer</span><span class="sxs-lookup"><span data-stu-id="bf4fb-247">proxyServer</span></span>|[<span data-ttu-id="bf4fb-248">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="bf4fb-248">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="bf4fb-249">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-249">Proxy Server.</span></span> <span data-ttu-id="bf4fb-250">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="bf4fb-251">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="bf4fb-251">optInToDeviceIdSharing</span></span>|<span data-ttu-id="bf4fb-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf4fb-252">Boolean</span></span>|<span data-ttu-id="bf4fb-253">选择将设备的 Id 共享到第三方 vpn 客户端，以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-253">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="bf4fb-254">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf4fb-254">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="bf4fb-255">响应</span><span class="sxs-lookup"><span data-stu-id="bf4fb-255">Response</span></span>
<span data-ttu-id="bf4fb-256">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-256">If successful, this method returns a `200 OK` response code and an updated [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf4fb-257">示例</span><span class="sxs-lookup"><span data-stu-id="bf4fb-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf4fb-258">请求</span><span class="sxs-lookup"><span data-stu-id="bf4fb-258">Request</span></span>
<span data-ttu-id="bf4fb-259">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-259">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bf4fb-260">响应</span><span class="sxs-lookup"><span data-stu-id="bf4fb-260">Response</span></span>
<span data-ttu-id="bf4fb-p129">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bf4fb-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



