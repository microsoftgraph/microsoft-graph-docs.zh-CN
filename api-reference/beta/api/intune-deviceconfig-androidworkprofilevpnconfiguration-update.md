---
title: 更新 androidWorkProfileVpnConfiguration
description: 更新 androidWorkProfileVpnConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0456ad3282119d3927eaeb943dec3babb984d51
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949866"
---
# <a name="update-androidworkprofilevpnconfiguration"></a><span data-ttu-id="b3d8b-103">更新 androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b3d8b-103">Update androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="b3d8b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3d8b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3d8b-106">更新[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-106">Update the properties of a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3d8b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b3d8b-107">Prerequisites</span></span>
<span data-ttu-id="b3d8b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3d8b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3d8b-110">Permission type</span></span>|<span data-ttu-id="b3d8b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b3d8b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3d8b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3d8b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3d8b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3d8b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3d8b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3d8b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3d8b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-115">Not supported.</span></span>|
|<span data-ttu-id="b3d8b-116">Application</span><span class="sxs-lookup"><span data-stu-id="b3d8b-116">Application</span></span>|<span data-ttu-id="b3d8b-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3d8b-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3d8b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3d8b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b3d8b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3d8b-119">Request headers</span></span>
|<span data-ttu-id="b3d8b-120">标头</span><span class="sxs-lookup"><span data-stu-id="b3d8b-120">Header</span></span>|<span data-ttu-id="b3d8b-121">值</span><span class="sxs-lookup"><span data-stu-id="b3d8b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3d8b-122">授权</span><span class="sxs-lookup"><span data-stu-id="b3d8b-122">Authorization</span></span>|<span data-ttu-id="b3d8b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3d8b-124">接受</span><span class="sxs-lookup"><span data-stu-id="b3d8b-124">Accept</span></span>|<span data-ttu-id="b3d8b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b3d8b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3d8b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3d8b-126">Request body</span></span>
<span data-ttu-id="b3d8b-127">在请求正文中，提供[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-127">In the request body, supply a JSON representation for the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

<span data-ttu-id="b3d8b-128">下表显示创建[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-128">The following table shows the properties that are required when you create the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span></span>

|<span data-ttu-id="b3d8b-129">属性</span><span class="sxs-lookup"><span data-stu-id="b3d8b-129">Property</span></span>|<span data-ttu-id="b3d8b-130">类型</span><span class="sxs-lookup"><span data-stu-id="b3d8b-130">Type</span></span>|<span data-ttu-id="b3d8b-131">说明</span><span class="sxs-lookup"><span data-stu-id="b3d8b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3d8b-132">id</span><span class="sxs-lookup"><span data-stu-id="b3d8b-132">id</span></span>|<span data-ttu-id="b3d8b-133">字符串</span><span class="sxs-lookup"><span data-stu-id="b3d8b-133">String</span></span>|<span data-ttu-id="b3d8b-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-134">Key of the entity.</span></span> <span data-ttu-id="b3d8b-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3d8b-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3d8b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3d8b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b3d8b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3d8b-137">DateTimeOffset</span></span>|<span data-ttu-id="b3d8b-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b3d8b-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3d8b-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3d8b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b3d8b-140">roleScopeTagIds</span></span>|<span data-ttu-id="b3d8b-141">String collection</span><span class="sxs-lookup"><span data-stu-id="b3d8b-141">String collection</span></span>|<span data-ttu-id="b3d8b-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b3d8b-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3d8b-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3d8b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b3d8b-144">supportsScopeTags</span></span>|<span data-ttu-id="b3d8b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3d8b-145">Boolean</span></span>|<span data-ttu-id="b3d8b-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b3d8b-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b3d8b-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b3d8b-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-149">This property is read-only.</span></span> <span data-ttu-id="b3d8b-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3d8b-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3d8b-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b3d8b-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b3d8b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b3d8b-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b3d8b-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b3d8b-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3d8b-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3d8b-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b3d8b-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b3d8b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b3d8b-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b3d8b-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b3d8b-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3d8b-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3d8b-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b3d8b-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b3d8b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b3d8b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b3d8b-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b3d8b-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3d8b-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3d8b-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3d8b-163">createdDateTime</span></span>|<span data-ttu-id="b3d8b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3d8b-164">DateTimeOffset</span></span>|<span data-ttu-id="b3d8b-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-165">DateTime the object was created.</span></span> <span data-ttu-id="b3d8b-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3d8b-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3d8b-167">说明</span><span class="sxs-lookup"><span data-stu-id="b3d8b-167">description</span></span>|<span data-ttu-id="b3d8b-168">String</span><span class="sxs-lookup"><span data-stu-id="b3d8b-168">String</span></span>|<span data-ttu-id="b3d8b-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b3d8b-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3d8b-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3d8b-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b3d8b-171">displayName</span></span>|<span data-ttu-id="b3d8b-172">String</span><span class="sxs-lookup"><span data-stu-id="b3d8b-172">String</span></span>|<span data-ttu-id="b3d8b-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b3d8b-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3d8b-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3d8b-175">version</span><span class="sxs-lookup"><span data-stu-id="b3d8b-175">version</span></span>|<span data-ttu-id="b3d8b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b3d8b-176">Int32</span></span>|<span data-ttu-id="b3d8b-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-177">Version of the device configuration.</span></span> <span data-ttu-id="b3d8b-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3d8b-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3d8b-179">connectionName</span><span class="sxs-lookup"><span data-stu-id="b3d8b-179">connectionName</span></span>|<span data-ttu-id="b3d8b-180">字符串</span><span class="sxs-lookup"><span data-stu-id="b3d8b-180">String</span></span>|<span data-ttu-id="b3d8b-181">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-181">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="b3d8b-182">connectionType</span><span class="sxs-lookup"><span data-stu-id="b3d8b-182">connectionType</span></span>|[<span data-ttu-id="b3d8b-183">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="b3d8b-183">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="b3d8b-184">连接类型。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-184">Connection type.</span></span> <span data-ttu-id="b3d8b-185">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix` 或 `paloAltoGlobalProtect`。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-185">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="b3d8b-186">role</span><span class="sxs-lookup"><span data-stu-id="b3d8b-186">role</span></span>|<span data-ttu-id="b3d8b-187">字符串</span><span class="sxs-lookup"><span data-stu-id="b3d8b-187">String</span></span>|<span data-ttu-id="b3d8b-188">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-188">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="b3d8b-189">型</span><span class="sxs-lookup"><span data-stu-id="b3d8b-189">realm</span></span>|<span data-ttu-id="b3d8b-190">字符串</span><span class="sxs-lookup"><span data-stu-id="b3d8b-190">String</span></span>|<span data-ttu-id="b3d8b-191">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-191">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="b3d8b-192">台</span><span class="sxs-lookup"><span data-stu-id="b3d8b-192">servers</span></span>|<span data-ttu-id="b3d8b-193">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="b3d8b-193">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="b3d8b-194">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-194">List of VPN Servers on the network.</span></span> <span data-ttu-id="b3d8b-195">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-195">Make sure end users can access these network locations.</span></span> <span data-ttu-id="b3d8b-196">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b3d8b-197">其次</span><span class="sxs-lookup"><span data-stu-id="b3d8b-197">fingerprint</span></span>|<span data-ttu-id="b3d8b-198">字符串</span><span class="sxs-lookup"><span data-stu-id="b3d8b-198">String</span></span>|<span data-ttu-id="b3d8b-199">指纹是一个字符串，用于验证 VPN 服务器是否可以信任，这仅在连接类型为 "检查点胶囊" VPN 时适用。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-199">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="b3d8b-200">customData</span><span class="sxs-lookup"><span data-stu-id="b3d8b-200">customData</span></span>|<span data-ttu-id="b3d8b-201">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b3d8b-201">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="b3d8b-202">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-202">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="b3d8b-203">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-203">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="b3d8b-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="b3d8b-204">customKeyValueData</span></span>|<span data-ttu-id="b3d8b-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b3d8b-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b3d8b-206">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-206">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="b3d8b-207">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-207">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="b3d8b-208">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b3d8b-208">authenticationMethod</span></span>|[<span data-ttu-id="b3d8b-209">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b3d8b-209">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="b3d8b-210">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-210">Authentication method.</span></span> <span data-ttu-id="b3d8b-211">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-211">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="b3d8b-212">响应</span><span class="sxs-lookup"><span data-stu-id="b3d8b-212">Response</span></span>
<span data-ttu-id="b3d8b-213">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-213">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3d8b-214">示例</span><span class="sxs-lookup"><span data-stu-id="b3d8b-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3d8b-215">请求</span><span class="sxs-lookup"><span data-stu-id="b3d8b-215">Request</span></span>
<span data-ttu-id="b3d8b-216">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1762

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
  "authenticationMethod": "usernameAndPassword"
}
```

### <a name="response"></a><span data-ttu-id="b3d8b-217">响应</span><span class="sxs-lookup"><span data-stu-id="b3d8b-217">Response</span></span>
<span data-ttu-id="b3d8b-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b3d8b-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1934

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
  "authenticationMethod": "usernameAndPassword"
}
```





