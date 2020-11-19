---
title: 更新 androidDeviceOwnerVpnConfiguration
description: 更新 androidDeviceOwnerVpnConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6af039e59db358f75e560a76d45c5fb2bb48df0b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49240102"
---
# <a name="update-androiddeviceownervpnconfiguration"></a><span data-ttu-id="7e332-103">更新 androidDeviceOwnerVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="7e332-103">Update androidDeviceOwnerVpnConfiguration</span></span>

<span data-ttu-id="7e332-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e332-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e332-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7e332-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e332-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7e332-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e332-107">更新 [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7e332-107">Update the properties of a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e332-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7e332-108">Prerequisites</span></span>
<span data-ttu-id="7e332-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e332-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e332-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e332-111">Permission type</span></span>|<span data-ttu-id="7e332-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7e332-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e332-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e332-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7e332-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e332-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7e332-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e332-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e332-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e332-116">Not supported.</span></span>|
|<span data-ttu-id="7e332-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e332-117">Application</span></span>|<span data-ttu-id="7e332-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e332-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e332-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e332-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7e332-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e332-120">Request headers</span></span>
|<span data-ttu-id="7e332-121">标头</span><span class="sxs-lookup"><span data-stu-id="7e332-121">Header</span></span>|<span data-ttu-id="7e332-122">值</span><span class="sxs-lookup"><span data-stu-id="7e332-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e332-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e332-123">Authorization</span></span>|<span data-ttu-id="7e332-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7e332-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e332-125">接受</span><span class="sxs-lookup"><span data-stu-id="7e332-125">Accept</span></span>|<span data-ttu-id="7e332-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7e332-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e332-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e332-127">Request body</span></span>
<span data-ttu-id="7e332-128">在请求正文中，提供 [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e332-128">In the request body, supply a JSON representation for the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

<span data-ttu-id="7e332-129">下表显示创建 [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7e332-129">The following table shows the properties that are required when you create the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md).</span></span>

|<span data-ttu-id="7e332-130">属性</span><span class="sxs-lookup"><span data-stu-id="7e332-130">Property</span></span>|<span data-ttu-id="7e332-131">类型</span><span class="sxs-lookup"><span data-stu-id="7e332-131">Type</span></span>|<span data-ttu-id="7e332-132">说明</span><span class="sxs-lookup"><span data-stu-id="7e332-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e332-133">id</span><span class="sxs-lookup"><span data-stu-id="7e332-133">id</span></span>|<span data-ttu-id="7e332-134">String</span><span class="sxs-lookup"><span data-stu-id="7e332-134">String</span></span>|<span data-ttu-id="7e332-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7e332-135">Key of the entity.</span></span> <span data-ttu-id="7e332-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e332-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e332-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e332-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7e332-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e332-138">DateTimeOffset</span></span>|<span data-ttu-id="7e332-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7e332-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7e332-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e332-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e332-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7e332-141">roleScopeTagIds</span></span>|<span data-ttu-id="7e332-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="7e332-142">String collection</span></span>|<span data-ttu-id="7e332-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="7e332-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7e332-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e332-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e332-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7e332-145">supportsScopeTags</span></span>|<span data-ttu-id="7e332-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e332-146">Boolean</span></span>|<span data-ttu-id="7e332-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="7e332-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7e332-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="7e332-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7e332-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="7e332-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7e332-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="7e332-150">This property is read-only.</span></span> <span data-ttu-id="7e332-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e332-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e332-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7e332-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7e332-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7e332-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7e332-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="7e332-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7e332-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e332-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e332-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7e332-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7e332-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7e332-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7e332-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="7e332-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7e332-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e332-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e332-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7e332-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7e332-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7e332-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7e332-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="7e332-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7e332-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e332-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e332-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e332-164">createdDateTime</span></span>|<span data-ttu-id="7e332-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e332-165">DateTimeOffset</span></span>|<span data-ttu-id="7e332-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7e332-166">DateTime the object was created.</span></span> <span data-ttu-id="7e332-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e332-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e332-168">description</span><span class="sxs-lookup"><span data-stu-id="7e332-168">description</span></span>|<span data-ttu-id="7e332-169">String</span><span class="sxs-lookup"><span data-stu-id="7e332-169">String</span></span>|<span data-ttu-id="7e332-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="7e332-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7e332-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e332-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e332-172">displayName</span><span class="sxs-lookup"><span data-stu-id="7e332-172">displayName</span></span>|<span data-ttu-id="7e332-173">String</span><span class="sxs-lookup"><span data-stu-id="7e332-173">String</span></span>|<span data-ttu-id="7e332-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="7e332-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7e332-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e332-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e332-176">version</span><span class="sxs-lookup"><span data-stu-id="7e332-176">version</span></span>|<span data-ttu-id="7e332-177">Int32</span><span class="sxs-lookup"><span data-stu-id="7e332-177">Int32</span></span>|<span data-ttu-id="7e332-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="7e332-178">Version of the device configuration.</span></span> <span data-ttu-id="7e332-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e332-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7e332-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7e332-180">authenticationMethod</span></span>|[<span data-ttu-id="7e332-181">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7e332-181">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="7e332-182">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="7e332-182">Authentication method.</span></span> <span data-ttu-id="7e332-183">继承自 [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="7e332-183">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="7e332-184">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="7e332-184">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="7e332-185">connectionName</span><span class="sxs-lookup"><span data-stu-id="7e332-185">connectionName</span></span>|<span data-ttu-id="7e332-186">String</span><span class="sxs-lookup"><span data-stu-id="7e332-186">String</span></span>|<span data-ttu-id="7e332-187">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="7e332-187">Connection name displayed to the user.</span></span> <span data-ttu-id="7e332-188">继承自 [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e332-188">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e332-189">role</span><span class="sxs-lookup"><span data-stu-id="7e332-189">role</span></span>|<span data-ttu-id="7e332-190">String</span><span class="sxs-lookup"><span data-stu-id="7e332-190">String</span></span>|<span data-ttu-id="7e332-191">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="7e332-191">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="7e332-192">继承自 [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e332-192">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e332-193">型</span><span class="sxs-lookup"><span data-stu-id="7e332-193">realm</span></span>|<span data-ttu-id="7e332-194">String</span><span class="sxs-lookup"><span data-stu-id="7e332-194">String</span></span>|<span data-ttu-id="7e332-195">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="7e332-195">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="7e332-196">继承自 [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e332-196">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e332-197">台</span><span class="sxs-lookup"><span data-stu-id="7e332-197">servers</span></span>|<span data-ttu-id="7e332-198">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e332-198">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="7e332-199">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="7e332-199">List of VPN Servers on the network.</span></span> <span data-ttu-id="7e332-200">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="7e332-200">Make sure end users can access these network locations.</span></span> <span data-ttu-id="7e332-201">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="7e332-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="7e332-202">继承自 [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7e332-202">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="7e332-203">connectionType</span><span class="sxs-lookup"><span data-stu-id="7e332-203">connectionType</span></span>|[<span data-ttu-id="7e332-204">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="7e332-204">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="7e332-205">连接类型。</span><span class="sxs-lookup"><span data-stu-id="7e332-205">Connection type.</span></span> <span data-ttu-id="7e332-206">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`、`microsoftTunnel`、`netMotionMobility`。</span><span class="sxs-lookup"><span data-stu-id="7e332-206">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="7e332-207">proxyServer</span><span class="sxs-lookup"><span data-stu-id="7e332-207">proxyServer</span></span>|[<span data-ttu-id="7e332-208">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="7e332-208">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="7e332-209">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="7e332-209">Proxy server.</span></span>|
|<span data-ttu-id="7e332-210">targetedPackageIds</span><span class="sxs-lookup"><span data-stu-id="7e332-210">targetedPackageIds</span></span>|<span data-ttu-id="7e332-211">String 集合</span><span class="sxs-lookup"><span data-stu-id="7e332-211">String collection</span></span>|<span data-ttu-id="7e332-212">目标应用程序包 Id。</span><span class="sxs-lookup"><span data-stu-id="7e332-212">Targeted App package IDs.</span></span>|
|<span data-ttu-id="7e332-213">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="7e332-213">targetedMobileApps</span></span>|<span data-ttu-id="7e332-214">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e332-214">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="7e332-215">目标移动应用。</span><span class="sxs-lookup"><span data-stu-id="7e332-215">Targeted mobile apps.</span></span> <span data-ttu-id="7e332-216">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="7e332-216">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7e332-217">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="7e332-217">alwaysOn</span></span>|<span data-ttu-id="7e332-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e332-218">Boolean</span></span>|<span data-ttu-id="7e332-219">是否启用始终启用的 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="7e332-219">Whether or not to enable always-on VPN connection.</span></span>|
|<span data-ttu-id="7e332-220">alwaysOnLockdown</span><span class="sxs-lookup"><span data-stu-id="7e332-220">alwaysOnLockdown</span></span>|<span data-ttu-id="7e332-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e332-221">Boolean</span></span>|<span data-ttu-id="7e332-222">如果启用了 always on VPN 连接，则在断开 VPN 连接时是否锁定网络流量。</span><span class="sxs-lookup"><span data-stu-id="7e332-222">If always-on VPN connection is enabled, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="7e332-223">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="7e332-223">microsoftTunnelSiteId</span></span>|<span data-ttu-id="7e332-224">String</span><span class="sxs-lookup"><span data-stu-id="7e332-224">String</span></span>|<span data-ttu-id="7e332-225">Microsoft 隧道站点 ID。</span><span class="sxs-lookup"><span data-stu-id="7e332-225">Microsoft Tunnel site ID.</span></span>|
|<span data-ttu-id="7e332-226">customData</span><span class="sxs-lookup"><span data-stu-id="7e332-226">customData</span></span>|<span data-ttu-id="7e332-227">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e332-227">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="7e332-228">用于定义特定于 VPN 提供程序的键/值对的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="7e332-228">Custom data to define key/value pairs specific to a VPN provider.</span></span> <span data-ttu-id="7e332-229">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="7e332-229">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="7e332-230">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="7e332-230">customKeyValueData</span></span>|<span data-ttu-id="7e332-231">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e332-231">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7e332-232">用于定义特定于 VPN 提供程序的键/值对的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="7e332-232">Custom data to define key/value pairs specific to a VPN provider.</span></span> <span data-ttu-id="7e332-233">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="7e332-233">This collection can contain a maximum of 25 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="7e332-234">响应</span><span class="sxs-lookup"><span data-stu-id="7e332-234">Response</span></span>
<span data-ttu-id="7e332-235">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7e332-235">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e332-236">示例</span><span class="sxs-lookup"><span data-stu-id="7e332-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e332-237">请求</span><span class="sxs-lookup"><span data-stu-id="7e332-237">Request</span></span>
<span data-ttu-id="7e332-238">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7e332-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2383

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
  "connectionType": "pulseSecure",
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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="7e332-239">响应</span><span class="sxs-lookup"><span data-stu-id="7e332-239">Response</span></span>
<span data-ttu-id="7e332-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7e332-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2555

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
  "connectionType": "pulseSecure",
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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value",
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
  ]
}
```




