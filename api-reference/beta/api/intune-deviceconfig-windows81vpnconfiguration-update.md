---
title: 更新 windows81VpnConfiguration
description: 更新 windows81VpnConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bc8df9cfff58a528126163439f5b5d5cfc44ad5b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37181992"
---
# <a name="update-windows81vpnconfiguration"></a><span data-ttu-id="5ba7d-103">更新 windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="5ba7d-103">Update windows81VpnConfiguration</span></span>

> <span data-ttu-id="5ba7d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ba7d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ba7d-106">更新[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-106">Update the properties of a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ba7d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5ba7d-107">Prerequisites</span></span>
<span data-ttu-id="5ba7d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ba7d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ba7d-110">Permission type</span></span>|<span data-ttu-id="5ba7d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5ba7d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ba7d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ba7d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ba7d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ba7d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ba7d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ba7d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ba7d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-115">Not supported.</span></span>|
|<span data-ttu-id="5ba7d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ba7d-116">Application</span></span>|<span data-ttu-id="5ba7d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ba7d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ba7d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ba7d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5ba7d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ba7d-119">Request headers</span></span>
|<span data-ttu-id="5ba7d-120">标头</span><span class="sxs-lookup"><span data-stu-id="5ba7d-120">Header</span></span>|<span data-ttu-id="5ba7d-121">值</span><span class="sxs-lookup"><span data-stu-id="5ba7d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ba7d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ba7d-122">Authorization</span></span>|<span data-ttu-id="5ba7d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ba7d-124">接受</span><span class="sxs-lookup"><span data-stu-id="5ba7d-124">Accept</span></span>|<span data-ttu-id="5ba7d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5ba7d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ba7d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ba7d-126">Request body</span></span>
<span data-ttu-id="5ba7d-127">在请求正文中，提供[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-127">In the request body, supply a JSON representation for the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="5ba7d-128">下表显示创建[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-128">The following table shows the properties that are required when you create the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span>

|<span data-ttu-id="5ba7d-129">属性</span><span class="sxs-lookup"><span data-stu-id="5ba7d-129">Property</span></span>|<span data-ttu-id="5ba7d-130">类型</span><span class="sxs-lookup"><span data-stu-id="5ba7d-130">Type</span></span>|<span data-ttu-id="5ba7d-131">说明</span><span class="sxs-lookup"><span data-stu-id="5ba7d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ba7d-132">id</span><span class="sxs-lookup"><span data-stu-id="5ba7d-132">id</span></span>|<span data-ttu-id="5ba7d-133">字符串</span><span class="sxs-lookup"><span data-stu-id="5ba7d-133">String</span></span>|<span data-ttu-id="5ba7d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-134">Key of the entity.</span></span> <span data-ttu-id="5ba7d-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ba7d-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ba7d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ba7d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5ba7d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ba7d-137">DateTimeOffset</span></span>|<span data-ttu-id="5ba7d-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5ba7d-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ba7d-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ba7d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5ba7d-140">roleScopeTagIds</span></span>|<span data-ttu-id="5ba7d-141">String collection</span><span class="sxs-lookup"><span data-stu-id="5ba7d-141">String collection</span></span>|<span data-ttu-id="5ba7d-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5ba7d-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ba7d-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ba7d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5ba7d-144">supportsScopeTags</span></span>|<span data-ttu-id="5ba7d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ba7d-145">Boolean</span></span>|<span data-ttu-id="5ba7d-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5ba7d-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5ba7d-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5ba7d-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-149">This property is read-only.</span></span> <span data-ttu-id="5ba7d-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ba7d-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ba7d-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5ba7d-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5ba7d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5ba7d-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5ba7d-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5ba7d-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ba7d-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ba7d-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5ba7d-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5ba7d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5ba7d-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5ba7d-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5ba7d-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ba7d-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ba7d-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5ba7d-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5ba7d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5ba7d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5ba7d-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5ba7d-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ba7d-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ba7d-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ba7d-163">createdDateTime</span></span>|<span data-ttu-id="5ba7d-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ba7d-164">DateTimeOffset</span></span>|<span data-ttu-id="5ba7d-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-165">DateTime the object was created.</span></span> <span data-ttu-id="5ba7d-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ba7d-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ba7d-167">说明</span><span class="sxs-lookup"><span data-stu-id="5ba7d-167">description</span></span>|<span data-ttu-id="5ba7d-168">String</span><span class="sxs-lookup"><span data-stu-id="5ba7d-168">String</span></span>|<span data-ttu-id="5ba7d-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5ba7d-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ba7d-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ba7d-171">displayName</span><span class="sxs-lookup"><span data-stu-id="5ba7d-171">displayName</span></span>|<span data-ttu-id="5ba7d-172">String</span><span class="sxs-lookup"><span data-stu-id="5ba7d-172">String</span></span>|<span data-ttu-id="5ba7d-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5ba7d-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ba7d-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ba7d-175">version</span><span class="sxs-lookup"><span data-stu-id="5ba7d-175">version</span></span>|<span data-ttu-id="5ba7d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="5ba7d-176">Int32</span></span>|<span data-ttu-id="5ba7d-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-177">Version of the device configuration.</span></span> <span data-ttu-id="5ba7d-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ba7d-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ba7d-179">connectionName</span><span class="sxs-lookup"><span data-stu-id="5ba7d-179">connectionName</span></span>|<span data-ttu-id="5ba7d-180">String</span><span class="sxs-lookup"><span data-stu-id="5ba7d-180">String</span></span>|<span data-ttu-id="5ba7d-181">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-181">Connection name displayed to the user.</span></span> <span data-ttu-id="5ba7d-182">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ba7d-182">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="5ba7d-183">台</span><span class="sxs-lookup"><span data-stu-id="5ba7d-183">servers</span></span>|<span data-ttu-id="5ba7d-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="5ba7d-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="5ba7d-185">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-185">List of VPN Servers on the network.</span></span> <span data-ttu-id="5ba7d-186">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-186">Make sure end users can access these network locations.</span></span> <span data-ttu-id="5ba7d-187">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-187">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="5ba7d-188">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ba7d-188">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="5ba7d-189">customXml</span><span class="sxs-lookup"><span data-stu-id="5ba7d-189">customXml</span></span>|<span data-ttu-id="5ba7d-190">Binary</span><span class="sxs-lookup"><span data-stu-id="5ba7d-190">Binary</span></span>|<span data-ttu-id="5ba7d-191">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-191">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="5ba7d-192">（UTF8 编码的字节数组）继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ba7d-192">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="5ba7d-193">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="5ba7d-193">applyOnlyToWindows81</span></span>|<span data-ttu-id="5ba7d-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ba7d-194">Boolean</span></span>|<span data-ttu-id="5ba7d-195">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-195">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="5ba7d-196">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-196">This property is read-only.</span></span>|
|<span data-ttu-id="5ba7d-197">connectionType</span><span class="sxs-lookup"><span data-stu-id="5ba7d-197">connectionType</span></span>|[<span data-ttu-id="5ba7d-198">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="5ba7d-198">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="5ba7d-199">连接类型。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-199">Connection type.</span></span> <span data-ttu-id="5ba7d-200">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-200">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="5ba7d-201">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="5ba7d-201">loginGroupOrDomain</span></span>|<span data-ttu-id="5ba7d-202">String</span><span class="sxs-lookup"><span data-stu-id="5ba7d-202">String</span></span>|<span data-ttu-id="5ba7d-203">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-203">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="5ba7d-204">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="5ba7d-204">enableSplitTunneling</span></span>|<span data-ttu-id="5ba7d-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ba7d-205">Boolean</span></span>|<span data-ttu-id="5ba7d-206">为 VPN 启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-206">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="5ba7d-207">proxyServer</span><span class="sxs-lookup"><span data-stu-id="5ba7d-207">proxyServer</span></span>|[<span data-ttu-id="5ba7d-208">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="5ba7d-208">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="5ba7d-209">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-209">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="5ba7d-210">响应</span><span class="sxs-lookup"><span data-stu-id="5ba7d-210">Response</span></span>
<span data-ttu-id="5ba7d-211">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-211">If successful, this method returns a `200 OK` response code and an updated [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ba7d-212">示例</span><span class="sxs-lookup"><span data-stu-id="5ba7d-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ba7d-213">请求</span><span class="sxs-lookup"><span data-stu-id="5ba7d-213">Request</span></span>
<span data-ttu-id="5ba7d-214">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1788

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="5ba7d-215">响应</span><span class="sxs-lookup"><span data-stu-id="5ba7d-215">Response</span></span>
<span data-ttu-id="5ba7d-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5ba7d-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1960

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
  "id": "6aa07da3-7da3-6aa0-a37d-a06aa37da06a",
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
  }
}
```




