---
title: 创建 androidDeviceOwnerVpnConfiguration
description: 创建新的 androidDeviceOwnerVpnConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2d704177b3bf866891e5b6ca1cc31b4ca29fee8c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49240248"
---
# <a name="create-androiddeviceownervpnconfiguration"></a><span data-ttu-id="2f97c-103">创建 androidDeviceOwnerVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f97c-103">Create androidDeviceOwnerVpnConfiguration</span></span>

<span data-ttu-id="2f97c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f97c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f97c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2f97c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f97c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f97c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f97c-107">创建新的 [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f97c-107">Create a new [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f97c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2f97c-108">Prerequisites</span></span>
<span data-ttu-id="2f97c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f97c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f97c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f97c-111">Permission type</span></span>|<span data-ttu-id="2f97c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2f97c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f97c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f97c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f97c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f97c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f97c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f97c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f97c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f97c-116">Not supported.</span></span>|
|<span data-ttu-id="2f97c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f97c-117">Application</span></span>|<span data-ttu-id="2f97c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f97c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f97c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f97c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2f97c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f97c-120">Request headers</span></span>
|<span data-ttu-id="2f97c-121">标头</span><span class="sxs-lookup"><span data-stu-id="2f97c-121">Header</span></span>|<span data-ttu-id="2f97c-122">值</span><span class="sxs-lookup"><span data-stu-id="2f97c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f97c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f97c-123">Authorization</span></span>|<span data-ttu-id="2f97c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2f97c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f97c-125">接受</span><span class="sxs-lookup"><span data-stu-id="2f97c-125">Accept</span></span>|<span data-ttu-id="2f97c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f97c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f97c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f97c-127">Request body</span></span>
<span data-ttu-id="2f97c-128">在请求正文中，提供 androidDeviceOwnerVpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f97c-128">In the request body, supply a JSON representation for the androidDeviceOwnerVpnConfiguration object.</span></span>

<span data-ttu-id="2f97c-129">下表显示创建 androidDeviceOwnerVpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2f97c-129">The following table shows the properties that are required when you create the androidDeviceOwnerVpnConfiguration.</span></span>

|<span data-ttu-id="2f97c-130">属性</span><span class="sxs-lookup"><span data-stu-id="2f97c-130">Property</span></span>|<span data-ttu-id="2f97c-131">类型</span><span class="sxs-lookup"><span data-stu-id="2f97c-131">Type</span></span>|<span data-ttu-id="2f97c-132">说明</span><span class="sxs-lookup"><span data-stu-id="2f97c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f97c-133">id</span><span class="sxs-lookup"><span data-stu-id="2f97c-133">id</span></span>|<span data-ttu-id="2f97c-134">String</span><span class="sxs-lookup"><span data-stu-id="2f97c-134">String</span></span>|<span data-ttu-id="2f97c-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2f97c-135">Key of the entity.</span></span> <span data-ttu-id="2f97c-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f97c-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f97c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f97c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2f97c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f97c-138">DateTimeOffset</span></span>|<span data-ttu-id="2f97c-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2f97c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2f97c-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f97c-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f97c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2f97c-141">roleScopeTagIds</span></span>|<span data-ttu-id="2f97c-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="2f97c-142">String collection</span></span>|<span data-ttu-id="2f97c-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2f97c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2f97c-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f97c-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f97c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2f97c-145">supportsScopeTags</span></span>|<span data-ttu-id="2f97c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f97c-146">Boolean</span></span>|<span data-ttu-id="2f97c-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="2f97c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2f97c-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="2f97c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2f97c-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="2f97c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2f97c-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2f97c-150">This property is read-only.</span></span> <span data-ttu-id="2f97c-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f97c-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f97c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2f97c-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2f97c-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2f97c-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2f97c-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="2f97c-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2f97c-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f97c-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f97c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2f97c-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2f97c-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2f97c-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2f97c-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2f97c-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2f97c-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f97c-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f97c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2f97c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2f97c-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2f97c-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2f97c-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="2f97c-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2f97c-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f97c-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f97c-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f97c-164">createdDateTime</span></span>|<span data-ttu-id="2f97c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f97c-165">DateTimeOffset</span></span>|<span data-ttu-id="2f97c-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2f97c-166">DateTime the object was created.</span></span> <span data-ttu-id="2f97c-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f97c-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f97c-168">description</span><span class="sxs-lookup"><span data-stu-id="2f97c-168">description</span></span>|<span data-ttu-id="2f97c-169">String</span><span class="sxs-lookup"><span data-stu-id="2f97c-169">String</span></span>|<span data-ttu-id="2f97c-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2f97c-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2f97c-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f97c-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f97c-172">displayName</span><span class="sxs-lookup"><span data-stu-id="2f97c-172">displayName</span></span>|<span data-ttu-id="2f97c-173">String</span><span class="sxs-lookup"><span data-stu-id="2f97c-173">String</span></span>|<span data-ttu-id="2f97c-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2f97c-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2f97c-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f97c-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f97c-176">version</span><span class="sxs-lookup"><span data-stu-id="2f97c-176">version</span></span>|<span data-ttu-id="2f97c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="2f97c-177">Int32</span></span>|<span data-ttu-id="2f97c-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2f97c-178">Version of the device configuration.</span></span> <span data-ttu-id="2f97c-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f97c-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f97c-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2f97c-180">authenticationMethod</span></span>|[<span data-ttu-id="2f97c-181">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2f97c-181">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="2f97c-182">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="2f97c-182">Authentication method.</span></span> <span data-ttu-id="2f97c-183">继承自 [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="2f97c-183">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="2f97c-184">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="2f97c-184">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="2f97c-185">connectionName</span><span class="sxs-lookup"><span data-stu-id="2f97c-185">connectionName</span></span>|<span data-ttu-id="2f97c-186">String</span><span class="sxs-lookup"><span data-stu-id="2f97c-186">String</span></span>|<span data-ttu-id="2f97c-187">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="2f97c-187">Connection name displayed to the user.</span></span> <span data-ttu-id="2f97c-188">继承自 [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f97c-188">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="2f97c-189">role</span><span class="sxs-lookup"><span data-stu-id="2f97c-189">role</span></span>|<span data-ttu-id="2f97c-190">String</span><span class="sxs-lookup"><span data-stu-id="2f97c-190">String</span></span>|<span data-ttu-id="2f97c-191">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="2f97c-191">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="2f97c-192">继承自 [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f97c-192">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="2f97c-193">型</span><span class="sxs-lookup"><span data-stu-id="2f97c-193">realm</span></span>|<span data-ttu-id="2f97c-194">String</span><span class="sxs-lookup"><span data-stu-id="2f97c-194">String</span></span>|<span data-ttu-id="2f97c-195">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="2f97c-195">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="2f97c-196">继承自 [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f97c-196">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="2f97c-197">台</span><span class="sxs-lookup"><span data-stu-id="2f97c-197">servers</span></span>|<span data-ttu-id="2f97c-198">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f97c-198">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="2f97c-199">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="2f97c-199">List of VPN Servers on the network.</span></span> <span data-ttu-id="2f97c-200">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="2f97c-200">Make sure end users can access these network locations.</span></span> <span data-ttu-id="2f97c-201">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2f97c-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="2f97c-202">继承自 [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f97c-202">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="2f97c-203">connectionType</span><span class="sxs-lookup"><span data-stu-id="2f97c-203">connectionType</span></span>|[<span data-ttu-id="2f97c-204">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="2f97c-204">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="2f97c-205">连接类型。</span><span class="sxs-lookup"><span data-stu-id="2f97c-205">Connection type.</span></span> <span data-ttu-id="2f97c-206">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`、`microsoftTunnel`、`netMotionMobility`。</span><span class="sxs-lookup"><span data-stu-id="2f97c-206">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="2f97c-207">proxyServer</span><span class="sxs-lookup"><span data-stu-id="2f97c-207">proxyServer</span></span>|[<span data-ttu-id="2f97c-208">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="2f97c-208">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="2f97c-209">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="2f97c-209">Proxy server.</span></span>|
|<span data-ttu-id="2f97c-210">targetedPackageIds</span><span class="sxs-lookup"><span data-stu-id="2f97c-210">targetedPackageIds</span></span>|<span data-ttu-id="2f97c-211">String 集合</span><span class="sxs-lookup"><span data-stu-id="2f97c-211">String collection</span></span>|<span data-ttu-id="2f97c-212">目标应用程序包 Id。</span><span class="sxs-lookup"><span data-stu-id="2f97c-212">Targeted App package IDs.</span></span>|
|<span data-ttu-id="2f97c-213">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="2f97c-213">targetedMobileApps</span></span>|<span data-ttu-id="2f97c-214">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f97c-214">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="2f97c-215">目标移动应用。</span><span class="sxs-lookup"><span data-stu-id="2f97c-215">Targeted mobile apps.</span></span> <span data-ttu-id="2f97c-216">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2f97c-216">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2f97c-217">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="2f97c-217">alwaysOn</span></span>|<span data-ttu-id="2f97c-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f97c-218">Boolean</span></span>|<span data-ttu-id="2f97c-219">是否启用始终启用的 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="2f97c-219">Whether or not to enable always-on VPN connection.</span></span>|
|<span data-ttu-id="2f97c-220">alwaysOnLockdown</span><span class="sxs-lookup"><span data-stu-id="2f97c-220">alwaysOnLockdown</span></span>|<span data-ttu-id="2f97c-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f97c-221">Boolean</span></span>|<span data-ttu-id="2f97c-222">如果启用了 always on VPN 连接，则在断开 VPN 连接时是否锁定网络流量。</span><span class="sxs-lookup"><span data-stu-id="2f97c-222">If always-on VPN connection is enabled, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="2f97c-223">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="2f97c-223">microsoftTunnelSiteId</span></span>|<span data-ttu-id="2f97c-224">String</span><span class="sxs-lookup"><span data-stu-id="2f97c-224">String</span></span>|<span data-ttu-id="2f97c-225">Microsoft 隧道站点 ID。</span><span class="sxs-lookup"><span data-stu-id="2f97c-225">Microsoft Tunnel site ID.</span></span>|
|<span data-ttu-id="2f97c-226">customData</span><span class="sxs-lookup"><span data-stu-id="2f97c-226">customData</span></span>|<span data-ttu-id="2f97c-227">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f97c-227">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="2f97c-228">用于定义特定于 VPN 提供程序的键/值对的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="2f97c-228">Custom data to define key/value pairs specific to a VPN provider.</span></span> <span data-ttu-id="2f97c-229">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="2f97c-229">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="2f97c-230">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="2f97c-230">customKeyValueData</span></span>|<span data-ttu-id="2f97c-231">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f97c-231">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="2f97c-232">用于定义特定于 VPN 提供程序的键/值对的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="2f97c-232">Custom data to define key/value pairs specific to a VPN provider.</span></span> <span data-ttu-id="2f97c-233">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="2f97c-233">This collection can contain a maximum of 25 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="2f97c-234">响应</span><span class="sxs-lookup"><span data-stu-id="2f97c-234">Response</span></span>
<span data-ttu-id="2f97c-235">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f97c-235">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f97c-236">示例</span><span class="sxs-lookup"><span data-stu-id="2f97c-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f97c-237">请求</span><span class="sxs-lookup"><span data-stu-id="2f97c-237">Request</span></span>
<span data-ttu-id="2f97c-238">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f97c-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="2f97c-239">响应</span><span class="sxs-lookup"><span data-stu-id="2f97c-239">Response</span></span>
<span data-ttu-id="2f97c-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2f97c-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




