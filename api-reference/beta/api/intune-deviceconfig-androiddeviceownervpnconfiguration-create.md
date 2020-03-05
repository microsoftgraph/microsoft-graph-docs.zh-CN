---
title: 创建 androidDeviceOwnerVpnConfiguration
description: 创建新的 androidDeviceOwnerVpnConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4a228ec6999b532190dfa636720356a0a9e7802c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444089"
---
# <a name="create-androiddeviceownervpnconfiguration"></a><span data-ttu-id="534bd-103">创建 androidDeviceOwnerVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="534bd-103">Create androidDeviceOwnerVpnConfiguration</span></span>

<span data-ttu-id="534bd-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="534bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="534bd-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="534bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="534bd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="534bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="534bd-107">创建新的[androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="534bd-107">Create a new [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="534bd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="534bd-108">Prerequisites</span></span>
<span data-ttu-id="534bd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="534bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="534bd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="534bd-111">Permission type</span></span>|<span data-ttu-id="534bd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="534bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="534bd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="534bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="534bd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="534bd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="534bd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="534bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="534bd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="534bd-116">Not supported.</span></span>|
|<span data-ttu-id="534bd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="534bd-117">Application</span></span>|<span data-ttu-id="534bd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="534bd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="534bd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="534bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="534bd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="534bd-120">Request headers</span></span>
|<span data-ttu-id="534bd-121">标头</span><span class="sxs-lookup"><span data-stu-id="534bd-121">Header</span></span>|<span data-ttu-id="534bd-122">值</span><span class="sxs-lookup"><span data-stu-id="534bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="534bd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="534bd-123">Authorization</span></span>|<span data-ttu-id="534bd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="534bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="534bd-125">接受</span><span class="sxs-lookup"><span data-stu-id="534bd-125">Accept</span></span>|<span data-ttu-id="534bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="534bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="534bd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="534bd-127">Request body</span></span>
<span data-ttu-id="534bd-128">在请求正文中，提供 androidDeviceOwnerVpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="534bd-128">In the request body, supply a JSON representation for the androidDeviceOwnerVpnConfiguration object.</span></span>

<span data-ttu-id="534bd-129">下表显示创建 androidDeviceOwnerVpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="534bd-129">The following table shows the properties that are required when you create the androidDeviceOwnerVpnConfiguration.</span></span>

|<span data-ttu-id="534bd-130">属性</span><span class="sxs-lookup"><span data-stu-id="534bd-130">Property</span></span>|<span data-ttu-id="534bd-131">类型</span><span class="sxs-lookup"><span data-stu-id="534bd-131">Type</span></span>|<span data-ttu-id="534bd-132">说明</span><span class="sxs-lookup"><span data-stu-id="534bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="534bd-133">id</span><span class="sxs-lookup"><span data-stu-id="534bd-133">id</span></span>|<span data-ttu-id="534bd-134">字符串</span><span class="sxs-lookup"><span data-stu-id="534bd-134">String</span></span>|<span data-ttu-id="534bd-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="534bd-135">Key of the entity.</span></span> <span data-ttu-id="534bd-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="534bd-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="534bd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="534bd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="534bd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="534bd-138">DateTimeOffset</span></span>|<span data-ttu-id="534bd-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="534bd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="534bd-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="534bd-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="534bd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="534bd-141">roleScopeTagIds</span></span>|<span data-ttu-id="534bd-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="534bd-142">String collection</span></span>|<span data-ttu-id="534bd-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="534bd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="534bd-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="534bd-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="534bd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="534bd-145">supportsScopeTags</span></span>|<span data-ttu-id="534bd-146">布尔</span><span class="sxs-lookup"><span data-stu-id="534bd-146">Boolean</span></span>|<span data-ttu-id="534bd-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="534bd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="534bd-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="534bd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="534bd-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="534bd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="534bd-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="534bd-150">This property is read-only.</span></span> <span data-ttu-id="534bd-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="534bd-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="534bd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="534bd-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="534bd-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="534bd-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="534bd-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="534bd-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="534bd-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="534bd-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="534bd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="534bd-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="534bd-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="534bd-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="534bd-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="534bd-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="534bd-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="534bd-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="534bd-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="534bd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="534bd-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="534bd-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="534bd-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="534bd-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="534bd-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="534bd-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="534bd-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="534bd-164">createdDateTime</span></span>|<span data-ttu-id="534bd-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="534bd-165">DateTimeOffset</span></span>|<span data-ttu-id="534bd-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="534bd-166">DateTime the object was created.</span></span> <span data-ttu-id="534bd-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="534bd-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="534bd-168">说明</span><span class="sxs-lookup"><span data-stu-id="534bd-168">description</span></span>|<span data-ttu-id="534bd-169">String</span><span class="sxs-lookup"><span data-stu-id="534bd-169">String</span></span>|<span data-ttu-id="534bd-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="534bd-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="534bd-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="534bd-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="534bd-172">displayName</span><span class="sxs-lookup"><span data-stu-id="534bd-172">displayName</span></span>|<span data-ttu-id="534bd-173">String</span><span class="sxs-lookup"><span data-stu-id="534bd-173">String</span></span>|<span data-ttu-id="534bd-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="534bd-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="534bd-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="534bd-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="534bd-176">version</span><span class="sxs-lookup"><span data-stu-id="534bd-176">version</span></span>|<span data-ttu-id="534bd-177">Int32</span><span class="sxs-lookup"><span data-stu-id="534bd-177">Int32</span></span>|<span data-ttu-id="534bd-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="534bd-178">Version of the device configuration.</span></span> <span data-ttu-id="534bd-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="534bd-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="534bd-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="534bd-180">authenticationMethod</span></span>|[<span data-ttu-id="534bd-181">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="534bd-181">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="534bd-182">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="534bd-182">Authentication method.</span></span> <span data-ttu-id="534bd-183">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="534bd-183">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="534bd-184">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="534bd-184">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="534bd-185">connectionName</span><span class="sxs-lookup"><span data-stu-id="534bd-185">connectionName</span></span>|<span data-ttu-id="534bd-186">String</span><span class="sxs-lookup"><span data-stu-id="534bd-186">String</span></span>|<span data-ttu-id="534bd-187">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="534bd-187">Connection name displayed to the user.</span></span> <span data-ttu-id="534bd-188">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="534bd-188">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="534bd-189">role</span><span class="sxs-lookup"><span data-stu-id="534bd-189">role</span></span>|<span data-ttu-id="534bd-190">String</span><span class="sxs-lookup"><span data-stu-id="534bd-190">String</span></span>|<span data-ttu-id="534bd-191">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="534bd-191">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="534bd-192">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="534bd-192">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="534bd-193">型</span><span class="sxs-lookup"><span data-stu-id="534bd-193">realm</span></span>|<span data-ttu-id="534bd-194">String</span><span class="sxs-lookup"><span data-stu-id="534bd-194">String</span></span>|<span data-ttu-id="534bd-195">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="534bd-195">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="534bd-196">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="534bd-196">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="534bd-197">台</span><span class="sxs-lookup"><span data-stu-id="534bd-197">servers</span></span>|<span data-ttu-id="534bd-198">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="534bd-198">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="534bd-199">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="534bd-199">List of VPN Servers on the network.</span></span> <span data-ttu-id="534bd-200">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="534bd-200">Make sure end users can access these network locations.</span></span> <span data-ttu-id="534bd-201">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="534bd-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="534bd-202">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="534bd-202">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="534bd-203">connectionType</span><span class="sxs-lookup"><span data-stu-id="534bd-203">connectionType</span></span>|[<span data-ttu-id="534bd-204">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="534bd-204">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="534bd-205">连接类型。</span><span class="sxs-lookup"><span data-stu-id="534bd-205">Connection type.</span></span> <span data-ttu-id="534bd-206">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`。</span><span class="sxs-lookup"><span data-stu-id="534bd-206">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|



## <a name="response"></a><span data-ttu-id="534bd-207">响应</span><span class="sxs-lookup"><span data-stu-id="534bd-207">Response</span></span>
<span data-ttu-id="534bd-208">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="534bd-208">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="534bd-209">示例</span><span class="sxs-lookup"><span data-stu-id="534bd-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="534bd-210">请求</span><span class="sxs-lookup"><span data-stu-id="534bd-210">Request</span></span>
<span data-ttu-id="534bd-211">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="534bd-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="534bd-212">响应</span><span class="sxs-lookup"><span data-stu-id="534bd-212">Response</span></span>
<span data-ttu-id="534bd-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="534bd-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





