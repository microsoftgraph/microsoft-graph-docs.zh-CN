---
title: 更新 macOSVpnConfiguration
description: 更新 macOSVpnConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ba55a346a2e597bfdce4d74e20df5eb5b671ab9c
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866529"
---
# <a name="update-macosvpnconfiguration"></a><span data-ttu-id="c2b0d-103">更新 macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c2b0d-103">Update macOSVpnConfiguration</span></span>

<span data-ttu-id="c2b0d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2b0d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2b0d-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2b0d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2b0d-107">更新 [macOSVpnConfiguration 对象](../resources/intune-deviceconfig-macosvpnconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-107">Update the properties of a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2b0d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c2b0d-108">Prerequisites</span></span>
<span data-ttu-id="c2b0d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2b0d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2b0d-111">Permission type</span></span>|<span data-ttu-id="c2b0d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2b0d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2b0d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2b0d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2b0d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2b0d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c2b0d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2b0d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2b0d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-116">Not supported.</span></span>|
|<span data-ttu-id="c2b0d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2b0d-117">Application</span></span>|<span data-ttu-id="c2b0d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2b0d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2b0d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2b0d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c2b0d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2b0d-120">Request headers</span></span>
|<span data-ttu-id="c2b0d-121">标头</span><span class="sxs-lookup"><span data-stu-id="c2b0d-121">Header</span></span>|<span data-ttu-id="c2b0d-122">值</span><span class="sxs-lookup"><span data-stu-id="c2b0d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2b0d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2b0d-123">Authorization</span></span>|<span data-ttu-id="c2b0d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2b0d-125">接受</span><span class="sxs-lookup"><span data-stu-id="c2b0d-125">Accept</span></span>|<span data-ttu-id="c2b0d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2b0d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2b0d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2b0d-127">Request body</span></span>
<span data-ttu-id="c2b0d-128">在请求正文中，提供 [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-128">In the request body, supply a JSON representation for the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="c2b0d-129">下表显示创建 [macOSVpnConfiguration 时所需的属性](../resources/intune-deviceconfig-macosvpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-129">The following table shows the properties that are required when you create the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

|<span data-ttu-id="c2b0d-130">属性</span><span class="sxs-lookup"><span data-stu-id="c2b0d-130">Property</span></span>|<span data-ttu-id="c2b0d-131">类型</span><span class="sxs-lookup"><span data-stu-id="c2b0d-131">Type</span></span>|<span data-ttu-id="c2b0d-132">说明</span><span class="sxs-lookup"><span data-stu-id="c2b0d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2b0d-133">id</span><span class="sxs-lookup"><span data-stu-id="c2b0d-133">id</span></span>|<span data-ttu-id="c2b0d-134">String</span><span class="sxs-lookup"><span data-stu-id="c2b0d-134">String</span></span>|<span data-ttu-id="c2b0d-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-135">Key of the entity.</span></span> <span data-ttu-id="c2b0d-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2b0d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c2b0d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2b0d-138">DateTimeOffset</span></span>|<span data-ttu-id="c2b0d-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c2b0d-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c2b0d-141">roleScopeTagIds</span></span>|<span data-ttu-id="c2b0d-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="c2b0d-142">String collection</span></span>|<span data-ttu-id="c2b0d-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c2b0d-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c2b0d-145">supportsScopeTags</span></span>|<span data-ttu-id="c2b0d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2b0d-146">Boolean</span></span>|<span data-ttu-id="c2b0d-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c2b0d-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c2b0d-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c2b0d-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-150">This property is read-only.</span></span> <span data-ttu-id="c2b0d-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c2b0d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c2b0d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c2b0d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c2b0d-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c2b0d-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c2b0d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c2b0d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c2b0d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c2b0d-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c2b0d-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c2b0d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c2b0d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c2b0d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c2b0d-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c2b0d-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c2b0d-164">createdDateTime</span></span>|<span data-ttu-id="c2b0d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2b0d-165">DateTimeOffset</span></span>|<span data-ttu-id="c2b0d-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-166">DateTime the object was created.</span></span> <span data-ttu-id="c2b0d-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-168">说明</span><span class="sxs-lookup"><span data-stu-id="c2b0d-168">description</span></span>|<span data-ttu-id="c2b0d-169">String</span><span class="sxs-lookup"><span data-stu-id="c2b0d-169">String</span></span>|<span data-ttu-id="c2b0d-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c2b0d-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c2b0d-172">displayName</span></span>|<span data-ttu-id="c2b0d-173">String</span><span class="sxs-lookup"><span data-stu-id="c2b0d-173">String</span></span>|<span data-ttu-id="c2b0d-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c2b0d-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-176">version</span><span class="sxs-lookup"><span data-stu-id="c2b0d-176">version</span></span>|<span data-ttu-id="c2b0d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c2b0d-177">Int32</span></span>|<span data-ttu-id="c2b0d-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-178">Version of the device configuration.</span></span> <span data-ttu-id="c2b0d-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="c2b0d-180">connectionName</span></span>|<span data-ttu-id="c2b0d-181">String</span><span class="sxs-lookup"><span data-stu-id="c2b0d-181">String</span></span>|<span data-ttu-id="c2b0d-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-182">Connection name displayed to the user.</span></span> <span data-ttu-id="c2b0d-183">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="c2b0d-184">connectionType</span></span>|[<span data-ttu-id="c2b0d-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="c2b0d-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="c2b0d-186">连接类型。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-186">Connection type.</span></span> <span data-ttu-id="c2b0d-187">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="c2b0d-188">可能的值是 `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` ：、、、、、、、、 `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` 。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="c2b0d-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="c2b0d-189">loginGroupOrDomain</span></span>|<span data-ttu-id="c2b0d-190">String</span><span class="sxs-lookup"><span data-stu-id="c2b0d-190">String</span></span>|<span data-ttu-id="c2b0d-191">连接类型设置为 Dell SonicWALL 移动连接时登录组或域。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="c2b0d-192">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-193">role</span><span class="sxs-lookup"><span data-stu-id="c2b0d-193">role</span></span>|<span data-ttu-id="c2b0d-194">String</span><span class="sxs-lookup"><span data-stu-id="c2b0d-194">String</span></span>|<span data-ttu-id="c2b0d-195">将连接类型设置为 Pulse Secure 时的角色。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="c2b0d-196">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-197">realm</span><span class="sxs-lookup"><span data-stu-id="c2b0d-197">realm</span></span>|<span data-ttu-id="c2b0d-198">String</span><span class="sxs-lookup"><span data-stu-id="c2b0d-198">String</span></span>|<span data-ttu-id="c2b0d-199">将连接类型设置为 Pulse Secure 时的领域。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="c2b0d-200">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-201">server</span><span class="sxs-lookup"><span data-stu-id="c2b0d-201">server</span></span>|[<span data-ttu-id="c2b0d-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="c2b0d-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="c2b0d-203">VPN 服务器。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-203">VPN Server on the network.</span></span> <span data-ttu-id="c2b0d-204">确保最终用户可以访问此网络位置。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="c2b0d-205">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-206">标识符</span><span class="sxs-lookup"><span data-stu-id="c2b0d-206">identifier</span></span>|<span data-ttu-id="c2b0d-207">String</span><span class="sxs-lookup"><span data-stu-id="c2b0d-207">String</span></span>|<span data-ttu-id="c2b0d-208">连接类型设置为自定义 VPN 时 VPN 供应商提供的标识符。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="c2b0d-209">例如：Cisco AnyConnect 使用 com.cisco.anyconnect.applevpn.plugin 形式的标识符 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-210">customData</span><span class="sxs-lookup"><span data-stu-id="c2b0d-210">customData</span></span>|<span data-ttu-id="c2b0d-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c2b0d-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="c2b0d-212">连接类型设置为自定义 VPN 时自定义数据。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="c2b0d-213">使用此字段启用 Intune 不支持但在 VPN 解决方案中提供的功能。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="c2b0d-214">请联系 VPN 供应商，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="c2b0d-215">此集合最多可包含 25 个元素。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="c2b0d-216">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="c2b0d-217">customKeyValueData</span></span>|<span data-ttu-id="c2b0d-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c2b0d-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c2b0d-219">连接类型设置为自定义 VPN 时自定义数据。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="c2b0d-220">使用此字段启用 Intune 不支持但在 VPN 解决方案中提供的功能。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="c2b0d-221">请联系 VPN 供应商，了解如何添加这些键/值对。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="c2b0d-222">此集合最多可包含 25 个元素。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="c2b0d-223">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="c2b0d-224">enableSplitTunneling</span></span>|<span data-ttu-id="c2b0d-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2b0d-225">Boolean</span></span>|<span data-ttu-id="c2b0d-226">通过 VPN 发送所有网络流量。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="c2b0d-227">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c2b0d-228">authenticationMethod</span></span>|[<span data-ttu-id="c2b0d-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c2b0d-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="c2b0d-230">此 VPN 连接的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="c2b0d-231">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="c2b0d-232">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="c2b0d-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="c2b0d-233">enablePerApp</span></span>|<span data-ttu-id="c2b0d-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2b0d-234">Boolean</span></span>|<span data-ttu-id="c2b0d-235">如果设置为 true，Per-App VPN 有效负载，稍后可关联到可在最终用户的 iOS 设备上触发此 VPN 连接的应用。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="c2b0d-236">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="c2b0d-237">safariDomains</span></span>|<span data-ttu-id="c2b0d-238">String 集合</span><span class="sxs-lookup"><span data-stu-id="c2b0d-238">String collection</span></span>|<span data-ttu-id="c2b0d-239">启用"每个应用此 VPN"设置时，Safari 域。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="c2b0d-240">除了与此 VPN 关联的应用之外，此处指定的 Safari 域还将能够触发此 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="c2b0d-241">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="c2b0d-242">onDemandRules</span></span>|<span data-ttu-id="c2b0d-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c2b0d-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="c2b0d-244">按需规则。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-244">On-Demand Rules.</span></span> <span data-ttu-id="c2b0d-245">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c2b0d-246">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-247">providerType</span><span class="sxs-lookup"><span data-stu-id="c2b0d-247">providerType</span></span>|[<span data-ttu-id="c2b0d-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="c2b0d-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="c2b0d-249">每个应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="c2b0d-250">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="c2b0d-251">可取值为：`notConfigured`、`appProxy`、`packetTunnel`。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="c2b0d-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="c2b0d-252">associatedDomains</span></span>|<span data-ttu-id="c2b0d-253">String 集合</span><span class="sxs-lookup"><span data-stu-id="c2b0d-253">String collection</span></span>|<span data-ttu-id="c2b0d-254">关联域 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="c2b0d-255">excludedDomains</span></span>|<span data-ttu-id="c2b0d-256">String 集合</span><span class="sxs-lookup"><span data-stu-id="c2b0d-256">String collection</span></span>|<span data-ttu-id="c2b0d-257">通过公共 Internet 而不是 VPN 访问的域，即使已激活每应用 VPN 也是如此。继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="c2b0d-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="c2b0d-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2b0d-259">Boolean</span></span>|<span data-ttu-id="c2b0d-260">切换以阻止用户在"设置"应用中禁用自动 VPN 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-261">disconnectOnIdle</span><span class="sxs-lookup"><span data-stu-id="c2b0d-261">disconnectOnIdle</span></span>|<span data-ttu-id="c2b0d-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2b0d-262">Boolean</span></span>|<span data-ttu-id="c2b0d-263">是否在按需连接空闲后断开连接 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-263">Whether to disconnect after on-demand connection idles Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-264">disconnectOnIdleTimerInSeconds</span><span class="sxs-lookup"><span data-stu-id="c2b0d-264">disconnectOnIdleTimerInSeconds</span></span>|<span data-ttu-id="c2b0d-265">Int32</span><span class="sxs-lookup"><span data-stu-id="c2b0d-265">Int32</span></span>|<span data-ttu-id="c2b0d-266">断开按需连接之前要等待的时间长度（秒）。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-266">The length of time in seconds to wait before disconnecting an on-demand connection.</span></span> <span data-ttu-id="c2b0d-267">有效值 0 至 65535 继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-267">Valid values 0 to 65535 Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-268">proxyServer</span><span class="sxs-lookup"><span data-stu-id="c2b0d-268">proxyServer</span></span>|[<span data-ttu-id="c2b0d-269">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="c2b0d-269">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="c2b0d-270">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-270">Proxy Server.</span></span> <span data-ttu-id="c2b0d-271">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-271">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2b0d-272">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="c2b0d-272">optInToDeviceIdSharing</span></span>|<span data-ttu-id="c2b0d-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2b0d-273">Boolean</span></span>|<span data-ttu-id="c2b0d-274">Opt-In将设备 ID 共享给第三方 vpn 客户端，以在网络访问控制验证期间使用。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-274">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="c2b0d-275">继承自 [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-275">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c2b0d-276">响应</span><span class="sxs-lookup"><span data-stu-id="c2b0d-276">Response</span></span>
<span data-ttu-id="c2b0d-277">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-277">If successful, this method returns a `200 OK` response code and an updated [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2b0d-278">示例</span><span class="sxs-lookup"><span data-stu-id="c2b0d-278">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2b0d-279">请求</span><span class="sxs-lookup"><span data-stu-id="c2b0d-279">Request</span></span>
<span data-ttu-id="c2b0d-280">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-280">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="c2b0d-281">响应</span><span class="sxs-lookup"><span data-stu-id="c2b0d-281">Response</span></span>
<span data-ttu-id="c2b0d-p131">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




