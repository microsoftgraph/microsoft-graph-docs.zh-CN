---
title: 创建 iosVpnConfiguration
description: 创建新的 iosVpnConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 82da02b7e9e49f09cbb0d4a5a023f23275937c92
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792819"
---
# <a name="create-iosvpnconfiguration"></a><span data-ttu-id="59072-103">创建 iosVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="59072-103">Create iosVpnConfiguration</span></span>

<span data-ttu-id="59072-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59072-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59072-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="59072-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59072-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="59072-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59072-107">创建新的 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="59072-107">Create a new [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59072-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="59072-108">Prerequisites</span></span>
<span data-ttu-id="59072-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59072-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59072-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="59072-111">Permission type</span></span>|<span data-ttu-id="59072-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="59072-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59072-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59072-113">Delegated (work or school account)</span></span>|<span data-ttu-id="59072-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59072-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="59072-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59072-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59072-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="59072-116">Not supported.</span></span>|
|<span data-ttu-id="59072-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="59072-117">Application</span></span>|<span data-ttu-id="59072-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59072-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59072-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59072-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="59072-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="59072-120">Request headers</span></span>
|<span data-ttu-id="59072-121">标头</span><span class="sxs-lookup"><span data-stu-id="59072-121">Header</span></span>|<span data-ttu-id="59072-122">值</span><span class="sxs-lookup"><span data-stu-id="59072-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59072-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="59072-123">Authorization</span></span>|<span data-ttu-id="59072-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="59072-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59072-125">接受</span><span class="sxs-lookup"><span data-stu-id="59072-125">Accept</span></span>|<span data-ttu-id="59072-126">application/json</span><span class="sxs-lookup"><span data-stu-id="59072-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59072-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="59072-127">Request body</span></span>
<span data-ttu-id="59072-128">在请求正文中，提供 iosVpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59072-128">In the request body, supply a JSON representation for the iosVpnConfiguration object.</span></span>

<span data-ttu-id="59072-129">下表显示创建 iosVpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="59072-129">The following table shows the properties that are required when you create the iosVpnConfiguration.</span></span>

|<span data-ttu-id="59072-130">属性</span><span class="sxs-lookup"><span data-stu-id="59072-130">Property</span></span>|<span data-ttu-id="59072-131">类型</span><span class="sxs-lookup"><span data-stu-id="59072-131">Type</span></span>|<span data-ttu-id="59072-132">说明</span><span class="sxs-lookup"><span data-stu-id="59072-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59072-133">id</span><span class="sxs-lookup"><span data-stu-id="59072-133">id</span></span>|<span data-ttu-id="59072-134">String</span><span class="sxs-lookup"><span data-stu-id="59072-134">String</span></span>|<span data-ttu-id="59072-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="59072-135">Key of the entity.</span></span> <span data-ttu-id="59072-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59072-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59072-137">lastModifiedDateTime</span></span>|<span data-ttu-id="59072-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59072-138">DateTimeOffset</span></span>|<span data-ttu-id="59072-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="59072-139">DateTime the object was last modified.</span></span> <span data-ttu-id="59072-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59072-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="59072-141">roleScopeTagIds</span></span>|<span data-ttu-id="59072-142">字符串集合</span><span class="sxs-lookup"><span data-stu-id="59072-142">String collection</span></span>|<span data-ttu-id="59072-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="59072-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="59072-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59072-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="59072-145">supportsScopeTags</span></span>|<span data-ttu-id="59072-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="59072-146">Boolean</span></span>|<span data-ttu-id="59072-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="59072-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="59072-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="59072-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="59072-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="59072-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="59072-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="59072-150">This property is read-only.</span></span> <span data-ttu-id="59072-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59072-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="59072-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="59072-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="59072-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="59072-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="59072-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="59072-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59072-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="59072-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="59072-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="59072-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="59072-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="59072-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="59072-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59072-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="59072-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="59072-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="59072-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="59072-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="59072-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="59072-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59072-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="59072-164">createdDateTime</span></span>|<span data-ttu-id="59072-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59072-165">DateTimeOffset</span></span>|<span data-ttu-id="59072-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="59072-166">DateTime the object was created.</span></span> <span data-ttu-id="59072-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59072-168">description</span><span class="sxs-lookup"><span data-stu-id="59072-168">description</span></span>|<span data-ttu-id="59072-169">String</span><span class="sxs-lookup"><span data-stu-id="59072-169">String</span></span>|<span data-ttu-id="59072-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="59072-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="59072-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59072-172">displayName</span><span class="sxs-lookup"><span data-stu-id="59072-172">displayName</span></span>|<span data-ttu-id="59072-173">String</span><span class="sxs-lookup"><span data-stu-id="59072-173">String</span></span>|<span data-ttu-id="59072-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="59072-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="59072-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59072-176">version</span><span class="sxs-lookup"><span data-stu-id="59072-176">version</span></span>|<span data-ttu-id="59072-177">Int32</span><span class="sxs-lookup"><span data-stu-id="59072-177">Int32</span></span>|<span data-ttu-id="59072-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="59072-178">Version of the device configuration.</span></span> <span data-ttu-id="59072-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59072-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="59072-180">connectionName</span></span>|<span data-ttu-id="59072-181">String</span><span class="sxs-lookup"><span data-stu-id="59072-181">String</span></span>|<span data-ttu-id="59072-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="59072-182">Connection name displayed to the user.</span></span> <span data-ttu-id="59072-183">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="59072-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="59072-184">connectionType</span></span>|[<span data-ttu-id="59072-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="59072-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="59072-186">连接类型。</span><span class="sxs-lookup"><span data-stu-id="59072-186">Connection type.</span></span> <span data-ttu-id="59072-187">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="59072-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="59072-188">可能的值为：、、、、、、、、、、、、、、、、、、 `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` 。</span><span class="sxs-lookup"><span data-stu-id="59072-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="59072-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="59072-189">loginGroupOrDomain</span></span>|<span data-ttu-id="59072-190">String</span><span class="sxs-lookup"><span data-stu-id="59072-190">String</span></span>|<span data-ttu-id="59072-191">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="59072-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="59072-192">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="59072-193">role</span><span class="sxs-lookup"><span data-stu-id="59072-193">role</span></span>|<span data-ttu-id="59072-194">String</span><span class="sxs-lookup"><span data-stu-id="59072-194">String</span></span>|<span data-ttu-id="59072-195">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="59072-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="59072-196">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="59072-197">型</span><span class="sxs-lookup"><span data-stu-id="59072-197">realm</span></span>|<span data-ttu-id="59072-198">String</span><span class="sxs-lookup"><span data-stu-id="59072-198">String</span></span>|<span data-ttu-id="59072-199">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="59072-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="59072-200">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="59072-201">服务器主板</span><span class="sxs-lookup"><span data-stu-id="59072-201">server</span></span>|[<span data-ttu-id="59072-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="59072-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="59072-203">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="59072-203">VPN Server on the network.</span></span> <span data-ttu-id="59072-204">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="59072-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="59072-205">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="59072-206">标识符</span><span class="sxs-lookup"><span data-stu-id="59072-206">identifier</span></span>|<span data-ttu-id="59072-207">String</span><span class="sxs-lookup"><span data-stu-id="59072-207">String</span></span>|<span data-ttu-id="59072-208">当连接类型设置为自定义 VPN 时，由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="59072-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="59072-209">例如： Cisco AnyConnect 使用从[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)继承的 AnyConnect applevpn 的标识符。</span><span class="sxs-lookup"><span data-stu-id="59072-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="59072-210">customData</span><span class="sxs-lookup"><span data-stu-id="59072-210">customData</span></span>|<span data-ttu-id="59072-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="59072-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="59072-212">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="59072-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="59072-213">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="59072-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="59072-214">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="59072-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="59072-215">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="59072-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="59072-216">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="59072-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="59072-217">customKeyValueData</span></span>|<span data-ttu-id="59072-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="59072-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="59072-219">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="59072-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="59072-220">使用此字段启用 Intune 不支持的功能，但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="59072-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="59072-221">请与你的 VPN 供应商联系，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="59072-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="59072-222">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="59072-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="59072-223">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="59072-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="59072-224">enableSplitTunneling</span></span>|<span data-ttu-id="59072-225">布尔值</span><span class="sxs-lookup"><span data-stu-id="59072-225">Boolean</span></span>|<span data-ttu-id="59072-226">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="59072-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="59072-227">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="59072-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="59072-228">authenticationMethod</span></span>|[<span data-ttu-id="59072-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="59072-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="59072-230">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="59072-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="59072-231">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="59072-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="59072-232">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="59072-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="59072-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="59072-233">enablePerApp</span></span>|<span data-ttu-id="59072-234">布尔值</span><span class="sxs-lookup"><span data-stu-id="59072-234">Boolean</span></span>|<span data-ttu-id="59072-235">将此设置为 true 将创建每个应用程序 VPN 有效负载，以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="59072-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="59072-236">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="59072-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="59072-237">safariDomains</span></span>|<span data-ttu-id="59072-238">字符串集合</span><span class="sxs-lookup"><span data-stu-id="59072-238">String collection</span></span>|<span data-ttu-id="59072-239">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="59072-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="59072-240">除了与此 VPN 关联的应用程序之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="59072-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="59072-241">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="59072-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="59072-242">onDemandRules</span></span>|<span data-ttu-id="59072-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="59072-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="59072-244">按需规则。</span><span class="sxs-lookup"><span data-stu-id="59072-244">On-Demand Rules.</span></span> <span data-ttu-id="59072-245">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="59072-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="59072-246">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="59072-247">providerType</span><span class="sxs-lookup"><span data-stu-id="59072-247">providerType</span></span>|[<span data-ttu-id="59072-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="59072-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="59072-249">每应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="59072-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="59072-250">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="59072-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="59072-251">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="59072-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="59072-252">proxyServer</span><span class="sxs-lookup"><span data-stu-id="59072-252">proxyServer</span></span>|[<span data-ttu-id="59072-253">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="59072-253">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="59072-254">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="59072-254">Proxy Server.</span></span> <span data-ttu-id="59072-255">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-255">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="59072-256">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="59072-256">optInToDeviceIdSharing</span></span>|<span data-ttu-id="59072-257">布尔值</span><span class="sxs-lookup"><span data-stu-id="59072-257">Boolean</span></span>|<span data-ttu-id="59072-258">选择将设备的 Id 共享到第三方 vpn 客户端，以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="59072-258">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="59072-259">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59072-259">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="59072-260">userDomain</span><span class="sxs-lookup"><span data-stu-id="59072-260">userDomain</span></span>|<span data-ttu-id="59072-261">String</span><span class="sxs-lookup"><span data-stu-id="59072-261">String</span></span>|<span data-ttu-id="59072-262">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="59072-262">Zscaler only.</span></span> <span data-ttu-id="59072-263">输入一个静态域，以便在 Zscaler 应用程序中预填充 "登录" 字段。</span><span class="sxs-lookup"><span data-stu-id="59072-263">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="59072-264">如果保留为空，则将改用用户的 Azure Active Directory 域。</span><span class="sxs-lookup"><span data-stu-id="59072-264">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="59072-265">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="59072-265">strictEnforcement</span></span>|<span data-ttu-id="59072-266">布尔值</span><span class="sxs-lookup"><span data-stu-id="59072-266">Boolean</span></span>|<span data-ttu-id="59072-267">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="59072-267">Zscaler only.</span></span> <span data-ttu-id="59072-268">阻止网络流量，直到用户登录到 Zscaler 应用程序。</span><span class="sxs-lookup"><span data-stu-id="59072-268">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="59072-269">"True" 表示阻止流量。</span><span class="sxs-lookup"><span data-stu-id="59072-269">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="59072-270">cloudName</span><span class="sxs-lookup"><span data-stu-id="59072-270">cloudName</span></span>|<span data-ttu-id="59072-271">String</span><span class="sxs-lookup"><span data-stu-id="59072-271">String</span></span>|<span data-ttu-id="59072-272">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="59072-272">Zscaler only.</span></span> <span data-ttu-id="59072-273">用户分配到的 Zscaler 云。</span><span class="sxs-lookup"><span data-stu-id="59072-273">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="59072-274">excludeList</span><span class="sxs-lookup"><span data-stu-id="59072-274">excludeList</span></span>|<span data-ttu-id="59072-275">字符串集合</span><span class="sxs-lookup"><span data-stu-id="59072-275">String collection</span></span>|<span data-ttu-id="59072-276">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="59072-276">Zscaler only.</span></span> <span data-ttu-id="59072-277">不通过 Zscaler 云发送的网络地址的列表。</span><span class="sxs-lookup"><span data-stu-id="59072-277">List of network addresses which are not sent through the Zscaler cloud.</span></span>|
|<span data-ttu-id="59072-278">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="59072-278">targetedMobileApps</span></span>|<span data-ttu-id="59072-279">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="59072-279">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="59072-280">目标移动应用。</span><span class="sxs-lookup"><span data-stu-id="59072-280">Targeted mobile apps.</span></span> <span data-ttu-id="59072-281">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="59072-281">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="59072-282">响应</span><span class="sxs-lookup"><span data-stu-id="59072-282">Response</span></span>
<span data-ttu-id="59072-283">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="59072-283">If successful, this method returns a `201 Created` response code and a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59072-284">示例</span><span class="sxs-lookup"><span data-stu-id="59072-284">Example</span></span>

### <a name="request"></a><span data-ttu-id="59072-285">请求</span><span class="sxs-lookup"><span data-stu-id="59072-285">Request</span></span>
<span data-ttu-id="59072-286">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="59072-286">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="59072-287">响应</span><span class="sxs-lookup"><span data-stu-id="59072-287">Response</span></span>
<span data-ttu-id="59072-p135">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="59072-p135">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



