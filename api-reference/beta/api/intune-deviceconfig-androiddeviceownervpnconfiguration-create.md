---
title: 创建 androidDeviceOwnerVpnConfiguration
description: 创建新的 androidDeviceOwnerVpnConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7d08abe8472f8f64a43ec26175de5d3a05ba901d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37169774"
---
# <a name="create-androiddeviceownervpnconfiguration"></a><span data-ttu-id="c36f9-103">创建 androidDeviceOwnerVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c36f9-103">Create androidDeviceOwnerVpnConfiguration</span></span>

> <span data-ttu-id="c36f9-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c36f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c36f9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c36f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c36f9-106">创建新的[androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c36f9-106">Create a new [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c36f9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c36f9-107">Prerequisites</span></span>
<span data-ttu-id="c36f9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c36f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c36f9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c36f9-110">Permission type</span></span>|<span data-ttu-id="c36f9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c36f9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c36f9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c36f9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c36f9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c36f9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c36f9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c36f9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c36f9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c36f9-115">Not supported.</span></span>|
|<span data-ttu-id="c36f9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c36f9-116">Application</span></span>|<span data-ttu-id="c36f9-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c36f9-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c36f9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c36f9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c36f9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c36f9-119">Request headers</span></span>
|<span data-ttu-id="c36f9-120">标头</span><span class="sxs-lookup"><span data-stu-id="c36f9-120">Header</span></span>|<span data-ttu-id="c36f9-121">值</span><span class="sxs-lookup"><span data-stu-id="c36f9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c36f9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c36f9-122">Authorization</span></span>|<span data-ttu-id="c36f9-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c36f9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c36f9-124">接受</span><span class="sxs-lookup"><span data-stu-id="c36f9-124">Accept</span></span>|<span data-ttu-id="c36f9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c36f9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c36f9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c36f9-126">Request body</span></span>
<span data-ttu-id="c36f9-127">在请求正文中，提供 androidDeviceOwnerVpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c36f9-127">In the request body, supply a JSON representation for the androidDeviceOwnerVpnConfiguration object.</span></span>

<span data-ttu-id="c36f9-128">下表显示创建 androidDeviceOwnerVpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c36f9-128">The following table shows the properties that are required when you create the androidDeviceOwnerVpnConfiguration.</span></span>

|<span data-ttu-id="c36f9-129">属性</span><span class="sxs-lookup"><span data-stu-id="c36f9-129">Property</span></span>|<span data-ttu-id="c36f9-130">类型</span><span class="sxs-lookup"><span data-stu-id="c36f9-130">Type</span></span>|<span data-ttu-id="c36f9-131">说明</span><span class="sxs-lookup"><span data-stu-id="c36f9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c36f9-132">id</span><span class="sxs-lookup"><span data-stu-id="c36f9-132">id</span></span>|<span data-ttu-id="c36f9-133">字符串</span><span class="sxs-lookup"><span data-stu-id="c36f9-133">String</span></span>|<span data-ttu-id="c36f9-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c36f9-134">Key of the entity.</span></span> <span data-ttu-id="c36f9-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c36f9-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c36f9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c36f9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c36f9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c36f9-137">DateTimeOffset</span></span>|<span data-ttu-id="c36f9-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c36f9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c36f9-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c36f9-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c36f9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c36f9-140">roleScopeTagIds</span></span>|<span data-ttu-id="c36f9-141">String collection</span><span class="sxs-lookup"><span data-stu-id="c36f9-141">String collection</span></span>|<span data-ttu-id="c36f9-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c36f9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c36f9-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c36f9-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c36f9-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c36f9-144">supportsScopeTags</span></span>|<span data-ttu-id="c36f9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c36f9-145">Boolean</span></span>|<span data-ttu-id="c36f9-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="c36f9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c36f9-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="c36f9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c36f9-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="c36f9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c36f9-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c36f9-149">This property is read-only.</span></span> <span data-ttu-id="c36f9-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c36f9-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c36f9-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c36f9-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c36f9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c36f9-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c36f9-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="c36f9-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c36f9-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c36f9-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c36f9-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c36f9-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c36f9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c36f9-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c36f9-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c36f9-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c36f9-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c36f9-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c36f9-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c36f9-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c36f9-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c36f9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c36f9-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c36f9-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c36f9-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c36f9-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c36f9-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c36f9-163">createdDateTime</span></span>|<span data-ttu-id="c36f9-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c36f9-164">DateTimeOffset</span></span>|<span data-ttu-id="c36f9-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c36f9-165">DateTime the object was created.</span></span> <span data-ttu-id="c36f9-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c36f9-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c36f9-167">说明</span><span class="sxs-lookup"><span data-stu-id="c36f9-167">description</span></span>|<span data-ttu-id="c36f9-168">String</span><span class="sxs-lookup"><span data-stu-id="c36f9-168">String</span></span>|<span data-ttu-id="c36f9-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c36f9-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c36f9-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c36f9-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c36f9-171">displayName</span><span class="sxs-lookup"><span data-stu-id="c36f9-171">displayName</span></span>|<span data-ttu-id="c36f9-172">String</span><span class="sxs-lookup"><span data-stu-id="c36f9-172">String</span></span>|<span data-ttu-id="c36f9-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c36f9-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c36f9-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c36f9-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c36f9-175">version</span><span class="sxs-lookup"><span data-stu-id="c36f9-175">version</span></span>|<span data-ttu-id="c36f9-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c36f9-176">Int32</span></span>|<span data-ttu-id="c36f9-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c36f9-177">Version of the device configuration.</span></span> <span data-ttu-id="c36f9-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c36f9-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c36f9-179">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c36f9-179">authenticationMethod</span></span>|[<span data-ttu-id="c36f9-180">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c36f9-180">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="c36f9-181">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="c36f9-181">Authentication method.</span></span> <span data-ttu-id="c36f9-182">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="c36f9-182">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="c36f9-183">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="c36f9-183">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="c36f9-184">connectionName</span><span class="sxs-lookup"><span data-stu-id="c36f9-184">connectionName</span></span>|<span data-ttu-id="c36f9-185">String</span><span class="sxs-lookup"><span data-stu-id="c36f9-185">String</span></span>|<span data-ttu-id="c36f9-186">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="c36f9-186">Connection name displayed to the user.</span></span> <span data-ttu-id="c36f9-187">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c36f9-187">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="c36f9-188">role</span><span class="sxs-lookup"><span data-stu-id="c36f9-188">role</span></span>|<span data-ttu-id="c36f9-189">String</span><span class="sxs-lookup"><span data-stu-id="c36f9-189">String</span></span>|<span data-ttu-id="c36f9-190">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="c36f9-190">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="c36f9-191">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c36f9-191">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="c36f9-192">型</span><span class="sxs-lookup"><span data-stu-id="c36f9-192">realm</span></span>|<span data-ttu-id="c36f9-193">String</span><span class="sxs-lookup"><span data-stu-id="c36f9-193">String</span></span>|<span data-ttu-id="c36f9-194">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="c36f9-194">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="c36f9-195">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c36f9-195">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="c36f9-196">台</span><span class="sxs-lookup"><span data-stu-id="c36f9-196">servers</span></span>|<span data-ttu-id="c36f9-197">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="c36f9-197">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="c36f9-198">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="c36f9-198">List of VPN Servers on the network.</span></span> <span data-ttu-id="c36f9-199">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="c36f9-199">Make sure end users can access these network locations.</span></span> <span data-ttu-id="c36f9-200">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c36f9-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c36f9-201">继承自[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c36f9-201">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="c36f9-202">connectionType</span><span class="sxs-lookup"><span data-stu-id="c36f9-202">connectionType</span></span>|[<span data-ttu-id="c36f9-203">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="c36f9-203">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="c36f9-204">连接类型。</span><span class="sxs-lookup"><span data-stu-id="c36f9-204">Connection type.</span></span> <span data-ttu-id="c36f9-205">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`。</span><span class="sxs-lookup"><span data-stu-id="c36f9-205">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|



## <a name="response"></a><span data-ttu-id="c36f9-206">响应</span><span class="sxs-lookup"><span data-stu-id="c36f9-206">Response</span></span>
<span data-ttu-id="c36f9-207">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c36f9-207">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c36f9-208">示例</span><span class="sxs-lookup"><span data-stu-id="c36f9-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="c36f9-209">请求</span><span class="sxs-lookup"><span data-stu-id="c36f9-209">Request</span></span>
<span data-ttu-id="c36f9-210">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c36f9-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c36f9-211">响应</span><span class="sxs-lookup"><span data-stu-id="c36f9-211">Response</span></span>
<span data-ttu-id="c36f9-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c36f9-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




