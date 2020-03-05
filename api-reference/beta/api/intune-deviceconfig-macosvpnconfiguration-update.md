---
title: 更新 macOSVpnConfiguration
description: 更新 macOSVpnConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c6ccf0638343628d9fb33316d1b380273bf4c7a7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448667"
---
# <a name="update-macosvpnconfiguration"></a><span data-ttu-id="5c546-103">更新 macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="5c546-103">Update macOSVpnConfiguration</span></span>

<span data-ttu-id="5c546-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5c546-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c546-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5c546-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c546-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5c546-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c546-107">更新[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5c546-107">Update the properties of a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c546-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5c546-108">Prerequisites</span></span>
<span data-ttu-id="5c546-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c546-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c546-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c546-111">Permission type</span></span>|<span data-ttu-id="5c546-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5c546-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c546-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c546-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c546-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c546-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5c546-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c546-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c546-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c546-116">Not supported.</span></span>|
|<span data-ttu-id="5c546-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c546-117">Application</span></span>|<span data-ttu-id="5c546-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c546-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c546-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c546-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5c546-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c546-120">Request headers</span></span>
|<span data-ttu-id="5c546-121">标头</span><span class="sxs-lookup"><span data-stu-id="5c546-121">Header</span></span>|<span data-ttu-id="5c546-122">值</span><span class="sxs-lookup"><span data-stu-id="5c546-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c546-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c546-123">Authorization</span></span>|<span data-ttu-id="5c546-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5c546-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c546-125">接受</span><span class="sxs-lookup"><span data-stu-id="5c546-125">Accept</span></span>|<span data-ttu-id="5c546-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c546-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c546-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c546-127">Request body</span></span>
<span data-ttu-id="5c546-128">在请求正文中，提供[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c546-128">In the request body, supply a JSON representation for the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="5c546-129">下表显示创建[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5c546-129">The following table shows the properties that are required when you create the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

|<span data-ttu-id="5c546-130">属性</span><span class="sxs-lookup"><span data-stu-id="5c546-130">Property</span></span>|<span data-ttu-id="5c546-131">类型</span><span class="sxs-lookup"><span data-stu-id="5c546-131">Type</span></span>|<span data-ttu-id="5c546-132">说明</span><span class="sxs-lookup"><span data-stu-id="5c546-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c546-133">id</span><span class="sxs-lookup"><span data-stu-id="5c546-133">id</span></span>|<span data-ttu-id="5c546-134">字符串</span><span class="sxs-lookup"><span data-stu-id="5c546-134">String</span></span>|<span data-ttu-id="5c546-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5c546-135">Key of the entity.</span></span> <span data-ttu-id="5c546-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c546-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5c546-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c546-138">DateTimeOffset</span></span>|<span data-ttu-id="5c546-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5c546-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5c546-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5c546-141">roleScopeTagIds</span></span>|<span data-ttu-id="5c546-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="5c546-142">String collection</span></span>|<span data-ttu-id="5c546-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="5c546-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5c546-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5c546-145">supportsScopeTags</span></span>|<span data-ttu-id="5c546-146">布尔</span><span class="sxs-lookup"><span data-stu-id="5c546-146">Boolean</span></span>|<span data-ttu-id="5c546-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="5c546-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5c546-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="5c546-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5c546-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="5c546-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5c546-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5c546-150">This property is read-only.</span></span> <span data-ttu-id="5c546-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5c546-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5c546-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5c546-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5c546-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="5c546-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5c546-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5c546-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5c546-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5c546-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5c546-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="5c546-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5c546-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5c546-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5c546-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5c546-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5c546-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="5c546-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5c546-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c546-164">createdDateTime</span></span>|<span data-ttu-id="5c546-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c546-165">DateTimeOffset</span></span>|<span data-ttu-id="5c546-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5c546-166">DateTime the object was created.</span></span> <span data-ttu-id="5c546-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-168">说明</span><span class="sxs-lookup"><span data-stu-id="5c546-168">description</span></span>|<span data-ttu-id="5c546-169">String</span><span class="sxs-lookup"><span data-stu-id="5c546-169">String</span></span>|<span data-ttu-id="5c546-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="5c546-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5c546-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-172">displayName</span><span class="sxs-lookup"><span data-stu-id="5c546-172">displayName</span></span>|<span data-ttu-id="5c546-173">String</span><span class="sxs-lookup"><span data-stu-id="5c546-173">String</span></span>|<span data-ttu-id="5c546-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="5c546-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5c546-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-176">version</span><span class="sxs-lookup"><span data-stu-id="5c546-176">version</span></span>|<span data-ttu-id="5c546-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5c546-177">Int32</span></span>|<span data-ttu-id="5c546-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5c546-178">Version of the device configuration.</span></span> <span data-ttu-id="5c546-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="5c546-180">connectionName</span></span>|<span data-ttu-id="5c546-181">String</span><span class="sxs-lookup"><span data-stu-id="5c546-181">String</span></span>|<span data-ttu-id="5c546-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="5c546-182">Connection name displayed to the user.</span></span> <span data-ttu-id="5c546-183">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="5c546-184">connectionType</span></span>|[<span data-ttu-id="5c546-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="5c546-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="5c546-186">连接类型。</span><span class="sxs-lookup"><span data-stu-id="5c546-186">Connection type.</span></span> <span data-ttu-id="5c546-187">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="5c546-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="5c546-188">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`customVpn`、`ciscoIPSec`、`citrix`、`ciscoAnyConnectV2`、`paloAltoGlobalProtect`、`zscalerPrivateAccess`、`f5Access2018`、`citrixSso`、`paloAltoGlobalProtectV2`、`ikEv2`、`alwaysOn`。</span><span class="sxs-lookup"><span data-stu-id="5c546-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span></span>|
|<span data-ttu-id="5c546-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="5c546-189">loginGroupOrDomain</span></span>|<span data-ttu-id="5c546-190">String</span><span class="sxs-lookup"><span data-stu-id="5c546-190">String</span></span>|<span data-ttu-id="5c546-191">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="5c546-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="5c546-192">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-193">role</span><span class="sxs-lookup"><span data-stu-id="5c546-193">role</span></span>|<span data-ttu-id="5c546-194">String</span><span class="sxs-lookup"><span data-stu-id="5c546-194">String</span></span>|<span data-ttu-id="5c546-195">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="5c546-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="5c546-196">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-197">型</span><span class="sxs-lookup"><span data-stu-id="5c546-197">realm</span></span>|<span data-ttu-id="5c546-198">String</span><span class="sxs-lookup"><span data-stu-id="5c546-198">String</span></span>|<span data-ttu-id="5c546-199">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="5c546-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="5c546-200">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-201">服务器主板</span><span class="sxs-lookup"><span data-stu-id="5c546-201">server</span></span>|[<span data-ttu-id="5c546-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="5c546-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="5c546-203">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="5c546-203">VPN Server on the network.</span></span> <span data-ttu-id="5c546-204">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="5c546-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="5c546-205">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-206">标识符</span><span class="sxs-lookup"><span data-stu-id="5c546-206">identifier</span></span>|<span data-ttu-id="5c546-207">String</span><span class="sxs-lookup"><span data-stu-id="5c546-207">String</span></span>|<span data-ttu-id="5c546-208">当连接类型设置为自定义 VPN 时，由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="5c546-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="5c546-209">例如： Cisco AnyConnect 使用从[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)继承的 AnyConnect applevpn 的标识符。</span><span class="sxs-lookup"><span data-stu-id="5c546-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-210">customData</span><span class="sxs-lookup"><span data-stu-id="5c546-210">customData</span></span>|<span data-ttu-id="5c546-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5c546-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="5c546-212">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="5c546-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="5c546-213">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="5c546-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="5c546-214">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="5c546-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="5c546-215">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="5c546-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="5c546-216">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="5c546-217">customKeyValueData</span></span>|<span data-ttu-id="5c546-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5c546-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="5c546-219">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="5c546-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="5c546-220">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="5c546-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="5c546-221">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="5c546-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="5c546-222">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="5c546-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="5c546-223">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="5c546-224">enableSplitTunneling</span></span>|<span data-ttu-id="5c546-225">布尔</span><span class="sxs-lookup"><span data-stu-id="5c546-225">Boolean</span></span>|<span data-ttu-id="5c546-226">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="5c546-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="5c546-227">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5c546-228">authenticationMethod</span></span>|[<span data-ttu-id="5c546-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5c546-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="5c546-230">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="5c546-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="5c546-231">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="5c546-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="5c546-232">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="5c546-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="5c546-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="5c546-233">enablePerApp</span></span>|<span data-ttu-id="5c546-234">布尔</span><span class="sxs-lookup"><span data-stu-id="5c546-234">Boolean</span></span>|<span data-ttu-id="5c546-235">将此设置为 true 将创建每个应用程序 VPN 有效负载，以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="5c546-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="5c546-236">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="5c546-237">safariDomains</span></span>|<span data-ttu-id="5c546-238">String 集合</span><span class="sxs-lookup"><span data-stu-id="5c546-238">String collection</span></span>|<span data-ttu-id="5c546-239">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="5c546-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="5c546-240">除了与此 VPN 关联的应用程序之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="5c546-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="5c546-241">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="5c546-242">onDemandRules</span></span>|<span data-ttu-id="5c546-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="5c546-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="5c546-244">按需规则。</span><span class="sxs-lookup"><span data-stu-id="5c546-244">On-Demand Rules.</span></span> <span data-ttu-id="5c546-245">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="5c546-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="5c546-246">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-247">proxyServer</span><span class="sxs-lookup"><span data-stu-id="5c546-247">proxyServer</span></span>|[<span data-ttu-id="5c546-248">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="5c546-248">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="5c546-249">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="5c546-249">Proxy Server.</span></span> <span data-ttu-id="5c546-250">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="5c546-251">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="5c546-251">optInToDeviceIdSharing</span></span>|<span data-ttu-id="5c546-252">布尔</span><span class="sxs-lookup"><span data-stu-id="5c546-252">Boolean</span></span>|<span data-ttu-id="5c546-253">选择将设备的 Id 共享到第三方 vpn 客户端，以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="5c546-253">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="5c546-254">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c546-254">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="5c546-255">响应</span><span class="sxs-lookup"><span data-stu-id="5c546-255">Response</span></span>
<span data-ttu-id="5c546-256">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5c546-256">If successful, this method returns a `200 OK` response code and an updated [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c546-257">示例</span><span class="sxs-lookup"><span data-stu-id="5c546-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c546-258">请求</span><span class="sxs-lookup"><span data-stu-id="5c546-258">Request</span></span>
<span data-ttu-id="5c546-259">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5c546-259">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5c546-260">响应</span><span class="sxs-lookup"><span data-stu-id="5c546-260">Response</span></span>
<span data-ttu-id="5c546-p129">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5c546-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





