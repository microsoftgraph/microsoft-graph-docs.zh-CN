---
title: 更新 androidWorkProfileVpnConfiguration
description: 更新 androidWorkProfileVpnConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0cb340181652b748cb59ea2337db6b070204739b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151582"
---
# <a name="update-androidworkprofilevpnconfiguration"></a><span data-ttu-id="42053-103">更新 androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="42053-103">Update androidWorkProfileVpnConfiguration</span></span>

<span data-ttu-id="42053-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42053-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42053-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="42053-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42053-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42053-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42053-107">更新 [androidWorkProfileVpnConfiguration 对象](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="42053-107">Update the properties of a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42053-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="42053-108">Prerequisites</span></span>
<span data-ttu-id="42053-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42053-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42053-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="42053-111">Permission type</span></span>|<span data-ttu-id="42053-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="42053-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42053-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42053-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42053-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42053-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="42053-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42053-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42053-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="42053-116">Not supported.</span></span>|
|<span data-ttu-id="42053-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="42053-117">Application</span></span>|<span data-ttu-id="42053-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42053-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42053-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42053-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="42053-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="42053-120">Request headers</span></span>
|<span data-ttu-id="42053-121">标头</span><span class="sxs-lookup"><span data-stu-id="42053-121">Header</span></span>|<span data-ttu-id="42053-122">值</span><span class="sxs-lookup"><span data-stu-id="42053-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42053-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="42053-123">Authorization</span></span>|<span data-ttu-id="42053-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="42053-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42053-125">接受</span><span class="sxs-lookup"><span data-stu-id="42053-125">Accept</span></span>|<span data-ttu-id="42053-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42053-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42053-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="42053-127">Request body</span></span>
<span data-ttu-id="42053-128">在请求正文中，提供 [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42053-128">In the request body, supply a JSON representation for the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

<span data-ttu-id="42053-129">下表显示创建 [androidWorkProfileVpnConfiguration 时所需的属性](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="42053-129">The following table shows the properties that are required when you create the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span></span>

|<span data-ttu-id="42053-130">属性</span><span class="sxs-lookup"><span data-stu-id="42053-130">Property</span></span>|<span data-ttu-id="42053-131">类型</span><span class="sxs-lookup"><span data-stu-id="42053-131">Type</span></span>|<span data-ttu-id="42053-132">说明</span><span class="sxs-lookup"><span data-stu-id="42053-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42053-133">id</span><span class="sxs-lookup"><span data-stu-id="42053-133">id</span></span>|<span data-ttu-id="42053-134">String</span><span class="sxs-lookup"><span data-stu-id="42053-134">String</span></span>|<span data-ttu-id="42053-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="42053-135">Key of the entity.</span></span> <span data-ttu-id="42053-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42053-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42053-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42053-137">lastModifiedDateTime</span></span>|<span data-ttu-id="42053-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42053-138">DateTimeOffset</span></span>|<span data-ttu-id="42053-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="42053-139">DateTime the object was last modified.</span></span> <span data-ttu-id="42053-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42053-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42053-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="42053-141">roleScopeTagIds</span></span>|<span data-ttu-id="42053-142">String collection</span><span class="sxs-lookup"><span data-stu-id="42053-142">String collection</span></span>|<span data-ttu-id="42053-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="42053-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="42053-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42053-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42053-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="42053-145">supportsScopeTags</span></span>|<span data-ttu-id="42053-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="42053-146">Boolean</span></span>|<span data-ttu-id="42053-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="42053-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="42053-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="42053-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="42053-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="42053-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="42053-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="42053-150">This property is read-only.</span></span> <span data-ttu-id="42053-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42053-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42053-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="42053-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="42053-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="42053-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="42053-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="42053-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="42053-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42053-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42053-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="42053-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="42053-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="42053-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="42053-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="42053-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="42053-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42053-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42053-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="42053-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="42053-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="42053-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="42053-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="42053-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="42053-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42053-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42053-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42053-164">createdDateTime</span></span>|<span data-ttu-id="42053-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42053-165">DateTimeOffset</span></span>|<span data-ttu-id="42053-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="42053-166">DateTime the object was created.</span></span> <span data-ttu-id="42053-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42053-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42053-168">说明</span><span class="sxs-lookup"><span data-stu-id="42053-168">description</span></span>|<span data-ttu-id="42053-169">String</span><span class="sxs-lookup"><span data-stu-id="42053-169">String</span></span>|<span data-ttu-id="42053-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="42053-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="42053-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42053-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42053-172">displayName</span><span class="sxs-lookup"><span data-stu-id="42053-172">displayName</span></span>|<span data-ttu-id="42053-173">String</span><span class="sxs-lookup"><span data-stu-id="42053-173">String</span></span>|<span data-ttu-id="42053-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="42053-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="42053-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42053-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42053-176">version</span><span class="sxs-lookup"><span data-stu-id="42053-176">version</span></span>|<span data-ttu-id="42053-177">Int32</span><span class="sxs-lookup"><span data-stu-id="42053-177">Int32</span></span>|<span data-ttu-id="42053-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="42053-178">Version of the device configuration.</span></span> <span data-ttu-id="42053-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42053-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42053-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="42053-180">connectionName</span></span>|<span data-ttu-id="42053-181">String</span><span class="sxs-lookup"><span data-stu-id="42053-181">String</span></span>|<span data-ttu-id="42053-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="42053-182">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="42053-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="42053-183">connectionType</span></span>|[<span data-ttu-id="42053-184">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="42053-184">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="42053-185">连接类型。</span><span class="sxs-lookup"><span data-stu-id="42053-185">Connection type.</span></span> <span data-ttu-id="42053-186">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`、`paloAltoGlobalProtect`、`microsoftTunnel`、`netMotionMobility`、`microsoftProtect`。</span><span class="sxs-lookup"><span data-stu-id="42053-186">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="42053-187">role</span><span class="sxs-lookup"><span data-stu-id="42053-187">role</span></span>|<span data-ttu-id="42053-188">String</span><span class="sxs-lookup"><span data-stu-id="42053-188">String</span></span>|<span data-ttu-id="42053-189">将连接类型设置为 Pulse Secure 时的角色。</span><span class="sxs-lookup"><span data-stu-id="42053-189">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="42053-190">realm</span><span class="sxs-lookup"><span data-stu-id="42053-190">realm</span></span>|<span data-ttu-id="42053-191">String</span><span class="sxs-lookup"><span data-stu-id="42053-191">String</span></span>|<span data-ttu-id="42053-192">将连接类型设置为 Pulse Secure 时的领域。</span><span class="sxs-lookup"><span data-stu-id="42053-192">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="42053-193">服务器</span><span class="sxs-lookup"><span data-stu-id="42053-193">servers</span></span>|<span data-ttu-id="42053-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) 集合</span><span class="sxs-lookup"><span data-stu-id="42053-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="42053-195">网络上 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="42053-195">List of VPN Servers on the network.</span></span> <span data-ttu-id="42053-196">确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="42053-196">Make sure end users can access these network locations.</span></span> <span data-ttu-id="42053-197">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="42053-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="42053-198">fingerprint</span><span class="sxs-lookup"><span data-stu-id="42053-198">fingerprint</span></span>|<span data-ttu-id="42053-199">String</span><span class="sxs-lookup"><span data-stu-id="42053-199">String</span></span>|<span data-ttu-id="42053-200">指纹是一个字符串，用于验证 VPN 服务器是否可信任，这仅适用于连接类型为"检查点胶囊式 VPN"时。</span><span class="sxs-lookup"><span data-stu-id="42053-200">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="42053-201">customData</span><span class="sxs-lookup"><span data-stu-id="42053-201">customData</span></span>|<span data-ttu-id="42053-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="42053-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="42053-203">连接类型设置为 Citrix 时自定义数据。</span><span class="sxs-lookup"><span data-stu-id="42053-203">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="42053-204">此集合最多可包含 25 个元素。</span><span class="sxs-lookup"><span data-stu-id="42053-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="42053-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="42053-205">customKeyValueData</span></span>|<span data-ttu-id="42053-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="42053-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="42053-207">连接类型设置为 Citrix 时自定义数据。</span><span class="sxs-lookup"><span data-stu-id="42053-207">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="42053-208">此集合最多可包含 25 个元素。</span><span class="sxs-lookup"><span data-stu-id="42053-208">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="42053-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="42053-209">authenticationMethod</span></span>|[<span data-ttu-id="42053-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="42053-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="42053-211">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="42053-211">Authentication method.</span></span> <span data-ttu-id="42053-212">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="42053-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="42053-213">proxyServer</span><span class="sxs-lookup"><span data-stu-id="42053-213">proxyServer</span></span>|[<span data-ttu-id="42053-214">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="42053-214">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="42053-215">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="42053-215">Proxy server.</span></span>|
|<span data-ttu-id="42053-216">targetedPackageIds</span><span class="sxs-lookup"><span data-stu-id="42053-216">targetedPackageIds</span></span>|<span data-ttu-id="42053-217">String collection</span><span class="sxs-lookup"><span data-stu-id="42053-217">String collection</span></span>|<span data-ttu-id="42053-218">目标应用包 ID。</span><span class="sxs-lookup"><span data-stu-id="42053-218">Targeted App package IDs.</span></span>|
|<span data-ttu-id="42053-219">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="42053-219">targetedMobileApps</span></span>|<span data-ttu-id="42053-220">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="42053-220">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="42053-221">目标移动应用。</span><span class="sxs-lookup"><span data-stu-id="42053-221">Targeted mobile apps.</span></span> <span data-ttu-id="42053-222">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="42053-222">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="42053-223">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="42053-223">alwaysOn</span></span>|<span data-ttu-id="42053-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="42053-224">Boolean</span></span>|<span data-ttu-id="42053-225">是否启用始终启用 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="42053-225">Whether or not to enable always-on VPN connection.</span></span>|
|<span data-ttu-id="42053-226">alwaysOnLockdown</span><span class="sxs-lookup"><span data-stu-id="42053-226">alwaysOnLockdown</span></span>|<span data-ttu-id="42053-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="42053-227">Boolean</span></span>|<span data-ttu-id="42053-228">如果始终启用 VPN 连接，是否在断开 VPN 连接时锁定网络流量。</span><span class="sxs-lookup"><span data-stu-id="42053-228">If always-on VPN connection is enabled, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="42053-229">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="42053-229">microsoftTunnelSiteId</span></span>|<span data-ttu-id="42053-230">String</span><span class="sxs-lookup"><span data-stu-id="42053-230">String</span></span>|<span data-ttu-id="42053-231">Microsoft 隧道站点 ID。</span><span class="sxs-lookup"><span data-stu-id="42053-231">Microsoft Tunnel site ID.</span></span>|



## <a name="response"></a><span data-ttu-id="42053-232">响应</span><span class="sxs-lookup"><span data-stu-id="42053-232">Response</span></span>
<span data-ttu-id="42053-233">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="42053-233">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42053-234">示例</span><span class="sxs-lookup"><span data-stu-id="42053-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="42053-235">请求</span><span class="sxs-lookup"><span data-stu-id="42053-235">Request</span></span>
<span data-ttu-id="42053-236">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="42053-236">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="42053-237">响应</span><span class="sxs-lookup"><span data-stu-id="42053-237">Response</span></span>
<span data-ttu-id="42053-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="42053-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




