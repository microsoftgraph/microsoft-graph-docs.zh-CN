---
title: 更新 androidWorkProfileVpnConfiguration
description: 更新 androidWorkProfileVpnConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 283524cfbf51540cb7ac8a1012c1bd4cb988f8ff
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123223"
---
# <a name="update-androidworkprofilevpnconfiguration"></a><span data-ttu-id="fc64e-103">更新 androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="fc64e-103">Update androidWorkProfileVpnConfiguration</span></span>

<span data-ttu-id="fc64e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc64e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc64e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fc64e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc64e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc64e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc64e-107">更新[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fc64e-107">Update the properties of a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc64e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fc64e-108">Prerequisites</span></span>
<span data-ttu-id="fc64e-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="fc64e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="fc64e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc64e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc64e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc64e-111">Permission type</span></span>|<span data-ttu-id="fc64e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fc64e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc64e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc64e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc64e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc64e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fc64e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc64e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc64e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc64e-116">Not supported.</span></span>|
|<span data-ttu-id="fc64e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc64e-117">Application</span></span>|<span data-ttu-id="fc64e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc64e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc64e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc64e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fc64e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc64e-120">Request headers</span></span>
|<span data-ttu-id="fc64e-121">标头</span><span class="sxs-lookup"><span data-stu-id="fc64e-121">Header</span></span>|<span data-ttu-id="fc64e-122">值</span><span class="sxs-lookup"><span data-stu-id="fc64e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc64e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc64e-123">Authorization</span></span>|<span data-ttu-id="fc64e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fc64e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc64e-125">接受</span><span class="sxs-lookup"><span data-stu-id="fc64e-125">Accept</span></span>|<span data-ttu-id="fc64e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc64e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc64e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc64e-127">Request body</span></span>
<span data-ttu-id="fc64e-128">在请求正文中，提供[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc64e-128">In the request body, supply a JSON representation for the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

<span data-ttu-id="fc64e-129">下表显示创建[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fc64e-129">The following table shows the properties that are required when you create the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span></span>

|<span data-ttu-id="fc64e-130">属性</span><span class="sxs-lookup"><span data-stu-id="fc64e-130">Property</span></span>|<span data-ttu-id="fc64e-131">类型</span><span class="sxs-lookup"><span data-stu-id="fc64e-131">Type</span></span>|<span data-ttu-id="fc64e-132">说明</span><span class="sxs-lookup"><span data-stu-id="fc64e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc64e-133">id</span><span class="sxs-lookup"><span data-stu-id="fc64e-133">id</span></span>|<span data-ttu-id="fc64e-134">字符串</span><span class="sxs-lookup"><span data-stu-id="fc64e-134">String</span></span>|<span data-ttu-id="fc64e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fc64e-135">Key of the entity.</span></span> <span data-ttu-id="fc64e-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc64e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc64e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc64e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fc64e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc64e-138">DateTimeOffset</span></span>|<span data-ttu-id="fc64e-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fc64e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fc64e-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc64e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc64e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fc64e-141">roleScopeTagIds</span></span>|<span data-ttu-id="fc64e-142">String collection</span><span class="sxs-lookup"><span data-stu-id="fc64e-142">String collection</span></span>|<span data-ttu-id="fc64e-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="fc64e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fc64e-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc64e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc64e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fc64e-145">supportsScopeTags</span></span>|<span data-ttu-id="fc64e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc64e-146">Boolean</span></span>|<span data-ttu-id="fc64e-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="fc64e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fc64e-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="fc64e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fc64e-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="fc64e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fc64e-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="fc64e-150">This property is read-only.</span></span> <span data-ttu-id="fc64e-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc64e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc64e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fc64e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="fc64e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fc64e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="fc64e-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="fc64e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="fc64e-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc64e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc64e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fc64e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="fc64e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fc64e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="fc64e-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="fc64e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="fc64e-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc64e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc64e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fc64e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="fc64e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fc64e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="fc64e-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="fc64e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="fc64e-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc64e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc64e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fc64e-164">createdDateTime</span></span>|<span data-ttu-id="fc64e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc64e-165">DateTimeOffset</span></span>|<span data-ttu-id="fc64e-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fc64e-166">DateTime the object was created.</span></span> <span data-ttu-id="fc64e-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc64e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc64e-168">说明</span><span class="sxs-lookup"><span data-stu-id="fc64e-168">description</span></span>|<span data-ttu-id="fc64e-169">String</span><span class="sxs-lookup"><span data-stu-id="fc64e-169">String</span></span>|<span data-ttu-id="fc64e-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="fc64e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fc64e-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc64e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc64e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="fc64e-172">displayName</span></span>|<span data-ttu-id="fc64e-173">String</span><span class="sxs-lookup"><span data-stu-id="fc64e-173">String</span></span>|<span data-ttu-id="fc64e-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="fc64e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fc64e-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc64e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc64e-176">version</span><span class="sxs-lookup"><span data-stu-id="fc64e-176">version</span></span>|<span data-ttu-id="fc64e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="fc64e-177">Int32</span></span>|<span data-ttu-id="fc64e-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="fc64e-178">Version of the device configuration.</span></span> <span data-ttu-id="fc64e-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc64e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc64e-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="fc64e-180">connectionName</span></span>|<span data-ttu-id="fc64e-181">String</span><span class="sxs-lookup"><span data-stu-id="fc64e-181">String</span></span>|<span data-ttu-id="fc64e-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="fc64e-182">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="fc64e-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="fc64e-183">connectionType</span></span>|[<span data-ttu-id="fc64e-184">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="fc64e-184">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="fc64e-185">连接类型。</span><span class="sxs-lookup"><span data-stu-id="fc64e-185">Connection type.</span></span> <span data-ttu-id="fc64e-186">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`、`paloAltoGlobalProtect`、`microsoftTunnel`。</span><span class="sxs-lookup"><span data-stu-id="fc64e-186">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`, `microsoftTunnel`.</span></span>|
|<span data-ttu-id="fc64e-187">role</span><span class="sxs-lookup"><span data-stu-id="fc64e-187">role</span></span>|<span data-ttu-id="fc64e-188">String</span><span class="sxs-lookup"><span data-stu-id="fc64e-188">String</span></span>|<span data-ttu-id="fc64e-189">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="fc64e-189">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="fc64e-190">型</span><span class="sxs-lookup"><span data-stu-id="fc64e-190">realm</span></span>|<span data-ttu-id="fc64e-191">String</span><span class="sxs-lookup"><span data-stu-id="fc64e-191">String</span></span>|<span data-ttu-id="fc64e-192">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="fc64e-192">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="fc64e-193">台</span><span class="sxs-lookup"><span data-stu-id="fc64e-193">servers</span></span>|<span data-ttu-id="fc64e-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="fc64e-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="fc64e-195">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="fc64e-195">List of VPN Servers on the network.</span></span> <span data-ttu-id="fc64e-196">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="fc64e-196">Make sure end users can access these network locations.</span></span> <span data-ttu-id="fc64e-197">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="fc64e-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="fc64e-198">其次</span><span class="sxs-lookup"><span data-stu-id="fc64e-198">fingerprint</span></span>|<span data-ttu-id="fc64e-199">String</span><span class="sxs-lookup"><span data-stu-id="fc64e-199">String</span></span>|<span data-ttu-id="fc64e-200">指纹是一个字符串，用于验证 VPN 服务器是否可以信任，这仅在连接类型为 "检查点胶囊" VPN 时适用。</span><span class="sxs-lookup"><span data-stu-id="fc64e-200">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="fc64e-201">customData</span><span class="sxs-lookup"><span data-stu-id="fc64e-201">customData</span></span>|<span data-ttu-id="fc64e-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fc64e-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="fc64e-203">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="fc64e-203">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="fc64e-204">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="fc64e-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="fc64e-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="fc64e-205">customKeyValueData</span></span>|<span data-ttu-id="fc64e-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fc64e-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="fc64e-207">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="fc64e-207">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="fc64e-208">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="fc64e-208">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="fc64e-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fc64e-209">authenticationMethod</span></span>|[<span data-ttu-id="fc64e-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fc64e-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="fc64e-211">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="fc64e-211">Authentication method.</span></span> <span data-ttu-id="fc64e-212">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="fc64e-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="fc64e-213">proxyServer</span><span class="sxs-lookup"><span data-stu-id="fc64e-213">proxyServer</span></span>|[<span data-ttu-id="fc64e-214">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="fc64e-214">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="fc64e-215">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="fc64e-215">Proxy server.</span></span>|
|<span data-ttu-id="fc64e-216">targetedPackageIds</span><span class="sxs-lookup"><span data-stu-id="fc64e-216">targetedPackageIds</span></span>|<span data-ttu-id="fc64e-217">String collection</span><span class="sxs-lookup"><span data-stu-id="fc64e-217">String collection</span></span>|<span data-ttu-id="fc64e-218">目标应用程序包 Id。</span><span class="sxs-lookup"><span data-stu-id="fc64e-218">Targeted App package IDs.</span></span>|
|<span data-ttu-id="fc64e-219">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="fc64e-219">alwaysOn</span></span>|<span data-ttu-id="fc64e-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc64e-220">Boolean</span></span>|<span data-ttu-id="fc64e-221">是否启用始终启用的 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="fc64e-221">Whether or not to enable always-on VPN connection.</span></span>|
|<span data-ttu-id="fc64e-222">alwaysOnLockdown</span><span class="sxs-lookup"><span data-stu-id="fc64e-222">alwaysOnLockdown</span></span>|<span data-ttu-id="fc64e-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc64e-223">Boolean</span></span>|<span data-ttu-id="fc64e-224">如果启用了 always on VPN 连接，则在断开 VPN 连接时是否锁定网络流量。</span><span class="sxs-lookup"><span data-stu-id="fc64e-224">If always-on VPN connection is enabled, whether or not to lock network traffic when that VPN is disconnected.</span></span>|



## <a name="response"></a><span data-ttu-id="fc64e-225">响应</span><span class="sxs-lookup"><span data-stu-id="fc64e-225">Response</span></span>
<span data-ttu-id="fc64e-226">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fc64e-226">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc64e-227">示例</span><span class="sxs-lookup"><span data-stu-id="fc64e-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc64e-228">请求</span><span class="sxs-lookup"><span data-stu-id="fc64e-228">Request</span></span>
<span data-ttu-id="fc64e-229">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fc64e-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2103

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
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
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
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
  "authenticationMethod": "usernameAndPassword",
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "targetedPackageIds": [
    "Targeted Package Ids value"
  ],
  "alwaysOn": true,
  "alwaysOnLockdown": true
}
```

### <a name="response"></a><span data-ttu-id="fc64e-230">响应</span><span class="sxs-lookup"><span data-stu-id="fc64e-230">Response</span></span>
<span data-ttu-id="fc64e-231">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="fc64e-231">Here is an example of the response.</span></span> <span data-ttu-id="fc64e-232">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="fc64e-232">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fc64e-233">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="fc64e-233">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2275

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
  "id": "32910378-0378-3291-7803-913278039132",
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
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
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
  "authenticationMethod": "usernameAndPassword",
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "targetedPackageIds": [
    "Targeted Package Ids value"
  ],
  "alwaysOn": true,
  "alwaysOnLockdown": true
}
```



