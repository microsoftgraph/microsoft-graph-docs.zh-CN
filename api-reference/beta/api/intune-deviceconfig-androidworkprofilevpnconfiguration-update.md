---
title: 更新 androidWorkProfileVpnConfiguration
description: 更新 androidWorkProfileVpnConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8f1b70cb5c6599584c812fdfe35a38f633277d00
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49226298"
---
# <a name="update-androidworkprofilevpnconfiguration"></a><span data-ttu-id="ca3f4-103">更新 androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca3f4-103">Update androidWorkProfileVpnConfiguration</span></span>

<span data-ttu-id="ca3f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca3f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca3f4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca3f4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca3f4-107">更新 [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-107">Update the properties of a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca3f4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ca3f4-108">Prerequisites</span></span>
<span data-ttu-id="ca3f4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca3f4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca3f4-111">Permission type</span></span>|<span data-ttu-id="ca3f4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ca3f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca3f4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca3f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca3f4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca3f4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca3f4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca3f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca3f4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-116">Not supported.</span></span>|
|<span data-ttu-id="ca3f4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca3f4-117">Application</span></span>|<span data-ttu-id="ca3f4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca3f4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca3f4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca3f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ca3f4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca3f4-120">Request headers</span></span>
|<span data-ttu-id="ca3f4-121">标头</span><span class="sxs-lookup"><span data-stu-id="ca3f4-121">Header</span></span>|<span data-ttu-id="ca3f4-122">值</span><span class="sxs-lookup"><span data-stu-id="ca3f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca3f4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca3f4-123">Authorization</span></span>|<span data-ttu-id="ca3f4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca3f4-125">接受</span><span class="sxs-lookup"><span data-stu-id="ca3f4-125">Accept</span></span>|<span data-ttu-id="ca3f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca3f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca3f4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca3f4-127">Request body</span></span>
<span data-ttu-id="ca3f4-128">在请求正文中，提供 [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-128">In the request body, supply a JSON representation for the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

<span data-ttu-id="ca3f4-129">下表显示创建 [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-129">The following table shows the properties that are required when you create the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span></span>

|<span data-ttu-id="ca3f4-130">属性</span><span class="sxs-lookup"><span data-stu-id="ca3f4-130">Property</span></span>|<span data-ttu-id="ca3f4-131">类型</span><span class="sxs-lookup"><span data-stu-id="ca3f4-131">Type</span></span>|<span data-ttu-id="ca3f4-132">说明</span><span class="sxs-lookup"><span data-stu-id="ca3f4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca3f4-133">id</span><span class="sxs-lookup"><span data-stu-id="ca3f4-133">id</span></span>|<span data-ttu-id="ca3f4-134">String</span><span class="sxs-lookup"><span data-stu-id="ca3f4-134">String</span></span>|<span data-ttu-id="ca3f4-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-135">Key of the entity.</span></span> <span data-ttu-id="ca3f4-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca3f4-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca3f4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca3f4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ca3f4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca3f4-138">DateTimeOffset</span></span>|<span data-ttu-id="ca3f4-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ca3f4-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca3f4-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca3f4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ca3f4-141">roleScopeTagIds</span></span>|<span data-ttu-id="ca3f4-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="ca3f4-142">String collection</span></span>|<span data-ttu-id="ca3f4-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ca3f4-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca3f4-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca3f4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ca3f4-145">supportsScopeTags</span></span>|<span data-ttu-id="ca3f4-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca3f4-146">Boolean</span></span>|<span data-ttu-id="ca3f4-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ca3f4-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ca3f4-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ca3f4-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-150">This property is read-only.</span></span> <span data-ttu-id="ca3f4-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca3f4-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca3f4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ca3f4-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ca3f4-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ca3f4-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ca3f4-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ca3f4-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca3f4-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca3f4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ca3f4-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ca3f4-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ca3f4-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ca3f4-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ca3f4-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca3f4-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca3f4-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ca3f4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ca3f4-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ca3f4-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ca3f4-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ca3f4-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca3f4-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca3f4-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca3f4-164">createdDateTime</span></span>|<span data-ttu-id="ca3f4-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca3f4-165">DateTimeOffset</span></span>|<span data-ttu-id="ca3f4-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-166">DateTime the object was created.</span></span> <span data-ttu-id="ca3f4-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca3f4-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca3f4-168">description</span><span class="sxs-lookup"><span data-stu-id="ca3f4-168">description</span></span>|<span data-ttu-id="ca3f4-169">String</span><span class="sxs-lookup"><span data-stu-id="ca3f4-169">String</span></span>|<span data-ttu-id="ca3f4-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ca3f4-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca3f4-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca3f4-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ca3f4-172">displayName</span></span>|<span data-ttu-id="ca3f4-173">String</span><span class="sxs-lookup"><span data-stu-id="ca3f4-173">String</span></span>|<span data-ttu-id="ca3f4-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ca3f4-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca3f4-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca3f4-176">version</span><span class="sxs-lookup"><span data-stu-id="ca3f4-176">version</span></span>|<span data-ttu-id="ca3f4-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ca3f4-177">Int32</span></span>|<span data-ttu-id="ca3f4-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-178">Version of the device configuration.</span></span> <span data-ttu-id="ca3f4-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca3f4-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca3f4-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="ca3f4-180">connectionName</span></span>|<span data-ttu-id="ca3f4-181">String</span><span class="sxs-lookup"><span data-stu-id="ca3f4-181">String</span></span>|<span data-ttu-id="ca3f4-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-182">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="ca3f4-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="ca3f4-183">connectionType</span></span>|[<span data-ttu-id="ca3f4-184">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="ca3f4-184">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="ca3f4-185">连接类型。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-185">Connection type.</span></span> <span data-ttu-id="ca3f4-186">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`、`paloAltoGlobalProtect`、`microsoftTunnel`、`netMotionMobility`。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-186">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="ca3f4-187">role</span><span class="sxs-lookup"><span data-stu-id="ca3f4-187">role</span></span>|<span data-ttu-id="ca3f4-188">String</span><span class="sxs-lookup"><span data-stu-id="ca3f4-188">String</span></span>|<span data-ttu-id="ca3f4-189">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-189">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="ca3f4-190">型</span><span class="sxs-lookup"><span data-stu-id="ca3f4-190">realm</span></span>|<span data-ttu-id="ca3f4-191">String</span><span class="sxs-lookup"><span data-stu-id="ca3f4-191">String</span></span>|<span data-ttu-id="ca3f4-192">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-192">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="ca3f4-193">台</span><span class="sxs-lookup"><span data-stu-id="ca3f4-193">servers</span></span>|<span data-ttu-id="ca3f4-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ca3f4-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="ca3f4-195">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-195">List of VPN Servers on the network.</span></span> <span data-ttu-id="ca3f4-196">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-196">Make sure end users can access these network locations.</span></span> <span data-ttu-id="ca3f4-197">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ca3f4-198">其次</span><span class="sxs-lookup"><span data-stu-id="ca3f4-198">fingerprint</span></span>|<span data-ttu-id="ca3f4-199">String</span><span class="sxs-lookup"><span data-stu-id="ca3f4-199">String</span></span>|<span data-ttu-id="ca3f4-200">指纹是一个字符串，用于验证 VPN 服务器是否可以信任，这仅在连接类型为 "检查点胶囊" VPN 时适用。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-200">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="ca3f4-201">customData</span><span class="sxs-lookup"><span data-stu-id="ca3f4-201">customData</span></span>|<span data-ttu-id="ca3f4-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ca3f4-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="ca3f4-203">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-203">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="ca3f4-204">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="ca3f4-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="ca3f4-205">customKeyValueData</span></span>|<span data-ttu-id="ca3f4-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ca3f4-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ca3f4-207">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-207">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="ca3f4-208">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-208">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="ca3f4-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ca3f4-209">authenticationMethod</span></span>|[<span data-ttu-id="ca3f4-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ca3f4-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="ca3f4-211">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-211">Authentication method.</span></span> <span data-ttu-id="ca3f4-212">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="ca3f4-213">proxyServer</span><span class="sxs-lookup"><span data-stu-id="ca3f4-213">proxyServer</span></span>|[<span data-ttu-id="ca3f4-214">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="ca3f4-214">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="ca3f4-215">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-215">Proxy server.</span></span>|
|<span data-ttu-id="ca3f4-216">targetedPackageIds</span><span class="sxs-lookup"><span data-stu-id="ca3f4-216">targetedPackageIds</span></span>|<span data-ttu-id="ca3f4-217">String 集合</span><span class="sxs-lookup"><span data-stu-id="ca3f4-217">String collection</span></span>|<span data-ttu-id="ca3f4-218">目标应用程序包 Id。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-218">Targeted App package IDs.</span></span>|
|<span data-ttu-id="ca3f4-219">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="ca3f4-219">targetedMobileApps</span></span>|<span data-ttu-id="ca3f4-220">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ca3f4-220">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ca3f4-221">目标移动应用。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-221">Targeted mobile apps.</span></span> <span data-ttu-id="ca3f4-222">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-222">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ca3f4-223">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="ca3f4-223">alwaysOn</span></span>|<span data-ttu-id="ca3f4-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca3f4-224">Boolean</span></span>|<span data-ttu-id="ca3f4-225">是否启用始终启用的 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-225">Whether or not to enable always-on VPN connection.</span></span>|
|<span data-ttu-id="ca3f4-226">alwaysOnLockdown</span><span class="sxs-lookup"><span data-stu-id="ca3f4-226">alwaysOnLockdown</span></span>|<span data-ttu-id="ca3f4-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca3f4-227">Boolean</span></span>|<span data-ttu-id="ca3f4-228">如果启用了 always on VPN 连接，则在断开 VPN 连接时是否锁定网络流量。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-228">If always-on VPN connection is enabled, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="ca3f4-229">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="ca3f4-229">microsoftTunnelSiteId</span></span>|<span data-ttu-id="ca3f4-230">String</span><span class="sxs-lookup"><span data-stu-id="ca3f4-230">String</span></span>|<span data-ttu-id="ca3f4-231">Microsoft 隧道站点 ID。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-231">Microsoft Tunnel site ID.</span></span>|



## <a name="response"></a><span data-ttu-id="ca3f4-232">响应</span><span class="sxs-lookup"><span data-stu-id="ca3f4-232">Response</span></span>
<span data-ttu-id="ca3f4-233">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-233">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca3f4-234">示例</span><span class="sxs-lookup"><span data-stu-id="ca3f4-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca3f4-235">请求</span><span class="sxs-lookup"><span data-stu-id="ca3f4-235">Request</span></span>
<span data-ttu-id="ca3f4-236">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2422

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
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "alwaysOn": true,
  "alwaysOnLockdown": true,
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```

### <a name="response"></a><span data-ttu-id="ca3f4-237">响应</span><span class="sxs-lookup"><span data-stu-id="ca3f4-237">Response</span></span>
<span data-ttu-id="ca3f4-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca3f4-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2594

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
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "alwaysOn": true,
  "alwaysOnLockdown": true,
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```




