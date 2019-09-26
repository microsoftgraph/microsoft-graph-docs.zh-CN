---
title: 创建 androidWorkProfileVpnConfiguration
description: 创建新的 androidWorkProfileVpnConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 41993fd59bdff17dbf61c37847a39162cba0d92d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37175650"
---
# <a name="create-androidworkprofilevpnconfiguration"></a><span data-ttu-id="34b7e-103">创建 androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="34b7e-103">Create androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="34b7e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="34b7e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34b7e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34b7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34b7e-106">创建新的[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="34b7e-106">Create a new [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34b7e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="34b7e-107">Prerequisites</span></span>
<span data-ttu-id="34b7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="34b7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34b7e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="34b7e-110">Permission type</span></span>|<span data-ttu-id="34b7e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="34b7e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34b7e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34b7e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34b7e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34b7e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34b7e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34b7e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34b7e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="34b7e-115">Not supported.</span></span>|
|<span data-ttu-id="34b7e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="34b7e-116">Application</span></span>|<span data-ttu-id="34b7e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34b7e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34b7e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34b7e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="34b7e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="34b7e-119">Request headers</span></span>
|<span data-ttu-id="34b7e-120">标头</span><span class="sxs-lookup"><span data-stu-id="34b7e-120">Header</span></span>|<span data-ttu-id="34b7e-121">值</span><span class="sxs-lookup"><span data-stu-id="34b7e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34b7e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="34b7e-122">Authorization</span></span>|<span data-ttu-id="34b7e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="34b7e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34b7e-124">接受</span><span class="sxs-lookup"><span data-stu-id="34b7e-124">Accept</span></span>|<span data-ttu-id="34b7e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34b7e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34b7e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="34b7e-126">Request body</span></span>
<span data-ttu-id="34b7e-127">在请求正文中，提供 androidWorkProfileVpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34b7e-127">In the request body, supply a JSON representation for the androidWorkProfileVpnConfiguration object.</span></span>

<span data-ttu-id="34b7e-128">下表显示创建 androidWorkProfileVpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="34b7e-128">The following table shows the properties that are required when you create the androidWorkProfileVpnConfiguration.</span></span>

