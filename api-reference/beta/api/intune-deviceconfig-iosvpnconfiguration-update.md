---
title: 更新 iosVpnConfiguration
description: 更新 iosVpnConfiguration 对象的属性。
author: tfitzmac
ms.openlocfilehash: b45e0d9eb395e93e876cfd874859b595b1ffa1a1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355641"
---
# <a name="update-iosvpnconfiguration"></a><span data-ttu-id="0ac20-103">更新 iosVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ac20-103">Update iosVpnConfiguration</span></span>

> <span data-ttu-id="0ac20-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0ac20-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ac20-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0ac20-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ac20-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0ac20-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ac20-107">更新[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0ac20-107">Update the properties of a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0ac20-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0ac20-108">Prerequisites</span></span>
<span data-ttu-id="0ac20-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0ac20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ac20-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ac20-111">Permission type</span></span>|<span data-ttu-id="0ac20-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0ac20-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ac20-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ac20-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ac20-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ac20-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ac20-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ac20-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ac20-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ac20-116">Not supported.</span></span>|
|<span data-ttu-id="0ac20-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ac20-117">Application</span></span>|<span data-ttu-id="0ac20-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ac20-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ac20-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ac20-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0ac20-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ac20-120">Request headers</span></span>
|<span data-ttu-id="0ac20-121">标头</span><span class="sxs-lookup"><span data-stu-id="0ac20-121">Header</span></span>|<span data-ttu-id="0ac20-122">值</span><span class="sxs-lookup"><span data-stu-id="0ac20-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ac20-123">授权</span><span class="sxs-lookup"><span data-stu-id="0ac20-123">Authorization</span></span>|<span data-ttu-id="0ac20-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0ac20-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ac20-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0ac20-125">Accept</span></span>|<span data-ttu-id="0ac20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ac20-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ac20-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ac20-127">Request body</span></span>
<span data-ttu-id="0ac20-128">在请求正文中，提供[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ac20-128">In the request body, supply a JSON representation for the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="0ac20-129">下表显示时创建[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0ac20-129">The following table shows the properties that are required when you create the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span>

|<span data-ttu-id="0ac20-130">属性</span><span class="sxs-lookup"><span data-stu-id="0ac20-130">Property</span></span>|<span data-ttu-id="0ac20-131">类型</span><span class="sxs-lookup"><span data-stu-id="0ac20-131">Type</span></span>|<span data-ttu-id="0ac20-132">说明</span><span class="sxs-lookup"><span data-stu-id="0ac20-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ac20-133">id</span><span class="sxs-lookup"><span data-stu-id="0ac20-133">id</span></span>|<span data-ttu-id="0ac20-134">String</span><span class="sxs-lookup"><span data-stu-id="0ac20-134">String</span></span>|<span data-ttu-id="0ac20-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0ac20-135">Key of the entity.</span></span> <span data-ttu-id="0ac20-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ac20-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0ac20-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ac20-138">DateTimeOffset</span></span>|<span data-ttu-id="0ac20-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0ac20-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0ac20-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0ac20-141">roleScopeTagIds</span></span>|<span data-ttu-id="0ac20-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="0ac20-142">String collection</span></span>|<span data-ttu-id="0ac20-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="0ac20-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0ac20-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0ac20-145">supportsScopeTags</span></span>|<span data-ttu-id="0ac20-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac20-146">Boolean</span></span>|<span data-ttu-id="0ac20-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="0ac20-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0ac20-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="0ac20-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0ac20-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="0ac20-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0ac20-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0ac20-150">This property is read-only.</span></span> <span data-ttu-id="0ac20-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ac20-152">createdDateTime</span></span>|<span data-ttu-id="0ac20-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ac20-153">DateTimeOffset</span></span>|<span data-ttu-id="0ac20-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0ac20-154">DateTime the object was created.</span></span> <span data-ttu-id="0ac20-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-156">description</span><span class="sxs-lookup"><span data-stu-id="0ac20-156">description</span></span>|<span data-ttu-id="0ac20-157">String</span><span class="sxs-lookup"><span data-stu-id="0ac20-157">String</span></span>|<span data-ttu-id="0ac20-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0ac20-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0ac20-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-160">displayName</span><span class="sxs-lookup"><span data-stu-id="0ac20-160">displayName</span></span>|<span data-ttu-id="0ac20-161">String</span><span class="sxs-lookup"><span data-stu-id="0ac20-161">String</span></span>|<span data-ttu-id="0ac20-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0ac20-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0ac20-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-164">version</span><span class="sxs-lookup"><span data-stu-id="0ac20-164">version</span></span>|<span data-ttu-id="0ac20-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0ac20-165">Int32</span></span>|<span data-ttu-id="0ac20-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0ac20-166">Version of the device configuration.</span></span> <span data-ttu-id="0ac20-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="0ac20-168">connectionName</span></span>|<span data-ttu-id="0ac20-169">字符串</span><span class="sxs-lookup"><span data-stu-id="0ac20-169">String</span></span>|<span data-ttu-id="0ac20-170">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="0ac20-170">Connection name displayed to the user.</span></span> <span data-ttu-id="0ac20-171">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-171">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-172">连接</span><span class="sxs-lookup"><span data-stu-id="0ac20-172">connectionType</span></span>|[<span data-ttu-id="0ac20-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="0ac20-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="0ac20-174">连接类型。</span><span class="sxs-lookup"><span data-stu-id="0ac20-174">Connection type.</span></span> <span data-ttu-id="0ac20-175">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="0ac20-175">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="0ac20-176">可能的值为： `ciscoAnyConnect`， `pulseSecure`， `f5EdgeClient`， `dellSonicWallMobileConnect`， `checkPointCapsuleVpn`， `customVpn`， `ciscoIPSec`， `citrix`， `ciscoAnyConnectV2`， `paloAltoGlobalProtect`， `zscalerPrivateAccess`， `f5Access2018`， `citrixSso`， `paloAltoGlobalProtectV2`。</span><span class="sxs-lookup"><span data-stu-id="0ac20-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="0ac20-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="0ac20-177">loginGroupOrDomain</span></span>|<span data-ttu-id="0ac20-178">字符串</span><span class="sxs-lookup"><span data-stu-id="0ac20-178">String</span></span>|<span data-ttu-id="0ac20-179">登录组或域时连接类型设置为 Dell 使 SonicWALL Mobile 连接。</span><span class="sxs-lookup"><span data-stu-id="0ac20-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="0ac20-180">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-180">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-181">role</span><span class="sxs-lookup"><span data-stu-id="0ac20-181">role</span></span>|<span data-ttu-id="0ac20-182">字符串</span><span class="sxs-lookup"><span data-stu-id="0ac20-182">String</span></span>|<span data-ttu-id="0ac20-183">当连接类型设置为脉冲安全角色。</span><span class="sxs-lookup"><span data-stu-id="0ac20-183">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="0ac20-184">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-184">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-185">领域</span><span class="sxs-lookup"><span data-stu-id="0ac20-185">realm</span></span>|<span data-ttu-id="0ac20-186">字符串</span><span class="sxs-lookup"><span data-stu-id="0ac20-186">String</span></span>|<span data-ttu-id="0ac20-187">当连接类型设置为脉冲安全领域。</span><span class="sxs-lookup"><span data-stu-id="0ac20-187">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="0ac20-188">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-188">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-189">服务器</span><span class="sxs-lookup"><span data-stu-id="0ac20-189">server</span></span>|[<span data-ttu-id="0ac20-190">vpnServer</span><span class="sxs-lookup"><span data-stu-id="0ac20-190">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="0ac20-191">在网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="0ac20-191">VPN Server on the network.</span></span> <span data-ttu-id="0ac20-192">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="0ac20-192">Make sure end users can access this network location.</span></span> <span data-ttu-id="0ac20-193">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-193">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-194">标识符</span><span class="sxs-lookup"><span data-stu-id="0ac20-194">identifier</span></span>|<span data-ttu-id="0ac20-195">字符串</span><span class="sxs-lookup"><span data-stu-id="0ac20-195">String</span></span>|<span data-ttu-id="0ac20-196">当连接类型设置为自定义 VPN VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="0ac20-196">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0ac20-197">例如： Cisco AnyConnect 使用[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)从窗体 com.cisco.anyconnect.applevpn.plugin 继承的标识符</span><span class="sxs-lookup"><span data-stu-id="0ac20-197">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-198">customData</span><span class="sxs-lookup"><span data-stu-id="0ac20-198">customData</span></span>|<span data-ttu-id="0ac20-199">[keyValue](../resources/intune-deviceconfig-keyvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="0ac20-199">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="0ac20-200">当设置为自定义 VPN 连接类型的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="0ac20-200">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0ac20-201">使用此字段启用不支持 Intune，但在 VPN 解决方案中可用的功能。</span><span class="sxs-lookup"><span data-stu-id="0ac20-201">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="0ac20-202">了解如何添加这些键/值对 VPN 供应商联系。</span><span class="sxs-lookup"><span data-stu-id="0ac20-202">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="0ac20-203">此集合可以包含最多 25 元素。</span><span class="sxs-lookup"><span data-stu-id="0ac20-203">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="0ac20-204">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="0ac20-205">customKeyValueData</span></span>|<span data-ttu-id="0ac20-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0ac20-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0ac20-207">当设置为自定义 VPN 连接类型的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="0ac20-207">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0ac20-208">使用此字段启用不支持 Intune，但在 VPN 解决方案中可用的功能。</span><span class="sxs-lookup"><span data-stu-id="0ac20-208">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="0ac20-209">了解如何添加这些键/值对 VPN 供应商联系。</span><span class="sxs-lookup"><span data-stu-id="0ac20-209">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="0ac20-210">此集合可以包含最多 25 元素。</span><span class="sxs-lookup"><span data-stu-id="0ac20-210">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="0ac20-211">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-211">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-212">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="0ac20-212">enableSplitTunneling</span></span>|<span data-ttu-id="0ac20-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac20-213">Boolean</span></span>|<span data-ttu-id="0ac20-214">将发送所有网络流量通过 VPN。</span><span class="sxs-lookup"><span data-stu-id="0ac20-214">Send all network traffic through VPN.</span></span> <span data-ttu-id="0ac20-215">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-216">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0ac20-216">authenticationMethod</span></span>|[<span data-ttu-id="0ac20-217">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0ac20-217">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="0ac20-218">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="0ac20-218">Authentication method for this VPN connection.</span></span> <span data-ttu-id="0ac20-219">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="0ac20-219">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="0ac20-220">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="0ac20-220">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="0ac20-221">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="0ac20-221">enablePerApp</span></span>|<span data-ttu-id="0ac20-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac20-222">Boolean</span></span>|<span data-ttu-id="0ac20-223">将此值设置为 true 时，创建更高版本可以是与可触发本 VPN 连接最终用户的 iOS 设备上的应用程序关联的每个应用程序 VPN 负载。</span><span class="sxs-lookup"><span data-stu-id="0ac20-223">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="0ac20-224">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-224">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-225">safariDomains</span><span class="sxs-lookup"><span data-stu-id="0ac20-225">safariDomains</span></span>|<span data-ttu-id="0ac20-226">String 集合</span><span class="sxs-lookup"><span data-stu-id="0ac20-226">String collection</span></span>|<span data-ttu-id="0ac20-227">Safari 域时启用此 VPN 每应用程序设置。</span><span class="sxs-lookup"><span data-stu-id="0ac20-227">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="0ac20-228">与此 VPN 关联的应用程序，除了 Safari 域指定此处还将能够触发本 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="0ac20-228">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="0ac20-229">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-229">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-230">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="0ac20-230">onDemandRules</span></span>|<span data-ttu-id="0ac20-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="0ac20-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="0ac20-232">按需规则。</span><span class="sxs-lookup"><span data-stu-id="0ac20-232">On-Demand Rules.</span></span> <span data-ttu-id="0ac20-233">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0ac20-233">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0ac20-234">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-234">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-235">代理服务器</span><span class="sxs-lookup"><span data-stu-id="0ac20-235">proxyServer</span></span>|[<span data-ttu-id="0ac20-236">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="0ac20-236">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="0ac20-237">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="0ac20-237">Proxy Server.</span></span> <span data-ttu-id="0ac20-238">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-238">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-239">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="0ac20-239">optInToDeviceIdSharing</span></span>|<span data-ttu-id="0ac20-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac20-240">Boolean</span></span>|<span data-ttu-id="0ac20-241">加入到共享网络访问控制验证过程中的第三方 vpn 客户端使用的设备的 Id。</span><span class="sxs-lookup"><span data-stu-id="0ac20-241">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="0ac20-242">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac20-242">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0ac20-243">提供程序类型</span><span class="sxs-lookup"><span data-stu-id="0ac20-243">providerType</span></span>|[<span data-ttu-id="0ac20-244">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="0ac20-244">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="0ac20-245">每个应用程序 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="0ac20-245">Provider type for per-app VPN.</span></span> <span data-ttu-id="0ac20-246">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="0ac20-246">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="0ac20-247">userDomain</span><span class="sxs-lookup"><span data-stu-id="0ac20-247">userDomain</span></span>|<span data-ttu-id="0ac20-248">字符串</span><span class="sxs-lookup"><span data-stu-id="0ac20-248">String</span></span>|<span data-ttu-id="0ac20-249">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="0ac20-249">Zscaler only.</span></span> <span data-ttu-id="0ac20-250">输入静态域预填充具有 Zscaler 应用程序中的登录字段。</span><span class="sxs-lookup"><span data-stu-id="0ac20-250">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="0ac20-251">如果这保留为空，将使用用户的 Azure Active Directory 域。</span><span class="sxs-lookup"><span data-stu-id="0ac20-251">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="0ac20-252">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="0ac20-252">strictEnforcement</span></span>|<span data-ttu-id="0ac20-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac20-253">Boolean</span></span>|<span data-ttu-id="0ac20-254">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="0ac20-254">Zscaler only.</span></span> <span data-ttu-id="0ac20-255">块到 Zscaler 应用程序直到用户迹象网络流量。</span><span class="sxs-lookup"><span data-stu-id="0ac20-255">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="0ac20-256">搕 rue 意味着阻止流量。</span><span class="sxs-lookup"><span data-stu-id="0ac20-256">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="0ac20-257">cloudName</span><span class="sxs-lookup"><span data-stu-id="0ac20-257">cloudName</span></span>|<span data-ttu-id="0ac20-258">字符串</span><span class="sxs-lookup"><span data-stu-id="0ac20-258">String</span></span>|<span data-ttu-id="0ac20-259">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="0ac20-259">Zscaler only.</span></span> <span data-ttu-id="0ac20-260">该用户分配给 Zscaler 云。</span><span class="sxs-lookup"><span data-stu-id="0ac20-260">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="0ac20-261">excludeList</span><span class="sxs-lookup"><span data-stu-id="0ac20-261">excludeList</span></span>|<span data-ttu-id="0ac20-262">String 集合</span><span class="sxs-lookup"><span data-stu-id="0ac20-262">String collection</span></span>|<span data-ttu-id="0ac20-263">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="0ac20-263">Zscaler only.</span></span> <span data-ttu-id="0ac20-264">不会通过 Zscaler 云发送的网络地址的列表。</span><span class="sxs-lookup"><span data-stu-id="0ac20-264">List of network addresses which are not sent through the Zscaler cloud.</span></span>|



## <a name="response"></a><span data-ttu-id="0ac20-265">响应</span><span class="sxs-lookup"><span data-stu-id="0ac20-265">Response</span></span>
<span data-ttu-id="0ac20-266">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0ac20-266">If successful, this method returns a `200 OK` response code and an updated [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ac20-267">示例</span><span class="sxs-lookup"><span data-stu-id="0ac20-267">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ac20-268">请求</span><span class="sxs-lookup"><span data-stu-id="0ac20-268">Request</span></span>
<span data-ttu-id="0ac20-269">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0ac20-269">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2048

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="0ac20-270">响应</span><span class="sxs-lookup"><span data-stu-id="0ac20-270">Response</span></span>
<span data-ttu-id="0ac20-p132">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0ac20-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2214

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
  "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
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
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ]
}
```





