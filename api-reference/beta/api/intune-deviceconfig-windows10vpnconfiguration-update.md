---
title: 更新 windows10VpnConfiguration
description: 更新 windows10VpnConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4da9793c58dcd93c1944fb2953964124aa5812a1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435019"
---
# <a name="update-windows10vpnconfiguration"></a><span data-ttu-id="8a627-103">更新 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="8a627-103">Update windows10VpnConfiguration</span></span>

<span data-ttu-id="8a627-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a627-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a627-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8a627-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a627-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8a627-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a627-107">更新 [windows10VpnConfiguration 对象](../resources/intune-deviceconfig-windows10vpnconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="8a627-107">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a627-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8a627-108">Prerequisites</span></span>
<span data-ttu-id="8a627-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a627-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a627-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a627-111">Permission type</span></span>|<span data-ttu-id="8a627-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8a627-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a627-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a627-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a627-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a627-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8a627-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a627-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a627-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a627-116">Not supported.</span></span>|
|<span data-ttu-id="8a627-117">Application</span><span class="sxs-lookup"><span data-stu-id="8a627-117">Application</span></span>|<span data-ttu-id="8a627-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a627-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a627-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a627-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8a627-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a627-120">Request headers</span></span>
|<span data-ttu-id="8a627-121">标头</span><span class="sxs-lookup"><span data-stu-id="8a627-121">Header</span></span>|<span data-ttu-id="8a627-122">值</span><span class="sxs-lookup"><span data-stu-id="8a627-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a627-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a627-123">Authorization</span></span>|<span data-ttu-id="8a627-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8a627-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a627-125">接受</span><span class="sxs-lookup"><span data-stu-id="8a627-125">Accept</span></span>|<span data-ttu-id="8a627-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a627-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a627-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a627-127">Request body</span></span>
<span data-ttu-id="8a627-128">在请求正文中，提供 [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a627-128">In the request body, supply a JSON representation for the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

<span data-ttu-id="8a627-129">下表显示创建 [windows10VpnConfiguration 时所需的属性](../resources/intune-deviceconfig-windows10vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="8a627-129">The following table shows the properties that are required when you create the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>

|<span data-ttu-id="8a627-130">属性</span><span class="sxs-lookup"><span data-stu-id="8a627-130">Property</span></span>|<span data-ttu-id="8a627-131">类型</span><span class="sxs-lookup"><span data-stu-id="8a627-131">Type</span></span>|<span data-ttu-id="8a627-132">说明</span><span class="sxs-lookup"><span data-stu-id="8a627-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a627-133">id</span><span class="sxs-lookup"><span data-stu-id="8a627-133">id</span></span>|<span data-ttu-id="8a627-134">String</span><span class="sxs-lookup"><span data-stu-id="8a627-134">String</span></span>|<span data-ttu-id="8a627-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8a627-135">Key of the entity.</span></span> <span data-ttu-id="8a627-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a627-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a627-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a627-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8a627-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a627-138">DateTimeOffset</span></span>|<span data-ttu-id="8a627-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8a627-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8a627-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a627-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a627-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8a627-141">roleScopeTagIds</span></span>|<span data-ttu-id="8a627-142">字符串集合</span><span class="sxs-lookup"><span data-stu-id="8a627-142">String collection</span></span>|<span data-ttu-id="8a627-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="8a627-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8a627-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a627-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a627-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8a627-145">supportsScopeTags</span></span>|<span data-ttu-id="8a627-146">布尔</span><span class="sxs-lookup"><span data-stu-id="8a627-146">Boolean</span></span>|<span data-ttu-id="8a627-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="8a627-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8a627-148">当此值为 false 且实体对范围用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="8a627-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8a627-149">对于在 Silverlight 中创建的旧策略，会发生此情况，可通过在 Azure 门户中删除和重新创建策略来解决此问题。</span><span class="sxs-lookup"><span data-stu-id="8a627-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8a627-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8a627-150">This property is read-only.</span></span> <span data-ttu-id="8a627-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a627-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a627-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8a627-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8a627-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8a627-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8a627-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="8a627-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8a627-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a627-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a627-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8a627-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8a627-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8a627-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8a627-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="8a627-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8a627-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a627-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a627-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8a627-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8a627-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8a627-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8a627-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="8a627-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8a627-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a627-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a627-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a627-164">createdDateTime</span></span>|<span data-ttu-id="8a627-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a627-165">DateTimeOffset</span></span>|<span data-ttu-id="8a627-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8a627-166">DateTime the object was created.</span></span> <span data-ttu-id="8a627-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a627-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a627-168">说明</span><span class="sxs-lookup"><span data-stu-id="8a627-168">description</span></span>|<span data-ttu-id="8a627-169">String</span><span class="sxs-lookup"><span data-stu-id="8a627-169">String</span></span>|<span data-ttu-id="8a627-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="8a627-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8a627-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a627-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a627-172">displayName</span><span class="sxs-lookup"><span data-stu-id="8a627-172">displayName</span></span>|<span data-ttu-id="8a627-173">String</span><span class="sxs-lookup"><span data-stu-id="8a627-173">String</span></span>|<span data-ttu-id="8a627-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="8a627-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8a627-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a627-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a627-176">version</span><span class="sxs-lookup"><span data-stu-id="8a627-176">version</span></span>|<span data-ttu-id="8a627-177">Int32</span><span class="sxs-lookup"><span data-stu-id="8a627-177">Int32</span></span>|<span data-ttu-id="8a627-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="8a627-178">Version of the device configuration.</span></span> <span data-ttu-id="8a627-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a627-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a627-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="8a627-180">connectionName</span></span>|<span data-ttu-id="8a627-181">String</span><span class="sxs-lookup"><span data-stu-id="8a627-181">String</span></span>|<span data-ttu-id="8a627-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="8a627-182">Connection name displayed to the user.</span></span> <span data-ttu-id="8a627-183">继承自 [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a627-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="8a627-184">服务器</span><span class="sxs-lookup"><span data-stu-id="8a627-184">servers</span></span>|<span data-ttu-id="8a627-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a627-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="8a627-186">网络上 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="8a627-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="8a627-187">确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="8a627-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="8a627-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="8a627-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="8a627-189">继承自 [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a627-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="8a627-190">customXml</span><span class="sxs-lookup"><span data-stu-id="8a627-190">customXml</span></span>|<span data-ttu-id="8a627-191">Binary</span><span class="sxs-lookup"><span data-stu-id="8a627-191">Binary</span></span>|<span data-ttu-id="8a627-192">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="8a627-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="8a627-193"> (UTF8 编码的字节数组) 继承自 [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a627-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="8a627-194">profileTarget</span><span class="sxs-lookup"><span data-stu-id="8a627-194">profileTarget</span></span>|[<span data-ttu-id="8a627-195">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="8a627-195">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="8a627-196">配置文件目标类型。</span><span class="sxs-lookup"><span data-stu-id="8a627-196">Profile target type.</span></span> <span data-ttu-id="8a627-197">可取值为：`user`、`device`、`autoPilotDevice`。</span><span class="sxs-lookup"><span data-stu-id="8a627-197">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="8a627-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="8a627-198">connectionType</span></span>|[<span data-ttu-id="8a627-199">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="8a627-199">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="8a627-200">连接类型。</span><span class="sxs-lookup"><span data-stu-id="8a627-200">Connection type.</span></span> <span data-ttu-id="8a627-201">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect`、`ciscoAnyConnect`。</span><span class="sxs-lookup"><span data-stu-id="8a627-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`, `ciscoAnyConnect`.</span></span>|
|<span data-ttu-id="8a627-202">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="8a627-202">enableSplitTunneling</span></span>|<span data-ttu-id="8a627-203">布尔</span><span class="sxs-lookup"><span data-stu-id="8a627-203">Boolean</span></span>|<span data-ttu-id="8a627-204">启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="8a627-204">Enable split tunneling.</span></span>|
|<span data-ttu-id="8a627-205">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="8a627-205">enableAlwaysOn</span></span>|<span data-ttu-id="8a627-206">布尔</span><span class="sxs-lookup"><span data-stu-id="8a627-206">Boolean</span></span>|<span data-ttu-id="8a627-207">启用 Always On 模式。</span><span class="sxs-lookup"><span data-stu-id="8a627-207">Enable Always On mode.</span></span>|
|<span data-ttu-id="8a627-208">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="8a627-208">enableDeviceTunnel</span></span>|<span data-ttu-id="8a627-209">布尔</span><span class="sxs-lookup"><span data-stu-id="8a627-209">Boolean</span></span>|<span data-ttu-id="8a627-210">启用设备隧道。</span><span class="sxs-lookup"><span data-stu-id="8a627-210">Enable device tunnel.</span></span>|
|<span data-ttu-id="8a627-211">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="8a627-211">enableDnsRegistration</span></span>|<span data-ttu-id="8a627-212">布尔</span><span class="sxs-lookup"><span data-stu-id="8a627-212">Boolean</span></span>|<span data-ttu-id="8a627-213">使用内部 DNS 启用 IP 地址注册。</span><span class="sxs-lookup"><span data-stu-id="8a627-213">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="8a627-214">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="8a627-214">dnsSuffixes</span></span>|<span data-ttu-id="8a627-215">字符串集合</span><span class="sxs-lookup"><span data-stu-id="8a627-215">String collection</span></span>|<span data-ttu-id="8a627-216">指定要添加到 DNS 搜索列表的 DNS 后缀，以正确路由短名称。</span><span class="sxs-lookup"><span data-stu-id="8a627-216">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="8a627-217">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8a627-217">authenticationMethod</span></span>|[<span data-ttu-id="8a627-218">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8a627-218">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="8a627-219">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="8a627-219">Authentication method.</span></span> <span data-ttu-id="8a627-220">可取值为：`certificate`、`usernameAndPassword`、`customEapXml`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="8a627-220">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span></span>|
|<span data-ttu-id="8a627-221">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="8a627-221">rememberUserCredentials</span></span>|<span data-ttu-id="8a627-222">布尔</span><span class="sxs-lookup"><span data-stu-id="8a627-222">Boolean</span></span>|<span data-ttu-id="8a627-223">请记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="8a627-223">Remember user credentials.</span></span>|
|<span data-ttu-id="8a627-224">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="8a627-224">enableConditionalAccess</span></span>|<span data-ttu-id="8a627-225">布尔</span><span class="sxs-lookup"><span data-stu-id="8a627-225">Boolean</span></span>|<span data-ttu-id="8a627-226">启用条件访问。</span><span class="sxs-lookup"><span data-stu-id="8a627-226">Enable conditional access.</span></span>|
|<span data-ttu-id="8a627-227">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="8a627-227">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="8a627-228">布尔</span><span class="sxs-lookup"><span data-stu-id="8a627-228">Boolean</span></span>|<span data-ttu-id="8a627-229">使用备用证书为 SSO (单一) 登录。</span><span class="sxs-lookup"><span data-stu-id="8a627-229">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="8a627-230">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="8a627-230">singleSignOnEku</span></span>|[<span data-ttu-id="8a627-231">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="8a627-231">extendedKeyUsage</span></span>](../resources/intune-shared-extendedkeyusage.md)|<span data-ttu-id="8a627-232">单一登录扩展密钥使用 (EKU) 。</span><span class="sxs-lookup"><span data-stu-id="8a627-232">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="8a627-233">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="8a627-233">singleSignOnIssuerHash</span></span>|<span data-ttu-id="8a627-234">String</span><span class="sxs-lookup"><span data-stu-id="8a627-234">String</span></span>|<span data-ttu-id="8a627-235">单一登录颁发者哈希。</span><span class="sxs-lookup"><span data-stu-id="8a627-235">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="8a627-236">eapXml</span><span class="sxs-lookup"><span data-stu-id="8a627-236">eapXml</span></span>|<span data-ttu-id="8a627-237">Binary</span><span class="sxs-lookup"><span data-stu-id="8a627-237">Binary</span></span>|<span data-ttu-id="8a627-238">可扩展身份验证协议 (EAP) XML。</span><span class="sxs-lookup"><span data-stu-id="8a627-238">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="8a627-239">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="8a627-239">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="8a627-240">proxyServer</span><span class="sxs-lookup"><span data-stu-id="8a627-240">proxyServer</span></span>|[<span data-ttu-id="8a627-241">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="8a627-241">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="8a627-242">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="8a627-242">Proxy Server.</span></span>|
|<span data-ttu-id="8a627-243">associatedApps</span><span class="sxs-lookup"><span data-stu-id="8a627-243">associatedApps</span></span>|<span data-ttu-id="8a627-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a627-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="8a627-245">关联应用。</span><span class="sxs-lookup"><span data-stu-id="8a627-245">Associated Apps.</span></span> <span data-ttu-id="8a627-246">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="8a627-246">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="8a627-247">仅AssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="8a627-247">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="8a627-248">布尔</span><span class="sxs-lookup"><span data-stu-id="8a627-248">Boolean</span></span>|<span data-ttu-id="8a627-249">只有关联的应用可以使用每个应用 VPN (连接) 。</span><span class="sxs-lookup"><span data-stu-id="8a627-249">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="8a627-250">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="8a627-250">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="8a627-251">String</span><span class="sxs-lookup"><span data-stu-id="8a627-251">String</span></span>|<span data-ttu-id="8a627-252">Windows 信息保护 (WIP) 域，以与此连接关联。</span><span class="sxs-lookup"><span data-stu-id="8a627-252">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="8a627-253">trafficRules</span><span class="sxs-lookup"><span data-stu-id="8a627-253">trafficRules</span></span>|<span data-ttu-id="8a627-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a627-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="8a627-255">流量规则。</span><span class="sxs-lookup"><span data-stu-id="8a627-255">Traffic rules.</span></span> <span data-ttu-id="8a627-256">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="8a627-256">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="8a627-257">routes</span><span class="sxs-lookup"><span data-stu-id="8a627-257">routes</span></span>|<span data-ttu-id="8a627-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a627-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="8a627-259">路由 (第三方提供商的可选) 。</span><span class="sxs-lookup"><span data-stu-id="8a627-259">Routes (optional for third-party providers).</span></span> <span data-ttu-id="8a627-260">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="8a627-260">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="8a627-261">dnsRules</span><span class="sxs-lookup"><span data-stu-id="8a627-261">dnsRules</span></span>|<span data-ttu-id="8a627-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a627-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="8a627-263">DNS 规则。</span><span class="sxs-lookup"><span data-stu-id="8a627-263">DNS rules.</span></span> <span data-ttu-id="8a627-264">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="8a627-264">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="8a627-265">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="8a627-265">trustedNetworkDomains</span></span>|<span data-ttu-id="8a627-266">字符串集合</span><span class="sxs-lookup"><span data-stu-id="8a627-266">String collection</span></span>|<span data-ttu-id="8a627-267">受信任的网络域</span><span class="sxs-lookup"><span data-stu-id="8a627-267">Trusted Network Domains</span></span>|
|<span data-ttu-id="8a627-268">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="8a627-268">cryptographySuite</span></span>|[<span data-ttu-id="8a627-269">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="8a627-269">cryptographySuite</span></span>](../resources/intune-deviceconfig-cryptographysuite.md)|<span data-ttu-id="8a627-270">Windows 10 及以上版 IKEv2 VPN 的加密套件安全设置</span><span class="sxs-lookup"><span data-stu-id="8a627-270">Cryptography Suite security settings for IKEv2 VPN in Windows10 and above</span></span> |



## <a name="response"></a><span data-ttu-id="8a627-271">响应</span><span class="sxs-lookup"><span data-stu-id="8a627-271">Response</span></span>
<span data-ttu-id="8a627-272">如果成功，此方法在响应正文中返回响应代码和更新 `200 OK` [的 windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8a627-272">If successful, this method returns a `200 OK` response code and an updated [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a627-273">示例</span><span class="sxs-lookup"><span data-stu-id="8a627-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a627-274">请求</span><span class="sxs-lookup"><span data-stu-id="8a627-274">Request</span></span>
<span data-ttu-id="8a627-275">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8a627-275">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4463

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
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
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ],
  "cryptographySuite": {
    "@odata.type": "microsoft.graph.cryptographySuite",
    "encryptionMethod": "des",
    "integrityCheckMethod": "sha1_96",
    "dhGroup": "group2",
    "cipherTransformConstants": "des",
    "authenticationTransformConstants": "sha1_96",
    "pfsGroup": "pfs2"
  }
}
```

### <a name="response"></a><span data-ttu-id="8a627-276">响应</span><span class="sxs-lookup"><span data-stu-id="8a627-276">Response</span></span>
<span data-ttu-id="8a627-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8a627-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4635

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
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
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ],
  "cryptographySuite": {
    "@odata.type": "microsoft.graph.cryptographySuite",
    "encryptionMethod": "des",
    "integrityCheckMethod": "sha1_96",
    "dhGroup": "group2",
    "cipherTransformConstants": "des",
    "authenticationTransformConstants": "sha1_96",
    "pfsGroup": "pfs2"
  }
}
```




