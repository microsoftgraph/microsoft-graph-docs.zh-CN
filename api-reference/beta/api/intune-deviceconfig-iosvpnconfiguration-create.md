---
title: 创建 iosVpnConfiguration
description: 创建新的 iosVpnConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de7cbc2a357de7d4187379d2320b5718a85030ee
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923109"
---
# <a name="create-iosvpnconfiguration"></a><span data-ttu-id="3d6ae-103">创建 iosVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="3d6ae-103">Create iosVpnConfiguration</span></span>

> <span data-ttu-id="3d6ae-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d6ae-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d6ae-106">创建新的[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-106">Create a new [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d6ae-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3d6ae-107">Prerequisites</span></span>
<span data-ttu-id="3d6ae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d6ae-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d6ae-110">Permission type</span></span>|<span data-ttu-id="3d6ae-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3d6ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d6ae-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d6ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3d6ae-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d6ae-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3d6ae-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d6ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d6ae-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-115">Not supported.</span></span>|
|<span data-ttu-id="3d6ae-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d6ae-116">Application</span></span>|<span data-ttu-id="3d6ae-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d6ae-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d6ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3d6ae-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d6ae-119">Request headers</span></span>
|<span data-ttu-id="3d6ae-120">标头</span><span class="sxs-lookup"><span data-stu-id="3d6ae-120">Header</span></span>|<span data-ttu-id="3d6ae-121">值</span><span class="sxs-lookup"><span data-stu-id="3d6ae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d6ae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d6ae-122">Authorization</span></span>|<span data-ttu-id="3d6ae-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d6ae-124">接受</span><span class="sxs-lookup"><span data-stu-id="3d6ae-124">Accept</span></span>|<span data-ttu-id="3d6ae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3d6ae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d6ae-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d6ae-126">Request body</span></span>
<span data-ttu-id="3d6ae-127">在请求正文中, 提供 iosVpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-127">In the request body, supply a JSON representation for the iosVpnConfiguration object.</span></span>

<span data-ttu-id="3d6ae-128">下表显示创建 iosVpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-128">The following table shows the properties that are required when you create the iosVpnConfiguration.</span></span>

|<span data-ttu-id="3d6ae-129">属性</span><span class="sxs-lookup"><span data-stu-id="3d6ae-129">Property</span></span>|<span data-ttu-id="3d6ae-130">类型</span><span class="sxs-lookup"><span data-stu-id="3d6ae-130">Type</span></span>|<span data-ttu-id="3d6ae-131">说明</span><span class="sxs-lookup"><span data-stu-id="3d6ae-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d6ae-132">id</span><span class="sxs-lookup"><span data-stu-id="3d6ae-132">id</span></span>|<span data-ttu-id="3d6ae-133">字符串</span><span class="sxs-lookup"><span data-stu-id="3d6ae-133">String</span></span>|<span data-ttu-id="3d6ae-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-134">Key of the entity.</span></span> <span data-ttu-id="3d6ae-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d6ae-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3d6ae-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d6ae-137">DateTimeOffset</span></span>|<span data-ttu-id="3d6ae-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3d6ae-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3d6ae-140">roleScopeTagIds</span></span>|<span data-ttu-id="3d6ae-141">String collection</span><span class="sxs-lookup"><span data-stu-id="3d6ae-141">String collection</span></span>|<span data-ttu-id="3d6ae-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3d6ae-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3d6ae-144">supportsScopeTags</span></span>|<span data-ttu-id="3d6ae-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d6ae-145">Boolean</span></span>|<span data-ttu-id="3d6ae-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3d6ae-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3d6ae-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3d6ae-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-149">This property is read-only.</span></span> <span data-ttu-id="3d6ae-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3d6ae-151">createdDateTime</span></span>|<span data-ttu-id="3d6ae-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d6ae-152">DateTimeOffset</span></span>|<span data-ttu-id="3d6ae-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-153">DateTime the object was created.</span></span> <span data-ttu-id="3d6ae-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-155">说明</span><span class="sxs-lookup"><span data-stu-id="3d6ae-155">description</span></span>|<span data-ttu-id="3d6ae-156">String</span><span class="sxs-lookup"><span data-stu-id="3d6ae-156">String</span></span>|<span data-ttu-id="3d6ae-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3d6ae-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-159">displayName</span><span class="sxs-lookup"><span data-stu-id="3d6ae-159">displayName</span></span>|<span data-ttu-id="3d6ae-160">String</span><span class="sxs-lookup"><span data-stu-id="3d6ae-160">String</span></span>|<span data-ttu-id="3d6ae-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3d6ae-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-163">version</span><span class="sxs-lookup"><span data-stu-id="3d6ae-163">version</span></span>|<span data-ttu-id="3d6ae-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3d6ae-164">Int32</span></span>|<span data-ttu-id="3d6ae-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-165">Version of the device configuration.</span></span> <span data-ttu-id="3d6ae-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="3d6ae-167">connectionName</span></span>|<span data-ttu-id="3d6ae-168">String</span><span class="sxs-lookup"><span data-stu-id="3d6ae-168">String</span></span>|<span data-ttu-id="3d6ae-169">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-169">Connection name displayed to the user.</span></span> <span data-ttu-id="3d6ae-170">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-170">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="3d6ae-171">connectionType</span></span>|[<span data-ttu-id="3d6ae-172">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="3d6ae-172">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="3d6ae-173">连接类型。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-173">Connection type.</span></span> <span data-ttu-id="3d6ae-174">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-174">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="3d6ae-175">可能的值为`ciscoAnyConnect`: `pulseSecure`、 `f5EdgeClient`、 `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `paloAltoGlobalProtectV2`、、、、、、、、、、、。 `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso`</span><span class="sxs-lookup"><span data-stu-id="3d6ae-175">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="3d6ae-176">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="3d6ae-176">loginGroupOrDomain</span></span>|<span data-ttu-id="3d6ae-177">String</span><span class="sxs-lookup"><span data-stu-id="3d6ae-177">String</span></span>|<span data-ttu-id="3d6ae-178">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-178">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="3d6ae-179">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-179">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-180">role</span><span class="sxs-lookup"><span data-stu-id="3d6ae-180">role</span></span>|<span data-ttu-id="3d6ae-181">String</span><span class="sxs-lookup"><span data-stu-id="3d6ae-181">String</span></span>|<span data-ttu-id="3d6ae-182">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-182">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="3d6ae-183">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-184">型</span><span class="sxs-lookup"><span data-stu-id="3d6ae-184">realm</span></span>|<span data-ttu-id="3d6ae-185">String</span><span class="sxs-lookup"><span data-stu-id="3d6ae-185">String</span></span>|<span data-ttu-id="3d6ae-186">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-186">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="3d6ae-187">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-188">服务器主板</span><span class="sxs-lookup"><span data-stu-id="3d6ae-188">server</span></span>|[<span data-ttu-id="3d6ae-189">vpnServer</span><span class="sxs-lookup"><span data-stu-id="3d6ae-189">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="3d6ae-190">网络上的 VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-190">VPN Server on the network.</span></span> <span data-ttu-id="3d6ae-191">请确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-191">Make sure end users can access this network location.</span></span> <span data-ttu-id="3d6ae-192">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-193">标识符</span><span class="sxs-lookup"><span data-stu-id="3d6ae-193">identifier</span></span>|<span data-ttu-id="3d6ae-194">String</span><span class="sxs-lookup"><span data-stu-id="3d6ae-194">String</span></span>|<span data-ttu-id="3d6ae-195">当连接类型设置为自定义 VPN 时, 由 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-195">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="3d6ae-196">例如: Cisco AnyConnect 使用从[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)继承的 AnyConnect applevpn 的标识符。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-196">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-197">customData</span><span class="sxs-lookup"><span data-stu-id="3d6ae-197">customData</span></span>|<span data-ttu-id="3d6ae-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3d6ae-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="3d6ae-199">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-199">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="3d6ae-200">使用此字段启用 Intune 不支持的功能, 但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-200">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="3d6ae-201">请与你的 VPN 供应商联系, 了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-201">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="3d6ae-202">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-202">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="3d6ae-203">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-203">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="3d6ae-204">customKeyValueData</span></span>|<span data-ttu-id="3d6ae-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3d6ae-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="3d6ae-206">将连接类型设置为自定义 VPN 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-206">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="3d6ae-207">使用此字段启用 Intune 不支持的功能, 但在你的 VPN 解决方案中可用。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-207">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="3d6ae-208">请与你的 VPN 供应商联系, 了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-208">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="3d6ae-209">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-209">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="3d6ae-210">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-210">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-211">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="3d6ae-211">enableSplitTunneling</span></span>|<span data-ttu-id="3d6ae-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d6ae-212">Boolean</span></span>|<span data-ttu-id="3d6ae-213">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-213">Send all network traffic through VPN.</span></span> <span data-ttu-id="3d6ae-214">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-214">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-215">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3d6ae-215">authenticationMethod</span></span>|[<span data-ttu-id="3d6ae-216">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3d6ae-216">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="3d6ae-217">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-217">Authentication method for this VPN connection.</span></span> <span data-ttu-id="3d6ae-218">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-218">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="3d6ae-219">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-219">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="3d6ae-220">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="3d6ae-220">enablePerApp</span></span>|<span data-ttu-id="3d6ae-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d6ae-221">Boolean</span></span>|<span data-ttu-id="3d6ae-222">将此设置为 true 将创建每个应用程序 VPN 有效负载, 以后可将其与可在最终用户的 iOS 设备上触发此 VPN 连接的应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-222">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="3d6ae-223">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-224">safariDomains</span><span class="sxs-lookup"><span data-stu-id="3d6ae-224">safariDomains</span></span>|<span data-ttu-id="3d6ae-225">String collection</span><span class="sxs-lookup"><span data-stu-id="3d6ae-225">String collection</span></span>|<span data-ttu-id="3d6ae-226">启用此 VPN 每应用程序设置时的 Safari 域。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-226">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="3d6ae-227">除了与此 VPN 关联的应用程序之外, 此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-227">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="3d6ae-228">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-228">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-229">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="3d6ae-229">onDemandRules</span></span>|<span data-ttu-id="3d6ae-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="3d6ae-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="3d6ae-231">按需规则。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-231">On-Demand Rules.</span></span> <span data-ttu-id="3d6ae-232">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-232">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="3d6ae-233">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-233">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-234">proxyServer</span><span class="sxs-lookup"><span data-stu-id="3d6ae-234">proxyServer</span></span>|[<span data-ttu-id="3d6ae-235">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="3d6ae-235">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="3d6ae-236">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-236">Proxy Server.</span></span> <span data-ttu-id="3d6ae-237">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-237">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-238">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="3d6ae-238">optInToDeviceIdSharing</span></span>|<span data-ttu-id="3d6ae-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d6ae-239">Boolean</span></span>|<span data-ttu-id="3d6ae-240">选择将设备的 Id 共享到第三方 vpn 客户端, 以便在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-240">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="3d6ae-241">继承自[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d6ae-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="3d6ae-242">providerType</span><span class="sxs-lookup"><span data-stu-id="3d6ae-242">providerType</span></span>|[<span data-ttu-id="3d6ae-243">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="3d6ae-243">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="3d6ae-244">每应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-244">Provider type for per-app VPN.</span></span> <span data-ttu-id="3d6ae-245">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-245">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="3d6ae-246">userDomain</span><span class="sxs-lookup"><span data-stu-id="3d6ae-246">userDomain</span></span>|<span data-ttu-id="3d6ae-247">String</span><span class="sxs-lookup"><span data-stu-id="3d6ae-247">String</span></span>|<span data-ttu-id="3d6ae-248">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-248">Zscaler only.</span></span> <span data-ttu-id="3d6ae-249">输入一个静态域, 以便在 Zscaler 应用程序中预填充 "登录" 字段。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-249">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="3d6ae-250">如果保留为空, 则将改用用户的 Azure Active Directory 域。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-250">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="3d6ae-251">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="3d6ae-251">strictEnforcement</span></span>|<span data-ttu-id="3d6ae-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d6ae-252">Boolean</span></span>|<span data-ttu-id="3d6ae-253">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-253">Zscaler only.</span></span> <span data-ttu-id="3d6ae-254">阻止网络流量, 直到用户登录到 Zscaler 应用程序。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-254">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="3d6ae-255">"True" 表示阻止流量。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-255">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="3d6ae-256">cloudName</span><span class="sxs-lookup"><span data-stu-id="3d6ae-256">cloudName</span></span>|<span data-ttu-id="3d6ae-257">String</span><span class="sxs-lookup"><span data-stu-id="3d6ae-257">String</span></span>|<span data-ttu-id="3d6ae-258">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-258">Zscaler only.</span></span> <span data-ttu-id="3d6ae-259">用户分配到的 Zscaler 云。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-259">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="3d6ae-260">excludeList</span><span class="sxs-lookup"><span data-stu-id="3d6ae-260">excludeList</span></span>|<span data-ttu-id="3d6ae-261">String collection</span><span class="sxs-lookup"><span data-stu-id="3d6ae-261">String collection</span></span>|<span data-ttu-id="3d6ae-262">仅 Zscaler。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-262">Zscaler only.</span></span> <span data-ttu-id="3d6ae-263">不通过 Zscaler 云发送的网络地址的列表。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-263">List of network addresses which are not sent through the Zscaler cloud.</span></span>|



## <a name="response"></a><span data-ttu-id="3d6ae-264">响应</span><span class="sxs-lookup"><span data-stu-id="3d6ae-264">Response</span></span>
<span data-ttu-id="3d6ae-265">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-265">If successful, this method returns a `201 Created` response code and a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d6ae-266">示例</span><span class="sxs-lookup"><span data-stu-id="3d6ae-266">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d6ae-267">请求</span><span class="sxs-lookup"><span data-stu-id="3d6ae-267">Request</span></span>
<span data-ttu-id="3d6ae-268">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-268">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2042

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="3d6ae-269">响应</span><span class="sxs-lookup"><span data-stu-id="3d6ae-269">Response</span></span>
<span data-ttu-id="3d6ae-p131">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3d6ae-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




