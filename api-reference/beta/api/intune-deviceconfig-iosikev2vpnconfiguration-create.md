---
title: 创建 iosikEv2VpnConfiguration
description: 创建新的 iosikEv2VpnConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 104a115acd07324c98ef7e3c8598734663dba7c3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442759"
---
# <a name="create-iosikev2vpnconfiguration"></a><span data-ttu-id="8e554-103">创建 iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="8e554-103">Create iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="8e554-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8e554-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e554-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8e554-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e554-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8e554-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e554-107">创建新的[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8e554-107">Create a new [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e554-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8e554-108">Prerequisites</span></span>
<span data-ttu-id="8e554-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e554-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e554-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e554-111">Permission type</span></span>|<span data-ttu-id="8e554-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8e554-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e554-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e554-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e554-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e554-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e554-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e554-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e554-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e554-116">Not supported.</span></span>|
|<span data-ttu-id="8e554-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e554-117">Application</span></span>|<span data-ttu-id="8e554-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e554-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e554-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e554-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8e554-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e554-120">Request headers</span></span>
|<span data-ttu-id="8e554-121">标头</span><span class="sxs-lookup"><span data-stu-id="8e554-121">Header</span></span>|<span data-ttu-id="8e554-122">值</span><span class="sxs-lookup"><span data-stu-id="8e554-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e554-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e554-123">Authorization</span></span>|<span data-ttu-id="8e554-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8e554-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e554-125">接受</span><span class="sxs-lookup"><span data-stu-id="8e554-125">Accept</span></span>|<span data-ttu-id="8e554-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e554-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e554-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e554-127">Request body</span></span>
<span data-ttu-id="8e554-128">在请求正文中，提供 iosikEv2VpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e554-128">In the request body, supply a JSON representation for the iosikEv2VpnConfiguration object.</span></span>

<span data-ttu-id="8e554-129">下表显示创建 iosikEv2VpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8e554-129">The following table shows the properties that are required when you create the iosikEv2VpnConfiguration.</span></span>

