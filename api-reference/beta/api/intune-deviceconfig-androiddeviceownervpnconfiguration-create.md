---
title: 创建 androidDeviceOwnerVpnConfiguration
description: 创建新的 androidDeviceOwnerVpnConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f407851267cd28928b4c7380e2aa97088102e170
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130523"
---
# <a name="create-androiddeviceownervpnconfiguration"></a><span data-ttu-id="f1be4-103">创建 androidDeviceOwnerVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1be4-103">Create androidDeviceOwnerVpnConfiguration</span></span>

<span data-ttu-id="f1be4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1be4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1be4-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f1be4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1be4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f1be4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1be4-107">创建新的 [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f1be4-107">Create a new [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1be4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f1be4-108">Prerequisites</span></span>
<span data-ttu-id="f1be4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1be4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1be4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1be4-111">Permission type</span></span>|<span data-ttu-id="f1be4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f1be4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1be4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1be4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1be4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1be4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1be4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1be4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1be4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1be4-116">Not supported.</span></span>|
|<span data-ttu-id="f1be4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1be4-117">Application</span></span>|<span data-ttu-id="f1be4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1be4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1be4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1be4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f1be4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1be4-120">Request headers</span></span>
|<span data-ttu-id="f1be4-121">标头</span><span class="sxs-lookup"><span data-stu-id="f1be4-121">Header</span></span>|<span data-ttu-id="f1be4-122">值</span><span class="sxs-lookup"><span data-stu-id="f1be4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1be4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1be4-123">Authorization</span></span>|<span data-ttu-id="f1be4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f1be4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1be4-125">接受</span><span class="sxs-lookup"><span data-stu-id="f1be4-125">Accept</span></span>|<span data-ttu-id="f1be4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1be4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1be4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1be4-127">Request body</span></span>
<span data-ttu-id="f1be4-128">在请求正文中，提供 androidDeviceOwnerVpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1be4-128">In the request body, supply a JSON representation for the androidDeviceOwnerVpnConfiguration object.</span></span>

<span data-ttu-id="f1be4-129">下表显示创建 androidDeviceOwnerVpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f1be4-129">The following table shows the properties that are required when you create the androidDeviceOwnerVpnConfiguration.</span></span>

|<span data-ttu-id="f1be4-130">属性</span><span class="sxs-lookup"><span data-stu-id="f1be4-130">Property</span></span>|<span data-ttu-id="f1be4-131">类型</span><span class="sxs-lookup"><span data-stu-id="f1be4-131">Type</span></span>|<span data-ttu-id="f1be4-132">说明</span><span class="sxs-lookup"><span data-stu-id="f1be4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1be4-133">id</span><span class="sxs-lookup"><span data-stu-id="f1be4-133">id</span></span>|<span data-ttu-id="f1be4-134">String</span><span class="sxs-lookup"><span data-stu-id="f1be4-134">String</span></span>|<span data-ttu-id="f1be4-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f1be4-135">Key of the entity.</span></span> <span data-ttu-id="f1be4-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1be4-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1be4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1be4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f1be4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1be4-138">DateTimeOffset</span></span>|<span data-ttu-id="f1be4-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f1be4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f1be4-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1be4-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1be4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f1be4-141">roleScopeTagIds</span></span>|<span data-ttu-id="f1be4-142">String collection</span><span class="sxs-lookup"><span data-stu-id="f1be4-142">String collection</span></span>|<span data-ttu-id="f1be4-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f1be4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f1be4-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1be4-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1be4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f1be4-145">supportsScopeTags</span></span>|<span data-ttu-id="f1be4-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1be4-146">Boolean</span></span>|<span data-ttu-id="f1be4-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="f1be4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f1be4-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="f1be4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f1be4-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="f1be4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f1be4-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f1be4-150">This property is read-only.</span></span> <span data-ttu-id="f1be4-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1be4-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1be4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f1be4-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f1be4-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f1be4-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f1be4-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="f1be4-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f1be4-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1be4-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1be4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f1be4-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f1be4-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f1be4-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f1be4-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f1be4-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f1be4-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1be4-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1be4-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f1be4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f1be4-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f1be4-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f1be4-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f1be4-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f1be4-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1be4-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1be4-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1be4-164">createdDateTime</span></span>|<span data-ttu-id="f1be4-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1be4-165">DateTimeOffset</span></span>|<span data-ttu-id="f1be4-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f1be4-166">DateTime the object was created.</span></span> <span data-ttu-id="f1be4-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1be4-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1be4-168">说明</span><span class="sxs-lookup"><span data-stu-id="f1be4-168">description</span></span>|<span data-ttu-id="f1be4-169">String</span><span class="sxs-lookup"><span data-stu-id="f1be4-169">String</span></span>|<span data-ttu-id="f1be4-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f1be4-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f1be4-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1be4-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1be4-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f1be4-172">displayName</span></span>|<span data-ttu-id="f1be4-173">String</span><span class="sxs-lookup"><span data-stu-id="f1be4-173">String</span></span>|<span data-ttu-id="f1be4-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f1be4-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f1be4-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1be4-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1be4-176">version</span><span class="sxs-lookup"><span data-stu-id="f1be4-176">version</span></span>|<span data-ttu-id="f1be4-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f1be4-177">Int32</span></span>|<span data-ttu-id="f1be4-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f1be4-178">Version of the device configuration.</span></span> <span data-ttu-id="f1be4-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1be4-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1be4-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f1be4-180">authenticationMethod</span></span>|[<span data-ttu-id="f1be4-181">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f1be4-181">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="f1be4-182">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="f1be4-182">Authentication method.</span></span> <span data-ttu-id="f1be4-183">继承自 [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="f1be4-183">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="f1be4-184">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="f1be4-184">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="f1be4-185">connectionName</span><span class="sxs-lookup"><span data-stu-id="f1be4-185">connectionName</span></span>|<span data-ttu-id="f1be4-186">String</span><span class="sxs-lookup"><span data-stu-id="f1be4-186">String</span></span>|<span data-ttu-id="f1be4-187">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="f1be4-187">Connection name displayed to the user.</span></span> <span data-ttu-id="f1be4-188">继承自 [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1be4-188">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="f1be4-189">role</span><span class="sxs-lookup"><span data-stu-id="f1be4-189">role</span></span>|<span data-ttu-id="f1be4-190">String</span><span class="sxs-lookup"><span data-stu-id="f1be4-190">String</span></span>|<span data-ttu-id="f1be4-191">将连接类型设置为 Pulse Secure 时的角色。</span><span class="sxs-lookup"><span data-stu-id="f1be4-191">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f1be4-192">继承自 [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1be4-192">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="f1be4-193">realm</span><span class="sxs-lookup"><span data-stu-id="f1be4-193">realm</span></span>|<span data-ttu-id="f1be4-194">String</span><span class="sxs-lookup"><span data-stu-id="f1be4-194">String</span></span>|<span data-ttu-id="f1be4-195">将连接类型设置为 Pulse Secure 时的领域。</span><span class="sxs-lookup"><span data-stu-id="f1be4-195">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f1be4-196">继承自 [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1be4-196">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="f1be4-197">服务器</span><span class="sxs-lookup"><span data-stu-id="f1be4-197">servers</span></span>|<span data-ttu-id="f1be4-198">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1be4-198">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="f1be4-199">网络上 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="f1be4-199">List of VPN Servers on the network.</span></span> <span data-ttu-id="f1be4-200">确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="f1be4-200">Make sure end users can access these network locations.</span></span> <span data-ttu-id="f1be4-201">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="f1be4-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f1be4-202">继承自 [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1be4-202">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="f1be4-203">connectionType</span><span class="sxs-lookup"><span data-stu-id="f1be4-203">connectionType</span></span>|[<span data-ttu-id="f1be4-204">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="f1be4-204">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="f1be4-205">连接类型。</span><span class="sxs-lookup"><span data-stu-id="f1be4-205">Connection type.</span></span> <span data-ttu-id="f1be4-206">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`、`microsoftTunnel`、`netMotionMobility`、`microsoftProtect`。</span><span class="sxs-lookup"><span data-stu-id="f1be4-206">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="f1be4-207">proxyServer</span><span class="sxs-lookup"><span data-stu-id="f1be4-207">proxyServer</span></span>|[<span data-ttu-id="f1be4-208">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="f1be4-208">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="f1be4-209">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="f1be4-209">Proxy server.</span></span>|
|<span data-ttu-id="f1be4-210">targetedPackageIds</span><span class="sxs-lookup"><span data-stu-id="f1be4-210">targetedPackageIds</span></span>|<span data-ttu-id="f1be4-211">String collection</span><span class="sxs-lookup"><span data-stu-id="f1be4-211">String collection</span></span>|<span data-ttu-id="f1be4-212">目标应用包 ID。</span><span class="sxs-lookup"><span data-stu-id="f1be4-212">Targeted App package IDs.</span></span>|
|<span data-ttu-id="f1be4-213">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="f1be4-213">targetedMobileApps</span></span>|<span data-ttu-id="f1be4-214">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1be4-214">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f1be4-215">目标移动应用。</span><span class="sxs-lookup"><span data-stu-id="f1be4-215">Targeted mobile apps.</span></span> <span data-ttu-id="f1be4-216">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="f1be4-216">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f1be4-217">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="f1be4-217">alwaysOn</span></span>|<span data-ttu-id="f1be4-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1be4-218">Boolean</span></span>|<span data-ttu-id="f1be4-219">是否启用始终启用 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="f1be4-219">Whether or not to enable always-on VPN connection.</span></span>|
|<span data-ttu-id="f1be4-220">alwaysOnLockdown</span><span class="sxs-lookup"><span data-stu-id="f1be4-220">alwaysOnLockdown</span></span>|<span data-ttu-id="f1be4-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1be4-221">Boolean</span></span>|<span data-ttu-id="f1be4-222">如果始终启用 VPN 连接，是否在断开 VPN 连接时锁定网络流量。</span><span class="sxs-lookup"><span data-stu-id="f1be4-222">If always-on VPN connection is enabled, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="f1be4-223">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="f1be4-223">microsoftTunnelSiteId</span></span>|<span data-ttu-id="f1be4-224">String</span><span class="sxs-lookup"><span data-stu-id="f1be4-224">String</span></span>|<span data-ttu-id="f1be4-225">Microsoft 隧道站点 ID。</span><span class="sxs-lookup"><span data-stu-id="f1be4-225">Microsoft Tunnel site ID.</span></span>|
|<span data-ttu-id="f1be4-226">customData</span><span class="sxs-lookup"><span data-stu-id="f1be4-226">customData</span></span>|<span data-ttu-id="f1be4-227">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1be4-227">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="f1be4-228">用于定义特定于 VPN 提供程序的键/值对的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="f1be4-228">Custom data to define key/value pairs specific to a VPN provider.</span></span> <span data-ttu-id="f1be4-229">此集合最多可包含 25 个元素。</span><span class="sxs-lookup"><span data-stu-id="f1be4-229">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="f1be4-230">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="f1be4-230">customKeyValueData</span></span>|<span data-ttu-id="f1be4-231">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1be4-231">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f1be4-232">用于定义特定于 VPN 提供程序的键/值对的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="f1be4-232">Custom data to define key/value pairs specific to a VPN provider.</span></span> <span data-ttu-id="f1be4-233">此集合最多可包含 25 个元素。</span><span class="sxs-lookup"><span data-stu-id="f1be4-233">This collection can contain a maximum of 25 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f1be4-234">响应</span><span class="sxs-lookup"><span data-stu-id="f1be4-234">Response</span></span>
<span data-ttu-id="f1be4-235">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f1be4-235">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1be4-236">示例</span><span class="sxs-lookup"><span data-stu-id="f1be4-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1be4-237">请求</span><span class="sxs-lookup"><span data-stu-id="f1be4-237">Request</span></span>
<span data-ttu-id="f1be4-238">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1be4-238">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f1be4-239">响应</span><span class="sxs-lookup"><span data-stu-id="f1be4-239">Response</span></span>
<span data-ttu-id="f1be4-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f1be4-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




