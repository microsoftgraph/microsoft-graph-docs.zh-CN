---
title: 创建 macOSVpnConfiguration
description: 创建新的 macOSVpnConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5668b8d553c4b4e9fb40628934e1e4bb572dd90a
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865325"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="794b7-103">创建 macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="794b7-103">Create macOSVpnConfiguration</span></span>

<span data-ttu-id="794b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="794b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="794b7-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="794b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="794b7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="794b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="794b7-107">创建新的 [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="794b7-107">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="794b7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="794b7-108">Prerequisites</span></span>
<span data-ttu-id="794b7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="794b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="794b7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="794b7-111">Permission type</span></span>|<span data-ttu-id="794b7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="794b7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="794b7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="794b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="794b7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="794b7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="794b7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="794b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="794b7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="794b7-116">Not supported.</span></span>|
|<span data-ttu-id="794b7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="794b7-117">Application</span></span>|<span data-ttu-id="794b7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="794b7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="794b7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="794b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="794b7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="794b7-120">Request headers</span></span>
|<span data-ttu-id="794b7-121">标头</span><span class="sxs-lookup"><span data-stu-id="794b7-121">Header</span></span>|<span data-ttu-id="794b7-122">值</span><span class="sxs-lookup"><span data-stu-id="794b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="794b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="794b7-123">Authorization</span></span>|<span data-ttu-id="794b7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="794b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="794b7-125">接受</span><span class="sxs-lookup"><span data-stu-id="794b7-125">Accept</span></span>|<span data-ttu-id="794b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="794b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="794b7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="794b7-127">Request body</span></span>
<span data-ttu-id="794b7-128">在请求正文中，提供 macOSVpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="794b7-128">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="794b7-129">下表显示创建 macOSVpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="794b7-129">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="794b7-130">属性</span><span class="sxs-lookup"><span data-stu-id="794b7-130">Property</span></span>|<span data-ttu-id="794b7-131">类型</span><span class="sxs-lookup"><span data-stu-id="794b7-131">Type</span></span>|<span data-ttu-id="794b7-132">说明</span><span class="sxs-lookup"><span data-stu-id="794b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="794b7-133">id</span><span class="sxs-lookup"><span data-stu-id="794b7-133">id</span></span>|<span data-ttu-id="794b7-134">String</span><span class="sxs-lookup"><span data-stu-id="794b7-134">String</span></span>|<span data-ttu-id="794b7-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="794b7-135">Key of the entity.</span></span> <span data-ttu-id="794b7-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="794b7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="794b7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="794b7-138">DateTimeOffset</span></span>|<span data-ttu-id="794b7-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="794b7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="794b7-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="794b7-141">roleScopeTagIds</span></span>|<span data-ttu-id="794b7-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="794b7-142">String collection</span></span>|<span data-ttu-id="794b7-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="794b7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="794b7-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="794b7-145">supportsScopeTags</span></span>|<span data-ttu-id="794b7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="794b7-146">Boolean</span></span>|<span data-ttu-id="794b7-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="794b7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="794b7-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="794b7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="794b7-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="794b7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="794b7-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="794b7-150">This property is read-only.</span></span> <span data-ttu-id="794b7-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="794b7-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="794b7-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="794b7-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="794b7-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="794b7-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="794b7-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="794b7-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="794b7-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="794b7-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="794b7-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="794b7-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="794b7-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="794b7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="794b7-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="794b7-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="794b7-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="794b7-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="794b7-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="794b7-164">createdDateTime</span></span>|<span data-ttu-id="794b7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="794b7-165">DateTimeOffset</span></span>|<span data-ttu-id="794b7-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="794b7-166">DateTime the object was created.</span></span> <span data-ttu-id="794b7-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-168">说明</span><span class="sxs-lookup"><span data-stu-id="794b7-168">description</span></span>|<span data-ttu-id="794b7-169">String</span><span class="sxs-lookup"><span data-stu-id="794b7-169">String</span></span>|<span data-ttu-id="794b7-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="794b7-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="794b7-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-172">displayName</span><span class="sxs-lookup"><span data-stu-id="794b7-172">displayName</span></span>|<span data-ttu-id="794b7-173">String</span><span class="sxs-lookup"><span data-stu-id="794b7-173">String</span></span>|<span data-ttu-id="794b7-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="794b7-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="794b7-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-176">version</span><span class="sxs-lookup"><span data-stu-id="794b7-176">version</span></span>|<span data-ttu-id="794b7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="794b7-177">Int32</span></span>|<span data-ttu-id="794b7-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="794b7-178">Version of the device configuration.</span></span> <span data-ttu-id="794b7-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="794b7-180">connectionName</span></span>|<span data-ttu-id="794b7-181">String</span><span class="sxs-lookup"><span data-stu-id="794b7-181">String</span></span>|<span data-ttu-id="794b7-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="794b7-182">Connection name displayed to the user.</span></span> <span data-ttu-id="794b7-183">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="794b7-184">connectionType</span></span>|[<span data-ttu-id="794b7-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="794b7-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="794b7-186">连接类型。</span><span class="sxs-lookup"><span data-stu-id="794b7-186">Connection type.</span></span> <span data-ttu-id="794b7-187">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="794b7-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="794b7-188">可能的值是 `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` ：、、、、、、、、 `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` 。</span><span class="sxs-lookup"><span data-stu-id="794b7-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="794b7-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="794b7-189">loginGroupOrDomain</span></span>|<span data-ttu-id="794b7-190">String</span><span class="sxs-lookup"><span data-stu-id="794b7-190">String</span></span>|<span data-ttu-id="794b7-191">连接类型设置为 Dell SonicWALL 移动连接时登录组或域。</span><span class="sxs-lookup"><span data-stu-id="794b7-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="794b7-192">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-193">role</span><span class="sxs-lookup"><span data-stu-id="794b7-193">role</span></span>|<span data-ttu-id="794b7-194">String</span><span class="sxs-lookup"><span data-stu-id="794b7-194">String</span></span>|<span data-ttu-id="794b7-195">将连接类型设置为 Pulse Secure 时的角色。</span><span class="sxs-lookup"><span data-stu-id="794b7-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="794b7-196">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-197">realm</span><span class="sxs-lookup"><span data-stu-id="794b7-197">realm</span></span>|<span data-ttu-id="794b7-198">String</span><span class="sxs-lookup"><span data-stu-id="794b7-198">String</span></span>|<span data-ttu-id="794b7-199">将连接类型设置为 Pulse Secure 时的领域。</span><span class="sxs-lookup"><span data-stu-id="794b7-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="794b7-200">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-201">server</span><span class="sxs-lookup"><span data-stu-id="794b7-201">server</span></span>|[<span data-ttu-id="794b7-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="794b7-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="794b7-203">VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="794b7-203">VPN Server on the network.</span></span> <span data-ttu-id="794b7-204">确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="794b7-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="794b7-205">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-206">标识符</span><span class="sxs-lookup"><span data-stu-id="794b7-206">identifier</span></span>|<span data-ttu-id="794b7-207">String</span><span class="sxs-lookup"><span data-stu-id="794b7-207">String</span></span>|<span data-ttu-id="794b7-208">连接类型设置为自定义 VPN 时 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="794b7-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="794b7-209">例如：Cisco AnyConnect 使用 com.cisco.anyconnect.applevpn.plugin 形式的标识符 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-210">customData</span><span class="sxs-lookup"><span data-stu-id="794b7-210">customData</span></span>|<span data-ttu-id="794b7-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="794b7-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="794b7-212">连接类型设置为自定义 VPN 时自定义数据。</span><span class="sxs-lookup"><span data-stu-id="794b7-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="794b7-213">使用此字段启用 Intune 不支持但在 VPN 解决方案中提供的功能。</span><span class="sxs-lookup"><span data-stu-id="794b7-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="794b7-214">请联系 VPN 供应商，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="794b7-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="794b7-215">此集合最多可包含 25 个元素。</span><span class="sxs-lookup"><span data-stu-id="794b7-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="794b7-216">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="794b7-217">customKeyValueData</span></span>|<span data-ttu-id="794b7-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="794b7-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="794b7-219">连接类型设置为自定义 VPN 时自定义数据。</span><span class="sxs-lookup"><span data-stu-id="794b7-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="794b7-220">使用此字段启用 Intune 不支持但在 VPN 解决方案中提供的功能。</span><span class="sxs-lookup"><span data-stu-id="794b7-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="794b7-221">请联系 VPN 供应商，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="794b7-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="794b7-222">此集合最多可包含 25 个元素。</span><span class="sxs-lookup"><span data-stu-id="794b7-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="794b7-223">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="794b7-224">enableSplitTunneling</span></span>|<span data-ttu-id="794b7-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="794b7-225">Boolean</span></span>|<span data-ttu-id="794b7-226">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="794b7-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="794b7-227">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="794b7-228">authenticationMethod</span></span>|[<span data-ttu-id="794b7-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="794b7-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="794b7-230">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="794b7-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="794b7-231">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="794b7-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="794b7-232">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="794b7-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="794b7-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="794b7-233">enablePerApp</span></span>|<span data-ttu-id="794b7-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="794b7-234">Boolean</span></span>|<span data-ttu-id="794b7-235">如果设置为 true，Per-App VPN 有效负载，稍后可关联到可在最终用户的 iOS 设备上触发此 VPN 连接的应用。</span><span class="sxs-lookup"><span data-stu-id="794b7-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="794b7-236">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="794b7-237">safariDomains</span></span>|<span data-ttu-id="794b7-238">String 集合</span><span class="sxs-lookup"><span data-stu-id="794b7-238">String collection</span></span>|<span data-ttu-id="794b7-239">启用"每个应用此 VPN"设置时，Safari 域。</span><span class="sxs-lookup"><span data-stu-id="794b7-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="794b7-240">除了与此 VPN 关联的应用之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="794b7-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="794b7-241">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="794b7-242">onDemandRules</span></span>|<span data-ttu-id="794b7-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="794b7-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="794b7-244">按需规则。</span><span class="sxs-lookup"><span data-stu-id="794b7-244">On-Demand Rules.</span></span> <span data-ttu-id="794b7-245">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="794b7-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="794b7-246">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-247">providerType</span><span class="sxs-lookup"><span data-stu-id="794b7-247">providerType</span></span>|[<span data-ttu-id="794b7-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="794b7-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="794b7-249">每个应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="794b7-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="794b7-250">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="794b7-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="794b7-251">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="794b7-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="794b7-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="794b7-252">associatedDomains</span></span>|<span data-ttu-id="794b7-253">String 集合</span><span class="sxs-lookup"><span data-stu-id="794b7-253">String collection</span></span>|<span data-ttu-id="794b7-254">关联域 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="794b7-255">excludedDomains</span></span>|<span data-ttu-id="794b7-256">String 集合</span><span class="sxs-lookup"><span data-stu-id="794b7-256">String collection</span></span>|<span data-ttu-id="794b7-257">通过公共 Internet 而不是 VPN 访问的域，即使已激活每应用 VPN 也是如此。继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="794b7-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="794b7-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="794b7-259">Boolean</span></span>|<span data-ttu-id="794b7-260">切换以阻止用户在"设置"应用中禁用自动 VPN 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-261">disconnectOnIdle</span><span class="sxs-lookup"><span data-stu-id="794b7-261">disconnectOnIdle</span></span>|<span data-ttu-id="794b7-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="794b7-262">Boolean</span></span>|<span data-ttu-id="794b7-263">是否在按需连接空闲后断开连接 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-263">Whether to disconnect after on-demand connection idles Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-264">disconnectOnIdleTimerInSeconds</span><span class="sxs-lookup"><span data-stu-id="794b7-264">disconnectOnIdleTimerInSeconds</span></span>|<span data-ttu-id="794b7-265">Int32</span><span class="sxs-lookup"><span data-stu-id="794b7-265">Int32</span></span>|<span data-ttu-id="794b7-266">断开按需连接之前要等待的时间长度（秒）。</span><span class="sxs-lookup"><span data-stu-id="794b7-266">The length of time in seconds to wait before disconnecting an on-demand connection.</span></span> <span data-ttu-id="794b7-267">有效值 0 至 65535 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-267">Valid values 0 to 65535 Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-268">proxyServer</span><span class="sxs-lookup"><span data-stu-id="794b7-268">proxyServer</span></span>|[<span data-ttu-id="794b7-269">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="794b7-269">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="794b7-270">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="794b7-270">Proxy Server.</span></span> <span data-ttu-id="794b7-271">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-271">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="794b7-272">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="794b7-272">optInToDeviceIdSharing</span></span>|<span data-ttu-id="794b7-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="794b7-273">Boolean</span></span>|<span data-ttu-id="794b7-274">Opt-In将设备 ID 共享给第三方 vpn 客户端，以在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="794b7-274">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="794b7-275">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="794b7-275">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="794b7-276">响应</span><span class="sxs-lookup"><span data-stu-id="794b7-276">Response</span></span>
<span data-ttu-id="794b7-277">如果成功，此方法在响应 `201 Created` 正文中返回 响应 [代码和 macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="794b7-277">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="794b7-278">示例</span><span class="sxs-lookup"><span data-stu-id="794b7-278">Example</span></span>

### <a name="request"></a><span data-ttu-id="794b7-279">请求</span><span class="sxs-lookup"><span data-stu-id="794b7-279">Request</span></span>
<span data-ttu-id="794b7-280">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="794b7-280">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2895

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
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
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
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
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "providerType": "appProxy",
  "associatedDomains": [
    "Associated Domains value"
  ],
  "excludedDomains": [
    "Excluded Domains value"
  ],
  "disableOnDemandUserOverride": true,
  "disconnectOnIdle": true,
  "disconnectOnIdleTimerInSeconds": 14,
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true
}
```

### <a name="response"></a><span data-ttu-id="794b7-281">响应</span><span class="sxs-lookup"><span data-stu-id="794b7-281">Response</span></span>
<span data-ttu-id="794b7-p131">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="794b7-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3067

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "id": "8ce00178-0178-8ce0-7801-e08c7801e08c",
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
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
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
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "providerType": "appProxy",
  "associatedDomains": [
    "Associated Domains value"
  ],
  "excludedDomains": [
    "Excluded Domains value"
  ],
  "disableOnDemandUserOverride": true,
  "disconnectOnIdle": true,
  "disconnectOnIdleTimerInSeconds": 14,
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true
}
```




