---
title: 更新 androidDeviceOwnerVpnConfiguration
description: 更新 androidDeviceOwnerVpnConfiguration 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 80ee2840eac3fb3d1d68f4b5f124521602e47809
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759652"
---
# <a name="update-androiddeviceownervpnconfiguration"></a><span data-ttu-id="1be62-103">更新 androidDeviceOwnerVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="1be62-103">Update androidDeviceOwnerVpnConfiguration</span></span>

> <span data-ttu-id="1be62-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1be62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1be62-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1be62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1be62-106">更新[androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1be62-106">Update the properties of a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1be62-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1be62-107">Prerequisites</span></span>
<span data-ttu-id="1be62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1be62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1be62-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1be62-110">Permission type</span></span>|<span data-ttu-id="1be62-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1be62-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1be62-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1be62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1be62-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1be62-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1be62-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1be62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1be62-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1be62-115">Not supported.</span></span>|
|<span data-ttu-id="1be62-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1be62-116">Application</span></span>|<span data-ttu-id="1be62-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1be62-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1be62-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1be62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1be62-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1be62-119">Request headers</span></span>
|<span data-ttu-id="1be62-120">标头</span><span class="sxs-lookup"><span data-stu-id="1be62-120">Header</span></span>|<span data-ttu-id="1be62-121">值</span><span class="sxs-lookup"><span data-stu-id="1be62-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1be62-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1be62-122">Authorization</span></span>|<span data-ttu-id="1be62-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1be62-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1be62-124">接受</span><span class="sxs-lookup"><span data-stu-id="1be62-124">Accept</span></span>|<span data-ttu-id="1be62-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1be62-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1be62-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1be62-126">Request body</span></span>
<span data-ttu-id="1be62-127">在请求正文中，提供[androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1be62-127">In the request body, supply a JSON representation for the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

<span data-ttu-id="1be62-128">下表显示创建[androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1be62-128">The following table shows the properties that are required when you create the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md).</span></span>

|<span data-ttu-id="1be62-129">属性</span><span class="sxs-lookup"><span data-stu-id="1be62-129">Property</span></span>|<span data-ttu-id="1be62-130">类型</span><span class="sxs-lookup"><span data-stu-id="1be62-130">Type</span></span>|<span data-ttu-id="1be62-131">说明</span><span class="sxs-lookup"><span data-stu-id="1be62-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1be62-132">id</span><span class="sxs-lookup"><span data-stu-id="1be62-132">id</span></span>|<span data-ttu-id="1be62-133">字符串</span><span class="sxs-lookup"><span data-stu-id="1be62-133">String</span></span>|<span data-ttu-id="1be62-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1be62-134">Key of the entity.</span></span> <span data-ttu-id="1be62-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1be62-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be62-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1be62-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1be62-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1be62-137">DateTimeOffset</span></span>|<span data-ttu-id="1be62-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1be62-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1be62-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1be62-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be62-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1be62-140">roleScopeTagIds</span></span>|<span data-ttu-id="1be62-141">String collection</span><span class="sxs-lookup"><span data-stu-id="1be62-141">String collection</span></span>|<span data-ttu-id="1be62-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="1be62-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1be62-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1be62-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be62-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1be62-144">supportsScopeTags</span></span>|<span data-ttu-id="1be62-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="1be62-145">Boolean</span></span>|<span data-ttu-id="1be62-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="1be62-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1be62-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="1be62-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1be62-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="1be62-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1be62-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1be62-149">This property is read-only.</span></span> <span data-ttu-id="1be62-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1be62-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be62-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1be62-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1be62-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1be62-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1be62-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="1be62-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1be62-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1be62-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be62-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1be62-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1be62-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1be62-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1be62-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1be62-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1be62-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1be62-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be62-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1be62-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1be62-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1be62-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1be62-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1be62-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1be62-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1be62-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be62-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1be62-163">createdDateTime</span></span>|<span data-ttu-id="1be62-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1be62-164">DateTimeOffset</span></span>|<span data-ttu-id="1be62-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1be62-165">DateTime the object was created.</span></span> <span data-ttu-id="1be62-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1be62-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be62-167">说明</span><span class="sxs-lookup"><span data-stu-id="1be62-167">description</span></span>|<span data-ttu-id="1be62-168">String</span><span class="sxs-lookup"><span data-stu-id="1be62-168">String</span></span>|<span data-ttu-id="1be62-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1be62-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1be62-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1be62-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be62-171">displayName</span><span class="sxs-lookup"><span data-stu-id="1be62-171">displayName</span></span>|<span data-ttu-id="1be62-172">String</span><span class="sxs-lookup"><span data-stu-id="1be62-172">String</span></span>|<span data-ttu-id="1be62-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1be62-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1be62-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1be62-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be62-175">version</span><span class="sxs-lookup"><span data-stu-id="1be62-175">version</span></span>|<span data-ttu-id="1be62-176">Int32</span><span class="sxs-lookup"><span data-stu-id="1be62-176">Int32</span></span>|<span data-ttu-id="1be62-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1be62-177">Version of the device configuration.</span></span> <span data-ttu-id="1be62-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1be62-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be62-179">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1be62-179">authenticationMethod</span></span>|[<span data-ttu-id="1be62-180">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1be62-180">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="1be62-181">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="1be62-181">Authentication method.</span></span> <span data-ttu-id="1be62-182">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="1be62-182">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="1be62-183">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="1be62-183">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="1be62-184">connectionName</span><span class="sxs-lookup"><span data-stu-id="1be62-184">connectionName</span></span>|<span data-ttu-id="1be62-185">String</span><span class="sxs-lookup"><span data-stu-id="1be62-185">String</span></span>|<span data-ttu-id="1be62-186">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="1be62-186">Connection name displayed to the user.</span></span> <span data-ttu-id="1be62-187">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1be62-187">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="1be62-188">role</span><span class="sxs-lookup"><span data-stu-id="1be62-188">role</span></span>|<span data-ttu-id="1be62-189">String</span><span class="sxs-lookup"><span data-stu-id="1be62-189">String</span></span>|<span data-ttu-id="1be62-190">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="1be62-190">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="1be62-191">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1be62-191">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="1be62-192">型</span><span class="sxs-lookup"><span data-stu-id="1be62-192">realm</span></span>|<span data-ttu-id="1be62-193">String</span><span class="sxs-lookup"><span data-stu-id="1be62-193">String</span></span>|<span data-ttu-id="1be62-194">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="1be62-194">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="1be62-195">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1be62-195">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="1be62-196">台</span><span class="sxs-lookup"><span data-stu-id="1be62-196">servers</span></span>|<span data-ttu-id="1be62-197">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="1be62-197">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="1be62-198">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="1be62-198">List of VPN Servers on the network.</span></span> <span data-ttu-id="1be62-199">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="1be62-199">Make sure end users can access these network locations.</span></span> <span data-ttu-id="1be62-200">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="1be62-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="1be62-201">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1be62-201">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="1be62-202">connectionType</span><span class="sxs-lookup"><span data-stu-id="1be62-202">connectionType</span></span>|[<span data-ttu-id="1be62-203">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="1be62-203">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="1be62-204">连接类型。</span><span class="sxs-lookup"><span data-stu-id="1be62-204">Connection type.</span></span> <span data-ttu-id="1be62-205">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`。</span><span class="sxs-lookup"><span data-stu-id="1be62-205">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|



## <a name="response"></a><span data-ttu-id="1be62-206">响应</span><span class="sxs-lookup"><span data-stu-id="1be62-206">Response</span></span>
<span data-ttu-id="1be62-207">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1be62-207">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1be62-208">示例</span><span class="sxs-lookup"><span data-stu-id="1be62-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="1be62-209">请求</span><span class="sxs-lookup"><span data-stu-id="1be62-209">Request</span></span>
<span data-ttu-id="1be62-210">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1be62-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1be62-211">响应</span><span class="sxs-lookup"><span data-stu-id="1be62-211">Response</span></span>
<span data-ttu-id="1be62-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1be62-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




