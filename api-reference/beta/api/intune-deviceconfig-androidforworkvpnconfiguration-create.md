---
title: 创建 androidForWorkVpnConfiguration
description: 创建新的 androidForWorkVpnConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5b7e427988918e7e1c68af57cb702d85ae522715
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123279"
---
# <a name="create-androidforworkvpnconfiguration"></a><span data-ttu-id="b5533-103">创建 androidForWorkVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b5533-103">Create androidForWorkVpnConfiguration</span></span>

<span data-ttu-id="b5533-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5533-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5533-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b5533-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5533-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5533-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5533-107">创建新的[androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b5533-107">Create a new [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5533-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b5533-108">Prerequisites</span></span>
<span data-ttu-id="b5533-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b5533-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b5533-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5533-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5533-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5533-111">Permission type</span></span>|<span data-ttu-id="b5533-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b5533-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5533-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5533-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5533-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5533-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b5533-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5533-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5533-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5533-116">Not supported.</span></span>|
|<span data-ttu-id="b5533-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5533-117">Application</span></span>|<span data-ttu-id="b5533-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5533-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5533-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5533-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b5533-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5533-120">Request headers</span></span>
|<span data-ttu-id="b5533-121">标头</span><span class="sxs-lookup"><span data-stu-id="b5533-121">Header</span></span>|<span data-ttu-id="b5533-122">值</span><span class="sxs-lookup"><span data-stu-id="b5533-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5533-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5533-123">Authorization</span></span>|<span data-ttu-id="b5533-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b5533-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5533-125">接受</span><span class="sxs-lookup"><span data-stu-id="b5533-125">Accept</span></span>|<span data-ttu-id="b5533-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b5533-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5533-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5533-127">Request body</span></span>
<span data-ttu-id="b5533-128">在请求正文中，提供 androidForWorkVpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5533-128">In the request body, supply a JSON representation for the androidForWorkVpnConfiguration object.</span></span>

<span data-ttu-id="b5533-129">下表显示创建 androidForWorkVpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b5533-129">The following table shows the properties that are required when you create the androidForWorkVpnConfiguration.</span></span>

|<span data-ttu-id="b5533-130">属性</span><span class="sxs-lookup"><span data-stu-id="b5533-130">Property</span></span>|<span data-ttu-id="b5533-131">类型</span><span class="sxs-lookup"><span data-stu-id="b5533-131">Type</span></span>|<span data-ttu-id="b5533-132">说明</span><span class="sxs-lookup"><span data-stu-id="b5533-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5533-133">id</span><span class="sxs-lookup"><span data-stu-id="b5533-133">id</span></span>|<span data-ttu-id="b5533-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b5533-134">String</span></span>|<span data-ttu-id="b5533-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b5533-135">Key of the entity.</span></span> <span data-ttu-id="b5533-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5533-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5533-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5533-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b5533-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5533-138">DateTimeOffset</span></span>|<span data-ttu-id="b5533-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b5533-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b5533-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5533-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5533-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b5533-141">roleScopeTagIds</span></span>|<span data-ttu-id="b5533-142">String collection</span><span class="sxs-lookup"><span data-stu-id="b5533-142">String collection</span></span>|<span data-ttu-id="b5533-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b5533-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b5533-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5533-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5533-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b5533-145">supportsScopeTags</span></span>|<span data-ttu-id="b5533-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5533-146">Boolean</span></span>|<span data-ttu-id="b5533-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="b5533-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b5533-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="b5533-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b5533-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="b5533-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b5533-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b5533-150">This property is read-only.</span></span> <span data-ttu-id="b5533-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5533-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5533-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b5533-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b5533-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b5533-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b5533-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="b5533-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b5533-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5533-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5533-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b5533-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b5533-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b5533-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b5533-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b5533-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b5533-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5533-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5533-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b5533-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b5533-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b5533-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b5533-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b5533-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b5533-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5533-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5533-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b5533-164">createdDateTime</span></span>|<span data-ttu-id="b5533-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5533-165">DateTimeOffset</span></span>|<span data-ttu-id="b5533-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b5533-166">DateTime the object was created.</span></span> <span data-ttu-id="b5533-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5533-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5533-168">说明</span><span class="sxs-lookup"><span data-stu-id="b5533-168">description</span></span>|<span data-ttu-id="b5533-169">String</span><span class="sxs-lookup"><span data-stu-id="b5533-169">String</span></span>|<span data-ttu-id="b5533-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b5533-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b5533-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5533-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5533-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b5533-172">displayName</span></span>|<span data-ttu-id="b5533-173">String</span><span class="sxs-lookup"><span data-stu-id="b5533-173">String</span></span>|<span data-ttu-id="b5533-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b5533-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b5533-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5533-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5533-176">version</span><span class="sxs-lookup"><span data-stu-id="b5533-176">version</span></span>|<span data-ttu-id="b5533-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b5533-177">Int32</span></span>|<span data-ttu-id="b5533-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b5533-178">Version of the device configuration.</span></span> <span data-ttu-id="b5533-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5533-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5533-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="b5533-180">connectionName</span></span>|<span data-ttu-id="b5533-181">String</span><span class="sxs-lookup"><span data-stu-id="b5533-181">String</span></span>|<span data-ttu-id="b5533-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="b5533-182">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="b5533-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="b5533-183">connectionType</span></span>|[<span data-ttu-id="b5533-184">androidForWorkVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="b5533-184">androidForWorkVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidforworkvpnconnectiontype.md)|<span data-ttu-id="b5533-185">连接类型。</span><span class="sxs-lookup"><span data-stu-id="b5533-185">Connection type.</span></span> <span data-ttu-id="b5533-186">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`。</span><span class="sxs-lookup"><span data-stu-id="b5533-186">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="b5533-187">role</span><span class="sxs-lookup"><span data-stu-id="b5533-187">role</span></span>|<span data-ttu-id="b5533-188">String</span><span class="sxs-lookup"><span data-stu-id="b5533-188">String</span></span>|<span data-ttu-id="b5533-189">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="b5533-189">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="b5533-190">型</span><span class="sxs-lookup"><span data-stu-id="b5533-190">realm</span></span>|<span data-ttu-id="b5533-191">String</span><span class="sxs-lookup"><span data-stu-id="b5533-191">String</span></span>|<span data-ttu-id="b5533-192">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="b5533-192">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="b5533-193">台</span><span class="sxs-lookup"><span data-stu-id="b5533-193">servers</span></span>|<span data-ttu-id="b5533-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="b5533-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="b5533-195">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="b5533-195">List of VPN Servers on the network.</span></span> <span data-ttu-id="b5533-196">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="b5533-196">Make sure end users can access these network locations.</span></span> <span data-ttu-id="b5533-197">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="b5533-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b5533-198">其次</span><span class="sxs-lookup"><span data-stu-id="b5533-198">fingerprint</span></span>|<span data-ttu-id="b5533-199">String</span><span class="sxs-lookup"><span data-stu-id="b5533-199">String</span></span>|<span data-ttu-id="b5533-200">指纹是一个字符串，用于验证 VPN 服务器是否可以信任，这仅在连接类型为 "检查点胶囊" VPN 时适用。</span><span class="sxs-lookup"><span data-stu-id="b5533-200">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="b5533-201">customData</span><span class="sxs-lookup"><span data-stu-id="b5533-201">customData</span></span>|<span data-ttu-id="b5533-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b5533-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="b5533-203">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="b5533-203">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="b5533-204">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="b5533-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="b5533-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="b5533-205">customKeyValueData</span></span>|<span data-ttu-id="b5533-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b5533-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b5533-207">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="b5533-207">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="b5533-208">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="b5533-208">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="b5533-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b5533-209">authenticationMethod</span></span>|[<span data-ttu-id="b5533-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b5533-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="b5533-211">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="b5533-211">Authentication method.</span></span> <span data-ttu-id="b5533-212">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="b5533-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|



## <a name="response"></a><span data-ttu-id="b5533-213">响应</span><span class="sxs-lookup"><span data-stu-id="b5533-213">Response</span></span>
<span data-ttu-id="b5533-214">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b5533-214">If successful, this method returns a `201 Created` response code and a [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5533-215">示例</span><span class="sxs-lookup"><span data-stu-id="b5533-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5533-216">请求</span><span class="sxs-lookup"><span data-stu-id="b5533-216">Request</span></span>
<span data-ttu-id="b5533-217">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5533-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1758

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="b5533-218">响应</span><span class="sxs-lookup"><span data-stu-id="b5533-218">Response</span></span>
<span data-ttu-id="b5533-219">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="b5533-219">Here is an example of the response.</span></span> <span data-ttu-id="b5533-220">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="b5533-220">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b5533-221">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b5533-221">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1930

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
  "id": "2cf4c52c-c52c-2cf4-2cc5-f42c2cc5f42c",
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