|<span data-ttu-id="34b7e-129">属性</span><span class="sxs-lookup"><span data-stu-id="34b7e-129">Property</span></span>|<span data-ttu-id="34b7e-130">类型</span><span class="sxs-lookup"><span data-stu-id="34b7e-130">Type</span></span>|<span data-ttu-id="34b7e-131">说明</span><span class="sxs-lookup"><span data-stu-id="34b7e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34b7e-132">id</span><span class="sxs-lookup"><span data-stu-id="34b7e-132">id</span></span>|<span data-ttu-id="34b7e-133">字符串</span><span class="sxs-lookup"><span data-stu-id="34b7e-133">String</span></span>|<span data-ttu-id="34b7e-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="34b7e-134">Key of the entity.</span></span> <span data-ttu-id="34b7e-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34b7e-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34b7e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34b7e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="34b7e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34b7e-137">DateTimeOffset</span></span>|<span data-ttu-id="34b7e-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="34b7e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="34b7e-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34b7e-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34b7e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="34b7e-140">roleScopeTagIds</span></span>|<span data-ttu-id="34b7e-141">String collection</span><span class="sxs-lookup"><span data-stu-id="34b7e-141">String collection</span></span>|<span data-ttu-id="34b7e-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="34b7e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="34b7e-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34b7e-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34b7e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="34b7e-144">supportsScopeTags</span></span>|<span data-ttu-id="34b7e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="34b7e-145">Boolean</span></span>|<span data-ttu-id="34b7e-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="34b7e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="34b7e-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="34b7e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="34b7e-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="34b7e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="34b7e-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="34b7e-149">This property is read-only.</span></span> <span data-ttu-id="34b7e-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34b7e-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34b7e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="34b7e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="34b7e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="34b7e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="34b7e-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="34b7e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="34b7e-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34b7e-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34b7e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="34b7e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="34b7e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="34b7e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="34b7e-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="34b7e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="34b7e-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34b7e-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34b7e-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="34b7e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="34b7e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="34b7e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="34b7e-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="34b7e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="34b7e-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34b7e-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34b7e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34b7e-163">createdDateTime</span></span>|<span data-ttu-id="34b7e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34b7e-164">DateTimeOffset</span></span>|<span data-ttu-id="34b7e-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="34b7e-165">DateTime the object was created.</span></span> <span data-ttu-id="34b7e-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34b7e-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34b7e-167">说明</span><span class="sxs-lookup"><span data-stu-id="34b7e-167">description</span></span>|<span data-ttu-id="34b7e-168">String</span><span class="sxs-lookup"><span data-stu-id="34b7e-168">String</span></span>|<span data-ttu-id="34b7e-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="34b7e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="34b7e-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34b7e-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34b7e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="34b7e-171">displayName</span></span>|<span data-ttu-id="34b7e-172">String</span><span class="sxs-lookup"><span data-stu-id="34b7e-172">String</span></span>|<span data-ttu-id="34b7e-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="34b7e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="34b7e-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34b7e-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34b7e-175">version</span><span class="sxs-lookup"><span data-stu-id="34b7e-175">version</span></span>|<span data-ttu-id="34b7e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="34b7e-176">Int32</span></span>|<span data-ttu-id="34b7e-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="34b7e-177">Version of the device configuration.</span></span> <span data-ttu-id="34b7e-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34b7e-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34b7e-179">connectionName</span><span class="sxs-lookup"><span data-stu-id="34b7e-179">connectionName</span></span>|<span data-ttu-id="34b7e-180">String</span><span class="sxs-lookup"><span data-stu-id="34b7e-180">String</span></span>|<span data-ttu-id="34b7e-181">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="34b7e-181">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="34b7e-182">connectionType</span><span class="sxs-lookup"><span data-stu-id="34b7e-182">connectionType</span></span>|[<span data-ttu-id="34b7e-183">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="34b7e-183">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="34b7e-184">连接类型。</span><span class="sxs-lookup"><span data-stu-id="34b7e-184">Connection type.</span></span> <span data-ttu-id="34b7e-185">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix` 或 `paloAltoGlobalProtect`。</span><span class="sxs-lookup"><span data-stu-id="34b7e-185">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="34b7e-186">role</span><span class="sxs-lookup"><span data-stu-id="34b7e-186">role</span></span>|<span data-ttu-id="34b7e-187">String</span><span class="sxs-lookup"><span data-stu-id="34b7e-187">String</span></span>|<span data-ttu-id="34b7e-188">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="34b7e-188">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="34b7e-189">型</span><span class="sxs-lookup"><span data-stu-id="34b7e-189">realm</span></span>|<span data-ttu-id="34b7e-190">String</span><span class="sxs-lookup"><span data-stu-id="34b7e-190">String</span></span>|<span data-ttu-id="34b7e-191">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="34b7e-191">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="34b7e-192">台</span><span class="sxs-lookup"><span data-stu-id="34b7e-192">servers</span></span>|<span data-ttu-id="34b7e-193">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="34b7e-193">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="34b7e-194">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="34b7e-194">List of VPN Servers on the network.</span></span> <span data-ttu-id="34b7e-195">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="34b7e-195">Make sure end users can access these network locations.</span></span> <span data-ttu-id="34b7e-196">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="34b7e-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="34b7e-197">其次</span><span class="sxs-lookup"><span data-stu-id="34b7e-197">fingerprint</span></span>|<span data-ttu-id="34b7e-198">String</span><span class="sxs-lookup"><span data-stu-id="34b7e-198">String</span></span>|<span data-ttu-id="34b7e-199">指纹是一个字符串，用于验证 VPN 服务器是否可以信任，这仅在连接类型为 "检查点胶囊" VPN 时适用。</span><span class="sxs-lookup"><span data-stu-id="34b7e-199">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="34b7e-200">customData</span><span class="sxs-lookup"><span data-stu-id="34b7e-200">customData</span></span>|<span data-ttu-id="34b7e-201">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="34b7e-201">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="34b7e-202">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="34b7e-202">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="34b7e-203">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="34b7e-203">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="34b7e-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="34b7e-204">customKeyValueData</span></span>|<span data-ttu-id="34b7e-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="34b7e-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="34b7e-206">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="34b7e-206">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="34b7e-207">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="34b7e-207">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="34b7e-208">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="34b7e-208">authenticationMethod</span></span>|[<span data-ttu-id="34b7e-209">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="34b7e-209">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="34b7e-210">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="34b7e-210">Authentication method.</span></span> <span data-ttu-id="34b7e-211">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="34b7e-211">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="34b7e-212">响应</span><span class="sxs-lookup"><span data-stu-id="34b7e-212">Response</span></span>
<span data-ttu-id="34b7e-213">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="34b7e-213">If successful, this method returns a `201 Created` response code and a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34b7e-214">示例</span><span class="sxs-lookup"><span data-stu-id="34b7e-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="34b7e-215">请求</span><span class="sxs-lookup"><span data-stu-id="34b7e-215">Request</span></span>
<span data-ttu-id="34b7e-216">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="34b7e-216">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="34b7e-217">响应</span><span class="sxs-lookup"><span data-stu-id="34b7e-217">Response</span></span>
<span data-ttu-id="34b7e-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="34b7e-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