|<span data-ttu-id="8e554-130">属性</span><span class="sxs-lookup"><span data-stu-id="8e554-130">Property</span></span>|<span data-ttu-id="8e554-131">类型</span><span class="sxs-lookup"><span data-stu-id="8e554-131">Type</span></span>|<span data-ttu-id="8e554-132">说明</span><span class="sxs-lookup"><span data-stu-id="8e554-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e554-133">id</span><span class="sxs-lookup"><span data-stu-id="8e554-133">id</span></span>|<span data-ttu-id="8e554-134">字符串</span><span class="sxs-lookup"><span data-stu-id="8e554-134">String</span></span>|<span data-ttu-id="8e554-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8e554-135">Key of the entity.</span></span> <span data-ttu-id="8e554-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e554-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8e554-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e554-138">DateTimeOffset</span></span>|<span data-ttu-id="8e554-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8e554-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8e554-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8e554-141">roleScopeTagIds</span></span>|<span data-ttu-id="8e554-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="8e554-142">String collection</span></span>|<span data-ttu-id="8e554-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="8e554-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8e554-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8e554-145">supportsScopeTags</span></span>|<span data-ttu-id="8e554-146">布尔</span><span class="sxs-lookup"><span data-stu-id="8e554-146">Boolean</span></span>|<span data-ttu-id="8e554-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="8e554-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8e554-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="8e554-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8e554-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="8e554-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8e554-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8e554-150">This property is read-only.</span></span> <span data-ttu-id="8e554-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8e554-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8e554-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8e554-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8e554-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="8e554-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8e554-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8e554-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8e554-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8e554-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8e554-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="8e554-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8e554-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8e554-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8e554-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8e554-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8e554-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="8e554-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8e554-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e554-164">createdDateTime</span></span>|<span data-ttu-id="8e554-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e554-165">DateTimeOffset</span></span>|<span data-ttu-id="8e554-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8e554-166">DateTime the object was created.</span></span> <span data-ttu-id="8e554-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-168">说明</span><span class="sxs-lookup"><span data-stu-id="8e554-168">description</span></span>|<span data-ttu-id="8e554-169">String</span><span class="sxs-lookup"><span data-stu-id="8e554-169">String</span></span>|<span data-ttu-id="8e554-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="8e554-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8e554-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-172">displayName</span><span class="sxs-lookup"><span data-stu-id="8e554-172">displayName</span></span>|<span data-ttu-id="8e554-173">String</span><span class="sxs-lookup"><span data-stu-id="8e554-173">String</span></span>|<span data-ttu-id="8e554-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="8e554-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8e554-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-176">version</span><span class="sxs-lookup"><span data-stu-id="8e554-176">version</span></span>|<span data-ttu-id="8e554-177">Int32</span><span class="sxs-lookup"><span data-stu-id="8e554-177">Int32</span></span>|<span data-ttu-id="8e554-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="8e554-178">Version of the device configuration.</span></span> <span data-ttu-id="8e554-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="8e554-180">connectionName</span></span>|<span data-ttu-id="8e554-181">String</span><span class="sxs-lookup"><span data-stu-id="8e554-181">String</span></span>|<span data-ttu-id="8e554-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="8e554-182">Connection name displayed to the user.</span></span> <span data-ttu-id="8e554-183">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="8e554-184">connectionType</span></span>|[<span data-ttu-id="8e554-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="8e554-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="8e554-186">连接类型。</span><span class="sxs-lookup"><span data-stu-id="8e554-186">Connection type.</span></span> <span data-ttu-id="8e554-187">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="8e554-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="8e554-188">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`customVpn`、`ciscoIPSec`、`citrix`、`ciscoAnyConnectV2`、`paloAltoGlobalProtect`、`zscalerPrivateAccess`、`f5Access2018`、`citrixSso`、`paloAltoGlobalProtectV2`、`ikEv2`、`alwaysOn`。</span><span class="sxs-lookup"><span data-stu-id="8e554-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span></span>|
|<span data-ttu-id="8e554-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="8e554-189">loginGroupOrDomain</span></span>|<span data-ttu-id="8e554-190">String</span><span class="sxs-lookup"><span data-stu-id="8e554-190">String</span></span>|<span data-ttu-id="8e554-191">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="8e554-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="8e554-192">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-193">role</span><span class="sxs-lookup"><span data-stu-id="8e554-193">role</span></span>|<span data-ttu-id="8e554-194">String</span><span class="sxs-lookup"><span data-stu-id="8e554-194">String</span></span>|<span data-ttu-id="8e554-195">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="8e554-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="8e554-196">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-197">型</span><span class="sxs-lookup"><span data-stu-id="8e554-197">realm</span></span>|<span data-ttu-id="8e554-198">String</span><span class="sxs-lookup"><span data-stu-id="8e554-198">String</span></span>|<span data-ttu-id="8e554-199">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="8e554-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="8e554-200">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-201">服务器主板</span><span class="sxs-lookup"><span data-stu-id="8e554-201">server</span></span>|[<span data-ttu-id="8e554-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="8e554-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="8e554-203">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="8e554-203">VPN Server on the network.</span></span> <span data-ttu-id="8e554-204">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="8e554-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="8e554-205">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-206">标识符</span><span class="sxs-lookup"><span data-stu-id="8e554-206">identifier</span></span>|<span data-ttu-id="8e554-207">String</span><span class="sxs-lookup"><span data-stu-id="8e554-207">String</span></span>|<span data-ttu-id="8e554-208">当连接类型设置为自定义 VPN 时，由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="8e554-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="8e554-209">例如： Cisco AnyConnect 使用从[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)继承的 AnyConnect applevpn 的标识符。</span><span class="sxs-lookup"><span data-stu-id="8e554-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-210">customData</span><span class="sxs-lookup"><span data-stu-id="8e554-210">customData</span></span>|<span data-ttu-id="8e554-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8e554-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="8e554-212">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="8e554-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="8e554-213">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="8e554-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="8e554-214">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="8e554-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="8e554-215">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="8e554-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="8e554-216">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="8e554-217">customKeyValueData</span></span>|<span data-ttu-id="8e554-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8e554-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="8e554-219">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="8e554-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="8e554-220">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="8e554-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="8e554-221">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="8e554-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="8e554-222">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="8e554-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="8e554-223">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="8e554-224">enableSplitTunneling</span></span>|<span data-ttu-id="8e554-225">布尔</span><span class="sxs-lookup"><span data-stu-id="8e554-225">Boolean</span></span>|<span data-ttu-id="8e554-226">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="8e554-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="8e554-227">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8e554-228">authenticationMethod</span></span>|[<span data-ttu-id="8e554-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8e554-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="8e554-230">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="8e554-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="8e554-231">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="8e554-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="8e554-232">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="8e554-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="8e554-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="8e554-233">enablePerApp</span></span>|<span data-ttu-id="8e554-234">布尔</span><span class="sxs-lookup"><span data-stu-id="8e554-234">Boolean</span></span>|<span data-ttu-id="8e554-235">将此设置为 true 将创建每个应用程序 VPN 有效负载，以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="8e554-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="8e554-236">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="8e554-237">safariDomains</span></span>|<span data-ttu-id="8e554-238">String 集合</span><span class="sxs-lookup"><span data-stu-id="8e554-238">String collection</span></span>|<span data-ttu-id="8e554-239">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="8e554-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="8e554-240">除了与此 VPN 关联的应用程序之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="8e554-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="8e554-241">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="8e554-242">onDemandRules</span></span>|<span data-ttu-id="8e554-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="8e554-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="8e554-244">按需规则。</span><span class="sxs-lookup"><span data-stu-id="8e554-244">On-Demand Rules.</span></span> <span data-ttu-id="8e554-245">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="8e554-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="8e554-246">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-247">proxyServer</span><span class="sxs-lookup"><span data-stu-id="8e554-247">proxyServer</span></span>|[<span data-ttu-id="8e554-248">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="8e554-248">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="8e554-249">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="8e554-249">Proxy Server.</span></span> <span data-ttu-id="8e554-250">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-251">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="8e554-251">optInToDeviceIdSharing</span></span>|<span data-ttu-id="8e554-252">布尔</span><span class="sxs-lookup"><span data-stu-id="8e554-252">Boolean</span></span>|<span data-ttu-id="8e554-253">选择将设备的 Id 共享到第三方 vpn 客户端，以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="8e554-253">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="8e554-254">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-254">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-255">providerType</span><span class="sxs-lookup"><span data-stu-id="8e554-255">providerType</span></span>|[<span data-ttu-id="8e554-256">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="8e554-256">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="8e554-257">每应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="8e554-257">Provider type for per-app VPN.</span></span> <span data-ttu-id="8e554-258">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="8e554-258">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="8e554-259">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="8e554-259">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="8e554-260">userDomain</span><span class="sxs-lookup"><span data-stu-id="8e554-260">userDomain</span></span>|<span data-ttu-id="8e554-261">String</span><span class="sxs-lookup"><span data-stu-id="8e554-261">String</span></span>|<span data-ttu-id="8e554-262">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="8e554-262">Zscaler only.</span></span> <span data-ttu-id="8e554-263">输入一个静态域，以便在 Zscaler 应用程序中预填充 "登录" 字段。</span><span class="sxs-lookup"><span data-stu-id="8e554-263">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="8e554-264">如果保留为空，则将改用用户的 Azure Active Directory 域。</span><span class="sxs-lookup"><span data-stu-id="8e554-264">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="8e554-265">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-265">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-266">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="8e554-266">strictEnforcement</span></span>|<span data-ttu-id="8e554-267">布尔</span><span class="sxs-lookup"><span data-stu-id="8e554-267">Boolean</span></span>|<span data-ttu-id="8e554-268">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="8e554-268">Zscaler only.</span></span> <span data-ttu-id="8e554-269">阻止网络流量，直到用户登录到 Zscaler 应用程序。</span><span class="sxs-lookup"><span data-stu-id="8e554-269">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="8e554-270">"True" 表示阻止流量。</span><span class="sxs-lookup"><span data-stu-id="8e554-270">"True" means traffic is blocked.</span></span> <span data-ttu-id="8e554-271">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-271">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-272">cloudName</span><span class="sxs-lookup"><span data-stu-id="8e554-272">cloudName</span></span>|<span data-ttu-id="8e554-273">String</span><span class="sxs-lookup"><span data-stu-id="8e554-273">String</span></span>|<span data-ttu-id="8e554-274">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="8e554-274">Zscaler only.</span></span> <span data-ttu-id="8e554-275">用户分配到的 Zscaler 云。</span><span class="sxs-lookup"><span data-stu-id="8e554-275">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="8e554-276">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-276">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-277">excludeList</span><span class="sxs-lookup"><span data-stu-id="8e554-277">excludeList</span></span>|<span data-ttu-id="8e554-278">String 集合</span><span class="sxs-lookup"><span data-stu-id="8e554-278">String collection</span></span>|<span data-ttu-id="8e554-279">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="8e554-279">Zscaler only.</span></span> <span data-ttu-id="8e554-280">不通过 Zscaler 云发送的网络地址的列表。</span><span class="sxs-lookup"><span data-stu-id="8e554-280">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="8e554-281">继承自[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e554-281">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="8e554-282">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="8e554-282">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="8e554-283">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="8e554-283">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="8e554-284">子安全关联参数</span><span class="sxs-lookup"><span data-stu-id="8e554-284">Child Security Association Parameters</span></span>|
|<span data-ttu-id="8e554-285">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="8e554-285">clientAuthenticationType</span></span>|[<span data-ttu-id="8e554-286">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="8e554-286">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="8e554-287">VPN 客户端将使用的客户端身份验证的类型。</span><span class="sxs-lookup"><span data-stu-id="8e554-287">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="8e554-288">可取值为：`userAuthentication`、`deviceAuthentication`。</span><span class="sxs-lookup"><span data-stu-id="8e554-288">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="8e554-289">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="8e554-289">deadPeerDetectionRate</span></span>|[<span data-ttu-id="8e554-290">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="8e554-290">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="8e554-291">确定检查等连接是否仍处于活动状态的频率。</span><span class="sxs-lookup"><span data-stu-id="8e554-291">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="8e554-292">.</span><span class="sxs-lookup"><span data-stu-id="8e554-292">.</span></span> <span data-ttu-id="8e554-293">可取值为：`medium`、`none`、`low`、`high`。</span><span class="sxs-lookup"><span data-stu-id="8e554-293">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="8e554-294">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="8e554-294">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="8e554-295">布尔</span><span class="sxs-lookup"><span data-stu-id="8e554-295">Boolean</span></span>|<span data-ttu-id="8e554-296">禁用 MOBIKE</span><span class="sxs-lookup"><span data-stu-id="8e554-296">Disable MOBIKE</span></span>|
|<span data-ttu-id="8e554-297">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="8e554-297">disableRedirect</span></span>|<span data-ttu-id="8e554-298">布尔</span><span class="sxs-lookup"><span data-stu-id="8e554-298">Boolean</span></span>|<span data-ttu-id="8e554-299">禁用重定向</span><span class="sxs-lookup"><span data-stu-id="8e554-299">Disable Redirect</span></span>|
|<span data-ttu-id="8e554-300">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="8e554-300">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="8e554-301">布尔</span><span class="sxs-lookup"><span data-stu-id="8e554-301">Boolean</span></span>|<span data-ttu-id="8e554-302">启用尽力吊销检查;服务器响应超时不会导致它失败</span><span class="sxs-lookup"><span data-stu-id="8e554-302">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="8e554-303">enableEAP</span><span class="sxs-lookup"><span data-stu-id="8e554-303">enableEAP</span></span>|<span data-ttu-id="8e554-304">布尔</span><span class="sxs-lookup"><span data-stu-id="8e554-304">Boolean</span></span>|<span data-ttu-id="8e554-305">启用仅 EAP 身份验证</span><span class="sxs-lookup"><span data-stu-id="8e554-305">Enables EAP only authentication</span></span>|
|<span data-ttu-id="8e554-306">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="8e554-306">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="8e554-307">布尔</span><span class="sxs-lookup"><span data-stu-id="8e554-307">Boolean</span></span>|<span data-ttu-id="8e554-308">启用完全向前保密（PFS）。</span><span class="sxs-lookup"><span data-stu-id="8e554-308">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="8e554-309">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="8e554-309">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="8e554-310">布尔</span><span class="sxs-lookup"><span data-stu-id="8e554-310">Boolean</span></span>|<span data-ttu-id="8e554-311">启用 "使用内部子网属性"。</span><span class="sxs-lookup"><span data-stu-id="8e554-311">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="8e554-312">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="8e554-312">localIdentifier</span></span>|[<span data-ttu-id="8e554-313">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="8e554-313">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="8e554-314">标识尝试通过 VPN 连接的客户端的方法。</span><span class="sxs-lookup"><span data-stu-id="8e554-314">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="8e554-315">.</span><span class="sxs-lookup"><span data-stu-id="8e554-315">.</span></span> <span data-ttu-id="8e554-316">可取值为：`deviceFQDN`、`empty`、`clientCertificateSubjectName`。</span><span class="sxs-lookup"><span data-stu-id="8e554-316">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="8e554-317">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="8e554-317">remoteIdentifier</span></span>|<span data-ttu-id="8e554-318">String</span><span class="sxs-lookup"><span data-stu-id="8e554-318">String</span></span>|<span data-ttu-id="8e554-319">IKEv2 服务器的地址。</span><span class="sxs-lookup"><span data-stu-id="8e554-319">Address of the IKEv2 server.</span></span> <span data-ttu-id="8e554-320">必须是 FQDN、UserFQDN、网络地址或 ASN1DN</span><span class="sxs-lookup"><span data-stu-id="8e554-320">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="8e554-321">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="8e554-321">securityAssociationParameters</span></span>|[<span data-ttu-id="8e554-322">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="8e554-322">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="8e554-323">安全关联参数</span><span class="sxs-lookup"><span data-stu-id="8e554-323">Security Association Parameters</span></span>|
|<span data-ttu-id="8e554-324">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="8e554-324">serverCertificateCommonName</span></span>|<span data-ttu-id="8e554-325">String</span><span class="sxs-lookup"><span data-stu-id="8e554-325">String</span></span>|<span data-ttu-id="8e554-326">服务器身份验证中使用的 IKEv2 服务器证书的公用名</span><span class="sxs-lookup"><span data-stu-id="8e554-326">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="8e554-327">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="8e554-327">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="8e554-328">String</span><span class="sxs-lookup"><span data-stu-id="8e554-328">String</span></span>|<span data-ttu-id="8e554-329">身份验证中使用的 IKEv2 服务器证书颁发者的颁发者公用名称</span><span class="sxs-lookup"><span data-stu-id="8e554-329">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="8e554-330">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="8e554-330">serverCertificateType</span></span>|[<span data-ttu-id="8e554-331">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="8e554-331">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="8e554-332">VPN 服务器将提供给 VPN 客户端进行身份验证的证书类型。</span><span class="sxs-lookup"><span data-stu-id="8e554-332">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="8e554-333">可取值为：`rsa`、`ecdsa256`、`ecdsa384`、`ecdsa521`。</span><span class="sxs-lookup"><span data-stu-id="8e554-333">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="8e554-334">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="8e554-334">sharedSecret</span></span>|<span data-ttu-id="8e554-335">String</span><span class="sxs-lookup"><span data-stu-id="8e554-335">String</span></span>|<span data-ttu-id="8e554-336">在选择共享密钥身份验证时使用</span><span class="sxs-lookup"><span data-stu-id="8e554-336">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="8e554-337">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8e554-337">tlsMaximumVersion</span></span>|<span data-ttu-id="8e554-338">String</span><span class="sxs-lookup"><span data-stu-id="8e554-338">String</span></span>|<span data-ttu-id="8e554-339">要与 EAP-TLS 身份验证一起使用的最大 TLS 版本</span><span class="sxs-lookup"><span data-stu-id="8e554-339">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="8e554-340">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8e554-340">tlsMinimumVersion</span></span>|<span data-ttu-id="8e554-341">String</span><span class="sxs-lookup"><span data-stu-id="8e554-341">String</span></span>|<span data-ttu-id="8e554-342">与 EAP-TLS 身份验证一起使用的最小 TLS 版本</span><span class="sxs-lookup"><span data-stu-id="8e554-342">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="8e554-343">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="8e554-343">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="8e554-344">布尔</span><span class="sxs-lookup"><span data-stu-id="8e554-344">Boolean</span></span>|<span data-ttu-id="8e554-345">允许使用安全关联参数，具体方法是将所有参数设置为设备的默认值，除非明确指定。</span><span class="sxs-lookup"><span data-stu-id="8e554-345">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="8e554-346">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="8e554-346">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="8e554-347">布尔</span><span class="sxs-lookup"><span data-stu-id="8e554-347">Boolean</span></span>|<span data-ttu-id="8e554-348">允许使用子安全关联参数，具体方法是将所有参数设置为设备的默认值，除非明确指定。</span><span class="sxs-lookup"><span data-stu-id="8e554-348">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="8e554-349">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="8e554-349">alwaysOnConfiguration</span></span>|[<span data-ttu-id="8e554-350">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="8e554-350">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="8e554-351">AlwaysOn 配置</span><span class="sxs-lookup"><span data-stu-id="8e554-351">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="8e554-352">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="8e554-352">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="8e554-353">布尔</span><span class="sxs-lookup"><span data-stu-id="8e554-353">Boolean</span></span>|<span data-ttu-id="8e554-354">确定是否始终启用 VPN</span><span class="sxs-lookup"><span data-stu-id="8e554-354">Determines if Always on VPN is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="8e554-355">响应</span><span class="sxs-lookup"><span data-stu-id="8e554-355">Response</span></span>
<span data-ttu-id="8e554-356">如果成功，此方法在响应`201 Created`正文中返回响应代码和[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8e554-356">If successful, this method returns a `201 Created` response code and a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e554-357">示例</span><span class="sxs-lookup"><span data-stu-id="8e554-357">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e554-358">请求</span><span class="sxs-lookup"><span data-stu-id="8e554-358">Request</span></span>
<span data-ttu-id="8e554-359">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8e554-359">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4984

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

### <a name="response"></a><span data-ttu-id="8e554-360">响应</span><span class="sxs-lookup"><span data-stu-id="8e554-360">Response</span></span>
<span data-ttu-id="8e554-p139">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8e554-p139">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 5156

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





