---
title: 创建 macOSVpnConfiguration
description: 创建新的 macOSVpnConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6e5d8839a5d1ef6a7a4c4cdd1f5dceac06341bc1
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792672"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="64777-103">创建 macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="64777-103">Create macOSVpnConfiguration</span></span>

<span data-ttu-id="64777-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64777-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64777-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="64777-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64777-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="64777-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64777-107">创建新的 [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="64777-107">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64777-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="64777-108">Prerequisites</span></span>
<span data-ttu-id="64777-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64777-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64777-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="64777-111">Permission type</span></span>|<span data-ttu-id="64777-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="64777-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64777-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64777-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64777-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64777-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64777-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64777-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64777-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="64777-116">Not supported.</span></span>|
|<span data-ttu-id="64777-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="64777-117">Application</span></span>|<span data-ttu-id="64777-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64777-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64777-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64777-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="64777-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="64777-120">Request headers</span></span>
|<span data-ttu-id="64777-121">标头</span><span class="sxs-lookup"><span data-stu-id="64777-121">Header</span></span>|<span data-ttu-id="64777-122">值</span><span class="sxs-lookup"><span data-stu-id="64777-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64777-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="64777-123">Authorization</span></span>|<span data-ttu-id="64777-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="64777-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64777-125">接受</span><span class="sxs-lookup"><span data-stu-id="64777-125">Accept</span></span>|<span data-ttu-id="64777-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64777-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64777-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="64777-127">Request body</span></span>
<span data-ttu-id="64777-128">在请求正文中，提供 macOSVpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64777-128">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="64777-129">下表显示创建 macOSVpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="64777-129">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="64777-130">属性</span><span class="sxs-lookup"><span data-stu-id="64777-130">Property</span></span>|<span data-ttu-id="64777-131">类型</span><span class="sxs-lookup"><span data-stu-id="64777-131">Type</span></span>|<span data-ttu-id="64777-132">说明</span><span class="sxs-lookup"><span data-stu-id="64777-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64777-133">id</span><span class="sxs-lookup"><span data-stu-id="64777-133">id</span></span>|<span data-ttu-id="64777-134">String</span><span class="sxs-lookup"><span data-stu-id="64777-134">String</span></span>|<span data-ttu-id="64777-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="64777-135">Key of the entity.</span></span> <span data-ttu-id="64777-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64777-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64777-137">lastModifiedDateTime</span></span>|<span data-ttu-id="64777-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64777-138">DateTimeOffset</span></span>|<span data-ttu-id="64777-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="64777-139">DateTime the object was last modified.</span></span> <span data-ttu-id="64777-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64777-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="64777-141">roleScopeTagIds</span></span>|<span data-ttu-id="64777-142">字符串集合</span><span class="sxs-lookup"><span data-stu-id="64777-142">String collection</span></span>|<span data-ttu-id="64777-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="64777-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="64777-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64777-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="64777-145">supportsScopeTags</span></span>|<span data-ttu-id="64777-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="64777-146">Boolean</span></span>|<span data-ttu-id="64777-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="64777-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="64777-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="64777-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="64777-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="64777-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="64777-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="64777-150">This property is read-only.</span></span> <span data-ttu-id="64777-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64777-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="64777-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="64777-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="64777-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="64777-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="64777-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="64777-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64777-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="64777-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="64777-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="64777-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="64777-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="64777-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="64777-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64777-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="64777-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="64777-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="64777-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="64777-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="64777-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="64777-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64777-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64777-164">createdDateTime</span></span>|<span data-ttu-id="64777-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64777-165">DateTimeOffset</span></span>|<span data-ttu-id="64777-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="64777-166">DateTime the object was created.</span></span> <span data-ttu-id="64777-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64777-168">description</span><span class="sxs-lookup"><span data-stu-id="64777-168">description</span></span>|<span data-ttu-id="64777-169">String</span><span class="sxs-lookup"><span data-stu-id="64777-169">String</span></span>|<span data-ttu-id="64777-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="64777-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="64777-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64777-172">displayName</span><span class="sxs-lookup"><span data-stu-id="64777-172">displayName</span></span>|<span data-ttu-id="64777-173">String</span><span class="sxs-lookup"><span data-stu-id="64777-173">String</span></span>|<span data-ttu-id="64777-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="64777-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="64777-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64777-176">version</span><span class="sxs-lookup"><span data-stu-id="64777-176">version</span></span>|<span data-ttu-id="64777-177">Int32</span><span class="sxs-lookup"><span data-stu-id="64777-177">Int32</span></span>|<span data-ttu-id="64777-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="64777-178">Version of the device configuration.</span></span> <span data-ttu-id="64777-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64777-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="64777-180">connectionName</span></span>|<span data-ttu-id="64777-181">String</span><span class="sxs-lookup"><span data-stu-id="64777-181">String</span></span>|<span data-ttu-id="64777-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="64777-182">Connection name displayed to the user.</span></span> <span data-ttu-id="64777-183">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64777-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="64777-184">connectionType</span></span>|[<span data-ttu-id="64777-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="64777-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="64777-186">连接类型。</span><span class="sxs-lookup"><span data-stu-id="64777-186">Connection type.</span></span> <span data-ttu-id="64777-187">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="64777-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="64777-188">可能的值为：、、、、、、、、、、、、、、、、、、 `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` 。</span><span class="sxs-lookup"><span data-stu-id="64777-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="64777-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="64777-189">loginGroupOrDomain</span></span>|<span data-ttu-id="64777-190">String</span><span class="sxs-lookup"><span data-stu-id="64777-190">String</span></span>|<span data-ttu-id="64777-191">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="64777-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="64777-192">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64777-193">role</span><span class="sxs-lookup"><span data-stu-id="64777-193">role</span></span>|<span data-ttu-id="64777-194">String</span><span class="sxs-lookup"><span data-stu-id="64777-194">String</span></span>|<span data-ttu-id="64777-195">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="64777-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="64777-196">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64777-197">型</span><span class="sxs-lookup"><span data-stu-id="64777-197">realm</span></span>|<span data-ttu-id="64777-198">String</span><span class="sxs-lookup"><span data-stu-id="64777-198">String</span></span>|<span data-ttu-id="64777-199">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="64777-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="64777-200">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64777-201">服务器主板</span><span class="sxs-lookup"><span data-stu-id="64777-201">server</span></span>|[<span data-ttu-id="64777-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="64777-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="64777-203">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="64777-203">VPN Server on the network.</span></span> <span data-ttu-id="64777-204">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="64777-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="64777-205">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64777-206">标识符</span><span class="sxs-lookup"><span data-stu-id="64777-206">identifier</span></span>|<span data-ttu-id="64777-207">String</span><span class="sxs-lookup"><span data-stu-id="64777-207">String</span></span>|<span data-ttu-id="64777-208">当连接类型设置为自定义 VPN 时，由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="64777-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="64777-209">例如： Cisco AnyConnect 使用从[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)继承的 AnyConnect applevpn 的标识符。</span><span class="sxs-lookup"><span data-stu-id="64777-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64777-210">customData</span><span class="sxs-lookup"><span data-stu-id="64777-210">customData</span></span>|<span data-ttu-id="64777-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="64777-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="64777-212">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="64777-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="64777-213">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="64777-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="64777-214">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="64777-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="64777-215">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="64777-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="64777-216">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64777-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="64777-217">customKeyValueData</span></span>|<span data-ttu-id="64777-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="64777-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="64777-219">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="64777-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="64777-220">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="64777-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="64777-221">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="64777-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="64777-222">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="64777-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="64777-223">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64777-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="64777-224">enableSplitTunneling</span></span>|<span data-ttu-id="64777-225">布尔值</span><span class="sxs-lookup"><span data-stu-id="64777-225">Boolean</span></span>|<span data-ttu-id="64777-226">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="64777-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="64777-227">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64777-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="64777-228">authenticationMethod</span></span>|[<span data-ttu-id="64777-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="64777-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="64777-230">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="64777-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="64777-231">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="64777-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="64777-232">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="64777-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="64777-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="64777-233">enablePerApp</span></span>|<span data-ttu-id="64777-234">布尔值</span><span class="sxs-lookup"><span data-stu-id="64777-234">Boolean</span></span>|<span data-ttu-id="64777-235">将此设置为 true 将创建每个应用程序 VPN 有效负载，以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="64777-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="64777-236">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64777-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="64777-237">safariDomains</span></span>|<span data-ttu-id="64777-238">字符串集合</span><span class="sxs-lookup"><span data-stu-id="64777-238">String collection</span></span>|<span data-ttu-id="64777-239">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="64777-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="64777-240">除了与此 VPN 关联的应用程序之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="64777-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="64777-241">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64777-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="64777-242">onDemandRules</span></span>|<span data-ttu-id="64777-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="64777-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="64777-244">按需规则。</span><span class="sxs-lookup"><span data-stu-id="64777-244">On-Demand Rules.</span></span> <span data-ttu-id="64777-245">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="64777-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="64777-246">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64777-247">providerType</span><span class="sxs-lookup"><span data-stu-id="64777-247">providerType</span></span>|[<span data-ttu-id="64777-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="64777-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="64777-249">每应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="64777-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="64777-250">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="64777-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="64777-251">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="64777-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="64777-252">proxyServer</span><span class="sxs-lookup"><span data-stu-id="64777-252">proxyServer</span></span>|[<span data-ttu-id="64777-253">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="64777-253">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="64777-254">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="64777-254">Proxy Server.</span></span> <span data-ttu-id="64777-255">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-255">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="64777-256">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="64777-256">optInToDeviceIdSharing</span></span>|<span data-ttu-id="64777-257">布尔值</span><span class="sxs-lookup"><span data-stu-id="64777-257">Boolean</span></span>|<span data-ttu-id="64777-258">选择将设备的 Id 共享到第三方 vpn 客户端，以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="64777-258">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="64777-259">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64777-259">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="64777-260">响应</span><span class="sxs-lookup"><span data-stu-id="64777-260">Response</span></span>
<span data-ttu-id="64777-261">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="64777-261">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64777-262">示例</span><span class="sxs-lookup"><span data-stu-id="64777-262">Example</span></span>

### <a name="request"></a><span data-ttu-id="64777-263">请求</span><span class="sxs-lookup"><span data-stu-id="64777-263">Request</span></span>
<span data-ttu-id="64777-264">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="64777-264">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2661

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
  "providerType": "appProxy",
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true
}
```

### <a name="response"></a><span data-ttu-id="64777-265">响应</span><span class="sxs-lookup"><span data-stu-id="64777-265">Response</span></span>
<span data-ttu-id="64777-p130">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="64777-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2833

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
  "providerType": "appProxy",
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true
}
```



