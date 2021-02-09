---
title: 创建 iosVpnConfiguration
description: 创建新的 iosVpnConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 62fbdb6406d2c33541ca82a324836d1f66c265ed
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155802"
---
# <a name="create-iosvpnconfiguration"></a><span data-ttu-id="72200-103">创建 iosVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="72200-103">Create iosVpnConfiguration</span></span>

<span data-ttu-id="72200-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72200-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72200-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="72200-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72200-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="72200-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72200-107">创建新的 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72200-107">Create a new [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72200-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="72200-108">Prerequisites</span></span>
<span data-ttu-id="72200-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72200-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72200-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="72200-111">Permission type</span></span>|<span data-ttu-id="72200-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="72200-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72200-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72200-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72200-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72200-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="72200-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72200-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72200-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="72200-116">Not supported.</span></span>|
|<span data-ttu-id="72200-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="72200-117">Application</span></span>|<span data-ttu-id="72200-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72200-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72200-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72200-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="72200-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="72200-120">Request headers</span></span>
|<span data-ttu-id="72200-121">标头</span><span class="sxs-lookup"><span data-stu-id="72200-121">Header</span></span>|<span data-ttu-id="72200-122">值</span><span class="sxs-lookup"><span data-stu-id="72200-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72200-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="72200-123">Authorization</span></span>|<span data-ttu-id="72200-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="72200-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72200-125">接受</span><span class="sxs-lookup"><span data-stu-id="72200-125">Accept</span></span>|<span data-ttu-id="72200-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72200-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72200-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="72200-127">Request body</span></span>
<span data-ttu-id="72200-128">在请求正文中，提供 iosVpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72200-128">In the request body, supply a JSON representation for the iosVpnConfiguration object.</span></span>

<span data-ttu-id="72200-129">下表显示创建 iosVpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="72200-129">The following table shows the properties that are required when you create the iosVpnConfiguration.</span></span>

