---
title: 更新 windowsPhone81VpnConfiguration
description: 更新 windowsPhone81VpnConfiguration 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 315faa431c23ddb36c57709ccf3baa0a15ffa1b6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42732970"
---
# <a name="update-windowsphone81vpnconfiguration"></a><span data-ttu-id="848c2-103">更新 windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="848c2-103">Update windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="848c2-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="848c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="848c2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="848c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="848c2-106">更新[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="848c2-106">Update the properties of a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="848c2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="848c2-107">Prerequisites</span></span>
<span data-ttu-id="848c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="848c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="848c2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="848c2-110">Permission type</span></span>|<span data-ttu-id="848c2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="848c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="848c2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="848c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="848c2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="848c2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="848c2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="848c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="848c2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="848c2-115">Not supported.</span></span>|
|<span data-ttu-id="848c2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="848c2-116">Application</span></span>|<span data-ttu-id="848c2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="848c2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="848c2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="848c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="848c2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="848c2-119">Request headers</span></span>
|<span data-ttu-id="848c2-120">标头</span><span class="sxs-lookup"><span data-stu-id="848c2-120">Header</span></span>|<span data-ttu-id="848c2-121">值</span><span class="sxs-lookup"><span data-stu-id="848c2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="848c2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="848c2-122">Authorization</span></span>|<span data-ttu-id="848c2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="848c2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="848c2-124">接受</span><span class="sxs-lookup"><span data-stu-id="848c2-124">Accept</span></span>|<span data-ttu-id="848c2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="848c2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="848c2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="848c2-126">Request body</span></span>
<span data-ttu-id="848c2-127">在请求正文中，提供[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="848c2-127">In the request body, supply a JSON representation for the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="848c2-128">下表显示创建[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="848c2-128">The following table shows the properties that are required when you create the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span></span>

|<span data-ttu-id="848c2-129">属性</span><span class="sxs-lookup"><span data-stu-id="848c2-129">Property</span></span>|<span data-ttu-id="848c2-130">类型</span><span class="sxs-lookup"><span data-stu-id="848c2-130">Type</span></span>|<span data-ttu-id="848c2-131">说明</span><span class="sxs-lookup"><span data-stu-id="848c2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="848c2-132">id</span><span class="sxs-lookup"><span data-stu-id="848c2-132">id</span></span>|<span data-ttu-id="848c2-133">字符串</span><span class="sxs-lookup"><span data-stu-id="848c2-133">String</span></span>|<span data-ttu-id="848c2-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="848c2-134">Key of the entity.</span></span> <span data-ttu-id="848c2-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="848c2-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="848c2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="848c2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="848c2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="848c2-137">DateTimeOffset</span></span>|<span data-ttu-id="848c2-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="848c2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="848c2-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="848c2-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="848c2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="848c2-140">roleScopeTagIds</span></span>|<span data-ttu-id="848c2-141">String collection</span><span class="sxs-lookup"><span data-stu-id="848c2-141">String collection</span></span>|<span data-ttu-id="848c2-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="848c2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="848c2-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="848c2-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="848c2-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="848c2-144">supportsScopeTags</span></span>|<span data-ttu-id="848c2-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="848c2-145">Boolean</span></span>|<span data-ttu-id="848c2-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="848c2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="848c2-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="848c2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="848c2-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="848c2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="848c2-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="848c2-149">This property is read-only.</span></span> <span data-ttu-id="848c2-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="848c2-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="848c2-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="848c2-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="848c2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="848c2-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="848c2-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="848c2-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="848c2-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="848c2-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="848c2-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="848c2-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="848c2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="848c2-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="848c2-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="848c2-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="848c2-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="848c2-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="848c2-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="848c2-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="848c2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="848c2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="848c2-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="848c2-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="848c2-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="848c2-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="848c2-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="848c2-163">createdDateTime</span></span>|<span data-ttu-id="848c2-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="848c2-164">DateTimeOffset</span></span>|<span data-ttu-id="848c2-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="848c2-165">DateTime the object was created.</span></span> <span data-ttu-id="848c2-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="848c2-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="848c2-167">说明</span><span class="sxs-lookup"><span data-stu-id="848c2-167">description</span></span>|<span data-ttu-id="848c2-168">String</span><span class="sxs-lookup"><span data-stu-id="848c2-168">String</span></span>|<span data-ttu-id="848c2-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="848c2-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="848c2-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="848c2-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="848c2-171">displayName</span><span class="sxs-lookup"><span data-stu-id="848c2-171">displayName</span></span>|<span data-ttu-id="848c2-172">String</span><span class="sxs-lookup"><span data-stu-id="848c2-172">String</span></span>|<span data-ttu-id="848c2-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="848c2-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="848c2-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="848c2-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="848c2-175">version</span><span class="sxs-lookup"><span data-stu-id="848c2-175">version</span></span>|<span data-ttu-id="848c2-176">Int32</span><span class="sxs-lookup"><span data-stu-id="848c2-176">Int32</span></span>|<span data-ttu-id="848c2-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="848c2-177">Version of the device configuration.</span></span> <span data-ttu-id="848c2-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="848c2-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="848c2-179">connectionName</span><span class="sxs-lookup"><span data-stu-id="848c2-179">connectionName</span></span>|<span data-ttu-id="848c2-180">String</span><span class="sxs-lookup"><span data-stu-id="848c2-180">String</span></span>|<span data-ttu-id="848c2-181">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="848c2-181">Connection name displayed to the user.</span></span> <span data-ttu-id="848c2-182">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="848c2-182">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="848c2-183">台</span><span class="sxs-lookup"><span data-stu-id="848c2-183">servers</span></span>|<span data-ttu-id="848c2-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="848c2-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="848c2-185">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="848c2-185">List of VPN Servers on the network.</span></span> <span data-ttu-id="848c2-186">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="848c2-186">Make sure end users can access these network locations.</span></span> <span data-ttu-id="848c2-187">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="848c2-187">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="848c2-188">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="848c2-188">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="848c2-189">customXml</span><span class="sxs-lookup"><span data-stu-id="848c2-189">customXml</span></span>|<span data-ttu-id="848c2-190">Binary</span><span class="sxs-lookup"><span data-stu-id="848c2-190">Binary</span></span>|<span data-ttu-id="848c2-191">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="848c2-191">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="848c2-192">（UTF8 编码的字节数组）继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="848c2-192">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="848c2-193">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="848c2-193">applyOnlyToWindows81</span></span>|<span data-ttu-id="848c2-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="848c2-194">Boolean</span></span>|<span data-ttu-id="848c2-195">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="848c2-195">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="848c2-196">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="848c2-196">This property is read-only.</span></span> <span data-ttu-id="848c2-197">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="848c2-197">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="848c2-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="848c2-198">connectionType</span></span>|[<span data-ttu-id="848c2-199">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="848c2-199">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="848c2-200">连接类型。</span><span class="sxs-lookup"><span data-stu-id="848c2-200">Connection type.</span></span> <span data-ttu-id="848c2-201">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="848c2-201">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="848c2-202">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`。</span><span class="sxs-lookup"><span data-stu-id="848c2-202">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="848c2-203">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="848c2-203">loginGroupOrDomain</span></span>|<span data-ttu-id="848c2-204">String</span><span class="sxs-lookup"><span data-stu-id="848c2-204">String</span></span>|<span data-ttu-id="848c2-205">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="848c2-205">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="848c2-206">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="848c2-206">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="848c2-207">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="848c2-207">enableSplitTunneling</span></span>|<span data-ttu-id="848c2-208">布尔值</span><span class="sxs-lookup"><span data-stu-id="848c2-208">Boolean</span></span>|<span data-ttu-id="848c2-209">为 VPN 启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="848c2-209">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="848c2-210">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="848c2-210">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="848c2-211">proxyServer</span><span class="sxs-lookup"><span data-stu-id="848c2-211">proxyServer</span></span>|[<span data-ttu-id="848c2-212">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="848c2-212">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="848c2-213">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="848c2-213">Proxy Server.</span></span> <span data-ttu-id="848c2-214">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="848c2-214">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="848c2-215">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="848c2-215">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="848c2-216">布尔值</span><span class="sxs-lookup"><span data-stu-id="848c2-216">Boolean</span></span>|<span data-ttu-id="848c2-217">在公司 Wi-fi 上绕过 VPN。</span><span class="sxs-lookup"><span data-stu-id="848c2-217">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="848c2-218">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="848c2-218">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="848c2-219">布尔值</span><span class="sxs-lookup"><span data-stu-id="848c2-219">Boolean</span></span>|<span data-ttu-id="848c2-220">绕过家庭 Wi-fi 上的 VPN。</span><span class="sxs-lookup"><span data-stu-id="848c2-220">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="848c2-221">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="848c2-221">authenticationMethod</span></span>|[<span data-ttu-id="848c2-222">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="848c2-222">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="848c2-223">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="848c2-223">Authentication method.</span></span> <span data-ttu-id="848c2-224">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="848c2-224">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="848c2-225">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="848c2-225">rememberUserCredentials</span></span>|<span data-ttu-id="848c2-226">布尔值</span><span class="sxs-lookup"><span data-stu-id="848c2-226">Boolean</span></span>|<span data-ttu-id="848c2-227">记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="848c2-227">Remember user credentials.</span></span>|
|<span data-ttu-id="848c2-228">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="848c2-228">dnsSuffixSearchList</span></span>|<span data-ttu-id="848c2-229">String collection</span><span class="sxs-lookup"><span data-stu-id="848c2-229">String collection</span></span>|<span data-ttu-id="848c2-230">DNS 后缀搜索列表。</span><span class="sxs-lookup"><span data-stu-id="848c2-230">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="848c2-231">响应</span><span class="sxs-lookup"><span data-stu-id="848c2-231">Response</span></span>
<span data-ttu-id="848c2-232">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="848c2-232">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="848c2-233">示例</span><span class="sxs-lookup"><span data-stu-id="848c2-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="848c2-234">请求</span><span class="sxs-lookup"><span data-stu-id="848c2-234">Request</span></span>
<span data-ttu-id="848c2-235">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="848c2-235">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="848c2-236">响应</span><span class="sxs-lookup"><span data-stu-id="848c2-236">Response</span></span>
<span data-ttu-id="848c2-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="848c2-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




