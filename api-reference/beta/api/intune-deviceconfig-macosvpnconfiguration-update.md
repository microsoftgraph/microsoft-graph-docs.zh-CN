---
title: 更新 macOSVpnConfiguration
description: 更新 macOSVpnConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8828cb86ffe3b5f366ce2300a879e06211ee04d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31786026"
---
# <a name="update-macosvpnconfiguration"></a><span data-ttu-id="47cd5-103">更新 macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="47cd5-103">Update macOSVpnConfiguration</span></span>

> <span data-ttu-id="47cd5-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="47cd5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47cd5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="47cd5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47cd5-106">更新[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="47cd5-106">Update the properties of a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47cd5-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="47cd5-107">Prerequisites</span></span>
<span data-ttu-id="47cd5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="47cd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47cd5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="47cd5-110">Permission type</span></span>|<span data-ttu-id="47cd5-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="47cd5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47cd5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47cd5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47cd5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47cd5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47cd5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47cd5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47cd5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="47cd5-115">Not supported.</span></span>|
|<span data-ttu-id="47cd5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="47cd5-116">Application</span></span>|<span data-ttu-id="47cd5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="47cd5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47cd5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47cd5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="47cd5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="47cd5-119">Request headers</span></span>
|<span data-ttu-id="47cd5-120">标头</span><span class="sxs-lookup"><span data-stu-id="47cd5-120">Header</span></span>|<span data-ttu-id="47cd5-121">值</span><span class="sxs-lookup"><span data-stu-id="47cd5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47cd5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="47cd5-122">Authorization</span></span>|<span data-ttu-id="47cd5-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="47cd5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47cd5-124">接受</span><span class="sxs-lookup"><span data-stu-id="47cd5-124">Accept</span></span>|<span data-ttu-id="47cd5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="47cd5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47cd5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="47cd5-126">Request body</span></span>
<span data-ttu-id="47cd5-127">在请求正文中, 提供[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47cd5-127">In the request body, supply a JSON representation for the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="47cd5-128">下表显示创建[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="47cd5-128">The following table shows the properties that are required when you create the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

|<span data-ttu-id="47cd5-129">属性</span><span class="sxs-lookup"><span data-stu-id="47cd5-129">Property</span></span>|<span data-ttu-id="47cd5-130">类型</span><span class="sxs-lookup"><span data-stu-id="47cd5-130">Type</span></span>|<span data-ttu-id="47cd5-131">说明</span><span class="sxs-lookup"><span data-stu-id="47cd5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47cd5-132">id</span><span class="sxs-lookup"><span data-stu-id="47cd5-132">id</span></span>|<span data-ttu-id="47cd5-133">String</span><span class="sxs-lookup"><span data-stu-id="47cd5-133">String</span></span>|<span data-ttu-id="47cd5-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="47cd5-134">Key of the entity.</span></span> <span data-ttu-id="47cd5-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47cd5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="47cd5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47cd5-137">DateTimeOffset</span></span>|<span data-ttu-id="47cd5-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="47cd5-138">DateTime the object was last modified.</span></span> <span data-ttu-id="47cd5-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="47cd5-140">roleScopeTagIds</span></span>|<span data-ttu-id="47cd5-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="47cd5-141">String collection</span></span>|<span data-ttu-id="47cd5-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="47cd5-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="47cd5-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="47cd5-144">supportsScopeTags</span></span>|<span data-ttu-id="47cd5-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="47cd5-145">Boolean</span></span>|<span data-ttu-id="47cd5-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="47cd5-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="47cd5-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="47cd5-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="47cd5-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="47cd5-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="47cd5-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="47cd5-149">This property is read-only.</span></span> <span data-ttu-id="47cd5-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47cd5-151">createdDateTime</span></span>|<span data-ttu-id="47cd5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47cd5-152">DateTimeOffset</span></span>|<span data-ttu-id="47cd5-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="47cd5-153">DateTime the object was created.</span></span> <span data-ttu-id="47cd5-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-155">description</span><span class="sxs-lookup"><span data-stu-id="47cd5-155">description</span></span>|<span data-ttu-id="47cd5-156">String</span><span class="sxs-lookup"><span data-stu-id="47cd5-156">String</span></span>|<span data-ttu-id="47cd5-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="47cd5-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="47cd5-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-159">displayName</span><span class="sxs-lookup"><span data-stu-id="47cd5-159">displayName</span></span>|<span data-ttu-id="47cd5-160">String</span><span class="sxs-lookup"><span data-stu-id="47cd5-160">String</span></span>|<span data-ttu-id="47cd5-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="47cd5-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="47cd5-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-163">version</span><span class="sxs-lookup"><span data-stu-id="47cd5-163">version</span></span>|<span data-ttu-id="47cd5-164">Int32</span><span class="sxs-lookup"><span data-stu-id="47cd5-164">Int32</span></span>|<span data-ttu-id="47cd5-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="47cd5-165">Version of the device configuration.</span></span> <span data-ttu-id="47cd5-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="47cd5-167">connectionName</span></span>|<span data-ttu-id="47cd5-168">String</span><span class="sxs-lookup"><span data-stu-id="47cd5-168">String</span></span>|<span data-ttu-id="47cd5-169">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="47cd5-169">Connection name displayed to the user.</span></span> <span data-ttu-id="47cd5-170">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-170">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="47cd5-171">connectionType</span></span>|[<span data-ttu-id="47cd5-172">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="47cd5-172">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="47cd5-173">连接类型。</span><span class="sxs-lookup"><span data-stu-id="47cd5-173">Connection type.</span></span> <span data-ttu-id="47cd5-174">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="47cd5-174">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="47cd5-175">可能的值为`ciscoAnyConnect`: `pulseSecure`、 `f5EdgeClient`、 `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `paloAltoGlobalProtectV2`、、、、、、、、、、、。 `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso`</span><span class="sxs-lookup"><span data-stu-id="47cd5-175">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="47cd5-176">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="47cd5-176">loginGroupOrDomain</span></span>|<span data-ttu-id="47cd5-177">String</span><span class="sxs-lookup"><span data-stu-id="47cd5-177">String</span></span>|<span data-ttu-id="47cd5-178">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="47cd5-178">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="47cd5-179">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-179">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-180">role</span><span class="sxs-lookup"><span data-stu-id="47cd5-180">role</span></span>|<span data-ttu-id="47cd5-181">String</span><span class="sxs-lookup"><span data-stu-id="47cd5-181">String</span></span>|<span data-ttu-id="47cd5-182">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="47cd5-182">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="47cd5-183">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-184">型</span><span class="sxs-lookup"><span data-stu-id="47cd5-184">realm</span></span>|<span data-ttu-id="47cd5-185">String</span><span class="sxs-lookup"><span data-stu-id="47cd5-185">String</span></span>|<span data-ttu-id="47cd5-186">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="47cd5-186">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="47cd5-187">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-188">服务器主板</span><span class="sxs-lookup"><span data-stu-id="47cd5-188">server</span></span>|[<span data-ttu-id="47cd5-189">vpnServer</span><span class="sxs-lookup"><span data-stu-id="47cd5-189">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="47cd5-190">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="47cd5-190">VPN Server on the network.</span></span> <span data-ttu-id="47cd5-191">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="47cd5-191">Make sure end users can access this network location.</span></span> <span data-ttu-id="47cd5-192">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-193">标识符</span><span class="sxs-lookup"><span data-stu-id="47cd5-193">identifier</span></span>|<span data-ttu-id="47cd5-194">String</span><span class="sxs-lookup"><span data-stu-id="47cd5-194">String</span></span>|<span data-ttu-id="47cd5-195">当连接类型设置为自定义 vpn 时, 由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="47cd5-195">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="47cd5-196">例如: Cisco AnyConnect 使用从[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)继承的 AnyConnect applevpn 的标识符。</span><span class="sxs-lookup"><span data-stu-id="47cd5-196">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-197">customData</span><span class="sxs-lookup"><span data-stu-id="47cd5-197">customData</span></span>|<span data-ttu-id="47cd5-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="47cd5-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="47cd5-199">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="47cd5-199">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="47cd5-200">使用此字段启用 Intune 不支持的功能, 但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="47cd5-200">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="47cd5-201">请与你的 VPN 供应商联系, 了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="47cd5-201">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="47cd5-202">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="47cd5-202">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="47cd5-203">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-203">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="47cd5-204">customKeyValueData</span></span>|<span data-ttu-id="47cd5-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="47cd5-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="47cd5-206">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="47cd5-206">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="47cd5-207">使用此字段启用 Intune 不支持的功能, 但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="47cd5-207">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="47cd5-208">请与你的 VPN 供应商联系, 了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="47cd5-208">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="47cd5-209">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="47cd5-209">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="47cd5-210">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-210">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-211">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="47cd5-211">enableSplitTunneling</span></span>|<span data-ttu-id="47cd5-212">布尔值</span><span class="sxs-lookup"><span data-stu-id="47cd5-212">Boolean</span></span>|<span data-ttu-id="47cd5-213">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="47cd5-213">Send all network traffic through VPN.</span></span> <span data-ttu-id="47cd5-214">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-214">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-215">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="47cd5-215">authenticationMethod</span></span>|[<span data-ttu-id="47cd5-216">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="47cd5-216">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="47cd5-217">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="47cd5-217">Authentication method for this VPN connection.</span></span> <span data-ttu-id="47cd5-218">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="47cd5-218">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="47cd5-219">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="47cd5-219">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="47cd5-220">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="47cd5-220">enablePerApp</span></span>|<span data-ttu-id="47cd5-221">布尔值</span><span class="sxs-lookup"><span data-stu-id="47cd5-221">Boolean</span></span>|<span data-ttu-id="47cd5-222">将此设置为 true 将创建每个应用程序 VPN 有效负载, 以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="47cd5-222">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="47cd5-223">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-224">safariDomains</span><span class="sxs-lookup"><span data-stu-id="47cd5-224">safariDomains</span></span>|<span data-ttu-id="47cd5-225">String 集合</span><span class="sxs-lookup"><span data-stu-id="47cd5-225">String collection</span></span>|<span data-ttu-id="47cd5-226">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="47cd5-226">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="47cd5-227">除了与此 vpn 关联的应用程序之外, 此处指定的 Safari 域还将能够触发此 vpn 连接。</span><span class="sxs-lookup"><span data-stu-id="47cd5-227">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="47cd5-228">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-228">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-229">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="47cd5-229">onDemandRules</span></span>|<span data-ttu-id="47cd5-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="47cd5-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="47cd5-231">按需规则。</span><span class="sxs-lookup"><span data-stu-id="47cd5-231">On-Demand Rules.</span></span> <span data-ttu-id="47cd5-232">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="47cd5-232">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="47cd5-233">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-233">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-234">proxyServer</span><span class="sxs-lookup"><span data-stu-id="47cd5-234">proxyServer</span></span>|[<span data-ttu-id="47cd5-235">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="47cd5-235">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="47cd5-236">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="47cd5-236">Proxy Server.</span></span> <span data-ttu-id="47cd5-237">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-237">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="47cd5-238">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="47cd5-238">optInToDeviceIdSharing</span></span>|<span data-ttu-id="47cd5-239">布尔值</span><span class="sxs-lookup"><span data-stu-id="47cd5-239">Boolean</span></span>|<span data-ttu-id="47cd5-240">选择将设备的 Id 共享到第三方 vpn 客户端, 以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="47cd5-240">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="47cd5-241">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47cd5-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="47cd5-242">响应</span><span class="sxs-lookup"><span data-stu-id="47cd5-242">Response</span></span>
<span data-ttu-id="47cd5-243">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="47cd5-243">If successful, this method returns a `200 OK` response code and an updated [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47cd5-244">示例</span><span class="sxs-lookup"><span data-stu-id="47cd5-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="47cd5-245">请求</span><span class="sxs-lookup"><span data-stu-id="47cd5-245">Request</span></span>
<span data-ttu-id="47cd5-246">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="47cd5-246">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1857

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="47cd5-247">响应</span><span class="sxs-lookup"><span data-stu-id="47cd5-247">Response</span></span>
<span data-ttu-id="47cd5-p126">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="47cd5-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2029

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "id": "8ce00178-0178-8ce0-7801-e08c7801e08c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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