|<span data-ttu-id="72200-130">属性</span><span class="sxs-lookup"><span data-stu-id="72200-130">Property</span></span>|<span data-ttu-id="72200-131">类型</span><span class="sxs-lookup"><span data-stu-id="72200-131">Type</span></span>|<span data-ttu-id="72200-132">说明</span><span class="sxs-lookup"><span data-stu-id="72200-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72200-133">id</span><span class="sxs-lookup"><span data-stu-id="72200-133">id</span></span>|<span data-ttu-id="72200-134">String</span><span class="sxs-lookup"><span data-stu-id="72200-134">String</span></span>|<span data-ttu-id="72200-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="72200-135">Key of the entity.</span></span> <span data-ttu-id="72200-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72200-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72200-137">lastModifiedDateTime</span></span>|<span data-ttu-id="72200-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72200-138">DateTimeOffset</span></span>|<span data-ttu-id="72200-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="72200-139">DateTime the object was last modified.</span></span> <span data-ttu-id="72200-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72200-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="72200-141">roleScopeTagIds</span></span>|<span data-ttu-id="72200-142">字符串集合</span><span class="sxs-lookup"><span data-stu-id="72200-142">String collection</span></span>|<span data-ttu-id="72200-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="72200-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="72200-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72200-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="72200-145">supportsScopeTags</span></span>|<span data-ttu-id="72200-146">布尔</span><span class="sxs-lookup"><span data-stu-id="72200-146">Boolean</span></span>|<span data-ttu-id="72200-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="72200-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="72200-148">如果此值为 false 且实体对范围用户不可见，则不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="72200-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="72200-149">这适用于在 Silverlight 中创建的旧策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="72200-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="72200-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="72200-150">This property is read-only.</span></span> <span data-ttu-id="72200-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72200-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="72200-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="72200-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="72200-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="72200-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="72200-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="72200-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72200-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="72200-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="72200-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="72200-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="72200-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="72200-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="72200-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72200-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="72200-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="72200-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="72200-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="72200-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="72200-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="72200-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72200-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="72200-164">createdDateTime</span></span>|<span data-ttu-id="72200-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72200-165">DateTimeOffset</span></span>|<span data-ttu-id="72200-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="72200-166">DateTime the object was created.</span></span> <span data-ttu-id="72200-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72200-168">说明</span><span class="sxs-lookup"><span data-stu-id="72200-168">description</span></span>|<span data-ttu-id="72200-169">String</span><span class="sxs-lookup"><span data-stu-id="72200-169">String</span></span>|<span data-ttu-id="72200-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="72200-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="72200-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72200-172">displayName</span><span class="sxs-lookup"><span data-stu-id="72200-172">displayName</span></span>|<span data-ttu-id="72200-173">String</span><span class="sxs-lookup"><span data-stu-id="72200-173">String</span></span>|<span data-ttu-id="72200-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="72200-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="72200-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72200-176">version</span><span class="sxs-lookup"><span data-stu-id="72200-176">version</span></span>|<span data-ttu-id="72200-177">Int32</span><span class="sxs-lookup"><span data-stu-id="72200-177">Int32</span></span>|<span data-ttu-id="72200-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="72200-178">Version of the device configuration.</span></span> <span data-ttu-id="72200-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72200-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="72200-180">connectionName</span></span>|<span data-ttu-id="72200-181">String</span><span class="sxs-lookup"><span data-stu-id="72200-181">String</span></span>|<span data-ttu-id="72200-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="72200-182">Connection name displayed to the user.</span></span> <span data-ttu-id="72200-183">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="72200-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="72200-184">connectionType</span></span>|[<span data-ttu-id="72200-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="72200-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="72200-186">连接类型。</span><span class="sxs-lookup"><span data-stu-id="72200-186">Connection type.</span></span> <span data-ttu-id="72200-187">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="72200-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="72200-188">可能的值是： `ciscoAnyConnect` ， ， ， ， ， ， ， ， `pulseSecure` ， `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` 。</span><span class="sxs-lookup"><span data-stu-id="72200-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="72200-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="72200-189">loginGroupOrDomain</span></span>|<span data-ttu-id="72200-190">String</span><span class="sxs-lookup"><span data-stu-id="72200-190">String</span></span>|<span data-ttu-id="72200-191">连接类型设置为 Dell SonicWALL Mobile Connection 时登录组或域。</span><span class="sxs-lookup"><span data-stu-id="72200-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="72200-192">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="72200-193">role</span><span class="sxs-lookup"><span data-stu-id="72200-193">role</span></span>|<span data-ttu-id="72200-194">String</span><span class="sxs-lookup"><span data-stu-id="72200-194">String</span></span>|<span data-ttu-id="72200-195">将连接类型设置为"脉冲安全"时的角色。</span><span class="sxs-lookup"><span data-stu-id="72200-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="72200-196">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="72200-197">realm</span><span class="sxs-lookup"><span data-stu-id="72200-197">realm</span></span>|<span data-ttu-id="72200-198">String</span><span class="sxs-lookup"><span data-stu-id="72200-198">String</span></span>|<span data-ttu-id="72200-199">连接类型设置为"脉冲安全"时的领域。</span><span class="sxs-lookup"><span data-stu-id="72200-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="72200-200">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="72200-201">server</span><span class="sxs-lookup"><span data-stu-id="72200-201">server</span></span>|[<span data-ttu-id="72200-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="72200-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="72200-203">网络 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="72200-203">VPN Server on the network.</span></span> <span data-ttu-id="72200-204">确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="72200-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="72200-205">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="72200-206">标识符</span><span class="sxs-lookup"><span data-stu-id="72200-206">identifier</span></span>|<span data-ttu-id="72200-207">String</span><span class="sxs-lookup"><span data-stu-id="72200-207">String</span></span>|<span data-ttu-id="72200-208">连接类型设置为自定义 VPN 时 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="72200-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="72200-209">例如：Cisco AnyConnect 使用窗体 com.cisco.anyconnect.applevpn.plugin 的标识符 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="72200-210">customData</span><span class="sxs-lookup"><span data-stu-id="72200-210">customData</span></span>|<span data-ttu-id="72200-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72200-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="72200-212">连接类型设置为自定义 VPN 时自定义数据。</span><span class="sxs-lookup"><span data-stu-id="72200-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="72200-213">使用此字段启用 Intune 不支持但在 VPN 解决方案中提供的功能。</span><span class="sxs-lookup"><span data-stu-id="72200-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="72200-214">请联系 VPN 供应商，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="72200-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="72200-215">此集合最多可包含 25 个元素。</span><span class="sxs-lookup"><span data-stu-id="72200-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="72200-216">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="72200-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="72200-217">customKeyValueData</span></span>|<span data-ttu-id="72200-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72200-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="72200-219">连接类型设置为自定义 VPN 时自定义数据。</span><span class="sxs-lookup"><span data-stu-id="72200-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="72200-220">使用此字段启用 Intune 不支持但在 VPN 解决方案中提供的功能。</span><span class="sxs-lookup"><span data-stu-id="72200-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="72200-221">请联系 VPN 供应商，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="72200-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="72200-222">此集合最多可包含 25 个元素。</span><span class="sxs-lookup"><span data-stu-id="72200-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="72200-223">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="72200-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="72200-224">enableSplitTunneling</span></span>|<span data-ttu-id="72200-225">布尔</span><span class="sxs-lookup"><span data-stu-id="72200-225">Boolean</span></span>|<span data-ttu-id="72200-226">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="72200-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="72200-227">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="72200-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="72200-228">authenticationMethod</span></span>|[<span data-ttu-id="72200-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="72200-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="72200-230">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="72200-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="72200-231">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="72200-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="72200-232">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="72200-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="72200-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="72200-233">enablePerApp</span></span>|<span data-ttu-id="72200-234">布尔</span><span class="sxs-lookup"><span data-stu-id="72200-234">Boolean</span></span>|<span data-ttu-id="72200-235">如果设置为 true，Per-App VPN 负载，稍后可以与在最终用户的 iOS 设备上触发此 VPN 连接的应用关联。</span><span class="sxs-lookup"><span data-stu-id="72200-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="72200-236">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="72200-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="72200-237">safariDomains</span></span>|<span data-ttu-id="72200-238">字符串集合</span><span class="sxs-lookup"><span data-stu-id="72200-238">String collection</span></span>|<span data-ttu-id="72200-239">启用此 VPN（每个应用）设置时，Safari 域。</span><span class="sxs-lookup"><span data-stu-id="72200-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="72200-240">除了与此 VPN 关联的应用之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="72200-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="72200-241">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="72200-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="72200-242">onDemandRules</span></span>|<span data-ttu-id="72200-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72200-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="72200-244">按需规则。</span><span class="sxs-lookup"><span data-stu-id="72200-244">On-Demand Rules.</span></span> <span data-ttu-id="72200-245">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="72200-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="72200-246">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="72200-247">providerType</span><span class="sxs-lookup"><span data-stu-id="72200-247">providerType</span></span>|[<span data-ttu-id="72200-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="72200-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="72200-249">每个应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="72200-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="72200-250">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="72200-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="72200-251">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="72200-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="72200-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="72200-252">associatedDomains</span></span>|<span data-ttu-id="72200-253">字符串集合</span><span class="sxs-lookup"><span data-stu-id="72200-253">String collection</span></span>|<span data-ttu-id="72200-254">关联的域 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="72200-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="72200-255">excludedDomains</span></span>|<span data-ttu-id="72200-256">字符串集合</span><span class="sxs-lookup"><span data-stu-id="72200-256">String collection</span></span>|<span data-ttu-id="72200-257">通过公共 Internet 而不是 VPN 访问的域，即使每个应用 VPN 已激活也是如此。继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="72200-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="72200-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="72200-259">布尔</span><span class="sxs-lookup"><span data-stu-id="72200-259">Boolean</span></span>|<span data-ttu-id="72200-260">切换以阻止用户在"设置"应用中禁用自动 VPN 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="72200-261">proxyServer</span><span class="sxs-lookup"><span data-stu-id="72200-261">proxyServer</span></span>|[<span data-ttu-id="72200-262">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="72200-262">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="72200-263">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="72200-263">Proxy Server.</span></span> <span data-ttu-id="72200-264">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-264">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="72200-265">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="72200-265">optInToDeviceIdSharing</span></span>|<span data-ttu-id="72200-266">布尔</span><span class="sxs-lookup"><span data-stu-id="72200-266">Boolean</span></span>|<span data-ttu-id="72200-267">Opt-In将设备 ID 共享给第三方 vpn 客户端，以在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="72200-267">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="72200-268">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72200-268">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="72200-269">userDomain</span><span class="sxs-lookup"><span data-stu-id="72200-269">userDomain</span></span>|<span data-ttu-id="72200-270">String</span><span class="sxs-lookup"><span data-stu-id="72200-270">String</span></span>|<span data-ttu-id="72200-271">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="72200-271">Zscaler only.</span></span> <span data-ttu-id="72200-272">输入静态域以在 Zscaler 应用中预填充登录字段。</span><span class="sxs-lookup"><span data-stu-id="72200-272">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="72200-273">如果此域留空，则改为使用用户的 Azure Active Directory 域。</span><span class="sxs-lookup"><span data-stu-id="72200-273">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="72200-274">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="72200-274">strictEnforcement</span></span>|<span data-ttu-id="72200-275">布尔</span><span class="sxs-lookup"><span data-stu-id="72200-275">Boolean</span></span>|<span data-ttu-id="72200-276">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="72200-276">Zscaler only.</span></span> <span data-ttu-id="72200-277">阻止网络流量，直到用户登录 Zscaler 应用。</span><span class="sxs-lookup"><span data-stu-id="72200-277">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="72200-278">"True"表示流量被阻止。</span><span class="sxs-lookup"><span data-stu-id="72200-278">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="72200-279">cloudName</span><span class="sxs-lookup"><span data-stu-id="72200-279">cloudName</span></span>|<span data-ttu-id="72200-280">String</span><span class="sxs-lookup"><span data-stu-id="72200-280">String</span></span>|<span data-ttu-id="72200-281">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="72200-281">Zscaler only.</span></span> <span data-ttu-id="72200-282">用户分配到的 Zscaler 云。</span><span class="sxs-lookup"><span data-stu-id="72200-282">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="72200-283">excludeList</span><span class="sxs-lookup"><span data-stu-id="72200-283">excludeList</span></span>|<span data-ttu-id="72200-284">字符串集合</span><span class="sxs-lookup"><span data-stu-id="72200-284">String collection</span></span>|<span data-ttu-id="72200-285">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="72200-285">Zscaler only.</span></span> <span data-ttu-id="72200-286">未通过 Zscaler 云发送的网络地址列表。</span><span class="sxs-lookup"><span data-stu-id="72200-286">List of network addresses which are not sent through the Zscaler cloud.</span></span>|
|<span data-ttu-id="72200-287">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="72200-287">targetedMobileApps</span></span>|<span data-ttu-id="72200-288">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72200-288">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="72200-289">目标移动应用。</span><span class="sxs-lookup"><span data-stu-id="72200-289">Targeted mobile apps.</span></span> <span data-ttu-id="72200-290">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="72200-290">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="72200-291">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="72200-291">microsoftTunnelSiteId</span></span>|<span data-ttu-id="72200-292">String</span><span class="sxs-lookup"><span data-stu-id="72200-292">String</span></span>|<span data-ttu-id="72200-293">Microsoft 隧道站点 ID。</span><span class="sxs-lookup"><span data-stu-id="72200-293">Microsoft Tunnel site ID.</span></span>|



## <a name="response"></a><span data-ttu-id="72200-294">响应</span><span class="sxs-lookup"><span data-stu-id="72200-294">Response</span></span>
<span data-ttu-id="72200-295">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72200-295">If successful, this method returns a `201 Created` response code and a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72200-296">示例</span><span class="sxs-lookup"><span data-stu-id="72200-296">Example</span></span>

### <a name="request"></a><span data-ttu-id="72200-297">请求</span><span class="sxs-lookup"><span data-stu-id="72200-297">Request</span></span>
<span data-ttu-id="72200-298">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="72200-298">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3298

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
  "associatedDomains": [
    "Associated Domains value"
  ],
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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```

### <a name="response"></a><span data-ttu-id="72200-299">响应</span><span class="sxs-lookup"><span data-stu-id="72200-299">Response</span></span>
<span data-ttu-id="72200-p135">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="72200-p135">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3470

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
  "associatedDomains": [
    "Associated Domains value"
  ],
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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```




