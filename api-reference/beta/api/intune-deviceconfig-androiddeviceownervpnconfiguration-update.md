---
title: 更新 androidDeviceOwnerVpnConfiguration
description: 更新 androidDeviceOwnerVpnConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ad72d3d23f2fd02aac31f1d1875cd87458504c42
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436042"
---
# <a name="update-androiddeviceownervpnconfiguration"></a><span data-ttu-id="ed377-103">更新 androidDeviceOwnerVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ed377-103">Update androidDeviceOwnerVpnConfiguration</span></span>

<span data-ttu-id="ed377-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed377-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed377-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ed377-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed377-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ed377-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed377-107">更新[androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ed377-107">Update the properties of a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed377-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ed377-108">Prerequisites</span></span>
<span data-ttu-id="ed377-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed377-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed377-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed377-111">Permission type</span></span>|<span data-ttu-id="ed377-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ed377-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed377-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed377-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed377-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed377-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ed377-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed377-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed377-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed377-116">Not supported.</span></span>|
|<span data-ttu-id="ed377-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed377-117">Application</span></span>|<span data-ttu-id="ed377-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed377-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed377-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed377-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ed377-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed377-120">Request headers</span></span>
|<span data-ttu-id="ed377-121">标头</span><span class="sxs-lookup"><span data-stu-id="ed377-121">Header</span></span>|<span data-ttu-id="ed377-122">值</span><span class="sxs-lookup"><span data-stu-id="ed377-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed377-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed377-123">Authorization</span></span>|<span data-ttu-id="ed377-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ed377-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed377-125">接受</span><span class="sxs-lookup"><span data-stu-id="ed377-125">Accept</span></span>|<span data-ttu-id="ed377-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed377-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed377-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed377-127">Request body</span></span>
<span data-ttu-id="ed377-128">在请求正文中，提供[androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed377-128">In the request body, supply a JSON representation for the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

<span data-ttu-id="ed377-129">下表显示创建[androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ed377-129">The following table shows the properties that are required when you create the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md).</span></span>

|<span data-ttu-id="ed377-130">属性</span><span class="sxs-lookup"><span data-stu-id="ed377-130">Property</span></span>|<span data-ttu-id="ed377-131">类型</span><span class="sxs-lookup"><span data-stu-id="ed377-131">Type</span></span>|<span data-ttu-id="ed377-132">说明</span><span class="sxs-lookup"><span data-stu-id="ed377-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed377-133">id</span><span class="sxs-lookup"><span data-stu-id="ed377-133">id</span></span>|<span data-ttu-id="ed377-134">字符串</span><span class="sxs-lookup"><span data-stu-id="ed377-134">String</span></span>|<span data-ttu-id="ed377-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ed377-135">Key of the entity.</span></span> <span data-ttu-id="ed377-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed377-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed377-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed377-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ed377-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed377-138">DateTimeOffset</span></span>|<span data-ttu-id="ed377-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ed377-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ed377-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed377-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed377-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ed377-141">roleScopeTagIds</span></span>|<span data-ttu-id="ed377-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="ed377-142">String collection</span></span>|<span data-ttu-id="ed377-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ed377-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ed377-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed377-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed377-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ed377-145">supportsScopeTags</span></span>|<span data-ttu-id="ed377-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed377-146">Boolean</span></span>|<span data-ttu-id="ed377-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="ed377-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ed377-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="ed377-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ed377-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="ed377-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ed377-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ed377-150">This property is read-only.</span></span> <span data-ttu-id="ed377-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed377-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed377-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ed377-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ed377-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ed377-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ed377-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="ed377-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ed377-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed377-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed377-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ed377-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ed377-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ed377-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ed377-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ed377-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ed377-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed377-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed377-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ed377-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ed377-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ed377-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ed377-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ed377-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ed377-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed377-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed377-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed377-164">createdDateTime</span></span>|<span data-ttu-id="ed377-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed377-165">DateTimeOffset</span></span>|<span data-ttu-id="ed377-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ed377-166">DateTime the object was created.</span></span> <span data-ttu-id="ed377-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed377-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed377-168">description</span><span class="sxs-lookup"><span data-stu-id="ed377-168">description</span></span>|<span data-ttu-id="ed377-169">String</span><span class="sxs-lookup"><span data-stu-id="ed377-169">String</span></span>|<span data-ttu-id="ed377-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ed377-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ed377-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed377-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed377-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ed377-172">displayName</span></span>|<span data-ttu-id="ed377-173">String</span><span class="sxs-lookup"><span data-stu-id="ed377-173">String</span></span>|<span data-ttu-id="ed377-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ed377-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ed377-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed377-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed377-176">version</span><span class="sxs-lookup"><span data-stu-id="ed377-176">version</span></span>|<span data-ttu-id="ed377-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ed377-177">Int32</span></span>|<span data-ttu-id="ed377-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ed377-178">Version of the device configuration.</span></span> <span data-ttu-id="ed377-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed377-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed377-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ed377-180">authenticationMethod</span></span>|[<span data-ttu-id="ed377-181">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ed377-181">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="ed377-182">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="ed377-182">Authentication method.</span></span> <span data-ttu-id="ed377-183">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="ed377-183">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="ed377-184">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="ed377-184">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="ed377-185">connectionName</span><span class="sxs-lookup"><span data-stu-id="ed377-185">connectionName</span></span>|<span data-ttu-id="ed377-186">String</span><span class="sxs-lookup"><span data-stu-id="ed377-186">String</span></span>|<span data-ttu-id="ed377-187">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="ed377-187">Connection name displayed to the user.</span></span> <span data-ttu-id="ed377-188">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed377-188">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="ed377-189">role</span><span class="sxs-lookup"><span data-stu-id="ed377-189">role</span></span>|<span data-ttu-id="ed377-190">String</span><span class="sxs-lookup"><span data-stu-id="ed377-190">String</span></span>|<span data-ttu-id="ed377-191">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="ed377-191">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="ed377-192">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed377-192">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="ed377-193">型</span><span class="sxs-lookup"><span data-stu-id="ed377-193">realm</span></span>|<span data-ttu-id="ed377-194">String</span><span class="sxs-lookup"><span data-stu-id="ed377-194">String</span></span>|<span data-ttu-id="ed377-195">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="ed377-195">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="ed377-196">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed377-196">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="ed377-197">台</span><span class="sxs-lookup"><span data-stu-id="ed377-197">servers</span></span>|<span data-ttu-id="ed377-198">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="ed377-198">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="ed377-199">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="ed377-199">List of VPN Servers on the network.</span></span> <span data-ttu-id="ed377-200">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="ed377-200">Make sure end users can access these network locations.</span></span> <span data-ttu-id="ed377-201">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="ed377-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ed377-202">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed377-202">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="ed377-203">connectionType</span><span class="sxs-lookup"><span data-stu-id="ed377-203">connectionType</span></span>|[<span data-ttu-id="ed377-204">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="ed377-204">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="ed377-205">连接类型。</span><span class="sxs-lookup"><span data-stu-id="ed377-205">Connection type.</span></span> <span data-ttu-id="ed377-206">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`。</span><span class="sxs-lookup"><span data-stu-id="ed377-206">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|



## <a name="response"></a><span data-ttu-id="ed377-207">响应</span><span class="sxs-lookup"><span data-stu-id="ed377-207">Response</span></span>
<span data-ttu-id="ed377-208">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ed377-208">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed377-209">示例</span><span class="sxs-lookup"><span data-stu-id="ed377-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed377-210">请求</span><span class="sxs-lookup"><span data-stu-id="ed377-210">Request</span></span>
<span data-ttu-id="ed377-211">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ed377-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1417

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerVpnConfiguration",
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
  "authenticationMethod": "usernameAndPassword",
  "connectionName": "Connection Name value",
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
  "connectionType": "pulseSecure"
}
```

### <a name="response"></a><span data-ttu-id="ed377-212">响应</span><span class="sxs-lookup"><span data-stu-id="ed377-212">Response</span></span>
<span data-ttu-id="ed377-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ed377-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1589

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerVpnConfiguration",
  "id": "972962e3-62e3-9729-e362-2997e3622997",
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
  "authenticationMethod": "usernameAndPassword",
  "connectionName": "Connection Name value",
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
  "connectionType": "pulseSecure"
}
```



