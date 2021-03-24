---
title: 更新 windowsPhone81VpnConfiguration
description: 更新 windowsPhone81VpnConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dff64eff56f177b0b242e9b68d89bdf3d30d7cbc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147117"
---
# <a name="update-windowsphone81vpnconfiguration"></a><span data-ttu-id="22037-103">更新 windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="22037-103">Update windowsPhone81VpnConfiguration</span></span>

<span data-ttu-id="22037-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22037-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22037-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="22037-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22037-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="22037-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22037-107">更新 [windowsPhone81VpnConfiguration 对象](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="22037-107">Update the properties of a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22037-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="22037-108">Prerequisites</span></span>
<span data-ttu-id="22037-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22037-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22037-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="22037-111">Permission type</span></span>|<span data-ttu-id="22037-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22037-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22037-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22037-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22037-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22037-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="22037-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22037-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22037-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="22037-116">Not supported.</span></span>|
|<span data-ttu-id="22037-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="22037-117">Application</span></span>|<span data-ttu-id="22037-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22037-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22037-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22037-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="22037-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="22037-120">Request headers</span></span>
|<span data-ttu-id="22037-121">标头</span><span class="sxs-lookup"><span data-stu-id="22037-121">Header</span></span>|<span data-ttu-id="22037-122">值</span><span class="sxs-lookup"><span data-stu-id="22037-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22037-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22037-123">Authorization</span></span>|<span data-ttu-id="22037-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="22037-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22037-125">接受</span><span class="sxs-lookup"><span data-stu-id="22037-125">Accept</span></span>|<span data-ttu-id="22037-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22037-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22037-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="22037-127">Request body</span></span>
<span data-ttu-id="22037-128">在请求正文中，提供 [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22037-128">In the request body, supply a JSON representation for the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="22037-129">下表显示创建 [windowsPhone81VpnConfiguration 时所需的属性](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="22037-129">The following table shows the properties that are required when you create the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span></span>

|<span data-ttu-id="22037-130">属性</span><span class="sxs-lookup"><span data-stu-id="22037-130">Property</span></span>|<span data-ttu-id="22037-131">类型</span><span class="sxs-lookup"><span data-stu-id="22037-131">Type</span></span>|<span data-ttu-id="22037-132">说明</span><span class="sxs-lookup"><span data-stu-id="22037-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22037-133">id</span><span class="sxs-lookup"><span data-stu-id="22037-133">id</span></span>|<span data-ttu-id="22037-134">String</span><span class="sxs-lookup"><span data-stu-id="22037-134">String</span></span>|<span data-ttu-id="22037-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="22037-135">Key of the entity.</span></span> <span data-ttu-id="22037-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22037-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22037-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22037-137">lastModifiedDateTime</span></span>|<span data-ttu-id="22037-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22037-138">DateTimeOffset</span></span>|<span data-ttu-id="22037-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="22037-139">DateTime the object was last modified.</span></span> <span data-ttu-id="22037-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22037-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22037-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="22037-141">roleScopeTagIds</span></span>|<span data-ttu-id="22037-142">String collection</span><span class="sxs-lookup"><span data-stu-id="22037-142">String collection</span></span>|<span data-ttu-id="22037-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="22037-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="22037-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22037-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22037-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="22037-145">supportsScopeTags</span></span>|<span data-ttu-id="22037-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="22037-146">Boolean</span></span>|<span data-ttu-id="22037-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="22037-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="22037-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="22037-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="22037-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="22037-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="22037-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="22037-150">This property is read-only.</span></span> <span data-ttu-id="22037-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22037-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22037-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="22037-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="22037-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="22037-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="22037-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="22037-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="22037-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22037-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22037-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="22037-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="22037-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="22037-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="22037-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="22037-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="22037-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22037-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22037-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="22037-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="22037-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="22037-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="22037-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="22037-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="22037-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22037-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22037-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22037-164">createdDateTime</span></span>|<span data-ttu-id="22037-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22037-165">DateTimeOffset</span></span>|<span data-ttu-id="22037-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="22037-166">DateTime the object was created.</span></span> <span data-ttu-id="22037-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22037-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22037-168">说明</span><span class="sxs-lookup"><span data-stu-id="22037-168">description</span></span>|<span data-ttu-id="22037-169">String</span><span class="sxs-lookup"><span data-stu-id="22037-169">String</span></span>|<span data-ttu-id="22037-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="22037-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="22037-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22037-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22037-172">displayName</span><span class="sxs-lookup"><span data-stu-id="22037-172">displayName</span></span>|<span data-ttu-id="22037-173">String</span><span class="sxs-lookup"><span data-stu-id="22037-173">String</span></span>|<span data-ttu-id="22037-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="22037-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="22037-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22037-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22037-176">version</span><span class="sxs-lookup"><span data-stu-id="22037-176">version</span></span>|<span data-ttu-id="22037-177">Int32</span><span class="sxs-lookup"><span data-stu-id="22037-177">Int32</span></span>|<span data-ttu-id="22037-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="22037-178">Version of the device configuration.</span></span> <span data-ttu-id="22037-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22037-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22037-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="22037-180">connectionName</span></span>|<span data-ttu-id="22037-181">String</span><span class="sxs-lookup"><span data-stu-id="22037-181">String</span></span>|<span data-ttu-id="22037-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="22037-182">Connection name displayed to the user.</span></span> <span data-ttu-id="22037-183">继承自 [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22037-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="22037-184">服务器</span><span class="sxs-lookup"><span data-stu-id="22037-184">servers</span></span>|<span data-ttu-id="22037-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) 集合</span><span class="sxs-lookup"><span data-stu-id="22037-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="22037-186">网络上 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="22037-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="22037-187">确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="22037-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="22037-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="22037-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="22037-189">继承自 [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22037-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="22037-190">customXml</span><span class="sxs-lookup"><span data-stu-id="22037-190">customXml</span></span>|<span data-ttu-id="22037-191">Binary</span><span class="sxs-lookup"><span data-stu-id="22037-191">Binary</span></span>|<span data-ttu-id="22037-192">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="22037-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="22037-193"> (UTF8 编码的字节数组) 继承自 [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22037-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="22037-194">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="22037-194">applyOnlyToWindows81</span></span>|<span data-ttu-id="22037-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="22037-195">Boolean</span></span>|<span data-ttu-id="22037-196">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="22037-196">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="22037-197">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="22037-197">This property is read-only.</span></span> <span data-ttu-id="22037-198">继承自 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22037-198">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="22037-199">connectionType</span><span class="sxs-lookup"><span data-stu-id="22037-199">connectionType</span></span>|[<span data-ttu-id="22037-200">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="22037-200">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="22037-201">连接类型。</span><span class="sxs-lookup"><span data-stu-id="22037-201">Connection type.</span></span> <span data-ttu-id="22037-202">继承自 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="22037-202">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="22037-203">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`。</span><span class="sxs-lookup"><span data-stu-id="22037-203">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="22037-204">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="22037-204">loginGroupOrDomain</span></span>|<span data-ttu-id="22037-205">String</span><span class="sxs-lookup"><span data-stu-id="22037-205">String</span></span>|<span data-ttu-id="22037-206">连接类型设置为 Dell SonicWALL 移动连接时登录组或域。</span><span class="sxs-lookup"><span data-stu-id="22037-206">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="22037-207">继承自 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22037-207">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="22037-208">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="22037-208">enableSplitTunneling</span></span>|<span data-ttu-id="22037-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="22037-209">Boolean</span></span>|<span data-ttu-id="22037-210">为 VPN 启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="22037-210">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="22037-211">继承自 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22037-211">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="22037-212">proxyServer</span><span class="sxs-lookup"><span data-stu-id="22037-212">proxyServer</span></span>|[<span data-ttu-id="22037-213">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="22037-213">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="22037-214">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="22037-214">Proxy Server.</span></span> <span data-ttu-id="22037-215">继承自 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22037-215">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="22037-216">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="22037-216">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="22037-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="22037-217">Boolean</span></span>|<span data-ttu-id="22037-218">在公司 WI-Fi 上绕过 VPN。</span><span class="sxs-lookup"><span data-stu-id="22037-218">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="22037-219">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="22037-219">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="22037-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="22037-220">Boolean</span></span>|<span data-ttu-id="22037-221">在家庭 WI-Fi 上绕过 VPN。</span><span class="sxs-lookup"><span data-stu-id="22037-221">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="22037-222">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="22037-222">authenticationMethod</span></span>|[<span data-ttu-id="22037-223">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="22037-223">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="22037-224">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="22037-224">Authentication method.</span></span> <span data-ttu-id="22037-225">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="22037-225">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="22037-226">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="22037-226">rememberUserCredentials</span></span>|<span data-ttu-id="22037-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="22037-227">Boolean</span></span>|<span data-ttu-id="22037-228">请记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="22037-228">Remember user credentials.</span></span>|
|<span data-ttu-id="22037-229">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="22037-229">dnsSuffixSearchList</span></span>|<span data-ttu-id="22037-230">String collection</span><span class="sxs-lookup"><span data-stu-id="22037-230">String collection</span></span>|<span data-ttu-id="22037-231">DNS 后缀搜索列表。</span><span class="sxs-lookup"><span data-stu-id="22037-231">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="22037-232">响应</span><span class="sxs-lookup"><span data-stu-id="22037-232">Response</span></span>
<span data-ttu-id="22037-233">如果成功，此方法在响应正文中返回 响应代码和更新 `200 OK` [的 windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="22037-233">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22037-234">示例</span><span class="sxs-lookup"><span data-stu-id="22037-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="22037-235">请求</span><span class="sxs-lookup"><span data-stu-id="22037-235">Request</span></span>
<span data-ttu-id="22037-236">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="22037-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2016

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
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
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="22037-237">响应</span><span class="sxs-lookup"><span data-stu-id="22037-237">Response</span></span>
<span data-ttu-id="22037-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="22037-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2188

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
  "id": "7cecc0db-c0db-7cec-dbc0-ec7cdbc0ec7c",
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
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```




